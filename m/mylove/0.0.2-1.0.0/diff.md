# Comparing `tmp/mylove-0.0.2.tar.gz` & `tmp/mylove-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mylove-0.0.2.tar", last modified: Wed Jul 26 08:27:10 2023, max compression
+gzip compressed data, was "mylove-1.0.0.tar", last modified: Wed Jul 26 08:34:35 2023, max compression
```

## Comparing `mylove-0.0.2.tar` & `mylove-1.0.0.tar`

### file list

```diff
@@ -1,2017 +1,2017 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.529309 mylove-0.0.2/
--rw-rw-rw-   0        0        0       82 2023-07-26 07:50:30.000000 mylove-0.0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1052 2023-07-26 07:51:29.000000 mylove-0.0.2/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-07-26 07:51:37.000000 mylove-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      750 2023-07-26 08:27:10.529309 mylove-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      139 2023-07-26 07:57:32.000000 mylove-0.0.2/Readme.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.458103 mylove-0.0.2/mylove/
--rw-rw-rw-   0        0        0     1891 2023-07-26 07:41:32.000000 mylove-0.0.2/mylove/__init__.py
--rw-rw-rw-   0        0        0    30672 2023-07-09 02:33:02.000000 mylove-0.0.2/mylove/h.jpg
--rw-rw-rw-   0        0        0      107 2023-07-26 07:53:56.000000 mylove-0.0.2/mylove/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.475014 mylove-0.0.2/mylove.egg-info/
--rw-rw-rw-   0        0        0      750 2023-07-26 08:27:08.000000 mylove-0.0.2/mylove.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    96481 2023-07-26 08:27:08.000000 mylove-0.0.2/mylove.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 08:27:08.000000 mylove-0.0.2/mylove.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-26 08:27:08.000000 mylove-0.0.2/mylove.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-26 08:27:08.000000 mylove-0.0.2/mylove.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 08:27:10.529309 mylove-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      792 2023-07-26 08:26:25.000000 mylove-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.449172 mylove-0.0.2/venv/
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.391724 mylove-0.0.2/venv/Lib/
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.477002 mylove-0.0.2/venv/Lib/site-packages/
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.593094 mylove-0.0.2/venv/Lib/site-packages/PIL/
--rw-rw-rw-   0        0        0     3359 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/BdfFontFile.py
--rw-rw-rw-   0        0        0    15940 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/BlpImagePlugin.py
--rw-rw-rw-   0        0        0    18138 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/BmpImagePlugin.py
--rw-rw-rw-   0        0        0     1629 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/BufrStubImagePlugin.py
--rw-rw-rw-   0        0        0     3003 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ContainerIO.py
--rw-rw-rw-   0        0        0     1796 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/CurImagePlugin.py
--rw-rw-rw-   0        0        0     2037 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/DcxImagePlugin.py
--rw-rw-rw-   0        0        0     9637 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/DdsImagePlugin.py
--rw-rw-rw-   0        0        0    15526 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/EpsImagePlugin.py
--rw-rw-rw-   0        0        0    10098 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ExifTags.py
--rw-rw-rw-   0        0        0     2132 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/FitsImagePlugin.py
--rw-rw-rw-   0        0        0     4614 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/FliImagePlugin.py
--rw-rw-rw-   0        0        0     2874 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/FontFile.py
--rw-rw-rw-   0        0        0     7214 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/FpxImagePlugin.py
--rw-rw-rw-   0        0        0     3541 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/FtexImagePlugin.py
--rw-rw-rw-   0        0        0     3010 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/GbrImagePlugin.py
--rw-rw-rw-   0        0        0     2704 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/GdImageFile.py
--rw-rw-rw-   0        0        0    36838 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/GifImagePlugin.py
--rw-rw-rw-   0        0        0     3533 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/GimpGradientFile.py
--rw-rw-rw-   0        0        0     1401 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/GimpPaletteFile.py
--rw-rw-rw-   0        0        0     1623 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/GribStubImagePlugin.py
--rw-rw-rw-   0        0        0     1626 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/Hdf5StubImagePlugin.py
--rw-rw-rw-   0        0        0    12325 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/IcnsImagePlugin.py
--rw-rw-rw-   0        0        0    11980 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/IcoImagePlugin.py
--rw-rw-rw-   0        0        0    11238 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImImagePlugin.py
--rw-rw-rw-   0        0        0   137166 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/Image.py
--rw-rw-rw-   0        0        0     7306 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImageChops.py
--rw-rw-rw-   0        0        0    38180 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImageCms.py
--rw-rw-rw-   0        0        0     9397 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImageColor.py
--rw-rw-rw-   0        0        0    36829 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImageDraw.py
--rw-rw-rw-   0        0        0     5694 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImageDraw2.py
--rw-rw-rw-   0        0        0     3293 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImageEnhance.py
--rw-rw-rw-   0        0        0    24312 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImageFile.py
--rw-rw-rw-   0        0        0    17110 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImageFilter.py
--rw-rw-rw-   0        0        0    43021 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImageFont.py
--rw-rw-rw-   0        0        0     5496 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImageGrab.py
--rw-rw-rw-   0        0        0     7620 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImageMath.py
--rw-rw-rw-   0        0        0     3004 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImageMode.py
--rw-rw-rw-   0        0        0     8231 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImageMorph.py
--rw-rw-rw-   0        0        0    22052 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImageOps.py
--rw-rw-rw-   0        0        0     8174 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImagePalette.py
--rw-rw-rw-   0        0        0      355 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImagePath.py
--rw-rw-rw-   0        0        0     6582 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImageQt.py
--rw-rw-rw-   0        0        0     1948 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImageSequence.py
--rw-rw-rw-   0        0        0     8631 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImageShow.py
--rw-rw-rw-   0        0        0     4072 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImageStat.py
--rw-rw-rw-   0        0        0     8744 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImageTk.py
--rw-rw-rw-   0        0        0     2985 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImageTransform.py
--rw-rw-rw-   0        0        0     7421 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImageWin.py
--rw-rw-rw-   0        0        0     2680 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/ImtImagePlugin.py
--rw-rw-rw-   0        0        0     6007 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/IptcImagePlugin.py
--rw-rw-rw-   0        0        0    11982 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/Jpeg2KImagePlugin.py
--rw-rw-rw-   0        0        0    29937 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/JpegImagePlugin.py
--rw-rw-rw-   0        0        0    12583 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/JpegPresets.py
--rw-rw-rw-   0        0        0     1871 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/McIdasImagePlugin.py
--rw-rw-rw-   0        0        0     2617 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/MicImagePlugin.py
--rw-rw-rw-   0        0        0     1905 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/MpegImagePlugin.py
--rw-rw-rw-   0        0        0     6486 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/MpoImagePlugin.py
--rw-rw-rw-   0        0        0     5806 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/MspImagePlugin.py
--rw-rw-rw-   0        0        0     6754 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/PSDraw.py
--rw-rw-rw-   0        0        0     1179 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/PaletteFile.py
--rw-rw-rw-   0        0        0     9369 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/PalmImagePlugin.py
--rw-rw-rw-   0        0        0     1558 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/PcdImagePlugin.py
--rw-rw-rw-   0        0        0     7013 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/PcfFontFile.py
--rw-rw-rw-   0        0        0     6242 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/PcxImagePlugin.py
--rw-rw-rw-   0        0        0     9264 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/PdfImagePlugin.py
--rw-rw-rw-   0        0        0    35397 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/PdfParser.py
--rw-rw-rw-   0        0        0     1720 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/PixarImagePlugin.py
--rw-rw-rw-   0        0        0    47830 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/PngImagePlugin.py
--rw-rw-rw-   0        0        0    11746 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/PpmImagePlugin.py
--rw-rw-rw-   0        0        0     7838 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/PsdImagePlugin.py
--rw-rw-rw-   0        0        0    10261 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/PyAccess.py
--rw-rw-rw-   0        0        0     3722 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/QoiImagePlugin.py
--rw-rw-rw-   0        0        0     6409 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/SgiImagePlugin.py
--rw-rw-rw-   0        0        0     9788 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/SpiderImagePlugin.py
--rw-rw-rw-   0        0        0     4537 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/SunImagePlugin.py
--rw-rw-rw-   0        0        0     1557 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/TarIO.py
--rw-rw-rw-   0        0        0     6830 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/TgaImagePlugin.py
--rw-rw-rw-   0        0        0    79171 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/TiffImagePlugin.py
--rw-rw-rw-   0        0        0    17374 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/TiffTags.py
--rw-rw-rw-   0        0        0     5642 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/WalImageFile.py
--rw-rw-rw-   0        0        0    11732 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/WebPImagePlugin.py
--rw-rw-rw-   0        0        0     4867 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/WmfImagePlugin.py
--rw-rw-rw-   0        0        0     2064 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/XVThumbImagePlugin.py
--rw-rw-rw-   0        0        0     2581 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/XbmImagePlugin.py
--rw-rw-rw-   0        0        0     3312 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/XpmImagePlugin.py
--rw-rw-rw-   0        0        0     2063 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/__init__.py
--rw-rw-rw-   0        0        0       44 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/__main__.py
--rw-rw-rw-   0        0        0     2145 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/_binary.py
--rw-rw-rw-   0        0        0     2005 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/_deprecate.py
--rw-rw-rw-   0        0        0      520 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/_tkinter_finder.py
--rw-rw-rw-   0        0        0      388 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/_util.py
--rw-rw-rw-   0        0        0       53 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/_version.py
--rw-rw-rw-   0        0        0     9947 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/PIL/features.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.594112 mylove-0.0.2/venv/Lib/site-packages/Pillow-10.0.0.dist-info/
--rw-rw-rw-   0        0        0        4 2023-07-26 07:38:26.000000 mylove-0.0.2/venv/Lib/site-packages/Pillow-10.0.0.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.595364 mylove-0.0.2/venv/Lib/site-packages/Pygments-2.15.1.dist-info/
--rw-rw-rw-   0        0        0       53 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/Pygments-2.15.1.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/Pygments-2.15.1.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.599238 mylove-0.0.2/venv/Lib/site-packages/SpeechRecognition-3.10.0.dist-info/
--rw-rw-rw-   0        0        0    18092 2023-07-26 07:38:31.000000 mylove-0.0.2/venv/Lib/site-packages/SpeechRecognition-3.10.0.dist-info/LICENSE-FLAC.txt
--rw-rw-rw-   0        0        0     1519 2023-07-26 07:38:31.000000 mylove-0.0.2/venv/Lib/site-packages/SpeechRecognition-3.10.0.dist-info/LICENSE.txt
--rw-rw-rw-   0        0        0       19 2023-07-26 07:38:31.000000 mylove-0.0.2/venv/Lib/site-packages/SpeechRecognition-3.10.0.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.601235 mylove-0.0.2/venv/Lib/site-packages/_distutils_hack/
--rw-rw-rw-   0        0        0     6128 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/_distutils_hack/__init__.py
--rw-rw-rw-   0        0        0       44 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/_distutils_hack/override.py
--rw-rw-rw-   0        0        0     5770 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/_virtualenv.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.610402 mylove-0.0.2/venv/Lib/site-packages/bleach/
--rw-rw-rw-   0        0        0     3649 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.615310 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/
--rw-rw-rw-   0        0        0        0 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.627174 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/
--rw-rw-rw-   0        0        0     1143 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/__init__.py
--rw-rw-rw-   0        0        0    16728 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_ihatexml.py
--rw-rw-rw-   0        0        0    32300 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_inputstream.py
--rw-rw-rw-   0        0        0    77028 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.630484 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/
--rw-rw-rw-   0        0        0      109 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/__init__.py
--rw-rw-rw-   0        0        0     1013 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/_base.py
--rw-rw-rw-   0        0        0     1763 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/py.py
--rw-rw-rw-   0        0        0     4919 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_utils.py
--rw-rw-rw-   0        0        0    83464 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.637312 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/
--rw-rw-rw-   0        0        0        0 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/__init__.py
--rw-rw-rw-   0        0        0      919 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/alphabeticalattributes.py
--rw-rw-rw-   0        0        0      286 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/base.py
--rw-rw-rw-   0        0        0     2945 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/inject_meta_charset.py
--rw-rw-rw-   0        0        0     3631 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/lint.py
--rw-rw-rw-   0        0        0    10588 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/optionaltags.py
--rw-rw-rw-   0        0        0    26885 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/sanitizer.py
--rw-rw-rw-   0        0        0     1214 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/whitespace.py
--rw-rw-rw-   0        0        0   117174 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/html5parser.py
--rw-rw-rw-   0        0        0    15747 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/serializer.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.641870 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/
--rw-rw-rw-   0        0        0      650 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/__init__.py
--rw-rw-rw-   0        0        0     1715 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/genshi.py
--rw-rw-rw-   0        0        0     1776 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/sax.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.647952 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/
--rw-rw-rw-   0        0        0     3592 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/__init__.py
--rw-rw-rw-   0        0        0    14553 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/base.py
--rw-rw-rw-   0        0        0     8925 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/dom.py
--rw-rw-rw-   0        0        0    12824 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/etree.py
--rw-rw-rw-   0        0        0    14754 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/etree_lxml.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.652957 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/
--rw-rw-rw-   0        0        0     5719 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/__init__.py
--rw-rw-rw-   0        0        0     7476 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/base.py
--rw-rw-rw-   0        0        0     1413 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/dom.py
--rw-rw-rw-   0        0        0     4539 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/etree.py
--rw-rw-rw-   0        0        0     6345 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/etree_lxml.py
--rw-rw-rw-   0        0        0     2309 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/genshi.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.628452 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/
--rw-rw-rw-   0        0        0        9 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/top_level.txt
--rw-rw-rw-   0        0        0    39023 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/parse.py
--rw-rw-rw-   0        0        0      184 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/vendor.txt
--rw-rw-rw-   0        0        0      752 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/callbacks.py
--rw-rw-rw-   0        0        0     2526 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/css_sanitizer.py
--rw-rw-rw-   0        0        0    22779 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/html5lib_shim.py
--rw-rw-rw-   0        0        0    22350 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/linkifier.py
--rw-rw-rw-   0        0        0       50 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/parse_shim.py
--rw-rw-rw-   0        0        0    21934 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach/sanitizer.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.611538 mylove-0.0.2/venv/Lib/site-packages/bleach-6.0.0.dist-info/
--rw-rw-rw-   0        0        0        7 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/bleach-6.0.0.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.656502 mylove-0.0.2/venv/Lib/site-packages/certifi/
--rw-rw-rw-   0        0        0       94 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/certifi/__init__.py
--rw-rw-rw-   0        0        0      243 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/certifi/__main__.py
--rw-rw-rw-   0        0        0     4219 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/certifi/core.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.657519 mylove-0.0.2/venv/Lib/site-packages/certifi-2023.5.7.dist-info/
--rw-rw-rw-   0        0        0        8 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/certifi-2023.5.7.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.665549 mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/
--rw-rw-rw-   0        0        0     1623 2023-07-26 07:38:29.000000 mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/__init__.py
--rw-rw-rw-   0        0        0    21723 2023-07-26 07:38:29.000000 mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/api.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.668995 mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/assets/
--rw-rw-rw-   0        0        0    21509 2023-07-26 07:38:29.000000 mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/assets/__init__.py
--rw-rw-rw-   0        0        0    12944 2023-07-26 07:38:29.000000 mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/cd.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.672478 mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/cli/
--rw-rw-rw-   0        0        0        0 2023-07-26 07:38:29.000000 mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/cli/__init__.py
--rw-rw-rw-   0        0        0    10040 2023-07-26 07:38:29.000000 mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/cli/normalizer.py
--rw-rw-rw-   0        0        0    19596 2023-07-26 07:38:29.000000 mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/constant.py
--rw-rw-rw-   0        0        0     2125 2023-07-26 07:38:29.000000 mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/legacy.py
--rw-rw-rw-   0        0        0    19264 2023-07-26 07:38:29.000000 mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/md.py
--rw-rw-rw-   0        0        0    11829 2023-07-26 07:38:29.000000 mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/models.py
--rw-rw-rw-   0        0        0    11992 2023-07-26 07:38:29.000000 mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/utils.py
--rw-rw-rw-   0        0        0       85 2023-07-26 07:38:29.000000 mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/version.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.667951 mylove-0.0.2/venv/Lib/site-packages/charset_normalizer-3.2.0.dist-info/
--rw-rw-rw-   0        0        0       76 2023-07-26 07:38:29.000000 mylove-0.0.2/venv/Lib/site-packages/charset_normalizer-3.2.0.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-07-26 07:38:29.000000 mylove-0.0.2/venv/Lib/site-packages/charset_normalizer-3.2.0.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.681663 mylove-0.0.2/venv/Lib/site-packages/docutils/
--rw-rw-rw-   0        0        0    10293 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/__init__.py
--rw-rw-rw-   0        0        0     3625 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/__main__.py
--rw-rw-rw-   0        0        0    33045 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/core.py
--rw-rw-rw-   0        0        0     3961 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/examples.py
--rw-rw-rw-   0        0        0    40002 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/frontend.py
--rw-rw-rw-   0        0        0    23958 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/io.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.715171 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/
--rw-rw-rw-   0        0        0     2921 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/__init__.py
--rw-rw-rw-   0        0        0     1831 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/af.py
--rw-rw-rw-   0        0        0     1943 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/ar.py
--rw-rw-rw-   0        0        0     1912 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/ca.py
--rw-rw-rw-   0        0        0     1900 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/cs.py
--rw-rw-rw-   0        0        0     1856 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/da.py
--rw-rw-rw-   0        0        0     1728 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/de.py
--rw-rw-rw-   0        0        0     1854 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/en.py
--rw-rw-rw-   0        0        0     1931 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/eo.py
--rw-rw-rw-   0        0        0     1906 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/es.py
--rw-rw-rw-   0        0        0     1958 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/fa.py
--rw-rw-rw-   0        0        0     1964 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/fi.py
--rw-rw-rw-   0        0        0     1831 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/fr.py
--rw-rw-rw-   0        0        0     1990 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/gl.py
--rw-rw-rw-   0        0        0     2692 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/he.py
--rw-rw-rw-   0        0        0     1814 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/it.py
--rw-rw-rw-   0        0        0     1890 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/ja.py
--rw-rw-rw-   0        0        0     1832 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/ko.py
--rw-rw-rw-   0        0        0     1919 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/lt.py
--rw-rw-rw-   0        0        0     1851 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/lv.py
--rw-rw-rw-   0        0        0     1871 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/nl.py
--rw-rw-rw-   0        0        0     1866 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/pl.py
--rw-rw-rw-   0        0        0     1929 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/pt_br.py
--rw-rw-rw-   0        0        0     2070 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/ru.py
--rw-rw-rw-   0        0        0     1832 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/sk.py
--rw-rw-rw-   0        0        0     1863 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/sv.py
--rw-rw-rw-   0        0        0     2062 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/uk.py
--rw-rw-rw-   0        0        0     1974 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/zh_cn.py
--rw-rw-rw-   0        0        0     2742 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/languages/zh_tw.py
--rw-rw-rw-   0        0        0    81006 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/nodes.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.719029 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/
--rw-rw-rw-   0        0        0     3724 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/__init__.py
--rw-rw-rw-   0        0        0     1765 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/commonmark_wrapper.py
--rw-rw-rw-   0        0        0      445 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/null.py
--rw-rw-rw-   0        0        0     5426 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/recommonmark_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.726876 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/
--rw-rw-rw-   0        0        0    15954 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.741256 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/
--rw-rw-rw-   0        0        0    14652 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/__init__.py
--rw-rw-rw-   0        0        0     2405 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/admonitions.py
--rw-rw-rw-   0        0        0     9883 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/body.py
--rw-rw-rw-   0        0        0      695 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/html.py
--rw-rw-rw-   0        0        0     6799 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/images.py
--rw-rw-rw-   0        0        0    26302 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/misc.py
--rw-rw-rw-   0        0        0     4247 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/parts.py
--rw-rw-rw-   0        0        0      831 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/references.py
--rw-rw-rw-   0        0        0    23825 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/tables.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.792793 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/
--rw-rw-rw-   0        0        0      670 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/README.txt
--rw-rw-rw-   0        0        0    10925 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsa.txt
--rw-rw-rw-   0        0        0     7242 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsb.txt
--rw-rw-rw-   0        0        0     1723 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsc.txt
--rw-rw-rw-   0        0        0     6721 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsn.txt
--rw-rw-rw-   0        0        0     3825 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamso.txt
--rw-rw-rw-   0        0        0    11763 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsr.txt
--rw-rw-rw-   0        0        0     3101 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isobox.txt
--rw-rw-rw-   0        0        0     4241 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isocyr1.txt
--rw-rw-rw-   0        0        0     1882 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isocyr2.txt
--rw-rw-rw-   0        0        0      869 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isodia.txt
--rw-rw-rw-   0        0        0     3010 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk1.txt
--rw-rw-rw-   0        0        0     1705 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk2.txt
--rw-rw-rw-   0        0        0     2880 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk3.txt
--rw-rw-rw-   0        0        0     3035 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk4-wide.txt
--rw-rw-rw-   0        0        0      372 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk4.txt
--rw-rw-rw-   0        0        0     4397 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isolat1.txt
--rw-rw-rw-   0        0        0     8466 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isolat2.txt
--rw-rw-rw-   0        0        0     3334 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk-wide.txt
--rw-rw-rw-   0        0        0      519 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk.txt
--rw-rw-rw-   0        0        0     1931 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomopf-wide.txt
--rw-rw-rw-   0        0        0      639 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomopf.txt
--rw-rw-rw-   0        0        0     3231 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomscr-wide.txt
--rw-rw-rw-   0        0        0      776 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomscr.txt
--rw-rw-rw-   0        0        0     4066 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isonum.txt
--rw-rw-rw-   0        0        0     4613 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isopub.txt
--rw-rw-rw-   0        0        0     9726 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isotech.txt
--rw-rw-rw-   0        0        0    45428 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/mmlalias.txt
--rw-rw-rw-   0        0        0     9010 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra-wide.txt
--rw-rw-rw-   0        0        0     6800 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra.txt
--rw-rw-rw-   0        0        0     1036 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/s5defs.txt
--rw-rw-rw-   0        0        0     6112 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-lat1.txt
--rw-rw-rw-   0        0        0     1945 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-special.txt
--rw-rw-rw-   0        0        0     7028 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-symbol.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.827775 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/
--rw-rw-rw-   0        0        0     1222 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/__init__.py
--rw-rw-rw-   0        0        0     3727 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/af.py
--rw-rw-rw-   0        0        0     3051 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ar.py
--rw-rw-rw-   0        0        0     4406 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ca.py
--rw-rw-rw-   0        0        0     4808 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/cs.py
--rw-rw-rw-   0        0        0     3719 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/da.py
--rw-rw-rw-   0        0        0     3547 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/de.py
--rw-rw-rw-   0        0        0     3514 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/en.py
--rw-rw-rw-   0        0        0     3825 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/eo.py
--rw-rw-rw-   0        0        0     4158 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/es.py
--rw-rw-rw-   0        0        0     3171 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/fa.py
--rw-rw-rw-   0        0        0     3526 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/fi.py
--rw-rw-rw-   0        0        0     3782 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/fr.py
--rw-rw-rw-   0        0        0     3632 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/gl.py
--rw-rw-rw-   0        0        0     3641 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/he.py
--rw-rw-rw-   0        0        0     3322 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/it.py
--rw-rw-rw-   0        0        0     3776 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ja.py
--rw-rw-rw-   0        0        0     3377 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ko.py
--rw-rw-rw-   0        0        0     3519 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/lt.py
--rw-rw-rw-   0        0        0     3376 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/lv.py
--rw-rw-rw-   0        0        0     3761 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/nl.py
--rw-rw-rw-   0        0        0     3443 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/pl.py
--rw-rw-rw-   0        0        0     3960 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/pt_br.py
--rw-rw-rw-   0        0        0     3398 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ru.py
--rw-rw-rw-   0        0        0     3947 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/sk.py
--rw-rw-rw-   0        0        0     3261 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/sv.py
--rw-rw-rw-   0        0        0     3441 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/uk.py
--rw-rw-rw-   0        0        0     3925 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/zh_cn.py
--rw-rw-rw-   0        0        0     5160 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/zh_tw.py
--rw-rw-rw-   0        0        0    16119 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/roles.py
--rw-rw-rw-   0        0        0   132550 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/states.py
--rw-rw-rw-   0        0        0    20912 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/tableparser.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.833640 mylove-0.0.2/venv/Lib/site-packages/docutils/readers/
--rw-rw-rw-   0        0        0     3520 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/readers/__init__.py
--rw-rw-rw-   0        0        0     1607 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/readers/doctree.py
--rw-rw-rw-   0        0        0     1523 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/readers/pep.py
--rw-rw-rw-   0        0        0     2324 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/readers/standalone.py
--rw-rw-rw-   0        0        0    56956 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/statemachine.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.846332 mylove-0.0.2/venv/Lib/site-packages/docutils/transforms/
--rw-rw-rw-   0        0        0     6870 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/transforms/__init__.py
--rw-rw-rw-   0        0        0     2151 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/transforms/components.py
--rw-rw-rw-   0        0        0    21371 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/transforms/frontmatter.py
--rw-rw-rw-   0        0        0     4873 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/transforms/misc.py
--rw-rw-rw-   0        0        0     6912 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/transforms/parts.py
--rw-rw-rw-   0        0        0    11111 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/transforms/peps.py
--rw-rw-rw-   0        0        0    36819 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/transforms/references.py
--rw-rw-rw-   0        0        0    12548 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/transforms/universal.py
--rw-rw-rw-   0        0        0     3057 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/transforms/writer_aux.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.858332 mylove-0.0.2/venv/Lib/site-packages/docutils/utils/
--rw-rw-rw-   0        0        0    29382 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/utils/__init__.py
--rw-rw-rw-   0        0        0     4920 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/utils/code_analyzer.py
--rw-rw-rw-   0        0        0     8105 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/utils/error_reporting.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.867602 mylove-0.0.2/venv/Lib/site-packages/docutils/utils/math/
--rw-rw-rw-   0        0        0     1825 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/utils/math/__init__.py
--rw-rw-rw-   0        0        0    51496 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/utils/math/latex2mathml.py
--rw-rw-rw-   0        0        0   107993 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/utils/math/math2html.py
--rw-rw-rw-   0        0        0     6760 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/utils/math/tex2mathml_extern.py
--rw-rw-rw-   0        0        0    37497 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/utils/math/tex2unichar.py
--rw-rw-rw-   0        0        0    18393 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/utils/math/unichar2tex.py
--rw-rw-rw-   0        0        0     5747 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/utils/punctuation_chars.py
--rw-rw-rw-   0        0        0     2695 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/utils/roman.py
--rw-rw-rw-   0        0        0    38972 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/utils/smartquotes.py
--rw-rw-rw-   0        0        0     6260 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/utils/urischemes.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.876770 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/
--rw-rw-rw-   0        0        0     4945 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/__init__.py
--rw-rw-rw-   0        0        0    70896 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/_html_base.py
--rw-rw-rw-   0        0        0     6763 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/docutils_xml.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.878960 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/html4css1/
--rw-rw-rw-   0        0        0    37675 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/html4css1/__init__.py
--rw-rw-rw-   0        0        0      114 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/html4css1/template.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.880983 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/
--rw-rw-rw-   0        0        0    16718 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/__init__.py
--rw-rw-rw-   0        0        0      114 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/template.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.882113 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/latex2e/
--rw-rw-rw-   0        0        0   137132 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/latex2e/__init__.py
--rw-rw-rw-   0        0        0    36654 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/manpage.py
--rw-rw-rw-   0        0        0      568 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/null.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.885305 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/odf_odt/
--rw-rw-rw-   0        0        0   132358 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/odf_odt/__init__.py
--rw-rw-rw-   0        0        0     2142 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/odf_odt/prepstyles.py
--rw-rw-rw-   0        0        0     4681 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/odf_odt/pygmentsformatter.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.890039 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/pep_html/
--rw-rw-rw-   0        0        0     3505 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/pep_html/__init__.py
--rw-rw-rw-   0        0        0     1001 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/pep_html/template.txt
--rw-rw-rw-   0        0        0     1032 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/pseudoxml.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.891107 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/s5_html/
--rw-rw-rw-   0        0        0    14517 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/s5_html/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.892110 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/
--rw-rw-rw-   0        0        0      278 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.893610 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/xetex/
--rw-rw-rw-   0        0        0     5736 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils/writers/xetex/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.686201 mylove-0.0.2/venv/Lib/site-packages/docutils-0.20.1.dist-info/
--rw-rw-rw-   0        0        0     6292 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils-0.20.1.dist-info/COPYING.txt
--rw-rw-rw-   0        0        0       53 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils-0.20.1.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Lib/site-packages/docutils-0.20.1.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.903023 mylove-0.0.2/venv/Lib/site-packages/idna/
--rw-rw-rw-   0        0        0      849 2023-07-26 07:38:28.000000 mylove-0.0.2/venv/Lib/site-packages/idna/__init__.py
--rw-rw-rw-   0        0        0     3374 2023-07-26 07:38:28.000000 mylove-0.0.2/venv/Lib/site-packages/idna/codec.py
--rw-rw-rw-   0        0        0      321 2023-07-26 07:38:28.000000 mylove-0.0.2/venv/Lib/site-packages/idna/compat.py
--rw-rw-rw-   0        0        0    12950 2023-07-26 07:38:28.000000 mylove-0.0.2/venv/Lib/site-packages/idna/core.py
--rw-rw-rw-   0        0        0    44375 2023-07-26 07:38:28.000000 mylove-0.0.2/venv/Lib/site-packages/idna/idnadata.py
--rw-rw-rw-   0        0        0     1881 2023-07-26 07:38:28.000000 mylove-0.0.2/venv/Lib/site-packages/idna/intranges.py
--rw-rw-rw-   0        0        0       21 2023-07-26 07:38:28.000000 mylove-0.0.2/venv/Lib/site-packages/idna/package_data.py
--rw-rw-rw-   0        0        0   206539 2023-07-26 07:38:29.000000 mylove-0.0.2/venv/Lib/site-packages/idna/uts46data.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.915730 mylove-0.0.2/venv/Lib/site-packages/importlib_metadata/
--rw-rw-rw-   0        0        0    30749 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/importlib_metadata/__init__.py
--rw-rw-rw-   0        0        0     2454 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/importlib_metadata/_adapters.py
--rw-rw-rw-   0        0        0      743 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/importlib_metadata/_collections.py
--rw-rw-rw-   0        0        0     1554 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/importlib_metadata/_compat.py
--rw-rw-rw-   0        0        0     2895 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/importlib_metadata/_functools.py
--rw-rw-rw-   0        0        0     2068 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/importlib_metadata/_itertools.py
--rw-rw-rw-   0        0        0     1613 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/importlib_metadata/_meta.py
--rw-rw-rw-   0        0        0     1098 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/importlib_metadata/_py39compat.py
--rw-rw-rw-   0        0        0     2166 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/importlib_metadata/_text.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.916827 mylove-0.0.2/venv/Lib/site-packages/importlib_metadata-6.8.0.dist-info/
--rw-rw-rw-   0        0        0       19 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/importlib_metadata-6.8.0.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.408319 mylove-0.0.2/venv/Lib/site-packages/jaraco/
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.925604 mylove-0.0.2/venv/Lib/site-packages/jaraco/classes/
--rw-rw-rw-   0        0        0        0 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/jaraco/classes/__init__.py
--rw-rw-rw-   0        0        0     1464 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/jaraco/classes/ancestry.py
--rw-rw-rw-   0        0        0     1853 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/jaraco/classes/meta.py
--rw-rw-rw-   0        0        0     3996 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/jaraco/classes/properties.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.917836 mylove-0.0.2/venv/Lib/site-packages/jaraco.classes-3.3.0.dist-info/
--rw-rw-rw-   0        0        0        7 2023-07-26 08:06:11.000000 mylove-0.0.2/venv/Lib/site-packages/jaraco.classes-3.3.0.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.944877 mylove-0.0.2/venv/Lib/site-packages/keyring/
--rw-rw-rw-   0        0        0      271 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/__init__.py
--rw-rw-rw-   0        0        0       71 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/__main__.py
--rw-rw-rw-   0        0        0      185 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/_compat.py
--rw-rw-rw-   0        0        0     3886 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/_properties_compat.py
--rw-rw-rw-   0        0        0     8100 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/backend.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.957926 mylove-0.0.2/venv/Lib/site-packages/keyring/backends/
--rw-rw-rw-   0        0        0     4692 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/backends/SecretService.py
--rw-rw-rw-   0        0        0     5814 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/backends/Windows.py
--rw-rw-rw-   0        0        0        0 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/backends/__init__.py
--rw-rw-rw-   0        0        0     2173 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/backends/chainer.py
--rw-rw-rw-   0        0        0      929 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/backends/fail.py
--rw-rw-rw-   0        0        0     5830 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/backends/kwallet.py
--rw-rw-rw-   0        0        0     5982 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/backends/libsecret.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.961297 mylove-0.0.2/venv/Lib/site-packages/keyring/backends/macOS/
--rw-rw-rw-   0        0        0     2689 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/backends/macOS/__init__.py
--rw-rw-rw-   0        0        0     4341 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/backends/macOS/api.py
--rw-rw-rw-   0        0        0      453 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/backends/null.py
--rw-rw-rw-   0        0        0     4475 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/cli.py
--rw-rw-rw-   0        0        0     1324 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/completion.py
--rw-rw-rw-   0        0        0     5731 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/core.py
--rw-rw-rw-   0        0        0     1593 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/credentials.py
--rw-rw-rw-   0        0        0      752 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/devpi_client.py
--rw-rw-rw-   0        0        0     1430 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/errors.py
--rw-rw-rw-   0        0        0     1231 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/http.py
--rw-rw-rw-   0        0        0      175 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/py312compat.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.968821 mylove-0.0.2/venv/Lib/site-packages/keyring/testing/
--rw-rw-rw-   0        0        0        0 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/testing/__init__.py
--rw-rw-rw-   0        0        0     6598 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/testing/backend.py
--rw-rw-rw-   0        0        0     1918 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/testing/util.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.974319 mylove-0.0.2/venv/Lib/site-packages/keyring/util/
--rw-rw-rw-   0        0        0      868 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/util/__init__.py
--rw-rw-rw-   0        0        0     2215 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring/util/platform_.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.947119 mylove-0.0.2/venv/Lib/site-packages/keyring-24.2.0.dist-info/
--rw-rw-rw-   0        0        0      334 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring-24.2.0.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/keyring-24.2.0.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.998806 mylove-0.0.2/venv/Lib/site-packages/markdown_it/
--rw-rw-rw-   0        0        0      113 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/__init__.py
--rw-rw-rw-   0        0        0      246 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/_compat.py
--rw-rw-rw-   0        0        0     2364 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/_punycode.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.011673 mylove-0.0.2/venv/Lib/site-packages/markdown_it/cli/
--rw-rw-rw-   0        0        0        0 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/cli/__init__.py
--rw-rw-rw-   0        0        0     2901 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/cli/parse.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.020190 mylove-0.0.2/venv/Lib/site-packages/markdown_it/common/
--rw-rw-rw-   0        0        0        0 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/common/__init__.py
--rw-rw-rw-   0        0        0      156 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/common/entities.py
--rw-rw-rw-   0        0        0      932 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/common/html_blocks.py
--rw-rw-rw-   0        0        0      929 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/common/html_re.py
--rw-rw-rw-   0        0        0     2568 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/common/normalize_url.py
--rw-rw-rw-   0        0        0    10728 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/common/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.028189 mylove-0.0.2/venv/Lib/site-packages/markdown_it/helpers/
--rw-rw-rw-   0        0        0      253 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/helpers/__init__.py
--rw-rw-rw-   0        0        0     1977 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/helpers/parse_link_destination.py
--rw-rw-rw-   0        0        0     1036 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/helpers/parse_link_label.py
--rw-rw-rw-   0        0        0     1425 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/helpers/parse_link_title.py
--rw-rw-rw-   0        0        0    12772 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/main.py
--rw-rw-rw-   0        0        0     3911 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/parser_block.py
--rw-rw-rw-   0        0        0     1010 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/parser_core.py
--rw-rw-rw-   0        0        0     4997 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/parser_inline.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.034963 mylove-0.0.2/venv/Lib/site-packages/markdown_it/presets/
--rw-rw-rw-   0        0        0      970 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/presets/__init__.py
--rw-rw-rw-   0        0        0     2868 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/presets/commonmark.py
--rw-rw-rw-   0        0        0     1810 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/presets/default.py
--rw-rw-rw-   0        0        0     2112 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/presets/zero.py
--rw-rw-rw-   0        0        0     9970 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/renderer.py
--rw-rw-rw-   0        0        0     9199 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/ruler.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.056635 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/
--rw-rw-rw-   0        0        0      553 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/__init__.py
--rw-rw-rw-   0        0        0     8887 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/blockquote.py
--rw-rw-rw-   0        0        0      859 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/code.py
--rw-rw-rw-   0        0        0     2537 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/fence.py
--rw-rw-rw-   0        0        0     1746 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/heading.py
--rw-rw-rw-   0        0        0     1226 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/hr.py
--rw-rw-rw-   0        0        0     2721 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/html_block.py
--rw-rw-rw-   0        0        0     2625 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/lheading.py
--rw-rw-rw-   0        0        0     9668 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/list.py
--rw-rw-rw-   0        0        0     1818 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/paragraph.py
--rw-rw-rw-   0        0        0     6168 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/reference.py
--rw-rw-rw-   0        0        0     8422 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/state_block.py
--rw-rw-rw-   0        0        0     6987 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/table.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.067284 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_core/
--rw-rw-rw-   0        0        0      394 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_core/__init__.py
--rw-rw-rw-   0        0        0      372 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_core/block.py
--rw-rw-rw-   0        0        0      325 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_core/inline.py
--rw-rw-rw-   0        0        0     5141 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_core/linkify.py
--rw-rw-rw-   0        0        0      402 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_core/normalize.py
--rw-rw-rw-   0        0        0     3470 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_core/replacements.py
--rw-rw-rw-   0        0        0     7443 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_core/smartquotes.py
--rw-rw-rw-   0        0        0      570 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_core/state_core.py
--rw-rw-rw-   0        0        0     1172 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_core/text_join.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.086118 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/
--rw-rw-rw-   0        0        0      696 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/__init__.py
--rw-rw-rw-   0        0        0     2079 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/autolink.py
--rw-rw-rw-   0        0        0     2037 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/backticks.py
--rw-rw-rw-   0        0        0     4851 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/balance_pairs.py
--rw-rw-rw-   0        0        0     3123 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/emphasis.py
--rw-rw-rw-   0        0        0     1651 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/entity.py
--rw-rw-rw-   0        0        0     1658 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/escape.py
--rw-rw-rw-   0        0        0     1493 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/fragments_join.py
--rw-rw-rw-   0        0        0     1130 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/html_inline.py
--rw-rw-rw-   0        0        0     4135 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/image.py
--rw-rw-rw-   0        0        0     4318 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/link.py
--rw-rw-rw-   0        0        0     1704 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/linkify.py
--rw-rw-rw-   0        0        0     1296 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/newline.py
--rw-rw-rw-   0        0        0     5101 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/state_inline.py
--rw-rw-rw-   0        0        0     3214 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/strikethrough.py
--rw-rw-rw-   0        0        0      901 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/text.py
--rw-rw-rw-   0        0        0     6439 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/token.py
--rw-rw-rw-   0        0        0    11421 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/tree.py
--rw-rw-rw-   0        0        0     5365 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.087224 mylove-0.0.2/venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/
--rw-rw-rw-   0        0        0       58 2023-07-26 08:06:10.000000 mylove-0.0.2/venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/entry_points.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.092718 mylove-0.0.2/venv/Lib/site-packages/mdurl/
--rw-rw-rw-   0        0        0      547 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/mdurl/__init__.py
--rw-rw-rw-   0        0        0     3004 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/mdurl/_decode.py
--rw-rw-rw-   0        0        0     2602 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/mdurl/_encode.py
--rw-rw-rw-   0        0        0      626 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/mdurl/_format.py
--rw-rw-rw-   0        0        0    11374 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/mdurl/_parse.py
--rw-rw-rw-   0        0        0      284 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/mdurl/_url.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.096174 mylove-0.0.2/venv/Lib/site-packages/more_itertools/
--rw-rw-rw-   0        0        0      149 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/more_itertools/__init__.py
--rw-rw-rw-   0        0        0   139056 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/more_itertools/more.py
--rw-rw-rw-   0        0        0    26447 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/more_itertools/recipes.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.099460 mylove-0.0.2/venv/Lib/site-packages/pip/
--rw-rw-rw-   0        0        0      357 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pip/__init__.py
--rw-rw-rw-   0        0        0     1198 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pip/__main__.py
--rw-rw-rw-   0        0        0     1444 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pip/__pip-runner__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.112696 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/
--rw-rw-rw-   0        0        0      573 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/__init__.py
--rw-rw-rw-   0        0        0    10234 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/build_env.py
--rw-rw-rw-   0        0        0    10734 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cache.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.124078 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cli/
--rw-rw-rw-   0        0        0      132 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cli/__init__.py
--rw-rw-rw-   0        0        0     6676 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py
--rw-rw-rw-   0        0        0     7842 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cli/base_command.py
--rw-rw-rw-   0        0        0    29381 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py
--rw-rw-rw-   0        0        0      774 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cli/command_context.py
--rw-rw-rw-   0        0        0     2472 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cli/main.py
--rw-rw-rw-   0        0        0     4338 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cli/main_parser.py
--rw-rw-rw-   0        0        0    10817 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cli/parser.py
--rw-rw-rw-   0        0        0     1968 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py
--rw-rw-rw-   0        0        0    18172 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cli/req_command.py
--rw-rw-rw-   0        0        0     5118 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cli/spinners.py
--rw-rw-rw-   0        0        0      116 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cli/status_codes.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.140393 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/
--rw-rw-rw-   0        0        0     3882 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/__init__.py
--rw-rw-rw-   0        0        0     7582 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/cache.py
--rw-rw-rw-   0        0        0     1685 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/check.py
--rw-rw-rw-   0        0        0     4129 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/completion.py
--rw-rw-rw-   0        0        0     9815 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/configuration.py
--rw-rw-rw-   0        0        0     6573 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/debug.py
--rw-rw-rw-   0        0        0     5289 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/download.py
--rw-rw-rw-   0        0        0     2951 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/freeze.py
--rw-rw-rw-   0        0        0     1703 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/hash.py
--rw-rw-rw-   0        0        0     1132 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/help.py
--rw-rw-rw-   0        0        0     4762 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/index.py
--rw-rw-rw-   0        0        0     3374 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/inspect.py
--rw-rw-rw-   0        0        0    31726 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/install.py
--rw-rw-rw-   0        0        0    12343 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/list.py
--rw-rw-rw-   0        0        0     5697 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/search.py
--rw-rw-rw-   0        0        0     6129 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/show.py
--rw-rw-rw-   0        0        0     3680 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/uninstall.py
--rw-rw-rw-   0        0        0     7396 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/wheel.py
--rw-rw-rw-   0        0        0    13529 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/configuration.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.146150 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/distributions/
--rw-rw-rw-   0        0        0      858 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/distributions/__init__.py
--rw-rw-rw-   0        0        0     1221 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/distributions/base.py
--rw-rw-rw-   0        0        0      729 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/distributions/installed.py
--rw-rw-rw-   0        0        0     6494 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/distributions/sdist.py
--rw-rw-rw-   0        0        0     1164 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/distributions/wheel.py
--rw-rw-rw-   0        0        0    20942 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.149182 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/index/
--rw-rw-rw-   0        0        0       30 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/index/__init__.py
--rw-rw-rw-   0        0        0    16503 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/index/collector.py
--rw-rw-rw-   0        0        0    37596 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/index/package_finder.py
--rw-rw-rw-   0        0        0     6557 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/index/sources.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.152825 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/locations/
--rw-rw-rw-   0        0        0    17552 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/locations/__init__.py
--rw-rw-rw-   0        0        0     6302 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/locations/_distutils.py
--rw-rw-rw-   0        0        0     7867 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py
--rw-rw-rw-   0        0        0     2573 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/locations/base.py
--rw-rw-rw-   0        0        0      340 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/main.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.158219 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/metadata/
--rw-rw-rw-   0        0        0     4280 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/metadata/__init__.py
--rw-rw-rw-   0        0        0     2595 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/metadata/_json.py
--rw-rw-rw-   0        0        0    25277 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/metadata/base.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.163028 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/metadata/importlib/
--rw-rw-rw-   0        0        0      107 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-rw-rw-   0        0        0     1882 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-rw-rw-   0        0        0     8181 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-rw-rw-   0        0        0     7457 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-rw-rw-   0        0        0     9773 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.174802 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/
--rw-rw-rw-   0        0        0       63 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/__init__.py
--rw-rw-rw-   0        0        0      990 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/candidate.py
--rw-rw-rw-   0        0        0     5877 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/direct_url.py
--rw-rw-rw-   0        0        0     2520 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/format_control.py
--rw-rw-rw-   0        0        0     1030 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/index.py
--rw-rw-rw-   0        0        0     2617 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/installation_report.py
--rw-rw-rw-   0        0        0    18083 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/link.py
--rw-rw-rw-   0        0        0      738 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/scheme.py
--rw-rw-rw-   0        0        0     4644 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/search_scope.py
--rw-rw-rw-   0        0        0     1907 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py
--rw-rw-rw-   0        0        0     3858 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/target_python.py
--rw-rw-rw-   0        0        0     3600 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/wheel.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.181911 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/network/
--rw-rw-rw-   0        0        0       50 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/network/__init__.py
--rw-rw-rw-   0        0        0    12190 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/network/auth.py
--rw-rw-rw-   0        0        0     2145 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/network/cache.py
--rw-rw-rw-   0        0        0     6096 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/network/download.py
--rw-rw-rw-   0        0        0     7638 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py
--rw-rw-rw-   0        0        0    18443 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/network/session.py
--rw-rw-rw-   0        0        0     4073 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/network/utils.py
--rw-rw-rw-   0        0        0     1791 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.186575 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/
--rw-rw-rw-   0        0        0        0 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.193126 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/build/
--rw-rw-rw-   0        0        0        0 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/build/__init__.py
--rw-rw-rw-   0        0        0     4133 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-rw-rw-   0        0        0     1404 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py
--rw-rw-rw-   0        0        0     1456 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-rw-rw-   0        0        0     2198 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-rw-rw-   0        0        0     1063 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py
--rw-rw-rw-   0        0        0     1405 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-rw-rw-   0        0        0     3064 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-rw-rw-   0        0        0     5109 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/check.py
--rw-rw-rw-   0        0        0     9784 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/freeze.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.197307 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/install/
--rw-rw-rw-   0        0        0       51 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/install/__init__.py
--rw-rw-rw-   0        0        0     1354 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-rw-rw-   0        0        0     4105 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py
--rw-rw-rw-   0        0        0    27407 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py
--rw-rw-rw-   0        0        0    25091 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/prepare.py
--rw-rw-rw-   0        0        0     7074 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/pyproject.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.201364 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/req/
--rw-rw-rw-   0        0        0     2807 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/req/__init__.py
--rw-rw-rw-   0        0        0    16611 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/req/constructors.py
--rw-rw-rw-   0        0        0    17646 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/req/req_file.py
--rw-rw-rw-   0        0        0    35600 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/req/req_install.py
--rw-rw-rw-   0        0        0     2858 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/req/req_set.py
--rw-rw-rw-   0        0        0    24045 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.204039 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/
--rw-rw-rw-   0        0        0        0 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/__init__.py
--rw-rw-rw-   0        0        0      583 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/base.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.206369 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/legacy/
--rw-rw-rw-   0        0        0        0 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-rw-rw-   0        0        0    24129 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.215400 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/
--rw-rw-rw-   0        0        0        0 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-rw-rw-   0        0        0     5220 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-rw-rw-   0        0        0    18963 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-rw-rw-   0        0        0    27878 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-rw-rw-   0        0        0     5705 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-rw-rw-   0        0        0     9914 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-rw-rw-   0        0        0     2526 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-rw-rw-   0        0        0     5455 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-rw-rw-   0        0        0    11533 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-rw-rw-   0        0        0     8020 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/self_outdated_check.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.241383 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/
--rw-rw-rw-   0        0        0        0 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/__init__.py
--rw-rw-rw-   0        0        0     1015 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/_log.py
--rw-rw-rw-   0        0        0     1665 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/appdirs.py
--rw-rw-rw-   0        0        0     1884 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/compat.py
--rw-rw-rw-   0        0        0     5377 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-rw-rw-   0        0        0      242 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/datetime.py
--rw-rw-rw-   0        0        0     5764 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/deprecation.py
--rw-rw-rw-   0        0        0     3206 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-rw-rw-   0        0        0     1115 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py
--rw-rw-rw-   0        0        0     2203 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/egg_link.py
--rw-rw-rw-   0        0        0     1169 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/encoding.py
--rw-rw-rw-   0        0        0     3064 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py
--rw-rw-rw-   0        0        0     5122 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/filesystem.py
--rw-rw-rw-   0        0        0      716 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/filetypes.py
--rw-rw-rw-   0        0        0     3110 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/glibc.py
--rw-rw-rw-   0        0        0     4831 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/hashes.py
--rw-rw-rw-   0        0        0      795 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-rw-rw-   0        0        0    11632 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/logging.py
--rw-rw-rw-   0        0        0    21617 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/misc.py
--rw-rw-rw-   0        0        0     1193 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/models.py
--rw-rw-rw-   0        0        0     2108 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/packaging.py
--rw-rw-rw-   0        0        0     5662 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
--rw-rw-rw-   0        0        0     9197 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/subprocess.py
--rw-rw-rw-   0        0        0     7702 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
--rw-rw-rw-   0        0        0     8821 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/unpacking.py
--rw-rw-rw-   0        0        0     1759 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/urls.py
--rw-rw-rw-   0        0        0     3459 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py
--rw-rw-rw-   0        0        0     4549 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/wheel.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.247426 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/vcs/
--rw-rw-rw-   0        0        0      596 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/vcs/__init__.py
--rw-rw-rw-   0        0        0     3518 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
--rw-rw-rw-   0        0        0    18116 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/vcs/git.py
--rw-rw-rw-   0        0        0     5238 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
--rw-rw-rw-   0        0        0    11728 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/vcs/subversion.py
--rw-rw-rw-   0        0        0    22811 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-rw-rw-   0        0        0    13079 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_internal/wheel_builder.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.250456 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/
--rw-rw-rw-   0        0        0     4966 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.260778 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/
--rw-rw-rw-   0        0        0      465 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-rw-rw-   0        0        0     1379 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-rw-rw-   0        0        0     5033 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-rw-rw-   0        0        0     1535 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.264041 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/
--rw-rw-rw-   0        0        0      242 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-rw-rw-   0        0        0     5271 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-rw-rw-   0        0        0     1033 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-rw-rw-   0        0        0      778 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-rw-rw-   0        0        0    16416 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-rw-rw-   0        0        0     3946 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-rw-rw-   0        0        0     4154 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-rw-rw-   0        0        0     7105 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-rw-rw-   0        0        0      774 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.266138 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/certifi/
--rw-rw-rw-   0        0        0       94 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
--rw-rw-rw-   0        0        0      255 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
--rw-rw-rw-   0        0        0     4279 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/certifi/core.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.308684 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/
--rw-rw-rw-   0        0        0     3705 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
--rw-rw-rw-   0        0        0    31274 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
--rw-rw-rw-   0        0        0     1741 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
--rw-rw-rw-   0        0        0     9608 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-rw-rw-   0        0        0     3817 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-rw-rw-   0        0        0     4801 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.310677 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/cli/
--rw-rw-rw-   0        0        0        0 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-rw-rw-   0        0        0     2406 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-rw-rw-   0        0        0     3559 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-rw-rw-   0        0        0     1838 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-rw-rw-   0        0        0     1619 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/enums.py
--rw-rw-rw-   0        0        0     3864 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
--rw-rw-rw-   0        0        0    12021 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
--rw-rw-rw-   0        0        0     3676 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-rw-rw-   0        0        0    13566 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-rw-rw-   0        0        0     1731 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-rw-rw-   0        0        0    36913 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-rw-rw-   0        0        0     1731 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-rw-rw-   0        0        0    20735 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-rw-rw-   0        0        0     1737 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-rw-rw-   0        0        0    13919 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-rw-rw-   0        0        0    25796 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-rw-rw-   0        0        0    42498 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-rw-rw-   0        0        0     1730 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py
--rw-rw-rw-   0        0        0    26797 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-rw-rw-   0        0        0   104562 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-rw-rw-   0        0        0    98484 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-rw-rw-   0        0        0    98196 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-rw-rw-   0        0        0   101363 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-rw-rw-   0        0        0   128035 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-rw-rw-   0        0        0   102774 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-rw-rw-   0        0        0    95372 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-rw-rw-   0        0        0     5260 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-rw-rw-   0        0        0     3367 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-rw-rw-   0        0        0     2056 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-rw-rw-   0        0        0    30068 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.312670 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/metadata/
--rw-rw-rw-   0        0        0        0 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-rw-rw-   0        0        0    13280 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-rw-rw-   0        0        0     6199 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-rw-rw-   0        0        0     4129 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-rw-rw-   0        0        0     3749 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-rw-rw-   0        0        0    13288 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-rw-rw-   0        0        0     8289 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-rw-rw-   0        0        0     2709 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-rw-rw-   0        0        0      242 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/version.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.319162 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/colorama/
--rw-rw-rw-   0        0        0      239 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
--rw-rw-rw-   0        0        0    10830 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-rw-rw-   0        0        0     1915 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
--rw-rw-rw-   0        0        0     5404 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/colorama/win32.py
--rw-rw-rw-   0        0        0     6438 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.333658 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/
--rw-rw-rw-   0        0        0      581 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
--rw-rw-rw-   0        0        0    41259 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/compat.py
--rw-rw-rw-   0        0        0    51697 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/database.py
--rw-rw-rw-   0        0        0    20834 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/index.py
--rw-rw-rw-   0        0        0    51991 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/locators.py
--rw-rw-rw-   0        0        0    14811 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
--rw-rw-rw-   0        0        0     5058 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/markers.py
--rw-rw-rw-   0        0        0    39801 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
--rw-rw-rw-   0        0        0    10820 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/resources.py
--rw-rw-rw-   0        0        0    18102 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
--rw-rw-rw-   0        0        0    66262 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/util.py
--rw-rw-rw-   0        0        0    23513 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/version.py
--rw-rw-rw-   0        0        0    43898 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.336131 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distro/
--rw-rw-rw-   0        0        0      981 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distro/__init__.py
--rw-rw-rw-   0        0        0       64 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distro/__main__.py
--rw-rw-rw-   0        0        0    48841 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distro/distro.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.347159 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/idna/
--rw-rw-rw-   0        0        0      849 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/idna/__init__.py
--rw-rw-rw-   0        0        0     3374 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/idna/codec.py
--rw-rw-rw-   0        0        0      321 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/idna/compat.py
--rw-rw-rw-   0        0        0    12950 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/idna/core.py
--rw-rw-rw-   0        0        0    44375 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
--rw-rw-rw-   0        0        0     1881 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/idna/intranges.py
--rw-rw-rw-   0        0        0       21 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/idna/package_data.py
--rw-rw-rw-   0        0        0   206539 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.352872 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/
--rw-rw-rw-   0        0        0     1132 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
--rw-rw-rw-   0        0        0     1081 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-rw-rw-   0        0        0     6080 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py
--rw-rw-rw-   0        0        0    34557 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.366181 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/packaging/
--rw-rw-rw-   0        0        0      661 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
--rw-rw-rw-   0        0        0      497 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
--rw-rw-rw-   0        0        0    11488 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     4378 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-rw-rw-   0        0        0     1431 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
--rw-rw-rw-   0        0        0     8487 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/packaging/markers.py
--rw-rw-rw-   0        0        0     4676 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
--rw-rw-rw-   0        0        0    30110 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
--rw-rw-rw-   0        0        0    15699 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/packaging/tags.py
--rw-rw-rw-   0        0        0     4200 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/packaging/utils.py
--rw-rw-rw-   0        0        0    14665 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/packaging/version.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.378242 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pep517/
--rw-rw-rw-   0        0        0      130 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pep517/__init__.py
--rw-rw-rw-   0        0        0      138 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pep517/_compat.py
--rw-rw-rw-   0        0        0     3443 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pep517/build.py
--rw-rw-rw-   0        0        0     6083 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pep517/check.py
--rw-rw-rw-   0        0        0     3994 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pep517/colorlog.py
--rw-rw-rw-   0        0        0      607 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pep517/dirtools.py
--rw-rw-rw-   0        0        0     6081 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pep517/envbuild.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.379258 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pep517/in_process/
--rw-rw-rw-   0        0        0      872 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pep517/in_process/__init__.py
--rw-rw-rw-   0        0        0    10801 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pep517/in_process/_in_process.py
--rw-rw-rw-   0        0        0     2520 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pep517/meta.py
--rw-rw-rw-   0        0        0    12721 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pep517/wrappers.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.381314 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pkg_resources/
--rw-rw-rw-   0        0        0   108287 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-rw-rw-   0        0        0      562 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.390334 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/
--rw-rw-rw-   0        0        0    12831 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-rw-rw-   0        0        0     1176 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-rw-rw-   0        0        0     4068 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py
--rw-rw-rw-   0        0        0     4910 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py
--rw-rw-rw-   0        0        0     2655 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py
--rw-rw-rw-   0        0        0     6910 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py
--rw-rw-rw-   0        0        0       78 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/version.py
--rw-rw-rw-   0        0        0     6439 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.410991 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/
--rw-rw-rw-   0        0        0     2999 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py
--rw-rw-rw-   0        0        0      353 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/__main__.py
--rw-rw-rw-   0        0        0    23685 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py
--rw-rw-rw-   0        0        0     1697 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/console.py
--rw-rw-rw-   0        0        0     1938 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/filter.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.412423 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/filters/
--rw-rw-rw-   0        0        0    40386 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-rw-rw-   0        0        0     2917 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.429198 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/
--rw-rw-rw-   0        0        0     4810 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-rw-rw-   0        0        0     4104 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-rw-rw-   0        0        0     3314 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-rw-rw-   0        0        0     5086 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-rw-rw-   0        0        0    35441 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-rw-rw-   0        0        0    21938 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-rw-rw-   0        0        0     5871 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-rw-rw-   0        0        0    19351 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-rw-rw-   0        0        0     5073 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-rw-rw-   0        0        0     2212 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-rw-rw-   0        0        0     5014 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-rw-rw-   0        0        0     7335 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-rw-rw-   0        0        0     4674 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-rw-rw-   0        0        0    11753 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-rw-rw-   0        0        0    32005 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.431191 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/lexers/
--rw-rw-rw-   0        0        0    11174 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-rw-rw-   0        0        0    70232 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-rw-rw-   0        0        0    53376 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-rw-rw-   0        0        0      986 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py
--rw-rw-rw-   0        0        0     2591 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py
--rw-rw-rw-   0        0        0     3072 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py
--rw-rw-rw-   0        0        0     3092 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py
--rw-rw-rw-   0        0        0     4630 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-rw-rw-   0        0        0     6257 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/style.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.432697 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/styles/
--rw-rw-rw-   0        0        0     3419 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-rw-rw-   0        0        0     6184 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/token.py
--rw-rw-rw-   0        0        0    63187 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py
--rw-rw-rw-   0        0        0     9110 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/util.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.448094 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/
--rw-rw-rw-   0        0        0     9171 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-rw-rw-   0        0        0     6426 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py
--rw-rw-rw-   0        0        0    12936 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py
--rw-rw-rw-   0        0        0   213344 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.449118 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/
--rw-rw-rw-   0        0        0    23685 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-rw-rw-   0        0        0     9023 2023-07-26 07:30:19.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-rw-rw-   0        0        0    39129 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-rw-rw-   0        0        0    25341 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py
--rw-rw-rw-   0        0        0    13402 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py
--rw-rw-rw-   0        0        0    10787 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-rw-rw-   0        0        0     6805 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.469889 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/
--rw-rw-rw-   0        0        0     5178 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/__init__.py
--rw-rw-rw-   0        0        0      440 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/__version__.py
--rw-rw-rw-   0        0        0     1397 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-rw-rw-   0        0        0    21443 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/adapters.py
--rw-rw-rw-   0        0        0     6377 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/api.py
--rw-rw-rw-   0        0        0    10187 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/auth.py
--rw-rw-rw-   0        0        0      575 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/certs.py
--rw-rw-rw-   0        0        0     1286 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/compat.py
--rw-rw-rw-   0        0        0    18560 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/cookies.py
--rw-rw-rw-   0        0        0     3823 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
--rw-rw-rw-   0        0        0     3879 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/help.py
--rw-rw-rw-   0        0        0      733 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/hooks.py
--rw-rw-rw-   0        0        0    35287 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/models.py
--rw-rw-rw-   0        0        0      695 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/packages.py
--rw-rw-rw-   0        0        0    30180 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/sessions.py
--rw-rw-rw-   0        0        0     4235 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
--rw-rw-rw-   0        0        0     2912 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/structures.py
--rw-rw-rw-   0        0        0    33240 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.475990 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/resolvelib/
--rw-rw-rw-   0        0        0      537 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.477152 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/
--rw-rw-rw-   0        0        0        0 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-rw-rw-   0        0        0      156 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-rw-rw-   0        0        0     5872 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py
--rw-rw-rw-   0        0        0     1583 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-rw-rw-   0        0        0    17592 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-rw-rw-   0        0        0     4794 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.548097 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/
--rw-rw-rw-   0        0        0     5944 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/__init__.py
--rw-rw-rw-   0        0        0     8808 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/__main__.py
--rw-rw-rw-   0        0        0    10096 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-rw-rw-   0        0        0   140235 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-rw-rw-   0        0        0     1064 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-rw-rw-   0        0        0     2114 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py
--rw-rw-rw-   0        0        0      265 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_extension.py
--rw-rw-rw-   0        0        0     9695 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py
--rw-rw-rw-   0        0        0     3225 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py
--rw-rw-rw-   0        0        0     1236 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_loop.py
--rw-rw-rw-   0        0        0     7063 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py
--rw-rw-rw-   0        0        0      423 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_pick.py
--rw-rw-rw-   0        0        0     5472 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py
--rw-rw-rw-   0        0        0    19919 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py
--rw-rw-rw-   0        0        0      351 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_stack.py
--rw-rw-rw-   0        0        0      417 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_timer.py
--rw-rw-rw-   0        0        0    22820 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py
--rw-rw-rw-   0        0        0     1926 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_windows.py
--rw-rw-rw-   0        0        0     2783 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-rw-rw-   0        0        0     1840 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py
--rw-rw-rw-   0        0        0      890 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/abc.py
--rw-rw-rw-   0        0        0    10368 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/align.py
--rw-rw-rw-   0        0        0     6820 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/ansi.py
--rw-rw-rw-   0        0        0     3264 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/bar.py
--rw-rw-rw-   0        0        0     9864 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/box.py
--rw-rw-rw-   0        0        0     4503 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/cells.py
--rw-rw-rw-   0        0        0    17957 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/color.py
--rw-rw-rw-   0        0        0     1054 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py
--rw-rw-rw-   0        0        0     7131 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/columns.py
--rw-rw-rw-   0        0        0    95885 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/console.py
--rw-rw-rw-   0        0        0     1288 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/constrain.py
--rw-rw-rw-   0        0        0     5497 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/containers.py
--rw-rw-rw-   0        0        0     6630 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/control.py
--rw-rw-rw-   0        0        0     7954 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py
--rw-rw-rw-   0        0        0      972 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py
--rw-rw-rw-   0        0        0     2501 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/emoji.py
--rw-rw-rw-   0        0        0      642 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/errors.py
--rw-rw-rw-   0        0        0     1616 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py
--rw-rw-rw-   0        0        0     2507 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/filesize.py
--rw-rw-rw-   0        0        0     9585 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py
--rw-rw-rw-   0        0        0     5051 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/json.py
--rw-rw-rw-   0        0        0     3252 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py
--rw-rw-rw-   0        0        0    14074 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/layout.py
--rw-rw-rw-   0        0        0    14172 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/live.py
--rw-rw-rw-   0        0        0     3667 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/live_render.py
--rw-rw-rw-   0        0        0    11471 2023-07-26 07:30:20.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/logging.py
--rw-rw-rw-   0        0        0     8198 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/markup.py
--rw-rw-rw-   0        0        0     5305 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/measure.py
--rw-rw-rw-   0        0        0     4970 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/padding.py
--rw-rw-rw-   0        0        0      828 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/pager.py
--rw-rw-rw-   0        0        0     3396 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/palette.py
--rw-rw-rw-   0        0        0     8744 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/panel.py
--rw-rw-rw-   0        0        0    36576 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/pretty.py
--rw-rw-rw-   0        0        0    59746 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/progress.py
--rw-rw-rw-   0        0        0     8161 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py
--rw-rw-rw-   0        0        0    11303 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/prompt.py
--rw-rw-rw-   0        0        0     1391 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/protocol.py
--rw-rw-rw-   0        0        0      166 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/region.py
--rw-rw-rw-   0        0        0     4449 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/repr.py
--rw-rw-rw-   0        0        0     4773 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/rule.py
--rw-rw-rw-   0        0        0     2842 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/scope.py
--rw-rw-rw-   0        0        0     1591 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/screen.py
--rw-rw-rw-   0        0        0    24224 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/segment.py
--rw-rw-rw-   0        0        0     4374 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/spinner.py
--rw-rw-rw-   0        0        0     4425 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/status.py
--rw-rw-rw-   0        0        0    26240 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/style.py
--rw-rw-rw-   0        0        0     1258 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/styled.py
--rw-rw-rw-   0        0        0    34697 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/syntax.py
--rw-rw-rw-   0        0        0    39515 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/table.py
--rw-rw-rw-   0        0        0     3370 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-rw-rw-   0        0        0    44666 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/text.py
--rw-rw-rw-   0        0        0     3627 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/theme.py
--rw-rw-rw-   0        0        0      102 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/themes.py
--rw-rw-rw-   0        0        0    26060 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/traceback.py
--rw-rw-rw-   0        0        0     9169 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/tree.py
--rw-rw-rw-   0        0        0    34549 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/six.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.558245 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/
--rw-rw-rw-   0        0        0    18364 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py
--rw-rw-rw-   0        0        0     3314 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-rw-rw-   0        0        0     1944 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py
--rw-rw-rw-   0        0        0     1496 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/after.py
--rw-rw-rw-   0        0        0     1376 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/before.py
--rw-rw-rw-   0        0        0     1908 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-rw-rw-   0        0        0     1383 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py
--rw-rw-rw-   0        0        0     7550 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py
--rw-rw-rw-   0        0        0     2790 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py
--rw-rw-rw-   0        0        0     2145 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-rw-rw-   0        0        0     8011 2023-07-26 07:30:21.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.561330 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tomli/
--rw-rw-rw-   0        0        0      396 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tomli/__init__.py
--rw-rw-rw-   0        0        0    22633 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py
--rw-rw-rw-   0        0        0     2943 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tomli/_re.py
--rw-rw-rw-   0        0        0      254 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tomli/_types.py
--rw-rw-rw-   0        0        0    80114 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/typing_extensions.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.570077 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/
--rw-rw-rw-   0        0        0     3333 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
--rw-rw-rw-   0        0        0    10811 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
--rw-rw-rw-   0        0        0       64 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/_version.py
--rw-rw-rw-   0        0        0    20070 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
--rw-rw-rw-   0        0        0    39093 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.577412 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/
--rw-rw-rw-   0        0        0        0 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-rw-rw-   0        0        0      957 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.580401 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
--rw-rw-rw-   0        0        0        0 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-rw-rw-   0        0        0    17632 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-rw-rw-   0        0        0    13922 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-rw-rw-   0        0        0    11034 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-rw-rw-   0        0        0     4538 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-rw-rw-   0        0        0    17182 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-rw-rw-   0        0        0    34448 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-rw-rw-   0        0        0     7097 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-rw-rw-   0        0        0     8217 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-rw-rw-   0        0        0     8579 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
--rw-rw-rw-   0        0        0     2440 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.581398 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/
--rw-rw-rw-   0        0        0        0 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.583917 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/
--rw-rw-rw-   0        0        0        0 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-rw-rw-   0        0        0     1417 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-rw-rw-   0        0        0    34665 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-rw-rw-   0        0        0    19786 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-rw-rw-   0        0        0     5985 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/request.py
--rw-rw-rw-   0        0        0    30109 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/response.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.597301 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/
--rw-rw-rw-   0        0        0     1155 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-rw-rw-   0        0        0     4901 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-rw-rw-   0        0        0     1605 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-rw-rw-   0        0        0      498 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-rw-rw-   0        0        0     3997 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
--rw-rw-rw-   0        0        0     3510 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
--rw-rw-rw-   0        0        0    22001 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-rw-rw-   0        0        0    17177 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-rw-rw-   0        0        0     5758 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-rw-rw-   0        0        0     6895 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-rw-rw-   0        0        0    10003 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-rw-rw-   0        0        0    14287 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
--rw-rw-rw-   0        0        0     5403 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-rw-rw-   0        0        0      469 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/vendor.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.601898 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/
--rw-rw-rw-   0        0        0    10579 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
--rw-rw-rw-   0        0        0     8979 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
--rw-rw-rw-   0        0        0     1305 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-rw-rw-   0        0        0     6563 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
--rw-rw-rw-   0        0        0     4307 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.101525 mylove-0.0.2/venv/Lib/site-packages/pip-22.3.1.dist-info/
--rw-rw-rw-   0        0        0     1093 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip-22.3.1.dist-info/LICENSE.txt
--rw-rw-rw-   0        0        0      125 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip-22.3.1.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Lib/site-packages/pip-22.3.1.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.602894 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/
--rw-rw-rw-   0        0        0   108568 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.605997 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/
--rw-rw-rw-   0        0        0        0 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
--rw-rw-rw-   0        0        0    24701 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.612711 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/
--rw-rw-rw-   0        0        0      506 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
--rw-rw-rw-   0        0        0     4504 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
--rw-rw-rw-   0        0        0     2741 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
--rw-rw-rw-   0        0        0     2706 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
--rw-rw-rw-   0        0        0      884 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
--rw-rw-rw-   0        0        0     3494 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
--rw-rw-rw-   0        0        0     3886 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
--rw-rw-rw-   0        0        0     3566 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
--rw-rw-rw-   0        0        0     2836 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.614734 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/
--rw-rw-rw-   0        0        0        0 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/__init__.py
--rw-rw-rw-   0        0        0     5420 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py
--rw-rw-rw-   0        0        0    13515 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.615904 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/
--rw-rw-rw-   0        0        0    15526 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.618949 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/
--rw-rw-rw-   0        0        0       83 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
--rw-rw-rw-   0        0        0   132569 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py
--rw-rw-rw-   0        0        0    18410 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.629119 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/
--rw-rw-rw-   0        0        0      661 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-rw-rw-   0        0        0      497 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-rw-rw-   0        0        0    11488 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     4378 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-rw-rw-   0        0        0     1431 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-rw-rw-   0        0        0     8496 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-rw-rw-   0        0        0     4706 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-rw-rw-   0        0        0    30110 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-rw-rw-   0        0        0    15699 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-rw-rw-   0        0        0     4200 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-rw-rw-   0        0        0    14665 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.637859 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/
--rw-rw-rw-   0        0        0     9159 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
--rw-rw-rw-   0        0        0     6426 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py
--rw-rw-rw-   0        0        0    12936 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/common.py
--rw-rw-rw-   0        0        0   213310 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/core.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.638856 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/
--rw-rw-rw-   0        0        0    23668 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
--rw-rw-rw-   0        0        0     9023 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
--rw-rw-rw-   0        0        0    39129 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
--rw-rw-rw-   0        0        0    25341 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/results.py
--rw-rw-rw-   0        0        0    13402 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py
--rw-rw-rw-   0        0        0    10787 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
--rw-rw-rw-   0        0        0     6805 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/util.py
--rw-rw-rw-   0        0        0     8425 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/zipp.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.639852 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/extern/
--rw-rw-rw-   0        0        0     2426 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/pkg_resources/extern/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.648032 mylove-0.0.2/venv/Lib/site-packages/pkginfo/
--rw-rw-rw-   0        0        0      266 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/pkginfo/__init__.py
--rw-rw-rw-   0        0        0     1198 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/pkginfo/bdist.py
--rw-rw-rw-   0        0        0     7415 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/pkginfo/commandline.py
--rw-rw-rw-   0        0        0     1577 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/pkginfo/develop.py
--rw-rw-rw-   0        0        0     4627 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/pkginfo/distribution.py
--rw-rw-rw-   0        0        0      518 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/pkginfo/index.py
--rw-rw-rw-   0        0        0     2492 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/pkginfo/installed.py
--rw-rw-rw-   0        0        0     2347 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/pkginfo/sdist.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.661633 mylove-0.0.2/venv/Lib/site-packages/pkginfo/tests/
--rw-rw-rw-   0        0        0     1342 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/pkginfo/tests/__init__.py
--rw-rw-rw-   0        0        0     2279 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/pkginfo/tests/test_bdist.py
--rw-rw-rw-   0        0        0    11722 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/pkginfo/tests/test_commandline.py
--rw-rw-rw-   0        0        0      831 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/pkginfo/tests/test_develop.py
--rw-rw-rw-   0        0        0    19377 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/pkginfo/tests/test_distribution.py
--rw-rw-rw-   0        0        0     2636 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/pkginfo/tests/test_index.py
--rw-rw-rw-   0        0        0     5460 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/pkginfo/tests/test_installed.py
--rw-rw-rw-   0        0        0     5481 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/pkginfo/tests/test_sdist.py
--rw-rw-rw-   0        0        0     6835 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/pkginfo/tests/test_utils.py
--rw-rw-rw-   0        0        0     4443 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/pkginfo/tests/test_wheel.py
--rw-rw-rw-   0        0        0     1786 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/pkginfo/utils.py
--rw-rw-rw-   0        0        0     1586 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/pkginfo/wheel.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.651071 mylove-0.0.2/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/
--rw-rw-rw-   0        0        0     1084 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/LICENSE.txt
--rw-rw-rw-   0        0        0       54 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-07-26 08:06:05.000000 mylove-0.0.2/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.675911 mylove-0.0.2/venv/Lib/site-packages/pygments/
--rw-rw-rw-   0        0        0     2959 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/__init__.py
--rw-rw-rw-   0        0        0      348 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/__main__.py
--rw-rw-rw-   0        0        0    23530 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/cmdline.py
--rw-rw-rw-   0        0        0     1697 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/console.py
--rw-rw-rw-   0        0        0     1938 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/filter.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.676914 mylove-0.0.2/venv/Lib/site-packages/pygments/filters/
--rw-rw-rw-   0        0        0    40338 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/filters/__init__.py
--rw-rw-rw-   0        0        0     4154 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/formatter.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.691301 mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/
--rw-rw-rw-   0        0        0     5388 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/__init__.py
--rw-rw-rw-   0        0        0     4176 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/_mapping.py
--rw-rw-rw-   0        0        0     3290 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/bbcode.py
--rw-rw-rw-   0        0        0     5070 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/groff.py
--rw-rw-rw-   0        0        0    35574 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/html.py
--rw-rw-rw-   0        0        0    21914 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/img.py
--rw-rw-rw-   0        0        0     4945 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/irc.py
--rw-rw-rw-   0        0        0    19303 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/latex.py
--rw-rw-rw-   0        0        0     5025 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/other.py
--rw-rw-rw-   0        0        0     2200 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/pangomarkup.py
--rw-rw-rw-   0        0        0     4990 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/rtf.py
--rw-rw-rw-   0        0        0     7299 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/svg.py
--rw-rw-rw-   0        0        0     4626 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/terminal.py
--rw-rw-rw-   0        0        0    11717 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/terminal256.py
--rw-rw-rw-   0        0        0    34541 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexer.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:09.964442 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/
--rw-rw-rw-   0        0        0    12082 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/__init__.py
--rw-rw-rw-   0        0        0     1543 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_ada_builtins.py
--rw-rw-rw-   0        0        0    27287 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_asy_builtins.py
--rw-rw-rw-   0        0        0    13994 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_cl_builtins.py
--rw-rw-rw-   0        0        0   105182 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_cocoa_builtins.py
--rw-rw-rw-   0        0        0    18414 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_csound_builtins.py
--rw-rw-rw-   0        0        0    12446 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_css_builtins.py
--rw-rw-rw-   0        0        0    11883 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_julia_builtins.py
--rw-rw-rw-   0        0        0   134510 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_lasso_builtins.py
--rw-rw-rw-   0        0        0   108094 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_lilypond_builtins.py
--rw-rw-rw-   0        0        0     8116 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_lua_builtins.py
--rw-rw-rw-   0        0        0    65633 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_mapping.py
--rw-rw-rw-   0        0        0    24713 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_mql_builtins.py
--rw-rw-rw-   0        0        0    25842 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_mysql_builtins.py
--rw-rw-rw-   0        0        0    49398 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_openedge_builtins.py
--rw-rw-rw-   0        0        0   107930 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_php_builtins.py
--rw-rw-rw-   0        0        0    13355 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_postgres_builtins.py
--rw-rw-rw-   0        0        0    12595 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_qlik_builtins.py
--rw-rw-rw-   0        0        0    32564 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_scheme_builtins.py
--rw-rw-rw-   0        0        0    52413 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_scilab_builtins.py
--rw-rw-rw-   0        0        0    26781 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_sourcemod_builtins.py
--rw-rw-rw-   0        0        0    13445 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_stan_builtins.py
--rw-rw-rw-   0        0        0    27227 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_stata_builtins.py
--rw-rw-rw-   0        0        0    15460 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_tsql_builtins.py
--rw-rw-rw-   0        0        0     1658 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_usd_builtins.py
--rw-rw-rw-   0        0        0     4225 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_vbscript_builtins.py
--rw-rw-rw-   0        0        0    57066 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_vim_builtins.py
--rw-rw-rw-   0        0        0    11676 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/actionscript.py
--rw-rw-rw-   0        0        0     5320 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/ada.py
--rw-rw-rw-   0        0        0      876 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/agile.py
--rw-rw-rw-   0        0        0     9873 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/algebra.py
--rw-rw-rw-   0        0        0     2606 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/ambient.py
--rw-rw-rw-   0        0        0     1670 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/amdgpu.py
--rw-rw-rw-   0        0        0     4177 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/ampl.py
--rw-rw-rw-   0        0        0    30766 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/apdlexer.py
--rw-rw-rw-   0        0        0     3405 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/apl.py
--rw-rw-rw-   0        0        0    11469 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/archetype.py
--rw-rw-rw-   0        0        0     3565 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/arrow.py
--rw-rw-rw-   0        0        0    11417 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/arturo.py
--rw-rw-rw-   0        0        0     1621 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/asc.py
--rw-rw-rw-   0        0        0    41243 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/asm.py
--rw-rw-rw-   0        0        0    19815 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/automation.py
--rw-rw-rw-   0        0        0     3021 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/bare.py
--rw-rw-rw-   0        0        0    27923 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/basic.py
--rw-rw-rw-   0        0        0     1652 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/bdd.py
--rw-rw-rw-   0        0        0     3211 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/berry.py
--rw-rw-rw-   0        0        0     4723 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/bibtex.py
--rw-rw-rw-   0        0        0     3915 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/boa.py
--rw-rw-rw-   0        0        0    28112 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/business.py
--rw-rw-rw-   0        0        0    17791 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/c_cpp.py
--rw-rw-rw-   0        0        0    29206 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/c_like.py
--rw-rw-rw-   0        0        0     2175 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/capnproto.py
--rw-rw-rw-   0        0        0     3231 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/carbon.py
--rw-rw-rw-   0        0        0     5182 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/cddl.py
--rw-rw-rw-   0        0        0     5157 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/chapel.py
--rw-rw-rw-   0        0        0     6395 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/clean.py
--rw-rw-rw-   0        0        0     3156 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/comal.py
--rw-rw-rw-   0        0        0     1407 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/compiled.py
--rw-rw-rw-   0        0        0    42338 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/configs.py
--rw-rw-rw-   0        0        0     4148 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/console.py
--rw-rw-rw-   0        0        0     1390 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/cplint.py
--rw-rw-rw-   0        0        0    15756 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/crystal.py
--rw-rw-rw-   0        0        0    16994 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/csound.py
--rw-rw-rw-   0        0        0    25322 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/css.py
--rw-rw-rw-   0        0        0     9875 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/d.py
--rw-rw-rw-   0        0        0     4607 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/dalvik.py
--rw-rw-rw-   0        0        0    26940 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/data.py
--rw-rw-rw-   0        0        0     8099 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/dax.py
--rw-rw-rw-   0        0        0     4020 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/devicetree.py
--rw-rw-rw-   0        0        0     5278 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/diff.py
--rw-rw-rw-   0        0        0    37623 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/dotnet.py
--rw-rw-rw-   0        0        0    36774 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/dsls.py
--rw-rw-rw-   0        0        0    10380 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/dylan.py
--rw-rw-rw-   0        0        0     6372 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/ecl.py
--rw-rw-rw-   0        0        0     2690 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/eiffel.py
--rw-rw-rw-   0        0        0     3152 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/elm.py
--rw-rw-rw-   0        0        0     6370 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/elpi.py
--rw-rw-rw-   0        0        0     4742 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/email.py
--rw-rw-rw-   0        0        0    19170 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/erlang.py
--rw-rw-rw-   0        0        0    10396 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/esoteric.py
--rw-rw-rw-   0        0        0     3273 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/ezhil.py
--rw-rw-rw-   0        0        0    19531 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/factor.py
--rw-rw-rw-   0        0        0    10197 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/fantom.py
--rw-rw-rw-   0        0        0     9646 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/felix.py
--rw-rw-rw-   0        0        0     1621 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/fift.py
--rw-rw-rw-   0        0        0     2668 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/floscript.py
--rw-rw-rw-   0        0        0     7194 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/forth.py
--rw-rw-rw-   0        0        0    10336 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/fortran.py
--rw-rw-rw-   0        0        0    26212 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/foxpro.py
--rw-rw-rw-   0        0        0    26914 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/freefem.py
--rw-rw-rw-   0        0        0     3622 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/func.py
--rw-rw-rw-   0        0        0      674 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/functional.py
--rw-rw-rw-   0        0        0     3732 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/futhark.py
--rw-rw-rw-   0        0        0      826 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/gcodelexer.py
--rw-rw-rw-   0        0        0     7543 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/gdscript.py
--rw-rw-rw-   0        0        0     3761 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/go.py
--rw-rw-rw-   0        0        0     7980 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/grammar_notation.py
--rw-rw-rw-   0        0        0     3861 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/graph.py
--rw-rw-rw-   0        0        0    39026 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/graphics.py
--rw-rw-rw-   0        0        0     1935 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/graphviz.py
--rw-rw-rw-   0        0        0     3991 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/gsql.py
--rw-rw-rw-   0        0        0    32898 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/haskell.py
--rw-rw-rw-   0        0        0    30976 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/haxe.py
--rw-rw-rw-   0        0        0    22520 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/hdl.py
--rw-rw-rw-   0        0        0     3603 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/hexdump.py
--rw-rw-rw-   0        0        0    19879 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/html.py
--rw-rw-rw-   0        0        0    15450 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/idl.py
--rw-rw-rw-   0        0        0    30631 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/igor.py
--rw-rw-rw-   0        0        0     3136 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/inferno.py
--rw-rw-rw-   0        0        0    13178 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/installers.py
--rw-rw-rw-   0        0        0    57119 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/int_fiction.py
--rw-rw-rw-   0        0        0     1906 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/iolang.py
--rw-rw-rw-   0        0        0     4854 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/j.py
--rw-rw-rw-   0        0        0    62859 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/javascript.py
--rw-rw-rw-   0        0        0     2059 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/jmespath.py
--rw-rw-rw-   0        0        0     3701 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/jslt.py
--rw-rw-rw-   0        0        0     5635 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/jsonnet.py
--rw-rw-rw-   0        0        0    11646 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/julia.py
--rw-rw-rw-   0        0        0    72929 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/jvm.py
--rw-rw-rw-   0        0        0    11406 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/kuin.py
--rw-rw-rw-   0        0        0     9753 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/lilypond.py
--rw-rw-rw-   0        0        0   144039 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/lisp.py
--rw-rw-rw-   0        0        0    31914 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/macaulay2.py
--rw-rw-rw-   0        0        0     7618 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/make.py
--rw-rw-rw-   0        0        0    58129 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/markup.py
--rw-rw-rw-   0        0        0      676 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/math.py
--rw-rw-rw-   0        0        0   132852 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/matlab.py
--rw-rw-rw-   0        0        0     2716 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/maxima.py
--rw-rw-rw-   0        0        0     4337 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/meson.py
--rw-rw-rw-   0        0        0     7538 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/mime.py
--rw-rw-rw-   0        0        0    13846 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/minecraft.py
--rw-rw-rw-   0        0        0     4604 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/mips.py
--rw-rw-rw-   0        0        0    35324 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/ml.py
--rw-rw-rw-   0        0        0    13524 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/modeling.py
--rw-rw-rw-   0        0        0    53073 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/modula2.py
--rw-rw-rw-   0        0        0     6290 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/monte.py
--rw-rw-rw-   0        0        0     9187 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/mosel.py
--rw-rw-rw-   0        0        0    63962 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/ncl.py
--rw-rw-rw-   0        0        0     6416 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/nimrod.py
--rw-rw-rw-   0        0        0     2726 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/nit.py
--rw-rw-rw-   0        0        0     4015 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/nix.py
--rw-rw-rw-   0        0        0     4169 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/oberon.py
--rw-rw-rw-   0        0        0    22961 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/objective.py
--rw-rw-rw-   0        0        0     2982 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/ooc.py
--rw-rw-rw-   0        0        0     1744 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/other.py
--rw-rw-rw-   0        0        0     2720 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/parasail.py
--rw-rw-rw-   0        0        0    25904 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/parsers.py
--rw-rw-rw-   0        0        0    30880 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/pascal.py
--rw-rw-rw-   0        0        0     8146 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/pawn.py
--rw-rw-rw-   0        0        0    39170 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/perl.py
--rw-rw-rw-   0        0        0    23252 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/phix.py
--rw-rw-rw-   0        0        0    13040 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/php.py
--rw-rw-rw-   0        0        0     1975 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/pointless.py
--rw-rw-rw-   0        0        0     3244 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/pony.py
--rw-rw-rw-   0        0        0    12677 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/praat.py
--rw-rw-rw-   0        0        0     1156 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/procfile.py
--rw-rw-rw-   0        0        0    12351 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/prolog.py
--rw-rw-rw-   0        0        0     4715 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/promql.py
--rw-rw-rw-   0        0        0    53376 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/python.py
--rw-rw-rw-   0        0        0     6932 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/q.py
--rw-rw-rw-   0        0        0     3665 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/qlik.py
--rw-rw-rw-   0        0        0     6072 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/qvt.py
--rw-rw-rw-   0        0        0     6185 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/r.py
--rw-rw-rw-   0        0        0    15790 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/rdf.py
--rw-rw-rw-   0        0        0    18248 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/rebol.py
--rw-rw-rw-   0        0        0     2902 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/resource.py
--rw-rw-rw-   0        0        0     5056 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/ride.py
--rw-rw-rw-   0        0        0     1128 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/rita.py
--rw-rw-rw-   0        0        0     1973 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/rnc.py
--rw-rw-rw-   0        0        0     1962 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/roboconf.py
--rw-rw-rw-   0        0        0    18449 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/robotframework.py
--rw-rw-rw-   0        0        0    22775 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/ruby.py
--rw-rw-rw-   0        0        0     8216 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/rust.py
--rw-rw-rw-   0        0        0     9400 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/sas.py
--rw-rw-rw-   0        0        0     4645 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/savi.py
--rw-rw-rw-   0        0        0     2239 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/scdoc.py
--rw-rw-rw-   0        0        0    70014 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/scripting.py
--rw-rw-rw-   0        0        0     1986 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/sgf.py
--rw-rw-rw-   0        0        0    36466 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/shell.py
--rw-rw-rw-   0        0        0     2441 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/sieve.py
--rw-rw-rw-   0        0        0     8482 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/slash.py
--rw-rw-rw-   0        0        0     7206 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/smalltalk.py
--rw-rw-rw-   0        0        0     2660 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/smithy.py
--rw-rw-rw-   0        0        0     2773 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/smv.py
--rw-rw-rw-   0        0        0     2732 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/snobol.py
--rw-rw-rw-   0        0        0     3127 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/solidity.py
--rw-rw-rw-   0        0        0     3330 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/sophia.py
--rw-rw-rw-   0        0        0     3414 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/special.py
--rw-rw-rw-   0        0        0     2733 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/spice.py
--rw-rw-rw-   0        0        0    42086 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/sql.py
--rw-rw-rw-   0        0        0     1693 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/srcinfo.py
--rw-rw-rw-   0        0        0     6416 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/stata.py
--rw-rw-rw-   0        0        0     3698 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/supercollider.py
--rw-rw-rw-   0        0        0     2639 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/tal.py
--rw-rw-rw-   0        0        0     5513 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/tcl.py
--rw-rw-rw-   0        0        0     3523 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/teal.py
--rw-rw-rw-   0        0        0    72610 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/templates.py
--rw-rw-rw-   0        0        0     9719 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/teraterm.py
--rw-rw-rw-   0        0        0    10767 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/testing.py
--rw-rw-rw-   0        0        0     1029 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/text.py
--rw-rw-rw-   0        0        0     7609 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/textedit.py
--rw-rw-rw-   0        0        0    15192 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/textfmts.py
--rw-rw-rw-   0        0        0    20157 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/theorem.py
--rw-rw-rw-   0        0        0     4228 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/thingsdb.py
--rw-rw-rw-   0        0        0     1377 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/tlb.py
--rw-rw-rw-   0        0        0    10457 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/tnt.py
--rw-rw-rw-   0        0        0     1474 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/trafficscript.py
--rw-rw-rw-   0        0        0     8207 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/typoscript.py
--rw-rw-rw-   0        0        0     8956 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/ul4.py
--rw-rw-rw-   0        0        0    18512 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/unicon.py
--rw-rw-rw-   0        0        0     6037 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/urbi.py
--rw-rw-rw-   0        0        0     3513 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/usd.py
--rw-rw-rw-   0        0        0     7273 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/varnish.py
--rw-rw-rw-   0        0        0     3885 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/verification.py
--rw-rw-rw-   0        0        0      894 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/web.py
--rw-rw-rw-   0        0        0     5699 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/webassembly.py
--rw-rw-rw-   0        0        0    10517 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/webidl.py
--rw-rw-rw-   0        0        0    40549 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/webmisc.py
--rw-rw-rw-   0        0        0    11920 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/wgsl.py
--rw-rw-rw-   0        0        0     4018 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/whiley.py
--rw-rw-rw-   0        0        0     4021 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/wowtoc.py
--rw-rw-rw-   0        0        0     3239 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/wren.py
--rw-rw-rw-   0        0        0     1920 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/x10.py
--rw-rw-rw-   0        0        0      902 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/xorg.py
--rw-rw-rw-   0        0        0     4500 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/yang.py
--rw-rw-rw-   0        0        0     3953 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/zig.py
--rw-rw-rw-   0        0        0      986 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/modeline.py
--rw-rw-rw-   0        0        0     2579 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/plugin.py
--rw-rw-rw-   0        0        0     3072 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/regexopt.py
--rw-rw-rw-   0        0        0     3092 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/scanner.py
--rw-rw-rw-   0        0        0     6816 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/sphinxext.py
--rw-rw-rw-   0        0        0     6245 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/style.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.016960 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/
--rw-rw-rw-   0        0        0     3676 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/__init__.py
--rw-rw-rw-   0        0        0      705 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/abap.py
--rw-rw-rw-   0        0        0     2216 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/algol.py
--rw-rw-rw-   0        0        0     2231 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/algol_nu.py
--rw-rw-rw-   0        0        0     4443 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/arduino.py
--rw-rw-rw-   0        0        0     2096 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/autumn.py
--rw-rw-rw-   0        0        0     1514 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/borland.py
--rw-rw-rw-   0        0        0     1308 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/bw.py
--rw-rw-rw-   0        0        0     2730 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/colorful.py
--rw-rw-rw-   0        0        0     2488 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/default.py
--rw-rw-rw-   0        0        0     3314 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/dracula.py
--rw-rw-rw-   0        0        0     2439 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/emacs.py
--rw-rw-rw-   0        0        0     2502 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/friendly.py
--rw-rw-rw-   0        0        0     2707 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/friendly_grayscale.py
--rw-rw-rw-   0        0        0     1274 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/fruity.py
--rw-rw-rw-   0        0        0     3481 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/gh_dark.py
--rw-rw-rw-   0        0        0     3230 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/gruvbox.py
--rw-rw-rw-   0        0        0      692 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/igor.py
--rw-rw-rw-   0        0        0     2302 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/inkpot.py
--rw-rw-rw-   0        0        0     2016 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/lilypond.py
--rw-rw-rw-   0        0        0     3117 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/lovelace.py
--rw-rw-rw-   0        0        0     2350 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/manni.py
--rw-rw-rw-   0        0        0     4083 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/material.py
--rw-rw-rw-   0        0        0     5063 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/monokai.py
--rw-rw-rw-   0        0        0     2703 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/murphy.py
--rw-rw-rw-   0        0        0     1948 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/native.py
--rw-rw-rw-   0        0        0     5244 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/nord.py
--rw-rw-rw-   0        0        0     1664 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/onedark.py
--rw-rw-rw-   0        0        0     5526 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/paraiso_dark.py
--rw-rw-rw-   0        0        0     5530 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/paraiso_light.py
--rw-rw-rw-   0        0        0     2425 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/pastie.py
--rw-rw-rw-   0        0        0     2128 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/perldoc.py
--rw-rw-rw-   0        0        0     2432 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/rainbow_dash.py
--rw-rw-rw-   0        0        0      874 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/rrt.py
--rw-rw-rw-   0        0        0     1393 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/sas.py
--rw-rw-rw-   0        0        0     4078 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/solarized.py
--rw-rw-rw-   0        0        0      770 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/staroffice.py
--rw-rw-rw-   0        0        0     1198 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/stata_dark.py
--rw-rw-rw-   0        0        0     1227 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/stata_light.py
--rw-rw-rw-   0        0        0     7039 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/tango.py
--rw-rw-rw-   0        0        0     1885 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/trac.py
--rw-rw-rw-   0        0        0     1922 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/vim.py
--rw-rw-rw-   0        0        0     1026 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/vs.py
--rw-rw-rw-   0        0        0     1453 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/xcode.py
--rw-rw-rw-   0        0        0     2148 2023-07-26 08:05:58.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/styles/zenburn.py
--rw-rw-rw-   0        0        0     6184 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/token.py
--rw-rw-rw-   0        0        0    63223 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/unistring.py
--rw-rw-rw-   0        0        0    10230 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pygments/util.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.019949 mylove-0.0.2/venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/
--rw-rw-rw-   0        0        0     1616 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/LICENSE.txt
--rw-rw-rw-   0        0        0       12 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.028965 mylove-0.0.2/venv/Lib/site-packages/readme_renderer/
--rw-rw-rw-   0        0        0     1119 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/readme_renderer/__about__.py
--rw-rw-rw-   0        0        0      573 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/readme_renderer/__init__.py
--rw-rw-rw-   0        0        0     2622 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/readme_renderer/__main__.py
--rw-rw-rw-   0        0        0     4290 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/readme_renderer/clean.py
--rw-rw-rw-   0        0        0     3595 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/readme_renderer/markdown.py
--rw-rw-rw-   0        0        0     4460 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/readme_renderer/rst.py
--rw-rw-rw-   0        0        0      823 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/readme_renderer/txt.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.030957 mylove-0.0.2/venv/Lib/site-packages/readme_renderer-40.0.dist-info/
--rw-rw-rw-   0        0        0       16 2023-07-26 08:06:14.000000 mylove-0.0.2/venv/Lib/site-packages/readme_renderer-40.0.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.049950 mylove-0.0.2/venv/Lib/site-packages/requests/
--rw-rw-rw-   0        0        0     4963 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/requests/__init__.py
--rw-rw-rw-   0        0        0      435 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/requests/__version__.py
--rw-rw-rw-   0        0        0     1495 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/requests/_internal_utils.py
--rw-rw-rw-   0        0        0    19553 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/requests/adapters.py
--rw-rw-rw-   0        0        0     6449 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/requests/api.py
--rw-rw-rw-   0        0        0    10187 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/requests/auth.py
--rw-rw-rw-   0        0        0      429 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/requests/certs.py
--rw-rw-rw-   0        0        0     1451 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/requests/compat.py
--rw-rw-rw-   0        0        0    18560 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/requests/cookies.py
--rw-rw-rw-   0        0        0     3811 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/requests/exceptions.py
--rw-rw-rw-   0        0        0     3875 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/requests/help.py
--rw-rw-rw-   0        0        0      733 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/requests/hooks.py
--rw-rw-rw-   0        0        0    35223 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/requests/models.py
--rw-rw-rw-   0        0        0      957 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/requests/packages.py
--rw-rw-rw-   0        0        0    30373 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/requests/sessions.py
--rw-rw-rw-   0        0        0     4235 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/requests/status_codes.py
--rw-rw-rw-   0        0        0     2912 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/requests/structures.py
--rw-rw-rw-   0        0        0    33448 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/requests/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.050947 mylove-0.0.2/venv/Lib/site-packages/requests-2.31.0.dist-info/
--rw-rw-rw-   0        0        0        9 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/requests-2.31.0.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.055448 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/
--rw-rw-rw-   0        0        0     1188 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/__init__.py
--rw-rw-rw-   0        0        0     9260 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/_compat.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.064948 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/
--rw-rw-rw-   0        0        0      370 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/__init__.py
--rw-rw-rw-   0        0        0     7539 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/appengine.py
--rw-rw-rw-   0        0        0     1404 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/fingerprint.py
--rw-rw-rw-   0        0        0     1396 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/host_header_ssl.py
--rw-rw-rw-   0        0        0     4789 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/socket_options.py
--rw-rw-rw-   0        0        0     2608 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/source.py
--rw-rw-rw-   0        0        0     2399 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/ssl.py
--rw-rw-rw-   0        0        0     7854 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/x509.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.069935 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/auth/
--rw-rw-rw-   0        0        0        0 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/auth/__init__.py
--rw-rw-rw-   0        0        0      910 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/auth/_digest_auth_compat.py
--rw-rw-rw-   0        0        0     4944 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/auth/guess.py
--rw-rw-rw-   0        0        0     4407 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/auth/handler.py
--rw-rw-rw-   0        0        0     3706 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/auth/http_proxy_digest.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.073433 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/cookies/
--rw-rw-rw-   0        0        0        0 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/cookies/__init__.py
--rw-rw-rw-   0        0        0      213 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/cookies/forgetful.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.076433 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/downloadutils/
--rw-rw-rw-   0        0        0        0 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/downloadutils/__init__.py
--rw-rw-rw-   0        0        0     6024 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/downloadutils/stream.py
--rw-rw-rw-   0        0        0     4365 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/downloadutils/tee.py
--rw-rw-rw-   0        0        0      695 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.079422 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/multipart/
--rw-rw-rw-   0        0        0      854 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/multipart/__init__.py
--rw-rw-rw-   0        0        0     4861 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/multipart/decoder.py
--rw-rw-rw-   0        0        0    20769 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/multipart/encoder.py
--rw-rw-rw-   0        0        0     3102 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/sessions.py
--rw-rw-rw-   0        0        0     4044 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/streaming_iterator.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.082922 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/threaded/
--rw-rw-rw-   0        0        0     3213 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/threaded/__init__.py
--rw-rw-rw-   0        0        0     6628 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/threaded/pool.py
--rw-rw-rw-   0        0        0     1465 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/threaded/thread.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.088938 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/utils/
--rw-rw-rw-   0        0        0        0 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/utils/__init__.py
--rw-rw-rw-   0        0        0     2558 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/utils/deprecated.py
--rw-rw-rw-   0        0        0     6522 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/utils/dump.py
--rw-rw-rw-   0        0        0     3233 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/utils/formdata.py
--rw-rw-rw-   0        0        0     4524 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/utils/user_agent.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.056444 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/
--rw-rw-rw-   0        0        0       18 2023-07-26 08:06:09.000000 mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.103937 mylove-0.0.2/venv/Lib/site-packages/rfc3986/
--rw-rw-rw-   0        0        0     1565 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/rfc3986/__init__.py
--rw-rw-rw-   0        0        0    13297 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/rfc3986/_mixin.py
--rw-rw-rw-   0        0        0     9048 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/rfc3986/abnf_regexp.py
--rw-rw-rw-   0        0        0     3862 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/rfc3986/api.py
--rw-rw-rw-   0        0        0    12709 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/rfc3986/builder.py
--rw-rw-rw-   0        0        0     1620 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/rfc3986/compat.py
--rw-rw-rw-   0        0        0     3614 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/rfc3986/exceptions.py
--rw-rw-rw-   0        0        0     5477 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/rfc3986/iri.py
--rw-rw-rw-   0        0        0     4114 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/rfc3986/misc.py
--rw-rw-rw-   0        0        0     5261 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/rfc3986/normalizers.py
--rw-rw-rw-   0        0        0    14599 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/rfc3986/parseresult.py
--rw-rw-rw-   0        0        0     5183 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/rfc3986/uri.py
--rw-rw-rw-   0        0        0    13676 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/rfc3986/validators.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.105942 mylove-0.0.2/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/
--rw-rw-rw-   0        0        0        8 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.190052 mylove-0.0.2/venv/Lib/site-packages/rich/
--rw-rw-rw-   0        0        0     6066 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/__init__.py
--rw-rw-rw-   0        0        0     8334 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/__main__.py
--rw-rw-rw-   0        0        0    10096 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/_cell_widths.py
--rw-rw-rw-   0        0        0   140235 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/_emoji_codes.py
--rw-rw-rw-   0        0        0     1064 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/_emoji_replace.py
--rw-rw-rw-   0        0        0     2100 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/_export_format.py
--rw-rw-rw-   0        0        0      241 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/_extension.py
--rw-rw-rw-   0        0        0      799 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/_fileno.py
--rw-rw-rw-   0        0        0     9695 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/_inspect.py
--rw-rw-rw-   0        0        0     3213 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/_log_render.py
--rw-rw-rw-   0        0        0     1236 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/_loop.py
--rw-rw-rw-   0        0        0     1387 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/_null_file.py
--rw-rw-rw-   0        0        0     7063 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/_palettes.py
--rw-rw-rw-   0        0        0      423 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/_pick.py
--rw-rw-rw-   0        0        0     5460 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/_ratio.py
--rw-rw-rw-   0        0        0    19919 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/_spinners.py
--rw-rw-rw-   0        0        0      351 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/_stack.py
--rw-rw-rw-   0        0        0      417 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/_timer.py
--rw-rw-rw-   0        0        0    22784 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/_win32_console.py
--rw-rw-rw-   0        0        0     1902 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/_windows.py
--rw-rw-rw-   0        0        0     2759 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/_windows_renderer.py
--rw-rw-rw-   0        0        0     1840 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/_wrap.py
--rw-rw-rw-   0        0        0      878 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/abc.py
--rw-rw-rw-   0        0        0    10320 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/align.py
--rw-rw-rw-   0        0        0     6906 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/ansi.py
--rw-rw-rw-   0        0        0     3264 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/bar.py
--rw-rw-rw-   0        0        0     9794 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/box.py
--rw-rw-rw-   0        0        0     4509 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/cells.py
--rw-rw-rw-   0        0        0    18224 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/color.py
--rw-rw-rw-   0        0        0     1054 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/color_triplet.py
--rw-rw-rw-   0        0        0     7131 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/columns.py
--rw-rw-rw-   0        0        0    99146 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/console.py
--rw-rw-rw-   0        0        0     1288 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/constrain.py
--rw-rw-rw-   0        0        0     5497 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/containers.py
--rw-rw-rw-   0        0        0     6606 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/control.py
--rw-rw-rw-   0        0        0     8046 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/default_styles.py
--rw-rw-rw-   0        0        0      924 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/diagnose.py
--rw-rw-rw-   0        0        0     2465 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/emoji.py
--rw-rw-rw-   0        0        0      642 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/errors.py
--rw-rw-rw-   0        0        0     1683 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/file_proxy.py
--rw-rw-rw-   0        0        0     2508 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/filesize.py
--rw-rw-rw-   0        0        0     9584 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/highlighter.py
--rw-rw-rw-   0        0        0     5020 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/json.py
--rw-rw-rw-   0        0        0     3228 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/jupyter.py
--rw-rw-rw-   0        0        0    13947 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/layout.py
--rw-rw-rw-   0        0        0    14273 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/live.py
--rw-rw-rw-   0        0        0     3655 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/live_render.py
--rw-rw-rw-   0        0        0    11891 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/logging.py
--rw-rw-rw-   0        0        0    26245 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/markdown.py
--rw-rw-rw-   0        0        0     8174 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/markup.py
--rw-rw-rw-   0        0        0     5305 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/measure.py
--rw-rw-rw-   0        0        0     4958 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/padding.py
--rw-rw-rw-   0        0        0      828 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/pager.py
--rw-rw-rw-   0        0        0     3288 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/palette.py
--rw-rw-rw-   0        0        0    10574 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/panel.py
--rw-rw-rw-   0        0        0    35816 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/pretty.py
--rw-rw-rw-   0        0        0    59694 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/progress.py
--rw-rw-rw-   0        0        0     8165 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/progress_bar.py
--rw-rw-rw-   0        0        0    11291 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/prompt.py
--rw-rw-rw-   0        0        0     1367 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/protocol.py
--rw-rw-rw-   0        0        0      166 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/region.py
--rw-rw-rw-   0        0        0     4419 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/repr.py
--rw-rw-rw-   0        0        0     4590 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/rule.py
--rw-rw-rw-   0        0        0     2831 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/scope.py
--rw-rw-rw-   0        0        0     1579 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/screen.py
--rw-rw-rw-   0        0        0    24211 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/segment.py
--rw-rw-rw-   0        0        0     4339 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/spinner.py
--rw-rw-rw-   0        0        0     4425 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/status.py
--rw-rw-rw-   0        0        0    27073 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/style.py
--rw-rw-rw-   0        0        0     1234 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/styled.py
--rw-rw-rw-   0        0        0    35065 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/syntax.py
--rw-rw-rw-   0        0        0    39648 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/table.py
--rw-rw-rw-   0        0        0     3370 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/terminal_theme.py
--rw-rw-rw-   0        0        0    45513 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/text.py
--rw-rw-rw-   0        0        0     3777 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/theme.py
--rw-rw-rw-   0        0        0      102 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/themes.py
--rw-rw-rw-   0        0        0    29532 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/traceback.py
--rw-rw-rw-   0        0        0     9109 2023-07-26 08:06:12.000000 mylove-0.0.2/venv/Lib/site-packages/rich/tree.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.215638 mylove-0.0.2/venv/Lib/site-packages/setuptools/
--rw-rw-rw-   0        0        0     8429 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/__init__.py
--rw-rw-rw-   0        0        0      218 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_deprecation_warning.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.248562 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/
--rw-rw-rw-   0        0        0      537 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/__init__.py
--rw-rw-rw-   0        0        0     1330 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/_collections.py
--rw-rw-rw-   0        0        0      411 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/_functools.py
--rw-rw-rw-   0        0        0      239 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/_macos_compat.py
--rw-rw-rw-   0        0        0    19672 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-rw-rw-   0        0        0     8603 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/archive_util.py
--rw-rw-rw-   0        0        0    14789 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-rw-rw-   0        0        0    47369 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py
--rw-rw-rw-   0        0        0    17973 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/cmd.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.273008 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/
--rw-rw-rw-   0        0        0      430 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/__init__.py
--rw-rw-rw-   0        0        0     1614 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py
--rw-rw-rw-   0        0        0     5441 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py
--rw-rw-rw-   0        0        0     4701 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-rw-rw-   0        0        0    22051 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-rw-rw-   0        0        0     5617 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/build.py
--rw-rw-rw-   0        0        0     7728 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py
--rw-rw-rw-   0        0        0    31558 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py
--rw-rw-rw-   0        0        0    16568 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py
--rw-rw-rw-   0        0        0     5624 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-rw-rw-   0        0        0     4888 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/check.py
--rw-rw-rw-   0        0        0     2603 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/clean.py
--rw-rw-rw-   0        0        0    13137 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/config.py
--rw-rw-rw-   0        0        0    30221 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/install.py
--rw-rw-rw-   0        0        0     2779 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py
--rw-rw-rw-   0        0        0     2785 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-rw-rw-   0        0        0     1189 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py
--rw-rw-rw-   0        0        0     8434 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py
--rw-rw-rw-   0        0        0     1936 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-rw-rw-   0        0        0      672 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py
--rw-rw-rw-   0        0        0    11765 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/register.py
--rw-rw-rw-   0        0        0    19241 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py
--rw-rw-rw-   0        0        0     7477 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/upload.py
--rw-rw-rw-   0        0        0     4920 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/config.py
--rw-rw-rw-   0        0        0     9451 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/core.py
--rw-rw-rw-   0        0        0    12537 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-rw-rw-   0        0        0      139 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/debug.py
--rw-rw-rw-   0        0        0     3423 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/dep_util.py
--rw-rw-rw-   0        0        0     8082 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/dir_util.py
--rw-rw-rw-   0        0        0    50186 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/dist.py
--rw-rw-rw-   0        0        0     3589 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/errors.py
--rw-rw-rw-   0        0        0    10270 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/extension.py
--rw-rw-rw-   0        0        0    17910 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-rw-rw-   0        0        0     8226 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/file_util.py
--rw-rw-rw-   0        0        0    13713 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/filelist.py
--rw-rw-rw-   0        0        0     1972 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/log.py
--rw-rw-rw-   0        0        0    30235 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-rw-rw-   0        0        0    23602 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py
--rw-rw-rw-   0        0        0      217 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/py38compat.py
--rw-rw-rw-   0        0        0      639 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/py39compat.py
--rw-rw-rw-   0        0        0     3517 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/spawn.py
--rw-rw-rw-   0        0        0    18858 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py
--rw-rw-rw-   0        0        0    12096 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/text_file.py
--rw-rw-rw-   0        0        0    15641 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py
--rw-rw-rw-   0        0        0    18128 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/util.py
--rw-rw-rw-   0        0        0    12952 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/version.py
--rw-rw-rw-   0        0        0     5248 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py
--rw-rw-rw-   0        0        0     1972 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_entry_points.py
--rw-rw-rw-   0        0        0     2392 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_imp.py
--rw-rw-rw-   0        0        0     1311 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_importlib.py
--rw-rw-rw-   0        0        0      675 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_itertools.py
--rw-rw-rw-   0        0        0      749 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_path.py
--rw-rw-rw-   0        0        0      501 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_reqs.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.276222 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/
--rw-rw-rw-   0        0        0        0 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.283003 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/
--rw-rw-rw-   0        0        0    30130 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
--rw-rw-rw-   0        0        0     1862 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
--rw-rw-rw-   0        0        0      743 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
--rw-rw-rw-   0        0        0     1828 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
--rw-rw-rw-   0        0        0     2895 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
--rw-rw-rw-   0        0        0     2068 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
--rw-rw-rw-   0        0        0     1154 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
--rw-rw-rw-   0        0        0     2166 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.291261 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/
--rw-rw-rw-   0        0        0      506 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/__init__.py
--rw-rw-rw-   0        0        0     4504 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
--rw-rw-rw-   0        0        0     2741 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py
--rw-rw-rw-   0        0        0     2706 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py
--rw-rw-rw-   0        0        0      884 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
--rw-rw-rw-   0        0        0     3494 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
--rw-rw-rw-   0        0        0     3886 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py
--rw-rw-rw-   0        0        0     3566 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py
--rw-rw-rw-   0        0        0     2836 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.294253 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/jaraco/
--rw-rw-rw-   0        0        0        0 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/jaraco/__init__.py
--rw-rw-rw-   0        0        0     5420 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py
--rw-rw-rw-   0        0        0    13512 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.296359 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/
--rw-rw-rw-   0        0        0    15517 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.298828 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/more_itertools/
--rw-rw-rw-   0        0        0       82 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-rw-rw-   0        0        0   117959 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-rw-rw-   0        0        0    16256 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-rw-rw-   0        0        0    15130 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.311861 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/
--rw-rw-rw-   0        0        0      661 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-rw-rw-   0        0        0      497 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-rw-rw-   0        0        0    11488 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     4378 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-rw-rw-   0        0        0     1431 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-rw-rw-   0        0        0     8493 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
--rw-rw-rw-   0        0        0     4700 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-rw-rw-   0        0        0    30110 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-rw-rw-   0        0        0    15699 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py
--rw-rw-rw-   0        0        0     4200 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
--rw-rw-rw-   0        0        0    14665 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.320557 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/
--rw-rw-rw-   0        0        0     9159 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/__init__.py
--rw-rw-rw-   0        0        0     6426 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/actions.py
--rw-rw-rw-   0        0        0    12936 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/common.py
--rw-rw-rw-   0        0        0   213310 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/core.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.322748 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/
--rw-rw-rw-   0        0        0    23668 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
--rw-rw-rw-   0        0        0     9023 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py
--rw-rw-rw-   0        0        0    39129 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/helpers.py
--rw-rw-rw-   0        0        0    25341 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/results.py
--rw-rw-rw-   0        0        0    13402 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/testing.py
--rw-rw-rw-   0        0        0    10787 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/unicode.py
--rw-rw-rw-   0        0        0     6805 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/util.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.350263 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/tomli/
--rw-rw-rw-   0        0        0      396 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/tomli/__init__.py
--rw-rw-rw-   0        0        0    22633 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py
--rw-rw-rw-   0        0        0     2943 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py
--rw-rw-rw-   0        0        0      254 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/tomli/_types.py
--rw-rw-rw-   0        0        0    87149 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py
--rw-rw-rw-   0        0        0     8425 2023-07-26 07:30:17.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/zipp.py
--rw-rw-rw-   0        0        0     7346 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/archive_util.py
--rw-rw-rw-   0        0        0    19539 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/build_meta.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.374804 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/
--rw-rw-rw-   0        0        0      396 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/__init__.py
--rw-rw-rw-   0        0        0     2381 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/alias.py
--rw-rw-rw-   0        0        0    16623 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/bdist_egg.py
--rw-rw-rw-   0        0        0     1182 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/bdist_rpm.py
--rw-rw-rw-   0        0        0     6589 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/build.py
--rw-rw-rw-   0        0        0     4415 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/build_clib.py
--rw-rw-rw-   0        0        0    15821 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/build_ext.py
--rw-rw-rw-   0        0        0    14115 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/build_py.py
--rw-rw-rw-   0        0        0     7012 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/develop.py
--rw-rw-rw-   0        0        0     4800 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/dist_info.py
--rw-rw-rw-   0        0        0    85662 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/easy_install.py
--rw-rw-rw-   0        0        0    31188 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/editable_wheel.py
--rw-rw-rw-   0        0        0    26795 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/egg_info.py
--rw-rw-rw-   0        0        0     5163 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/install.py
--rw-rw-rw-   0        0        0     2226 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/install_egg_info.py
--rw-rw-rw-   0        0        0     3875 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/install_lib.py
--rw-rw-rw-   0        0        0     2612 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/install_scripts.py
--rw-rw-rw-   0        0        0     4946 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/py36compat.py
--rw-rw-rw-   0        0        0      468 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/register.py
--rw-rw-rw-   0        0        0     2128 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/rotate.py
--rw-rw-rw-   0        0        0      658 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/saveopts.py
--rw-rw-rw-   0        0        0     7071 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/sdist.py
--rw-rw-rw-   0        0        0     5086 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/setopt.py
--rw-rw-rw-   0        0        0     8102 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/test.py
--rw-rw-rw-   0        0        0      462 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/upload.py
--rw-rw-rw-   0        0        0     7494 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/command/upload_docs.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.377861 mylove-0.0.2/venv/Lib/site-packages/setuptools/config/
--rw-rw-rw-   0        0        0     1121 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/config/__init__.py
--rw-rw-rw-   0        0        0    13398 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.383147 mylove-0.0.2/venv/Lib/site-packages/setuptools/config/_validate_pyproject/
--rw-rw-rw-   0        0        0     1038 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py
--rw-rw-rw-   0        0        0    11266 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
--rw-rw-rw-   0        0        0     1153 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
--rw-rw-rw-   0        0        0     1612 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
--rw-rw-rw-   0        0        0   269900 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
--rw-rw-rw-   0        0        0     8736 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py
--rw-rw-rw-   0        0        0    16319 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/config/expand.py
--rw-rw-rw-   0        0        0    19304 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/config/pyprojecttoml.py
--rw-rw-rw-   0        0        0    25198 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/config/setupcfg.py
--rw-rw-rw-   0        0        0      949 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/dep_util.py
--rw-rw-rw-   0        0        0     5499 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/depends.py
--rw-rw-rw-   0        0        0    20799 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/discovery.py
--rw-rw-rw-   0        0        0    45578 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/dist.py
--rw-rw-rw-   0        0        0     2464 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/errors.py
--rw-rw-rw-   0        0        0     5591 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/extension.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.383147 mylove-0.0.2/venv/Lib/site-packages/setuptools/extern/
--rw-rw-rw-   0        0        0     2512 2023-07-26 07:30:16.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/extern/__init__.py
--rw-rw-rw-   0        0        0     4873 2023-07-26 07:30:14.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/glob.py
--rw-rw-rw-   0        0        0     3824 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/installer.py
--rw-rw-rw-   0        0        0      812 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/launch.py
--rw-rw-rw-   0        0        0     1210 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/logging.py
--rw-rw-rw-   0        0        0     4857 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/monkey.py
--rw-rw-rw-   0        0        0    47724 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/msvc.py
--rw-rw-rw-   0        0        0     3093 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/namespaces.py
--rw-rw-rw-   0        0        0    40329 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/package_index.py
--rw-rw-rw-   0        0        0      245 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/py34compat.py
--rw-rw-rw-   0        0        0    14348 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/sandbox.py
--rw-rw-rw-   0        0        0      941 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/unicode_utils.py
--rw-rw-rw-   0        0        0      144 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/version.py
--rw-rw-rw-   0        0        0     8376 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/wheel.py
--rw-rw-rw-   0        0        0      718 2023-07-26 07:30:15.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools/windows_support.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.217661 mylove-0.0.2/venv/Lib/site-packages/setuptools-65.5.1.dist-info/
--rw-rw-rw-   0        0        0     2740 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools-65.5.1.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0       41 2023-07-26 07:30:18.000000 mylove-0.0.2/venv/Lib/site-packages/setuptools-65.5.1.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.384196 mylove-0.0.2/venv/Lib/site-packages/six-1.16.0.dist-info/
--rw-rw-rw-   0        0        0        4 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/six-1.16.0.dist-info/top_level.txt
--rw-rw-rw-   0        0        0    34549 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/six.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.388430 mylove-0.0.2/venv/Lib/site-packages/speech_recognition/
--rw-rw-rw-   0        0        0    94078 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/speech_recognition/__init__.py
--rw-rw-rw-   0        0        0      833 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/speech_recognition/__main__.py
--rw-rw-rw-   0        0        0    14807 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/speech_recognition/audio.py
--rw-rw-rw-   0        0        0      273 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/speech_recognition/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.443004 mylove-0.0.2/venv/Lib/site-packages/speech_recognition/pocketsphinx-data/
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.390422 mylove-0.0.2/venv/Lib/site-packages/speech_recognition/pocketsphinx-data/en-US/
--rw-rw-rw-   0        0        0     1537 2023-07-26 07:38:30.000000 mylove-0.0.2/venv/Lib/site-packages/speech_recognition/pocketsphinx-data/en-US/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.391418 mylove-0.0.2/venv/Lib/site-packages/speech_recognition/recognizers/
--rw-rw-rw-   0        0        0        0 2023-07-26 07:38:31.000000 mylove-0.0.2/venv/Lib/site-packages/speech_recognition/recognizers/__init__.py
--rw-rw-rw-   0        0        0     1492 2023-07-26 07:38:31.000000 mylove-0.0.2/venv/Lib/site-packages/speech_recognition/recognizers/whisper.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.401915 mylove-0.0.2/venv/Lib/site-packages/twine/
--rw-rw-rw-   0        0        0     1343 2023-07-26 08:06:15.000000 mylove-0.0.2/venv/Lib/site-packages/twine/__init__.py
--rw-rw-rw-   0        0        0     1475 2023-07-26 08:06:15.000000 mylove-0.0.2/venv/Lib/site-packages/twine/__main__.py
--rw-rw-rw-   0        0        0     3129 2023-07-26 08:06:15.000000 mylove-0.0.2/venv/Lib/site-packages/twine/auth.py
--rw-rw-rw-   0        0        0     3738 2023-07-26 08:06:15.000000 mylove-0.0.2/venv/Lib/site-packages/twine/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.409409 mylove-0.0.2/venv/Lib/site-packages/twine/commands/
--rw-rw-rw-   0        0        0     1802 2023-07-26 08:06:15.000000 mylove-0.0.2/venv/Lib/site-packages/twine/commands/__init__.py
--rw-rw-rw-   0        0        0     5727 2023-07-26 08:06:15.000000 mylove-0.0.2/venv/Lib/site-packages/twine/commands/check.py
--rw-rw-rw-   0        0        0     2904 2023-07-26 08:06:15.000000 mylove-0.0.2/venv/Lib/site-packages/twine/commands/register.py
--rw-rw-rw-   0        0        0     7469 2023-07-26 08:06:15.000000 mylove-0.0.2/venv/Lib/site-packages/twine/commands/upload.py
--rw-rw-rw-   0        0        0     3814 2023-07-26 08:06:15.000000 mylove-0.0.2/venv/Lib/site-packages/twine/exceptions.py
--rw-rw-rw-   0        0        0    11024 2023-07-26 08:06:15.000000 mylove-0.0.2/venv/Lib/site-packages/twine/package.py
--rw-rw-rw-   0        0        0     8713 2023-07-26 08:06:15.000000 mylove-0.0.2/venv/Lib/site-packages/twine/repository.py
--rw-rw-rw-   0        0        0    12269 2023-07-26 08:06:15.000000 mylove-0.0.2/venv/Lib/site-packages/twine/settings.py
--rw-rw-rw-   0        0        0    10867 2023-07-26 08:06:15.000000 mylove-0.0.2/venv/Lib/site-packages/twine/utils.py
--rw-rw-rw-   0        0        0     3049 2023-07-26 08:06:15.000000 mylove-0.0.2/venv/Lib/site-packages/twine/wheel.py
--rw-rw-rw-   0        0        0     1795 2023-07-26 08:06:15.000000 mylove-0.0.2/venv/Lib/site-packages/twine/wininst.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.403417 mylove-0.0.2/venv/Lib/site-packages/twine-4.0.2.dist-info/
--rw-rw-rw-   0        0        0      185 2023-07-26 08:06:15.000000 mylove-0.0.2/venv/Lib/site-packages/twine-4.0.2.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-26 08:06:15.000000 mylove-0.0.2/venv/Lib/site-packages/twine-4.0.2.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.420079 mylove-0.0.2/venv/Lib/site-packages/urllib3/
--rw-rw-rw-   0        0        0     5283 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/__init__.py
--rw-rw-rw-   0        0        0     5651 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/_base_connection.py
--rw-rw-rw-   0        0        0    15561 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/_collections.py
--rw-rw-rw-   0        0        0     7756 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/_request_methods.py
--rw-rw-rw-   0        0        0       98 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/_version.py
--rw-rw-rw-   0        0        0    33622 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/connection.py
--rw-rw-rw-   0        0        0    42961 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/connectionpool.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.424144 mylove-0.0.2/venv/Lib/site-packages/urllib3/contrib/
--rw-rw-rw-   0        0        0        0 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/contrib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.427250 mylove-0.0.2/venv/Lib/site-packages/urllib3/contrib/_securetransport/
--rw-rw-rw-   0        0        0        0 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/contrib/_securetransport/__init__.py
--rw-rw-rw-   0        0        0    14452 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/contrib/_securetransport/bindings.py
--rw-rw-rw-   0        0        0    16220 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/contrib/_securetransport/low_level.py
--rw-rw-rw-   0        0        0    19437 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/contrib/pyopenssl.py
--rw-rw-rw-   0        0        0    34121 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/contrib/securetransport.py
--rw-rw-rw-   0        0        0     7715 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/contrib/socks.py
--rw-rw-rw-   0        0        0     9385 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/exceptions.py
--rw-rw-rw-   0        0        0    11026 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/fields.py
--rw-rw-rw-   0        0        0     2395 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/filepost.py
--rw-rw-rw-   0        0        0    22648 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/poolmanager.py
--rw-rw-rw-   0        0        0    40092 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/response.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.440421 mylove-0.0.2/venv/Lib/site-packages/urllib3/util/
--rw-rw-rw-   0        0        0     1051 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/util/__init__.py
--rw-rw-rw-   0        0        0     4462 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/util/connection.py
--rw-rw-rw-   0        0        0     1148 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/util/proxy.py
--rw-rw-rw-   0        0        0     8111 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/util/request.py
--rw-rw-rw-   0        0        0     3374 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/util/response.py
--rw-rw-rw-   0        0        0    18374 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/util/retry.py
--rw-rw-rw-   0        0        0    18860 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/util/ssl_.py
--rw-rw-rw-   0        0        0     5812 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/util/ssl_match_hostname.py
--rw-rw-rw-   0        0        0     9045 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/util/ssltransport.py
--rw-rw-rw-   0        0        0    10529 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/util/timeout.py
--rw-rw-rw-   0        0        0    15213 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/util/url.py
--rw-rw-rw-   0        0        0     1146 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/util/util.py
--rw-rw-rw-   0        0        0     4423 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3/util/wait.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:08.445185 mylove-0.0.2/venv/Lib/site-packages/urllib3-2.0.3.dist-info/
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.421077 mylove-0.0.2/venv/Lib/site-packages/urllib3-2.0.3.dist-info/licenses/
--rw-rw-rw-   0        0        0     1093 2023-07-26 07:38:25.000000 mylove-0.0.2/venv/Lib/site-packages/urllib3-2.0.3.dist-info/licenses/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.445933 mylove-0.0.2/venv/Lib/site-packages/webencodings/
--rw-rw-rw-   0        0        0    10579 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/webencodings/__init__.py
--rw-rw-rw-   0        0        0     8979 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/webencodings/labels.py
--rw-rw-rw-   0        0        0     1305 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/webencodings/mklabels.py
--rw-rw-rw-   0        0        0     6563 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/webencodings/tests.py
--rw-rw-rw-   0        0        0     4307 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/webencodings/x_user_defined.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.446930 mylove-0.0.2/venv/Lib/site-packages/webencodings-0.5.1.dist-info/
--rw-rw-rw-   0        0        0       13 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/webencodings-0.5.1.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.454420 mylove-0.0.2/venv/Lib/site-packages/wheel/
--rw-rw-rw-   0        0        0       59 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/wheel/__init__.py
--rw-rw-rw-   0        0        0      455 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/wheel/__main__.py
--rw-rw-rw-   0        0        0      746 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/wheel/_setuptools_logging.py
--rw-rw-rw-   0        0        0    19293 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/wheel/bdist_wheel.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.461402 mylove-0.0.2/venv/Lib/site-packages/wheel/cli/
--rw-rw-rw-   0        0        0     2384 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/wheel/cli/__init__.py
--rw-rw-rw-   0        0        0     9427 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/wheel/cli/convert.py
--rw-rw-rw-   0        0        0     3383 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/wheel/cli/pack.py
--rw-rw-rw-   0        0        0      659 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/wheel/cli/unpack.py
--rw-rw-rw-   0        0        0    16145 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/wheel/macosx_libfile.py
--rw-rw-rw-   0        0        0     3727 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/wheel/metadata.py
--rw-rw-rw-   0        0        0      621 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/wheel/util.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.462905 mylove-0.0.2/venv/Lib/site-packages/wheel/vendored/
--rw-rw-rw-   0        0        0        0 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/wheel/vendored/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.465954 mylove-0.0.2/venv/Lib/site-packages/wheel/vendored/packaging/
--rw-rw-rw-   0        0        0        0 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/wheel/vendored/packaging/__init__.py
--rw-rw-rw-   0        0        0    11489 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/wheel/vendored/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     4374 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/wheel/vendored/packaging/_musllinux.py
--rw-rw-rw-   0        0        0    15612 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/wheel/vendored/packaging/tags.py
--rw-rw-rw-   0        0        0     7536 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/wheel/wheelfile.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.458412 mylove-0.0.2/venv/Lib/site-packages/wheel-0.38.4.dist-info/
--rw-rw-rw-   0        0        0     1107 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/wheel-0.38.4.dist-info/LICENSE.txt
--rw-rw-rw-   0        0        0      107 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/wheel-0.38.4.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-26 07:30:13.000000 mylove-0.0.2/venv/Lib/site-packages/wheel-0.38.4.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.470938 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/
--rw-rw-rw-   0        0        0      206 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.474435 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/
--rw-rw-rw-   0        0        0     1564 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/__init__.py
--rw-rw-rw-   0        0        0      190 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/_winerrors.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.482801 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/
--rw-rw-rw-   0        0        0      259 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/__init__.py
--rw-rw-rw-   0        0        0     5161 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/_authentication.py
--rw-rw-rw-   0        0        0      547 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/_common.py
--rw-rw-rw-   0        0        0      741 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/_dll.py
--rw-rw-rw-   0        0        0      295 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/_nl_support.py
--rw-rw-rw-   0        0        0     4423 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/_resource.py
--rw-rw-rw-   0        0        0      840 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/_system_information.py
--rw-rw-rw-   0        0        0      314 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/_time.py
--rw-rw-rw-   0        0        0     2557 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/_util.py
--rw-rw-rw-   0        0        0      148 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/compat.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.495362 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/
--rw-rw-rw-   0        0        0      261 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/__init__.py
--rw-rw-rw-   0        0        0     3700 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_authentication.py
--rw-rw-rw-   0        0        0     1170 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_common.py
--rw-rw-rw-   0        0        0      531 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_dll.py
--rw-rw-rw-   0        0        0      303 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_nl_support.py
--rw-rw-rw-   0        0        0     4116 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_resource.py
--rw-rw-rw-   0        0        0      905 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_system_information.py
--rw-rw-rw-   0        0        0      327 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_time.py
--rw-rw-rw-   0        0        0     1952 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_util.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.499609 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/pywin32/
--rw-rw-rw-   0        0        0      342 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/pywin32/__init__.py
--rw-rw-rw-   0        0        0      967 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/pywin32/pywintypes.py
--rw-rw-rw-   0        0        0     7430 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/pywin32/win32api.py
--rw-rw-rw-   0        0        0     4656 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/pywin32/win32cred.py
--rw-rw-rw-   0        0        0      337 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/pywintypes.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.505261 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/tests/
--rw-rw-rw-   0        0        0      672 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/tests/__init__.py
--rw-rw-rw-   0        0        0     1017 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/tests/test_backends.py
--rw-rw-rw-   0        0        0    11383 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/tests/test_win32api.py
--rw-rw-rw-   0        0        0     7718 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/tests/test_win32cred.py
--rw-rw-rw-   0        0        0       22 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/version.py
--rw-rw-rw-   0        0        0      333 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/win32api.py
--rw-rw-rw-   0        0        0      335 2023-07-26 08:05:57.000000 mylove-0.0.2/venv/Lib/site-packages/win32ctypes/win32cred.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.509319 mylove-0.0.2/venv/Lib/site-packages/zipp/
--rw-rw-rw-   0        0        0    10453 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/zipp/__init__.py
--rw-rw-rw-   0        0        0      893 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/zipp/glob.py
--rw-rw-rw-   0        0        0      219 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/zipp/py310compat.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.511312 mylove-0.0.2/venv/Lib/site-packages/zipp-3.16.2.dist-info/
--rw-rw-rw-   0        0        0        5 2023-07-26 08:05:56.000000 mylove-0.0.2/venv/Lib/site-packages/zipp-3.16.2.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:27:10.528150 mylove-0.0.2/venv/Scripts/
--rw-rw-rw-   0        0        0     1169 2023-07-26 07:30:22.000000 mylove-0.0.2/venv/Scripts/activate_this.py
--rw-rw-rw-   0        0        0      657 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Scripts/rst2html.py
--rw-rw-rw-   0        0        0      779 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Scripts/rst2html4.py
--rw-rw-rw-   0        0        0     1114 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Scripts/rst2html5.py
--rw-rw-rw-   0        0        0      856 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Scripts/rst2latex.py
--rw-rw-rw-   0        0        0      679 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Scripts/rst2man.py
--rw-rw-rw-   0        0        0      845 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Scripts/rst2odt.py
--rw-rw-rw-   0        0        0      651 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Scripts/rst2odt_prepstyles.py
--rw-rw-rw-   0        0        0      664 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Scripts/rst2pseudoxml.py
--rw-rw-rw-   0        0        0      700 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Scripts/rst2s5.py
--rw-rw-rw-   0        0        0      936 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Scripts/rst2xetex.py
--rw-rw-rw-   0        0        0      665 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Scripts/rst2xml.py
--rw-rw-rw-   0        0        0      733 2023-07-26 08:06:06.000000 mylove-0.0.2/venv/Scripts/rstpep2html.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.256535 mylove-1.0.0/
+-rw-rw-rw-   0        0        0       82 2023-07-26 07:50:30.000000 mylove-1.0.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1052 2023-07-26 07:51:29.000000 mylove-1.0.0/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-07-26 07:51:37.000000 mylove-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      750 2023-07-26 08:34:35.256535 mylove-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      139 2023-07-26 07:57:32.000000 mylove-1.0.0/Readme.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.660694 mylove-1.0.0/mylove/
+-rw-rw-rw-   0        0        0     1985 2023-07-26 08:33:55.000000 mylove-1.0.0/mylove/__init__.py
+-rw-rw-rw-   0        0        0    30672 2023-07-09 02:33:02.000000 mylove-1.0.0/mylove/h.jpg
+-rw-rw-rw-   0        0        0      107 2023-07-26 07:53:56.000000 mylove-1.0.0/mylove/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.680338 mylove-1.0.0/mylove.egg-info/
+-rw-rw-rw-   0        0        0      750 2023-07-26 08:34:33.000000 mylove-1.0.0/mylove.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    96481 2023-07-26 08:34:33.000000 mylove-1.0.0/mylove.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 08:34:33.000000 mylove-1.0.0/mylove.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-26 08:34:33.000000 mylove-1.0.0/mylove.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-26 08:34:33.000000 mylove-1.0.0/mylove.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 08:34:35.256535 mylove-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      792 2023-07-26 08:34:31.000000 mylove-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.654714 mylove-1.0.0/venv/
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.595911 mylove-1.0.0/venv/Lib/
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.682347 mylove-1.0.0/venv/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.764072 mylove-1.0.0/venv/Lib/site-packages/PIL/
+-rw-rw-rw-   0        0        0     3359 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/BdfFontFile.py
+-rw-rw-rw-   0        0        0    15940 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/BlpImagePlugin.py
+-rw-rw-rw-   0        0        0    18138 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/BmpImagePlugin.py
+-rw-rw-rw-   0        0        0     1629 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/BufrStubImagePlugin.py
+-rw-rw-rw-   0        0        0     3003 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ContainerIO.py
+-rw-rw-rw-   0        0        0     1796 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/CurImagePlugin.py
+-rw-rw-rw-   0        0        0     2037 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/DcxImagePlugin.py
+-rw-rw-rw-   0        0        0     9637 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/DdsImagePlugin.py
+-rw-rw-rw-   0        0        0    15526 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/EpsImagePlugin.py
+-rw-rw-rw-   0        0        0    10098 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ExifTags.py
+-rw-rw-rw-   0        0        0     2132 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/FitsImagePlugin.py
+-rw-rw-rw-   0        0        0     4614 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/FliImagePlugin.py
+-rw-rw-rw-   0        0        0     2874 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/FontFile.py
+-rw-rw-rw-   0        0        0     7214 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/FpxImagePlugin.py
+-rw-rw-rw-   0        0        0     3541 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/FtexImagePlugin.py
+-rw-rw-rw-   0        0        0     3010 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/GbrImagePlugin.py
+-rw-rw-rw-   0        0        0     2704 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/GdImageFile.py
+-rw-rw-rw-   0        0        0    36838 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/GifImagePlugin.py
+-rw-rw-rw-   0        0        0     3533 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/GimpGradientFile.py
+-rw-rw-rw-   0        0        0     1401 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/GimpPaletteFile.py
+-rw-rw-rw-   0        0        0     1623 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/GribStubImagePlugin.py
+-rw-rw-rw-   0        0        0     1626 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/Hdf5StubImagePlugin.py
+-rw-rw-rw-   0        0        0    12325 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/IcnsImagePlugin.py
+-rw-rw-rw-   0        0        0    11980 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/IcoImagePlugin.py
+-rw-rw-rw-   0        0        0    11238 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImImagePlugin.py
+-rw-rw-rw-   0        0        0   137166 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/Image.py
+-rw-rw-rw-   0        0        0     7306 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImageChops.py
+-rw-rw-rw-   0        0        0    38180 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImageCms.py
+-rw-rw-rw-   0        0        0     9397 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImageColor.py
+-rw-rw-rw-   0        0        0    36829 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImageDraw.py
+-rw-rw-rw-   0        0        0     5694 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImageDraw2.py
+-rw-rw-rw-   0        0        0     3293 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImageEnhance.py
+-rw-rw-rw-   0        0        0    24312 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImageFile.py
+-rw-rw-rw-   0        0        0    17110 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImageFilter.py
+-rw-rw-rw-   0        0        0    43021 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImageFont.py
+-rw-rw-rw-   0        0        0     5496 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImageGrab.py
+-rw-rw-rw-   0        0        0     7620 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImageMath.py
+-rw-rw-rw-   0        0        0     3004 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImageMode.py
+-rw-rw-rw-   0        0        0     8231 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImageMorph.py
+-rw-rw-rw-   0        0        0    22052 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImageOps.py
+-rw-rw-rw-   0        0        0     8174 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImagePalette.py
+-rw-rw-rw-   0        0        0      355 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImagePath.py
+-rw-rw-rw-   0        0        0     6582 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImageQt.py
+-rw-rw-rw-   0        0        0     1948 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImageSequence.py
+-rw-rw-rw-   0        0        0     8631 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImageShow.py
+-rw-rw-rw-   0        0        0     4072 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImageStat.py
+-rw-rw-rw-   0        0        0     8744 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImageTk.py
+-rw-rw-rw-   0        0        0     2985 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImageTransform.py
+-rw-rw-rw-   0        0        0     7421 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImageWin.py
+-rw-rw-rw-   0        0        0     2680 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/ImtImagePlugin.py
+-rw-rw-rw-   0        0        0     6007 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/IptcImagePlugin.py
+-rw-rw-rw-   0        0        0    11982 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/Jpeg2KImagePlugin.py
+-rw-rw-rw-   0        0        0    29937 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/JpegImagePlugin.py
+-rw-rw-rw-   0        0        0    12583 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/JpegPresets.py
+-rw-rw-rw-   0        0        0     1871 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/McIdasImagePlugin.py
+-rw-rw-rw-   0        0        0     2617 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/MicImagePlugin.py
+-rw-rw-rw-   0        0        0     1905 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/MpegImagePlugin.py
+-rw-rw-rw-   0        0        0     6486 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/MpoImagePlugin.py
+-rw-rw-rw-   0        0        0     5806 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/MspImagePlugin.py
+-rw-rw-rw-   0        0        0     6754 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/PSDraw.py
+-rw-rw-rw-   0        0        0     1179 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/PaletteFile.py
+-rw-rw-rw-   0        0        0     9369 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/PalmImagePlugin.py
+-rw-rw-rw-   0        0        0     1558 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/PcdImagePlugin.py
+-rw-rw-rw-   0        0        0     7013 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/PcfFontFile.py
+-rw-rw-rw-   0        0        0     6242 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/PcxImagePlugin.py
+-rw-rw-rw-   0        0        0     9264 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/PdfImagePlugin.py
+-rw-rw-rw-   0        0        0    35397 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/PdfParser.py
+-rw-rw-rw-   0        0        0     1720 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/PixarImagePlugin.py
+-rw-rw-rw-   0        0        0    47830 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/PngImagePlugin.py
+-rw-rw-rw-   0        0        0    11746 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/PpmImagePlugin.py
+-rw-rw-rw-   0        0        0     7838 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/PsdImagePlugin.py
+-rw-rw-rw-   0        0        0    10261 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/PyAccess.py
+-rw-rw-rw-   0        0        0     3722 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/QoiImagePlugin.py
+-rw-rw-rw-   0        0        0     6409 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/SgiImagePlugin.py
+-rw-rw-rw-   0        0        0     9788 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/SpiderImagePlugin.py
+-rw-rw-rw-   0        0        0     4537 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/SunImagePlugin.py
+-rw-rw-rw-   0        0        0     1557 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/TarIO.py
+-rw-rw-rw-   0        0        0     6830 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/TgaImagePlugin.py
+-rw-rw-rw-   0        0        0    79171 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/TiffImagePlugin.py
+-rw-rw-rw-   0        0        0    17374 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/TiffTags.py
+-rw-rw-rw-   0        0        0     5642 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/WalImageFile.py
+-rw-rw-rw-   0        0        0    11732 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/WebPImagePlugin.py
+-rw-rw-rw-   0        0        0     4867 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/WmfImagePlugin.py
+-rw-rw-rw-   0        0        0     2064 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/XVThumbImagePlugin.py
+-rw-rw-rw-   0        0        0     2581 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/XbmImagePlugin.py
+-rw-rw-rw-   0        0        0     3312 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/XpmImagePlugin.py
+-rw-rw-rw-   0        0        0     2063 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/__main__.py
+-rw-rw-rw-   0        0        0     2145 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/_binary.py
+-rw-rw-rw-   0        0        0     2005 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/_deprecate.py
+-rw-rw-rw-   0        0        0      520 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/_tkinter_finder.py
+-rw-rw-rw-   0        0        0      388 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/_util.py
+-rw-rw-rw-   0        0        0       53 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/_version.py
+-rw-rw-rw-   0        0        0     9947 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/PIL/features.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.765069 mylove-1.0.0/venv/Lib/site-packages/Pillow-10.0.0.dist-info/
+-rw-rw-rw-   0        0        0        4 2023-07-26 07:38:26.000000 mylove-1.0.0/venv/Lib/site-packages/Pillow-10.0.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.766065 mylove-1.0.0/venv/Lib/site-packages/Pygments-2.15.1.dist-info/
+-rw-rw-rw-   0        0        0       53 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/Pygments-2.15.1.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/Pygments-2.15.1.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.769055 mylove-1.0.0/venv/Lib/site-packages/SpeechRecognition-3.10.0.dist-info/
+-rw-rw-rw-   0        0        0    18092 2023-07-26 07:38:31.000000 mylove-1.0.0/venv/Lib/site-packages/SpeechRecognition-3.10.0.dist-info/LICENSE-FLAC.txt
+-rw-rw-rw-   0        0        0     1519 2023-07-26 07:38:31.000000 mylove-1.0.0/venv/Lib/site-packages/SpeechRecognition-3.10.0.dist-info/LICENSE.txt
+-rw-rw-rw-   0        0        0       19 2023-07-26 07:38:31.000000 mylove-1.0.0/venv/Lib/site-packages/SpeechRecognition-3.10.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.771047 mylove-1.0.0/venv/Lib/site-packages/_distutils_hack/
+-rw-rw-rw-   0        0        0     6128 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/_distutils_hack/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/_distutils_hack/override.py
+-rw-rw-rw-   0        0        0     5770 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/_virtualenv.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.776032 mylove-1.0.0/venv/Lib/site-packages/bleach/
+-rw-rw-rw-   0        0        0     3649 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.780020 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/
+-rw-rw-rw-   0        0        0        0 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.787991 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/
+-rw-rw-rw-   0        0        0     1143 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/__init__.py
+-rw-rw-rw-   0        0        0    16728 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/_ihatexml.py
+-rw-rw-rw-   0        0        0    32300 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/_inputstream.py
+-rw-rw-rw-   0        0        0    77028 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/_tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.791978 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/
+-rw-rw-rw-   0        0        0      109 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/__init__.py
+-rw-rw-rw-   0        0        0     1013 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/_base.py
+-rw-rw-rw-   0        0        0     1763 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/py.py
+-rw-rw-rw-   0        0        0     4919 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/_utils.py
+-rw-rw-rw-   0        0        0    83464 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.798954 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/
+-rw-rw-rw-   0        0        0        0 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/__init__.py
+-rw-rw-rw-   0        0        0      919 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/alphabeticalattributes.py
+-rw-rw-rw-   0        0        0      286 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/base.py
+-rw-rw-rw-   0        0        0     2945 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/inject_meta_charset.py
+-rw-rw-rw-   0        0        0     3631 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/lint.py
+-rw-rw-rw-   0        0        0    10588 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/optionaltags.py
+-rw-rw-rw-   0        0        0    26885 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/sanitizer.py
+-rw-rw-rw-   0        0        0     1214 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/whitespace.py
+-rw-rw-rw-   0        0        0   117174 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/html5parser.py
+-rw-rw-rw-   0        0        0    15747 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/serializer.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.801945 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/
+-rw-rw-rw-   0        0        0      650 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/__init__.py
+-rw-rw-rw-   0        0        0     1715 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/genshi.py
+-rw-rw-rw-   0        0        0     1776 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/sax.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.806928 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/
+-rw-rw-rw-   0        0        0     3592 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/__init__.py
+-rw-rw-rw-   0        0        0    14553 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/base.py
+-rw-rw-rw-   0        0        0     8925 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/dom.py
+-rw-rw-rw-   0        0        0    12824 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/etree.py
+-rw-rw-rw-   0        0        0    14754 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/etree_lxml.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.811915 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/
+-rw-rw-rw-   0        0        0     5719 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/__init__.py
+-rw-rw-rw-   0        0        0     7476 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/base.py
+-rw-rw-rw-   0        0        0     1413 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/dom.py
+-rw-rw-rw-   0        0        0     4539 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/etree.py
+-rw-rw-rw-   0        0        0     6345 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/etree_lxml.py
+-rw-rw-rw-   0        0        0     2309 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/genshi.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.788987 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/
+-rw-rw-rw-   0        0        0        9 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/top_level.txt
+-rw-rw-rw-   0        0        0    39023 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/parse.py
+-rw-rw-rw-   0        0        0      184 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/vendor.txt
+-rw-rw-rw-   0        0        0      752 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/callbacks.py
+-rw-rw-rw-   0        0        0     2526 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/css_sanitizer.py
+-rw-rw-rw-   0        0        0    22779 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/html5lib_shim.py
+-rw-rw-rw-   0        0        0    22350 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/linkifier.py
+-rw-rw-rw-   0        0        0       50 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/parse_shim.py
+-rw-rw-rw-   0        0        0    21934 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach/sanitizer.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.777029 mylove-1.0.0/venv/Lib/site-packages/bleach-6.0.0.dist-info/
+-rw-rw-rw-   0        0        0        7 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/bleach-6.0.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.814901 mylove-1.0.0/venv/Lib/site-packages/certifi/
+-rw-rw-rw-   0        0        0       94 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/certifi/__init__.py
+-rw-rw-rw-   0        0        0      243 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/certifi/__main__.py
+-rw-rw-rw-   0        0        0     4219 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/certifi/core.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.815897 mylove-1.0.0/venv/Lib/site-packages/certifi-2023.5.7.dist-info/
+-rw-rw-rw-   0        0        0        8 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/certifi-2023.5.7.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.822874 mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/
+-rw-rw-rw-   0        0        0     1623 2023-07-26 07:38:29.000000 mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/__init__.py
+-rw-rw-rw-   0        0        0    21723 2023-07-26 07:38:29.000000 mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/api.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.825865 mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/assets/
+-rw-rw-rw-   0        0        0    21509 2023-07-26 07:38:29.000000 mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/assets/__init__.py
+-rw-rw-rw-   0        0        0    12944 2023-07-26 07:38:29.000000 mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/cd.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.826861 mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/cli/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:38:29.000000 mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/cli/__init__.py
+-rw-rw-rw-   0        0        0    10040 2023-07-26 07:38:29.000000 mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/cli/normalizer.py
+-rw-rw-rw-   0        0        0    19596 2023-07-26 07:38:29.000000 mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/constant.py
+-rw-rw-rw-   0        0        0     2125 2023-07-26 07:38:29.000000 mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/legacy.py
+-rw-rw-rw-   0        0        0    19264 2023-07-26 07:38:29.000000 mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/md.py
+-rw-rw-rw-   0        0        0    11829 2023-07-26 07:38:29.000000 mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/models.py
+-rw-rw-rw-   0        0        0    11992 2023-07-26 07:38:29.000000 mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/utils.py
+-rw-rw-rw-   0        0        0       85 2023-07-26 07:38:29.000000 mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/version.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.824869 mylove-1.0.0/venv/Lib/site-packages/charset_normalizer-3.2.0.dist-info/
+-rw-rw-rw-   0        0        0       76 2023-07-26 07:38:29.000000 mylove-1.0.0/venv/Lib/site-packages/charset_normalizer-3.2.0.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-07-26 07:38:29.000000 mylove-1.0.0/venv/Lib/site-packages/charset_normalizer-3.2.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.834834 mylove-1.0.0/venv/Lib/site-packages/docutils/
+-rw-rw-rw-   0        0        0    10293 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/__init__.py
+-rw-rw-rw-   0        0        0     3625 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/__main__.py
+-rw-rw-rw-   0        0        0    33045 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/core.py
+-rw-rw-rw-   0        0        0     3961 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/examples.py
+-rw-rw-rw-   0        0        0    40002 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/frontend.py
+-rw-rw-rw-   0        0        0    23958 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/io.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.862741 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/
+-rw-rw-rw-   0        0        0     2921 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/__init__.py
+-rw-rw-rw-   0        0        0     1831 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/af.py
+-rw-rw-rw-   0        0        0     1943 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/ar.py
+-rw-rw-rw-   0        0        0     1912 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/ca.py
+-rw-rw-rw-   0        0        0     1900 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/cs.py
+-rw-rw-rw-   0        0        0     1856 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/da.py
+-rw-rw-rw-   0        0        0     1728 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/de.py
+-rw-rw-rw-   0        0        0     1854 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/en.py
+-rw-rw-rw-   0        0        0     1931 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/eo.py
+-rw-rw-rw-   0        0        0     1906 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/es.py
+-rw-rw-rw-   0        0        0     1958 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/fa.py
+-rw-rw-rw-   0        0        0     1964 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/fi.py
+-rw-rw-rw-   0        0        0     1831 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/fr.py
+-rw-rw-rw-   0        0        0     1990 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/gl.py
+-rw-rw-rw-   0        0        0     2692 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/he.py
+-rw-rw-rw-   0        0        0     1814 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/it.py
+-rw-rw-rw-   0        0        0     1890 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/ja.py
+-rw-rw-rw-   0        0        0     1832 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/ko.py
+-rw-rw-rw-   0        0        0     1919 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/lt.py
+-rw-rw-rw-   0        0        0     1851 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/lv.py
+-rw-rw-rw-   0        0        0     1871 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/nl.py
+-rw-rw-rw-   0        0        0     1866 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/pl.py
+-rw-rw-rw-   0        0        0     1929 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/pt_br.py
+-rw-rw-rw-   0        0        0     2070 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/ru.py
+-rw-rw-rw-   0        0        0     1832 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/sk.py
+-rw-rw-rw-   0        0        0     1863 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/sv.py
+-rw-rw-rw-   0        0        0     2062 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/uk.py
+-rw-rw-rw-   0        0        0     1974 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/zh_cn.py
+-rw-rw-rw-   0        0        0     2742 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/languages/zh_tw.py
+-rw-rw-rw-   0        0        0    81006 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/nodes.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.865731 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/
+-rw-rw-rw-   0        0        0     3724 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/__init__.py
+-rw-rw-rw-   0        0        0     1765 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/commonmark_wrapper.py
+-rw-rw-rw-   0        0        0      445 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/null.py
+-rw-rw-rw-   0        0        0     5426 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/recommonmark_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.870715 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/
+-rw-rw-rw-   0        0        0    15954 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.880963 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/directives/
+-rw-rw-rw-   0        0        0    14652 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/directives/__init__.py
+-rw-rw-rw-   0        0        0     2405 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/directives/admonitions.py
+-rw-rw-rw-   0        0        0     9883 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/directives/body.py
+-rw-rw-rw-   0        0        0      695 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/directives/html.py
+-rw-rw-rw-   0        0        0     6799 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/directives/images.py
+-rw-rw-rw-   0        0        0    26302 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/directives/misc.py
+-rw-rw-rw-   0        0        0     4247 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/directives/parts.py
+-rw-rw-rw-   0        0        0      831 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/directives/references.py
+-rw-rw-rw-   0        0        0    23825 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/directives/tables.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.913812 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/
+-rw-rw-rw-   0        0        0      670 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/README.txt
+-rw-rw-rw-   0        0        0    10925 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsa.txt
+-rw-rw-rw-   0        0        0     7242 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsb.txt
+-rw-rw-rw-   0        0        0     1723 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsc.txt
+-rw-rw-rw-   0        0        0     6721 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsn.txt
+-rw-rw-rw-   0        0        0     3825 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isoamso.txt
+-rw-rw-rw-   0        0        0    11763 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsr.txt
+-rw-rw-rw-   0        0        0     3101 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isobox.txt
+-rw-rw-rw-   0        0        0     4241 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isocyr1.txt
+-rw-rw-rw-   0        0        0     1882 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isocyr2.txt
+-rw-rw-rw-   0        0        0      869 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isodia.txt
+-rw-rw-rw-   0        0        0     3010 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk1.txt
+-rw-rw-rw-   0        0        0     1705 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk2.txt
+-rw-rw-rw-   0        0        0     2880 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk3.txt
+-rw-rw-rw-   0        0        0     3035 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk4-wide.txt
+-rw-rw-rw-   0        0        0      372 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk4.txt
+-rw-rw-rw-   0        0        0     4397 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isolat1.txt
+-rw-rw-rw-   0        0        0     8466 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isolat2.txt
+-rw-rw-rw-   0        0        0     3334 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk-wide.txt
+-rw-rw-rw-   0        0        0      519 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk.txt
+-rw-rw-rw-   0        0        0     1931 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isomopf-wide.txt
+-rw-rw-rw-   0        0        0      639 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isomopf.txt
+-rw-rw-rw-   0        0        0     3231 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isomscr-wide.txt
+-rw-rw-rw-   0        0        0      776 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isomscr.txt
+-rw-rw-rw-   0        0        0     4066 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isonum.txt
+-rw-rw-rw-   0        0        0     4613 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isopub.txt
+-rw-rw-rw-   0        0        0     9726 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isotech.txt
+-rw-rw-rw-   0        0        0    45428 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/mmlalias.txt
+-rw-rw-rw-   0        0        0     9010 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra-wide.txt
+-rw-rw-rw-   0        0        0     6800 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra.txt
+-rw-rw-rw-   0        0        0     1036 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/s5defs.txt
+-rw-rw-rw-   0        0        0     6112 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-lat1.txt
+-rw-rw-rw-   0        0        0     1945 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-special.txt
+-rw-rw-rw-   0        0        0     7028 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-symbol.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.937669 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/
+-rw-rw-rw-   0        0        0     1222 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/__init__.py
+-rw-rw-rw-   0        0        0     3727 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/af.py
+-rw-rw-rw-   0        0        0     3051 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/ar.py
+-rw-rw-rw-   0        0        0     4406 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/ca.py
+-rw-rw-rw-   0        0        0     4808 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/cs.py
+-rw-rw-rw-   0        0        0     3719 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/da.py
+-rw-rw-rw-   0        0        0     3547 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/de.py
+-rw-rw-rw-   0        0        0     3514 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/en.py
+-rw-rw-rw-   0        0        0     3825 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/eo.py
+-rw-rw-rw-   0        0        0     4158 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/es.py
+-rw-rw-rw-   0        0        0     3171 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/fa.py
+-rw-rw-rw-   0        0        0     3526 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/fi.py
+-rw-rw-rw-   0        0        0     3782 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/fr.py
+-rw-rw-rw-   0        0        0     3632 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/gl.py
+-rw-rw-rw-   0        0        0     3641 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/he.py
+-rw-rw-rw-   0        0        0     3322 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/it.py
+-rw-rw-rw-   0        0        0     3776 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/ja.py
+-rw-rw-rw-   0        0        0     3377 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/ko.py
+-rw-rw-rw-   0        0        0     3519 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/lt.py
+-rw-rw-rw-   0        0        0     3376 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/lv.py
+-rw-rw-rw-   0        0        0     3761 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/nl.py
+-rw-rw-rw-   0        0        0     3443 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/pl.py
+-rw-rw-rw-   0        0        0     3960 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/pt_br.py
+-rw-rw-rw-   0        0        0     3398 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/ru.py
+-rw-rw-rw-   0        0        0     3947 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/sk.py
+-rw-rw-rw-   0        0        0     3261 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/sv.py
+-rw-rw-rw-   0        0        0     3441 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/uk.py
+-rw-rw-rw-   0        0        0     3925 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/zh_cn.py
+-rw-rw-rw-   0        0        0     5160 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/zh_tw.py
+-rw-rw-rw-   0        0        0    16119 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/roles.py
+-rw-rw-rw-   0        0        0   132550 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/states.py
+-rw-rw-rw-   0        0        0    20912 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/tableparser.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.940659 mylove-1.0.0/venv/Lib/site-packages/docutils/readers/
+-rw-rw-rw-   0        0        0     3520 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/readers/__init__.py
+-rw-rw-rw-   0        0        0     1607 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/readers/doctree.py
+-rw-rw-rw-   0        0        0     1523 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/readers/pep.py
+-rw-rw-rw-   0        0        0     2324 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/readers/standalone.py
+-rw-rw-rw-   0        0        0    56956 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/statemachine.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.948632 mylove-1.0.0/venv/Lib/site-packages/docutils/transforms/
+-rw-rw-rw-   0        0        0     6870 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/transforms/__init__.py
+-rw-rw-rw-   0        0        0     2151 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/transforms/components.py
+-rw-rw-rw-   0        0        0    21371 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/transforms/frontmatter.py
+-rw-rw-rw-   0        0        0     4873 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/transforms/misc.py
+-rw-rw-rw-   0        0        0     6912 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/transforms/parts.py
+-rw-rw-rw-   0        0        0    11111 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/transforms/peps.py
+-rw-rw-rw-   0        0        0    36819 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/transforms/references.py
+-rw-rw-rw-   0        0        0    12548 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/transforms/universal.py
+-rw-rw-rw-   0        0        0     3057 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/transforms/writer_aux.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.954612 mylove-1.0.0/venv/Lib/site-packages/docutils/utils/
+-rw-rw-rw-   0        0        0    29382 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/utils/__init__.py
+-rw-rw-rw-   0        0        0     4920 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/utils/code_analyzer.py
+-rw-rw-rw-   0        0        0     8105 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/utils/error_reporting.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.959595 mylove-1.0.0/venv/Lib/site-packages/docutils/utils/math/
+-rw-rw-rw-   0        0        0     1825 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/utils/math/__init__.py
+-rw-rw-rw-   0        0        0    51496 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/utils/math/latex2mathml.py
+-rw-rw-rw-   0        0        0   107993 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/utils/math/math2html.py
+-rw-rw-rw-   0        0        0     6760 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/utils/math/tex2mathml_extern.py
+-rw-rw-rw-   0        0        0    37497 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/utils/math/tex2unichar.py
+-rw-rw-rw-   0        0        0    18393 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/utils/math/unichar2tex.py
+-rw-rw-rw-   0        0        0     5747 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/utils/punctuation_chars.py
+-rw-rw-rw-   0        0        0     2695 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/utils/roman.py
+-rw-rw-rw-   0        0        0    38972 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/utils/smartquotes.py
+-rw-rw-rw-   0        0        0     6260 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/utils/urischemes.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.964582 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/
+-rw-rw-rw-   0        0        0     4945 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/__init__.py
+-rw-rw-rw-   0        0        0    70896 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/_html_base.py
+-rw-rw-rw-   0        0        0     6763 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/docutils_xml.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.966573 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/html4css1/
+-rw-rw-rw-   0        0        0    37675 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/html4css1/__init__.py
+-rw-rw-rw-   0        0        0      114 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/html4css1/template.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.967570 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/html5_polyglot/
+-rw-rw-rw-   0        0        0    16718 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/html5_polyglot/__init__.py
+-rw-rw-rw-   0        0        0      114 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/html5_polyglot/template.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.968566 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/latex2e/
+-rw-rw-rw-   0        0        0   137132 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/latex2e/__init__.py
+-rw-rw-rw-   0        0        0    36654 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/manpage.py
+-rw-rw-rw-   0        0        0      568 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/null.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.971557 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/odf_odt/
+-rw-rw-rw-   0        0        0   132358 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/odf_odt/__init__.py
+-rw-rw-rw-   0        0        0     2142 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/odf_odt/prepstyles.py
+-rw-rw-rw-   0        0        0     4681 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/odf_odt/pygmentsformatter.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.973549 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/pep_html/
+-rw-rw-rw-   0        0        0     3505 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/pep_html/__init__.py
+-rw-rw-rw-   0        0        0     1001 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/pep_html/template.txt
+-rw-rw-rw-   0        0        0     1032 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/pseudoxml.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.974547 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/s5_html/
+-rw-rw-rw-   0        0        0    14517 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/s5_html/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.975543 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/s5_html/themes/
+-rw-rw-rw-   0        0        0      278 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/s5_html/themes/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.975543 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/xetex/
+-rw-rw-rw-   0        0        0     5736 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils/writers/xetex/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.836828 mylove-1.0.0/venv/Lib/site-packages/docutils-0.20.1.dist-info/
+-rw-rw-rw-   0        0        0     6292 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils-0.20.1.dist-info/COPYING.txt
+-rw-rw-rw-   0        0        0       53 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils-0.20.1.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Lib/site-packages/docutils-0.20.1.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.982520 mylove-1.0.0/venv/Lib/site-packages/idna/
+-rw-rw-rw-   0        0        0      849 2023-07-26 07:38:28.000000 mylove-1.0.0/venv/Lib/site-packages/idna/__init__.py
+-rw-rw-rw-   0        0        0     3374 2023-07-26 07:38:28.000000 mylove-1.0.0/venv/Lib/site-packages/idna/codec.py
+-rw-rw-rw-   0        0        0      321 2023-07-26 07:38:28.000000 mylove-1.0.0/venv/Lib/site-packages/idna/compat.py
+-rw-rw-rw-   0        0        0    12950 2023-07-26 07:38:28.000000 mylove-1.0.0/venv/Lib/site-packages/idna/core.py
+-rw-rw-rw-   0        0        0    44375 2023-07-26 07:38:28.000000 mylove-1.0.0/venv/Lib/site-packages/idna/idnadata.py
+-rw-rw-rw-   0        0        0     1881 2023-07-26 07:38:28.000000 mylove-1.0.0/venv/Lib/site-packages/idna/intranges.py
+-rw-rw-rw-   0        0        0       21 2023-07-26 07:38:28.000000 mylove-1.0.0/venv/Lib/site-packages/idna/package_data.py
+-rw-rw-rw-   0        0        0   206539 2023-07-26 07:38:29.000000 mylove-1.0.0/venv/Lib/site-packages/idna/uts46data.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.989999 mylove-1.0.0/venv/Lib/site-packages/importlib_metadata/
+-rw-rw-rw-   0        0        0    30749 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/importlib_metadata/__init__.py
+-rw-rw-rw-   0        0        0     2454 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/importlib_metadata/_adapters.py
+-rw-rw-rw-   0        0        0      743 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/importlib_metadata/_collections.py
+-rw-rw-rw-   0        0        0     1554 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/importlib_metadata/_compat.py
+-rw-rw-rw-   0        0        0     2895 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/importlib_metadata/_functools.py
+-rw-rw-rw-   0        0        0     2068 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/importlib_metadata/_itertools.py
+-rw-rw-rw-   0        0        0     1613 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/importlib_metadata/_meta.py
+-rw-rw-rw-   0        0        0     1098 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/importlib_metadata/_py39compat.py
+-rw-rw-rw-   0        0        0     2166 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/importlib_metadata/_text.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.990999 mylove-1.0.0/venv/Lib/site-packages/importlib_metadata-6.8.0.dist-info/
+-rw-rw-rw-   0        0        0       19 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/importlib_metadata-6.8.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.609863 mylove-1.0.0/venv/Lib/site-packages/jaraco/
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.995494 mylove-1.0.0/venv/Lib/site-packages/jaraco/classes/
+-rw-rw-rw-   0        0        0        0 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/jaraco/classes/__init__.py
+-rw-rw-rw-   0        0        0     1464 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/jaraco/classes/ancestry.py
+-rw-rw-rw-   0        0        0     1853 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/jaraco/classes/meta.py
+-rw-rw-rw-   0        0        0     3996 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/jaraco/classes/properties.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.991996 mylove-1.0.0/venv/Lib/site-packages/jaraco.classes-3.3.0.dist-info/
+-rw-rw-rw-   0        0        0        7 2023-07-26 08:06:11.000000 mylove-1.0.0/venv/Lib/site-packages/jaraco.classes-3.3.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.006456 mylove-1.0.0/venv/Lib/site-packages/keyring/
+-rw-rw-rw-   0        0        0      271 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/__init__.py
+-rw-rw-rw-   0        0        0       71 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/__main__.py
+-rw-rw-rw-   0        0        0      185 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/_compat.py
+-rw-rw-rw-   0        0        0     3886 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/_properties_compat.py
+-rw-rw-rw-   0        0        0     8100 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/backend.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.015426 mylove-1.0.0/venv/Lib/site-packages/keyring/backends/
+-rw-rw-rw-   0        0        0     4692 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/backends/SecretService.py
+-rw-rw-rw-   0        0        0     5814 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/backends/Windows.py
+-rw-rw-rw-   0        0        0        0 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/backends/__init__.py
+-rw-rw-rw-   0        0        0     2173 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/backends/chainer.py
+-rw-rw-rw-   0        0        0      929 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/backends/fail.py
+-rw-rw-rw-   0        0        0     5830 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/backends/kwallet.py
+-rw-rw-rw-   0        0        0     5982 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/backends/libsecret.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.017420 mylove-1.0.0/venv/Lib/site-packages/keyring/backends/macOS/
+-rw-rw-rw-   0        0        0     2689 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/backends/macOS/__init__.py
+-rw-rw-rw-   0        0        0     4341 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/backends/macOS/api.py
+-rw-rw-rw-   0        0        0      453 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/backends/null.py
+-rw-rw-rw-   0        0        0     4475 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/cli.py
+-rw-rw-rw-   0        0        0     1324 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/completion.py
+-rw-rw-rw-   0        0        0     5731 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/core.py
+-rw-rw-rw-   0        0        0     1593 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/credentials.py
+-rw-rw-rw-   0        0        0      752 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/devpi_client.py
+-rw-rw-rw-   0        0        0     1430 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/errors.py
+-rw-rw-rw-   0        0        0     1231 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/http.py
+-rw-rw-rw-   0        0        0      175 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/py312compat.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.019420 mylove-1.0.0/venv/Lib/site-packages/keyring/testing/
+-rw-rw-rw-   0        0        0        0 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/testing/__init__.py
+-rw-rw-rw-   0        0        0     6598 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/testing/backend.py
+-rw-rw-rw-   0        0        0     1918 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/testing/util.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.020411 mylove-1.0.0/venv/Lib/site-packages/keyring/util/
+-rw-rw-rw-   0        0        0      868 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/util/__init__.py
+-rw-rw-rw-   0        0        0     2215 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring/util/platform_.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.008449 mylove-1.0.0/venv/Lib/site-packages/keyring-24.2.0.dist-info/
+-rw-rw-rw-   0        0        0      334 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring-24.2.0.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/keyring-24.2.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.031374 mylove-1.0.0/venv/Lib/site-packages/markdown_it/
+-rw-rw-rw-   0        0        0      113 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/__init__.py
+-rw-rw-rw-   0        0        0      246 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/_compat.py
+-rw-rw-rw-   0        0        0     2364 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/_punycode.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.032370 mylove-1.0.0/venv/Lib/site-packages/markdown_it/cli/
+-rw-rw-rw-   0        0        0        0 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/cli/__init__.py
+-rw-rw-rw-   0        0        0     2901 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/cli/parse.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.037353 mylove-1.0.0/venv/Lib/site-packages/markdown_it/common/
+-rw-rw-rw-   0        0        0        0 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/common/__init__.py
+-rw-rw-rw-   0        0        0      156 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/common/entities.py
+-rw-rw-rw-   0        0        0      932 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/common/html_blocks.py
+-rw-rw-rw-   0        0        0      929 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/common/html_re.py
+-rw-rw-rw-   0        0        0     2568 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/common/normalize_url.py
+-rw-rw-rw-   0        0        0    10728 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/common/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.041340 mylove-1.0.0/venv/Lib/site-packages/markdown_it/helpers/
+-rw-rw-rw-   0        0        0      253 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1977 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/helpers/parse_link_destination.py
+-rw-rw-rw-   0        0        0     1036 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/helpers/parse_link_label.py
+-rw-rw-rw-   0        0        0     1425 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/helpers/parse_link_title.py
+-rw-rw-rw-   0        0        0    12772 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/main.py
+-rw-rw-rw-   0        0        0     3911 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/parser_block.py
+-rw-rw-rw-   0        0        0     1010 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/parser_core.py
+-rw-rw-rw-   0        0        0     4997 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/parser_inline.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.044330 mylove-1.0.0/venv/Lib/site-packages/markdown_it/presets/
+-rw-rw-rw-   0        0        0      970 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/presets/__init__.py
+-rw-rw-rw-   0        0        0     2868 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/presets/commonmark.py
+-rw-rw-rw-   0        0        0     1810 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/presets/default.py
+-rw-rw-rw-   0        0        0     2112 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/presets/zero.py
+-rw-rw-rw-   0        0        0     9970 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/renderer.py
+-rw-rw-rw-   0        0        0     9199 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/ruler.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.054297 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/
+-rw-rw-rw-   0        0        0      553 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/__init__.py
+-rw-rw-rw-   0        0        0     8887 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/blockquote.py
+-rw-rw-rw-   0        0        0      859 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/code.py
+-rw-rw-rw-   0        0        0     2537 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/fence.py
+-rw-rw-rw-   0        0        0     1746 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/heading.py
+-rw-rw-rw-   0        0        0     1226 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/hr.py
+-rw-rw-rw-   0        0        0     2721 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/html_block.py
+-rw-rw-rw-   0        0        0     2625 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/lheading.py
+-rw-rw-rw-   0        0        0     9668 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/list.py
+-rw-rw-rw-   0        0        0     1818 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/paragraph.py
+-rw-rw-rw-   0        0        0     6168 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/reference.py
+-rw-rw-rw-   0        0        0     8422 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/state_block.py
+-rw-rw-rw-   0        0        0     6987 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/table.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.062271 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_core/
+-rw-rw-rw-   0        0        0      394 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_core/__init__.py
+-rw-rw-rw-   0        0        0      372 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_core/block.py
+-rw-rw-rw-   0        0        0      325 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_core/inline.py
+-rw-rw-rw-   0        0        0     5141 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_core/linkify.py
+-rw-rw-rw-   0        0        0      402 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_core/normalize.py
+-rw-rw-rw-   0        0        0     3470 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_core/replacements.py
+-rw-rw-rw-   0        0        0     7443 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_core/smartquotes.py
+-rw-rw-rw-   0        0        0      570 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_core/state_core.py
+-rw-rw-rw-   0        0        0     1172 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_core/text_join.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.074230 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/
+-rw-rw-rw-   0        0        0      696 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/__init__.py
+-rw-rw-rw-   0        0        0     2079 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/autolink.py
+-rw-rw-rw-   0        0        0     2037 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/backticks.py
+-rw-rw-rw-   0        0        0     4851 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/balance_pairs.py
+-rw-rw-rw-   0        0        0     3123 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/emphasis.py
+-rw-rw-rw-   0        0        0     1651 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/entity.py
+-rw-rw-rw-   0        0        0     1658 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/escape.py
+-rw-rw-rw-   0        0        0     1493 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/fragments_join.py
+-rw-rw-rw-   0        0        0     1130 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/html_inline.py
+-rw-rw-rw-   0        0        0     4135 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/image.py
+-rw-rw-rw-   0        0        0     4318 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/link.py
+-rw-rw-rw-   0        0        0     1704 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/linkify.py
+-rw-rw-rw-   0        0        0     1296 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/newline.py
+-rw-rw-rw-   0        0        0     5101 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/state_inline.py
+-rw-rw-rw-   0        0        0     3214 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/strikethrough.py
+-rw-rw-rw-   0        0        0      901 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/text.py
+-rw-rw-rw-   0        0        0     6439 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/token.py
+-rw-rw-rw-   0        0        0    11421 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/tree.py
+-rw-rw-rw-   0        0        0     5365 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.075235 mylove-1.0.0/venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/
+-rw-rw-rw-   0        0        0       58 2023-07-26 08:06:10.000000 mylove-1.0.0/venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/entry_points.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.081207 mylove-1.0.0/venv/Lib/site-packages/mdurl/
+-rw-rw-rw-   0        0        0      547 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/mdurl/__init__.py
+-rw-rw-rw-   0        0        0     3004 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/mdurl/_decode.py
+-rw-rw-rw-   0        0        0     2602 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/mdurl/_encode.py
+-rw-rw-rw-   0        0        0      626 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/mdurl/_format.py
+-rw-rw-rw-   0        0        0    11374 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/mdurl/_parse.py
+-rw-rw-rw-   0        0        0      284 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/mdurl/_url.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.084198 mylove-1.0.0/venv/Lib/site-packages/more_itertools/
+-rw-rw-rw-   0        0        0      149 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/more_itertools/__init__.py
+-rw-rw-rw-   0        0        0   139056 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/more_itertools/more.py
+-rw-rw-rw-   0        0        0    26447 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/more_itertools/recipes.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.086190 mylove-1.0.0/venv/Lib/site-packages/pip/
+-rw-rw-rw-   0        0        0      357 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pip/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pip/__main__.py
+-rw-rw-rw-   0        0        0     1444 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pip/__pip-runner__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.096157 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/
+-rw-rw-rw-   0        0        0      573 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/__init__.py
+-rw-rw-rw-   0        0        0    10234 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/build_env.py
+-rw-rw-rw-   0        0        0    10734 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cache.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.107628 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cli/
+-rw-rw-rw-   0        0        0      132 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cli/__init__.py
+-rw-rw-rw-   0        0        0     6676 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py
+-rw-rw-rw-   0        0        0     7842 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cli/base_command.py
+-rw-rw-rw-   0        0        0    29381 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-rw-rw-   0        0        0      774 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cli/command_context.py
+-rw-rw-rw-   0        0        0     2472 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cli/main.py
+-rw-rw-rw-   0        0        0     4338 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cli/main_parser.py
+-rw-rw-rw-   0        0        0    10817 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cli/parser.py
+-rw-rw-rw-   0        0        0     1968 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py
+-rw-rw-rw-   0        0        0    18172 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cli/req_command.py
+-rw-rw-rw-   0        0        0     5118 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cli/spinners.py
+-rw-rw-rw-   0        0        0      116 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cli/status_codes.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.123092 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/
+-rw-rw-rw-   0        0        0     3882 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/__init__.py
+-rw-rw-rw-   0        0        0     7582 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/cache.py
+-rw-rw-rw-   0        0        0     1685 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/check.py
+-rw-rw-rw-   0        0        0     4129 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/completion.py
+-rw-rw-rw-   0        0        0     9815 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/configuration.py
+-rw-rw-rw-   0        0        0     6573 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/debug.py
+-rw-rw-rw-   0        0        0     5289 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/download.py
+-rw-rw-rw-   0        0        0     2951 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/freeze.py
+-rw-rw-rw-   0        0        0     1703 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/hash.py
+-rw-rw-rw-   0        0        0     1132 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/help.py
+-rw-rw-rw-   0        0        0     4762 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/index.py
+-rw-rw-rw-   0        0        0     3374 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/inspect.py
+-rw-rw-rw-   0        0        0    31726 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/install.py
+-rw-rw-rw-   0        0        0    12343 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/list.py
+-rw-rw-rw-   0        0        0     5697 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/search.py
+-rw-rw-rw-   0        0        0     6129 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/show.py
+-rw-rw-rw-   0        0        0     3680 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/uninstall.py
+-rw-rw-rw-   0        0        0     7396 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/wheel.py
+-rw-rw-rw-   0        0        0    13529 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/configuration.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.128083 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/distributions/
+-rw-rw-rw-   0        0        0      858 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/distributions/__init__.py
+-rw-rw-rw-   0        0        0     1221 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/distributions/base.py
+-rw-rw-rw-   0        0        0      729 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/distributions/installed.py
+-rw-rw-rw-   0        0        0     6494 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/distributions/sdist.py
+-rw-rw-rw-   0        0        0     1164 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/distributions/wheel.py
+-rw-rw-rw-   0        0        0    20942 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.132063 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/index/
+-rw-rw-rw-   0        0        0       30 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/index/__init__.py
+-rw-rw-rw-   0        0        0    16503 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/index/collector.py
+-rw-rw-rw-   0        0        0    37596 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/index/package_finder.py
+-rw-rw-rw-   0        0        0     6557 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/index/sources.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.135052 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/locations/
+-rw-rw-rw-   0        0        0    17552 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/locations/__init__.py
+-rw-rw-rw-   0        0        0     6302 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/locations/_distutils.py
+-rw-rw-rw-   0        0        0     7867 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-rw-rw-   0        0        0     2573 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/locations/base.py
+-rw-rw-rw-   0        0        0      340 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/main.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.139038 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/metadata/
+-rw-rw-rw-   0        0        0     4280 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/metadata/__init__.py
+-rw-rw-rw-   0        0        0     2595 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/metadata/_json.py
+-rw-rw-rw-   0        0        0    25277 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/metadata/base.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.142028 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/
+-rw-rw-rw-   0        0        0      107 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-rw-rw-   0        0        0     1882 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-rw-rw-   0        0        0     8181 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-rw-rw-   0        0        0     7457 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-rw-rw-   0        0        0     9773 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.153987 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/
+-rw-rw-rw-   0        0        0       63 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/__init__.py
+-rw-rw-rw-   0        0        0      990 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/candidate.py
+-rw-rw-rw-   0        0        0     5877 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/direct_url.py
+-rw-rw-rw-   0        0        0     2520 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/format_control.py
+-rw-rw-rw-   0        0        0     1030 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/index.py
+-rw-rw-rw-   0        0        0     2617 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/installation_report.py
+-rw-rw-rw-   0        0        0    18083 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/link.py
+-rw-rw-rw-   0        0        0      738 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/scheme.py
+-rw-rw-rw-   0        0        0     4644 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/search_scope.py
+-rw-rw-rw-   0        0        0     1907 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py
+-rw-rw-rw-   0        0        0     3858 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/target_python.py
+-rw-rw-rw-   0        0        0     3600 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/wheel.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.162471 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/network/
+-rw-rw-rw-   0        0        0       50 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/network/__init__.py
+-rw-rw-rw-   0        0        0    12190 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/network/auth.py
+-rw-rw-rw-   0        0        0     2145 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/network/cache.py
+-rw-rw-rw-   0        0        0     6096 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/network/download.py
+-rw-rw-rw-   0        0        0     7638 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-rw-rw-   0        0        0    18443 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/network/session.py
+-rw-rw-rw-   0        0        0     4073 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/network/utils.py
+-rw-rw-rw-   0        0        0     1791 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.165459 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.171439 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/build/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/build/__init__.py
+-rw-rw-rw-   0        0        0     4133 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-rw-rw-   0        0        0     1404 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py
+-rw-rw-rw-   0        0        0     1456 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-rw-rw-   0        0        0     2198 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-rw-rw-   0        0        0     1063 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py
+-rw-rw-rw-   0        0        0     1405 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-rw-rw-   0        0        0     3064 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-rw-rw-   0        0        0     5109 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/check.py
+-rw-rw-rw-   0        0        0     9784 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/freeze.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.174429 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/install/
+-rw-rw-rw-   0        0        0       51 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/install/__init__.py
+-rw-rw-rw-   0        0        0     1354 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-rw-rw-   0        0        0     4105 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py
+-rw-rw-rw-   0        0        0    27407 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py
+-rw-rw-rw-   0        0        0    25091 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/prepare.py
+-rw-rw-rw-   0        0        0     7074 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/pyproject.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.179413 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/req/
+-rw-rw-rw-   0        0        0     2807 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/req/__init__.py
+-rw-rw-rw-   0        0        0    16611 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/req/constructors.py
+-rw-rw-rw-   0        0        0    17646 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/req/req_file.py
+-rw-rw-rw-   0        0        0    35600 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/req/req_install.py
+-rw-rw-rw-   0        0        0     2858 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/req/req_set.py
+-rw-rw-rw-   0        0        0    24045 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.181406 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/__init__.py
+-rw-rw-rw-   0        0        0      583 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/base.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.182402 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/legacy/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-rw-rw-   0        0        0    24129 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.189379 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-rw-rw-   0        0        0     5220 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-rw-rw-   0        0        0    18963 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-rw-rw-   0        0        0    27878 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-rw-rw-   0        0        0     5705 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-rw-rw-   0        0        0     9914 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-rw-rw-   0        0        0     2526 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-rw-rw-   0        0        0     5455 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-rw-rw-   0        0        0    11533 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-rw-rw-   0        0        0     8020 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/self_outdated_check.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.216120 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/__init__.py
+-rw-rw-rw-   0        0        0     1015 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/_log.py
+-rw-rw-rw-   0        0        0     1665 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/appdirs.py
+-rw-rw-rw-   0        0        0     1884 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/compat.py
+-rw-rw-rw-   0        0        0     5377 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-rw-rw-   0        0        0      242 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/datetime.py
+-rw-rw-rw-   0        0        0     5764 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/deprecation.py
+-rw-rw-rw-   0        0        0     3206 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-rw-rw-   0        0        0     1115 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py
+-rw-rw-rw-   0        0        0     2203 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/egg_link.py
+-rw-rw-rw-   0        0        0     1169 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/encoding.py
+-rw-rw-rw-   0        0        0     3064 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py
+-rw-rw-rw-   0        0        0     5122 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/filesystem.py
+-rw-rw-rw-   0        0        0      716 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/filetypes.py
+-rw-rw-rw-   0        0        0     3110 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/glibc.py
+-rw-rw-rw-   0        0        0     4831 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/hashes.py
+-rw-rw-rw-   0        0        0      795 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-rw-rw-   0        0        0    11632 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/logging.py
+-rw-rw-rw-   0        0        0    21617 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/misc.py
+-rw-rw-rw-   0        0        0     1193 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/models.py
+-rw-rw-rw-   0        0        0     2108 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/packaging.py
+-rw-rw-rw-   0        0        0     5662 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-rw-rw-   0        0        0     9197 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/subprocess.py
+-rw-rw-rw-   0        0        0     7702 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
+-rw-rw-rw-   0        0        0     8821 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/unpacking.py
+-rw-rw-rw-   0        0        0     1759 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/urls.py
+-rw-rw-rw-   0        0        0     3459 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py
+-rw-rw-rw-   0        0        0     4549 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/wheel.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.222416 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/vcs/
+-rw-rw-rw-   0        0        0      596 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/vcs/__init__.py
+-rw-rw-rw-   0        0        0     3518 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
+-rw-rw-rw-   0        0        0    18116 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/vcs/git.py
+-rw-rw-rw-   0        0        0     5238 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
+-rw-rw-rw-   0        0        0    11728 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/vcs/subversion.py
+-rw-rw-rw-   0        0        0    22811 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-rw-rw-   0        0        0    13079 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_internal/wheel_builder.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.226400 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/
+-rw-rw-rw-   0        0        0     4966 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.236571 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/
+-rw-rw-rw-   0        0        0      465 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-rw-rw-   0        0        0     1379 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-rw-rw-   0        0        0     5033 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-rw-rw-   0        0        0     1535 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.238564 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/
+-rw-rw-rw-   0        0        0      242 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-rw-rw-   0        0        0     5271 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-rw-rw-   0        0        0     1033 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-rw-rw-   0        0        0      778 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-rw-rw-   0        0        0    16416 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-rw-rw-   0        0        0     3946 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-rw-rw-   0        0        0     4154 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-rw-rw-   0        0        0     7105 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-rw-rw-   0        0        0      774 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.241563 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/certifi/
+-rw-rw-rw-   0        0        0       94 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
+-rw-rw-rw-   0        0        0      255 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
+-rw-rw-rw-   0        0        0     4279 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/certifi/core.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.287622 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/
+-rw-rw-rw-   0        0        0     3705 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
+-rw-rw-rw-   0        0        0    31274 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-rw-rw-   0        0        0     1741 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-rw-rw-   0        0        0     9608 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-rw-rw-   0        0        0     3817 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-rw-rw-   0        0        0     4801 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.288619 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/cli/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-rw-rw-   0        0        0     2406 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-rw-rw-   0        0        0     3559 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-rw-rw-   0        0        0     1838 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-rw-rw-   0        0        0     1619 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/enums.py
+-rw-rw-rw-   0        0        0     3864 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
+-rw-rw-rw-   0        0        0    12021 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
+-rw-rw-rw-   0        0        0     3676 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-rw-rw-   0        0        0    13566 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-rw-rw-   0        0        0     1731 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-rw-rw-   0        0        0    36913 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-rw-rw-   0        0        0     1731 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-rw-rw-   0        0        0    20735 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-rw-rw-   0        0        0     1737 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-rw-rw-   0        0        0    13919 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-rw-rw-   0        0        0    25796 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-rw-rw-   0        0        0    42498 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-rw-rw-   0        0        0     1730 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-rw-rw-   0        0        0    26797 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-rw-rw-   0        0        0   104562 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-rw-rw-   0        0        0    98484 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-rw-rw-   0        0        0    98196 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-rw-rw-   0        0        0   101363 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-rw-rw-   0        0        0   128035 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-rw-rw-   0        0        0   102774 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-rw-rw-   0        0        0    95372 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-rw-rw-   0        0        0     5260 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-rw-rw-   0        0        0     3367 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-rw-rw-   0        0        0     2056 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-rw-rw-   0        0        0    30068 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.290613 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/metadata/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-rw-rw-   0        0        0    13280 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-rw-rw-   0        0        0     6199 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-rw-rw-   0        0        0     4129 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-rw-rw-   0        0        0     3749 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-rw-rw-   0        0        0    13288 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-rw-rw-   0        0        0     8289 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-rw-rw-   0        0        0     2709 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-rw-rw-   0        0        0      242 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/version.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.297777 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/colorama/
+-rw-rw-rw-   0        0        0      239 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
+-rw-rw-rw-   0        0        0    10830 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-rw-rw-   0        0        0     1915 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
+-rw-rw-rw-   0        0        0     5404 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/colorama/win32.py
+-rw-rw-rw-   0        0        0     6438 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.310565 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/
+-rw-rw-rw-   0        0        0      581 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
+-rw-rw-rw-   0        0        0    41259 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/compat.py
+-rw-rw-rw-   0        0        0    51697 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/database.py
+-rw-rw-rw-   0        0        0    20834 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/index.py
+-rw-rw-rw-   0        0        0    51991 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/locators.py
+-rw-rw-rw-   0        0        0    14811 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
+-rw-rw-rw-   0        0        0     5058 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/markers.py
+-rw-rw-rw-   0        0        0    39801 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
+-rw-rw-rw-   0        0        0    10820 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/resources.py
+-rw-rw-rw-   0        0        0    18102 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
+-rw-rw-rw-   0        0        0    66262 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/util.py
+-rw-rw-rw-   0        0        0    23513 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/version.py
+-rw-rw-rw-   0        0        0    43898 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.313995 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distro/
+-rw-rw-rw-   0        0        0      981 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distro/__init__.py
+-rw-rw-rw-   0        0        0       64 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distro/__main__.py
+-rw-rw-rw-   0        0        0    48841 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distro/distro.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.321833 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/idna/
+-rw-rw-rw-   0        0        0      849 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/idna/__init__.py
+-rw-rw-rw-   0        0        0     3374 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/idna/codec.py
+-rw-rw-rw-   0        0        0      321 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/idna/compat.py
+-rw-rw-rw-   0        0        0    12950 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/idna/core.py
+-rw-rw-rw-   0        0        0    44375 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
+-rw-rw-rw-   0        0        0     1881 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/idna/intranges.py
+-rw-rw-rw-   0        0        0       21 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/idna/package_data.py
+-rw-rw-rw-   0        0        0   206539 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.325818 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/msgpack/
+-rw-rw-rw-   0        0        0     1132 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-rw-rw-   0        0        0     1081 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-rw-rw-   0        0        0     6080 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py
+-rw-rw-rw-   0        0        0    34557 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.334886 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/packaging/
+-rw-rw-rw-   0        0        0      661 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
+-rw-rw-rw-   0        0        0      497 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0    11488 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     4378 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     1431 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     8487 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     4676 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    30110 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    15699 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4200 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    14665 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.343446 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pep517/
+-rw-rw-rw-   0        0        0      130 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pep517/__init__.py
+-rw-rw-rw-   0        0        0      138 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pep517/_compat.py
+-rw-rw-rw-   0        0        0     3443 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pep517/build.py
+-rw-rw-rw-   0        0        0     6083 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pep517/check.py
+-rw-rw-rw-   0        0        0     3994 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pep517/colorlog.py
+-rw-rw-rw-   0        0        0      607 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pep517/dirtools.py
+-rw-rw-rw-   0        0        0     6081 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pep517/envbuild.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.346769 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pep517/in_process/
+-rw-rw-rw-   0        0        0      872 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pep517/in_process/__init__.py
+-rw-rw-rw-   0        0        0    10801 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pep517/in_process/_in_process.py
+-rw-rw-rw-   0        0        0     2520 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pep517/meta.py
+-rw-rw-rw-   0        0        0    12721 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pep517/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.348763 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/
+-rw-rw-rw-   0        0        0   108287 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-rw-rw-   0        0        0      562 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.353745 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/platformdirs/
+-rw-rw-rw-   0        0        0    12831 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-rw-rw-   0        0        0     1176 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-rw-rw-   0        0        0     4068 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py
+-rw-rw-rw-   0        0        0     4910 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py
+-rw-rw-rw-   0        0        0     2655 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-rw-rw-   0        0        0     6910 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-rw-rw-   0        0        0       78 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/platformdirs/version.py
+-rw-rw-rw-   0        0        0     6439 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.367279 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/
+-rw-rw-rw-   0        0        0     2999 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py
+-rw-rw-rw-   0        0        0      353 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/__main__.py
+-rw-rw-rw-   0        0        0    23685 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-rw-rw-   0        0        0     1697 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/console.py
+-rw-rw-rw-   0        0        0     1938 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/filter.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.367279 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/filters/
+-rw-rw-rw-   0        0        0    40386 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-rw-rw-   0        0        0     2917 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.380680 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/
+-rw-rw-rw-   0        0        0     4810 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-rw-rw-   0        0        0     4104 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-rw-rw-   0        0        0     3314 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-rw-rw-   0        0        0     5086 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-rw-rw-   0        0        0    35441 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-rw-rw-   0        0        0    21938 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-rw-rw-   0        0        0     5871 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-rw-rw-   0        0        0    19351 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-rw-rw-   0        0        0     5073 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-rw-rw-   0        0        0     2212 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-rw-rw-   0        0        0     5014 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-rw-rw-   0        0        0     7335 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-rw-rw-   0        0        0     4674 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-rw-rw-   0        0        0    11753 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-rw-rw-   0        0        0    32005 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.384161 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/
+-rw-rw-rw-   0        0        0    11174 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-rw-rw-   0        0        0    70232 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-rw-rw-   0        0        0    53376 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-rw-rw-   0        0        0      986 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py
+-rw-rw-rw-   0        0        0     2591 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py
+-rw-rw-rw-   0        0        0     3072 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-rw-rw-   0        0        0     3092 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py
+-rw-rw-rw-   0        0        0     4630 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-rw-rw-   0        0        0     6257 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/style.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.385215 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/styles/
+-rw-rw-rw-   0        0        0     3419 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-rw-rw-   0        0        0     6184 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/token.py
+-rw-rw-rw-   0        0        0    63187 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py
+-rw-rw-rw-   0        0        0     9110 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/util.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.394915 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/
+-rw-rw-rw-   0        0        0     9171 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-rw-rw-   0        0        0     6426 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-rw-rw-   0        0        0    12936 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py
+-rw-rw-rw-   0        0        0   213344 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.395912 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/
+-rw-rw-rw-   0        0        0    23685 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-rw-rw-   0        0        0     9023 2023-07-26 07:30:19.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-rw-rw-   0        0        0    39129 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-rw-rw-   0        0        0    25341 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py
+-rw-rw-rw-   0        0        0    13402 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-rw-rw-   0        0        0    10787 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-rw-rw-   0        0        0     6805 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.416384 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/
+-rw-rw-rw-   0        0        0     5178 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/__init__.py
+-rw-rw-rw-   0        0        0      440 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/__version__.py
+-rw-rw-rw-   0        0        0     1397 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-rw-rw-   0        0        0    21443 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/adapters.py
+-rw-rw-rw-   0        0        0     6377 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/api.py
+-rw-rw-rw-   0        0        0    10187 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/auth.py
+-rw-rw-rw-   0        0        0      575 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/certs.py
+-rw-rw-rw-   0        0        0     1286 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/compat.py
+-rw-rw-rw-   0        0        0    18560 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/cookies.py
+-rw-rw-rw-   0        0        0     3823 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
+-rw-rw-rw-   0        0        0     3879 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/help.py
+-rw-rw-rw-   0        0        0      733 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/hooks.py
+-rw-rw-rw-   0        0        0    35287 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/models.py
+-rw-rw-rw-   0        0        0      695 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/packages.py
+-rw-rw-rw-   0        0        0    30180 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/sessions.py
+-rw-rw-rw-   0        0        0     4235 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
+-rw-rw-rw-   0        0        0     2912 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/structures.py
+-rw-rw-rw-   0        0        0    33240 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.421366 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/resolvelib/
+-rw-rw-rw-   0        0        0      537 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.422362 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-rw-rw-   0        0        0      156 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-rw-rw-   0        0        0     5872 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-rw-rw-   0        0        0     1583 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-rw-rw-   0        0        0    17592 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-rw-rw-   0        0        0     4794 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.479998 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/
+-rw-rw-rw-   0        0        0     5944 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/__init__.py
+-rw-rw-rw-   0        0        0     8808 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/__main__.py
+-rw-rw-rw-   0        0        0    10096 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-rw-rw-   0        0        0   140235 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-rw-rw-   0        0        0     1064 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-rw-rw-   0        0        0     2114 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py
+-rw-rw-rw-   0        0        0      265 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_extension.py
+-rw-rw-rw-   0        0        0     9695 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py
+-rw-rw-rw-   0        0        0     3225 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py
+-rw-rw-rw-   0        0        0     1236 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_loop.py
+-rw-rw-rw-   0        0        0     7063 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py
+-rw-rw-rw-   0        0        0      423 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_pick.py
+-rw-rw-rw-   0        0        0     5472 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py
+-rw-rw-rw-   0        0        0    19919 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py
+-rw-rw-rw-   0        0        0      351 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_stack.py
+-rw-rw-rw-   0        0        0      417 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_timer.py
+-rw-rw-rw-   0        0        0    22820 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-rw-rw-   0        0        0     1926 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_windows.py
+-rw-rw-rw-   0        0        0     2783 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-rw-rw-   0        0        0     1840 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py
+-rw-rw-rw-   0        0        0      890 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/abc.py
+-rw-rw-rw-   0        0        0    10368 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/align.py
+-rw-rw-rw-   0        0        0     6820 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/ansi.py
+-rw-rw-rw-   0        0        0     3264 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/bar.py
+-rw-rw-rw-   0        0        0     9864 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/box.py
+-rw-rw-rw-   0        0        0     4503 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/cells.py
+-rw-rw-rw-   0        0        0    17957 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/color.py
+-rw-rw-rw-   0        0        0     1054 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-rw-rw-   0        0        0     7131 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/columns.py
+-rw-rw-rw-   0        0        0    95885 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/console.py
+-rw-rw-rw-   0        0        0     1288 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/constrain.py
+-rw-rw-rw-   0        0        0     5497 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/containers.py
+-rw-rw-rw-   0        0        0     6630 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/control.py
+-rw-rw-rw-   0        0        0     7954 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py
+-rw-rw-rw-   0        0        0      972 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py
+-rw-rw-rw-   0        0        0     2501 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/emoji.py
+-rw-rw-rw-   0        0        0      642 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/errors.py
+-rw-rw-rw-   0        0        0     1616 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-rw-rw-   0        0        0     2507 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/filesize.py
+-rw-rw-rw-   0        0        0     9585 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py
+-rw-rw-rw-   0        0        0     5051 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/json.py
+-rw-rw-rw-   0        0        0     3252 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py
+-rw-rw-rw-   0        0        0    14074 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/layout.py
+-rw-rw-rw-   0        0        0    14172 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/live.py
+-rw-rw-rw-   0        0        0     3667 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/live_render.py
+-rw-rw-rw-   0        0        0    11471 2023-07-26 07:30:20.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/logging.py
+-rw-rw-rw-   0        0        0     8198 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/markup.py
+-rw-rw-rw-   0        0        0     5305 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/measure.py
+-rw-rw-rw-   0        0        0     4970 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/padding.py
+-rw-rw-rw-   0        0        0      828 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/pager.py
+-rw-rw-rw-   0        0        0     3396 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/palette.py
+-rw-rw-rw-   0        0        0     8744 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/panel.py
+-rw-rw-rw-   0        0        0    36576 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/pretty.py
+-rw-rw-rw-   0        0        0    59746 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/progress.py
+-rw-rw-rw-   0        0        0     8161 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-rw-rw-   0        0        0    11303 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/prompt.py
+-rw-rw-rw-   0        0        0     1391 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/protocol.py
+-rw-rw-rw-   0        0        0      166 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/region.py
+-rw-rw-rw-   0        0        0     4449 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/repr.py
+-rw-rw-rw-   0        0        0     4773 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/rule.py
+-rw-rw-rw-   0        0        0     2842 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/scope.py
+-rw-rw-rw-   0        0        0     1591 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/screen.py
+-rw-rw-rw-   0        0        0    24224 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/segment.py
+-rw-rw-rw-   0        0        0     4374 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/spinner.py
+-rw-rw-rw-   0        0        0     4425 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/status.py
+-rw-rw-rw-   0        0        0    26240 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/style.py
+-rw-rw-rw-   0        0        0     1258 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/styled.py
+-rw-rw-rw-   0        0        0    34697 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/syntax.py
+-rw-rw-rw-   0        0        0    39515 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/table.py
+-rw-rw-rw-   0        0        0     3370 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-rw-rw-   0        0        0    44666 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/text.py
+-rw-rw-rw-   0        0        0     3627 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/theme.py
+-rw-rw-rw-   0        0        0      102 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/themes.py
+-rw-rw-rw-   0        0        0    26060 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/traceback.py
+-rw-rw-rw-   0        0        0     9169 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/tree.py
+-rw-rw-rw-   0        0        0    34549 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/six.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.489900 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tenacity/
+-rw-rw-rw-   0        0        0    18364 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-rw-rw-   0        0        0     3314 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-rw-rw-   0        0        0     1944 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-rw-rw-   0        0        0     1496 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tenacity/after.py
+-rw-rw-rw-   0        0        0     1376 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tenacity/before.py
+-rw-rw-rw-   0        0        0     1908 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-rw-rw-   0        0        0     1383 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py
+-rw-rw-rw-   0        0        0     7550 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py
+-rw-rw-rw-   0        0        0     2790 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py
+-rw-rw-rw-   0        0        0     2145 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-rw-rw-   0        0        0     8011 2023-07-26 07:30:21.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.493891 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tomli/
+-rw-rw-rw-   0        0        0      396 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tomli/__init__.py
+-rw-rw-rw-   0        0        0    22633 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py
+-rw-rw-rw-   0        0        0     2943 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tomli/_re.py
+-rw-rw-rw-   0        0        0      254 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tomli/_types.py
+-rw-rw-rw-   0        0        0    80114 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/typing_extensions.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.502720 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/
+-rw-rw-rw-   0        0        0     3333 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-rw-rw-   0        0        0    10811 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-rw-rw-   0        0        0       64 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/_version.py
+-rw-rw-rw-   0        0        0    20070 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
+-rw-rw-rw-   0        0        0    39093 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.507703 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-rw-rw-   0        0        0      957 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.509552 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-rw-rw-   0        0        0    17632 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-rw-rw-   0        0        0    13922 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-rw-rw-   0        0        0    11034 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-rw-rw-   0        0        0     4538 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-rw-rw-   0        0        0    17182 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-rw-rw-   0        0        0    34448 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-rw-rw-   0        0        0     7097 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-rw-rw-   0        0        0     8217 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-rw-rw-   0        0        0     8579 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
+-rw-rw-rw-   0        0        0     2440 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.511549 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.512545 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-rw-rw-   0        0        0     1417 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-rw-rw-   0        0        0    34665 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-rw-rw-   0        0        0    19786 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-rw-rw-   0        0        0     5985 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/request.py
+-rw-rw-rw-   0        0        0    30109 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/response.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.523869 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/
+-rw-rw-rw-   0        0        0     1155 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-rw-rw-   0        0        0     4901 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-rw-rw-   0        0        0     1605 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-rw-rw-   0        0        0      498 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-rw-rw-   0        0        0     3997 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-rw-rw-   0        0        0     3510 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-rw-rw-   0        0        0    22001 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-rw-rw-   0        0        0    17177 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-rw-rw-   0        0        0     5758 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-rw-rw-   0        0        0     6895 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-rw-rw-   0        0        0    10003 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-rw-rw-   0        0        0    14287 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-rw-rw-   0        0        0     5403 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-rw-rw-   0        0        0      469 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/vendor.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.526858 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/webencodings/
+-rw-rw-rw-   0        0        0    10579 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-rw-rw-   0        0        0     8979 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
+-rw-rw-rw-   0        0        0     1305 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-rw-rw-   0        0        0     6563 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
+-rw-rw-rw-   0        0        0     4307 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.088184 mylove-1.0.0/venv/Lib/site-packages/pip-22.3.1.dist-info/
+-rw-rw-rw-   0        0        0     1093 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip-22.3.1.dist-info/LICENSE.txt
+-rw-rw-rw-   0        0        0      125 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip-22.3.1.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Lib/site-packages/pip-22.3.1.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.527854 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/
+-rw-rw-rw-   0        0        0   108568 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.530925 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
+-rw-rw-rw-   0        0        0    24701 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.536901 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-rw-rw-   0        0        0      506 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
+-rw-rw-rw-   0        0        0     4504 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
+-rw-rw-rw-   0        0        0     2741 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
+-rw-rw-rw-   0        0        0     2706 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
+-rw-rw-rw-   0        0        0      884 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
+-rw-rw-rw-   0        0        0     3494 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
+-rw-rw-rw-   0        0        0     3886 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
+-rw-rw-rw-   0        0        0     3566 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
+-rw-rw-rw-   0        0        0     2836 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.539342 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/__init__.py
+-rw-rw-rw-   0        0        0     5420 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py
+-rw-rw-rw-   0        0        0    13515 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.540338 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/
+-rw-rw-rw-   0        0        0    15526 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.542332 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-rw-rw-   0        0        0       83 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
+-rw-rw-rw-   0        0        0   132569 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py
+-rw-rw-rw-   0        0        0    18410 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.554739 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/
+-rw-rw-rw-   0        0        0      661 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rw-rw-rw-   0        0        0      497 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0    11488 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     4378 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     1431 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     8496 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     4706 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    30110 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    15699 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4200 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    14665 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.564704 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/
+-rw-rw-rw-   0        0        0     9159 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
+-rw-rw-rw-   0        0        0     6426 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py
+-rw-rw-rw-   0        0        0    12936 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/common.py
+-rw-rw-rw-   0        0        0   213310 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/core.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.565703 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/
+-rw-rw-rw-   0        0        0    23668 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
+-rw-rw-rw-   0        0        0     9023 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
+-rw-rw-rw-   0        0        0    39129 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
+-rw-rw-rw-   0        0        0    25341 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/results.py
+-rw-rw-rw-   0        0        0    13402 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py
+-rw-rw-rw-   0        0        0    10787 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
+-rw-rw-rw-   0        0        0     6805 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/util.py
+-rw-rw-rw-   0        0        0     8425 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/zipp.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.566699 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/extern/
+-rw-rw-rw-   0        0        0     2426 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/pkg_resources/extern/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.573674 mylove-1.0.0/venv/Lib/site-packages/pkginfo/
+-rw-rw-rw-   0        0        0      266 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/pkginfo/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/pkginfo/bdist.py
+-rw-rw-rw-   0        0        0     7415 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/pkginfo/commandline.py
+-rw-rw-rw-   0        0        0     1577 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/pkginfo/develop.py
+-rw-rw-rw-   0        0        0     4627 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/pkginfo/distribution.py
+-rw-rw-rw-   0        0        0      518 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/pkginfo/index.py
+-rw-rw-rw-   0        0        0     2492 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/pkginfo/installed.py
+-rw-rw-rw-   0        0        0     2347 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/pkginfo/sdist.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.583488 mylove-1.0.0/venv/Lib/site-packages/pkginfo/tests/
+-rw-rw-rw-   0        0        0     1342 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/pkginfo/tests/__init__.py
+-rw-rw-rw-   0        0        0     2279 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/pkginfo/tests/test_bdist.py
+-rw-rw-rw-   0        0        0    11722 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/pkginfo/tests/test_commandline.py
+-rw-rw-rw-   0        0        0      831 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/pkginfo/tests/test_develop.py
+-rw-rw-rw-   0        0        0    19377 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/pkginfo/tests/test_distribution.py
+-rw-rw-rw-   0        0        0     2636 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/pkginfo/tests/test_index.py
+-rw-rw-rw-   0        0        0     5460 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/pkginfo/tests/test_installed.py
+-rw-rw-rw-   0        0        0     5481 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/pkginfo/tests/test_sdist.py
+-rw-rw-rw-   0        0        0     6835 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/pkginfo/tests/test_utils.py
+-rw-rw-rw-   0        0        0     4443 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/pkginfo/tests/test_wheel.py
+-rw-rw-rw-   0        0        0     1786 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/pkginfo/utils.py
+-rw-rw-rw-   0        0        0     1586 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/pkginfo/wheel.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.575514 mylove-1.0.0/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/
+-rw-rw-rw-   0        0        0     1084 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/LICENSE.txt
+-rw-rw-rw-   0        0        0       54 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-07-26 08:06:05.000000 mylove-1.0.0/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.595700 mylove-1.0.0/venv/Lib/site-packages/pygments/
+-rw-rw-rw-   0        0        0     2959 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/__init__.py
+-rw-rw-rw-   0        0        0      348 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/__main__.py
+-rw-rw-rw-   0        0        0    23530 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/cmdline.py
+-rw-rw-rw-   0        0        0     1697 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/console.py
+-rw-rw-rw-   0        0        0     1938 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/filter.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.596696 mylove-1.0.0/venv/Lib/site-packages/pygments/filters/
+-rw-rw-rw-   0        0        0    40338 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/filters/__init__.py
+-rw-rw-rw-   0        0        0     4154 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/formatter.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.606935 mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/
+-rw-rw-rw-   0        0        0     5388 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/__init__.py
+-rw-rw-rw-   0        0        0     4176 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/_mapping.py
+-rw-rw-rw-   0        0        0     3290 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/bbcode.py
+-rw-rw-rw-   0        0        0     5070 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/groff.py
+-rw-rw-rw-   0        0        0    35574 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/html.py
+-rw-rw-rw-   0        0        0    21914 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/img.py
+-rw-rw-rw-   0        0        0     4945 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/irc.py
+-rw-rw-rw-   0        0        0    19303 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/latex.py
+-rw-rw-rw-   0        0        0     5025 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/other.py
+-rw-rw-rw-   0        0        0     2200 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/pangomarkup.py
+-rw-rw-rw-   0        0        0     4990 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/rtf.py
+-rw-rw-rw-   0        0        0     7299 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/svg.py
+-rw-rw-rw-   0        0        0     4626 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/terminal.py
+-rw-rw-rw-   0        0        0    11717 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/terminal256.py
+-rw-rw-rw-   0        0        0    34541 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexer.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.813461 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/
+-rw-rw-rw-   0        0        0    12082 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/__init__.py
+-rw-rw-rw-   0        0        0     1543 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_ada_builtins.py
+-rw-rw-rw-   0        0        0    27287 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_asy_builtins.py
+-rw-rw-rw-   0        0        0    13994 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_cl_builtins.py
+-rw-rw-rw-   0        0        0   105182 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_cocoa_builtins.py
+-rw-rw-rw-   0        0        0    18414 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_csound_builtins.py
+-rw-rw-rw-   0        0        0    12446 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_css_builtins.py
+-rw-rw-rw-   0        0        0    11883 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_julia_builtins.py
+-rw-rw-rw-   0        0        0   134510 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_lasso_builtins.py
+-rw-rw-rw-   0        0        0   108094 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_lilypond_builtins.py
+-rw-rw-rw-   0        0        0     8116 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_lua_builtins.py
+-rw-rw-rw-   0        0        0    65633 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_mapping.py
+-rw-rw-rw-   0        0        0    24713 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_mql_builtins.py
+-rw-rw-rw-   0        0        0    25842 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_mysql_builtins.py
+-rw-rw-rw-   0        0        0    49398 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_openedge_builtins.py
+-rw-rw-rw-   0        0        0   107930 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_php_builtins.py
+-rw-rw-rw-   0        0        0    13355 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_postgres_builtins.py
+-rw-rw-rw-   0        0        0    12595 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_qlik_builtins.py
+-rw-rw-rw-   0        0        0    32564 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_scheme_builtins.py
+-rw-rw-rw-   0        0        0    52413 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_scilab_builtins.py
+-rw-rw-rw-   0        0        0    26781 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_sourcemod_builtins.py
+-rw-rw-rw-   0        0        0    13445 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_stan_builtins.py
+-rw-rw-rw-   0        0        0    27227 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_stata_builtins.py
+-rw-rw-rw-   0        0        0    15460 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_tsql_builtins.py
+-rw-rw-rw-   0        0        0     1658 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_usd_builtins.py
+-rw-rw-rw-   0        0        0     4225 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_vbscript_builtins.py
+-rw-rw-rw-   0        0        0    57066 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_vim_builtins.py
+-rw-rw-rw-   0        0        0    11676 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/actionscript.py
+-rw-rw-rw-   0        0        0     5320 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/ada.py
+-rw-rw-rw-   0        0        0      876 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/agile.py
+-rw-rw-rw-   0        0        0     9873 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/algebra.py
+-rw-rw-rw-   0        0        0     2606 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/ambient.py
+-rw-rw-rw-   0        0        0     1670 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/amdgpu.py
+-rw-rw-rw-   0        0        0     4177 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/ampl.py
+-rw-rw-rw-   0        0        0    30766 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/apdlexer.py
+-rw-rw-rw-   0        0        0     3405 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/apl.py
+-rw-rw-rw-   0        0        0    11469 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/archetype.py
+-rw-rw-rw-   0        0        0     3565 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/arrow.py
+-rw-rw-rw-   0        0        0    11417 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/arturo.py
+-rw-rw-rw-   0        0        0     1621 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/asc.py
+-rw-rw-rw-   0        0        0    41243 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/asm.py
+-rw-rw-rw-   0        0        0    19815 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/automation.py
+-rw-rw-rw-   0        0        0     3021 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/bare.py
+-rw-rw-rw-   0        0        0    27923 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/basic.py
+-rw-rw-rw-   0        0        0     1652 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/bdd.py
+-rw-rw-rw-   0        0        0     3211 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/berry.py
+-rw-rw-rw-   0        0        0     4723 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/bibtex.py
+-rw-rw-rw-   0        0        0     3915 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/boa.py
+-rw-rw-rw-   0        0        0    28112 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/business.py
+-rw-rw-rw-   0        0        0    17791 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/c_cpp.py
+-rw-rw-rw-   0        0        0    29206 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/c_like.py
+-rw-rw-rw-   0        0        0     2175 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/capnproto.py
+-rw-rw-rw-   0        0        0     3231 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/carbon.py
+-rw-rw-rw-   0        0        0     5182 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/cddl.py
+-rw-rw-rw-   0        0        0     5157 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/chapel.py
+-rw-rw-rw-   0        0        0     6395 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/clean.py
+-rw-rw-rw-   0        0        0     3156 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/comal.py
+-rw-rw-rw-   0        0        0     1407 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/compiled.py
+-rw-rw-rw-   0        0        0    42338 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/configs.py
+-rw-rw-rw-   0        0        0     4148 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/console.py
+-rw-rw-rw-   0        0        0     1390 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/cplint.py
+-rw-rw-rw-   0        0        0    15756 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/crystal.py
+-rw-rw-rw-   0        0        0    16994 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/csound.py
+-rw-rw-rw-   0        0        0    25322 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/css.py
+-rw-rw-rw-   0        0        0     9875 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/d.py
+-rw-rw-rw-   0        0        0     4607 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/dalvik.py
+-rw-rw-rw-   0        0        0    26940 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/data.py
+-rw-rw-rw-   0        0        0     8099 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/dax.py
+-rw-rw-rw-   0        0        0     4020 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/devicetree.py
+-rw-rw-rw-   0        0        0     5278 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/diff.py
+-rw-rw-rw-   0        0        0    37623 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/dotnet.py
+-rw-rw-rw-   0        0        0    36774 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/dsls.py
+-rw-rw-rw-   0        0        0    10380 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/dylan.py
+-rw-rw-rw-   0        0        0     6372 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/ecl.py
+-rw-rw-rw-   0        0        0     2690 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/eiffel.py
+-rw-rw-rw-   0        0        0     3152 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/elm.py
+-rw-rw-rw-   0        0        0     6370 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/elpi.py
+-rw-rw-rw-   0        0        0     4742 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/email.py
+-rw-rw-rw-   0        0        0    19170 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/erlang.py
+-rw-rw-rw-   0        0        0    10396 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/esoteric.py
+-rw-rw-rw-   0        0        0     3273 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/ezhil.py
+-rw-rw-rw-   0        0        0    19531 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/factor.py
+-rw-rw-rw-   0        0        0    10197 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/fantom.py
+-rw-rw-rw-   0        0        0     9646 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/felix.py
+-rw-rw-rw-   0        0        0     1621 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/fift.py
+-rw-rw-rw-   0        0        0     2668 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/floscript.py
+-rw-rw-rw-   0        0        0     7194 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/forth.py
+-rw-rw-rw-   0        0        0    10336 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/fortran.py
+-rw-rw-rw-   0        0        0    26212 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/foxpro.py
+-rw-rw-rw-   0        0        0    26914 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/freefem.py
+-rw-rw-rw-   0        0        0     3622 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/func.py
+-rw-rw-rw-   0        0        0      674 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/functional.py
+-rw-rw-rw-   0        0        0     3732 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/futhark.py
+-rw-rw-rw-   0        0        0      826 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/gcodelexer.py
+-rw-rw-rw-   0        0        0     7543 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/gdscript.py
+-rw-rw-rw-   0        0        0     3761 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/go.py
+-rw-rw-rw-   0        0        0     7980 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/grammar_notation.py
+-rw-rw-rw-   0        0        0     3861 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/graph.py
+-rw-rw-rw-   0        0        0    39026 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/graphics.py
+-rw-rw-rw-   0        0        0     1935 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/graphviz.py
+-rw-rw-rw-   0        0        0     3991 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/gsql.py
+-rw-rw-rw-   0        0        0    32898 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/haskell.py
+-rw-rw-rw-   0        0        0    30976 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/haxe.py
+-rw-rw-rw-   0        0        0    22520 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/hdl.py
+-rw-rw-rw-   0        0        0     3603 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/hexdump.py
+-rw-rw-rw-   0        0        0    19879 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/html.py
+-rw-rw-rw-   0        0        0    15450 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/idl.py
+-rw-rw-rw-   0        0        0    30631 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/igor.py
+-rw-rw-rw-   0        0        0     3136 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/inferno.py
+-rw-rw-rw-   0        0        0    13178 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/installers.py
+-rw-rw-rw-   0        0        0    57119 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/int_fiction.py
+-rw-rw-rw-   0        0        0     1906 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/iolang.py
+-rw-rw-rw-   0        0        0     4854 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/j.py
+-rw-rw-rw-   0        0        0    62859 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/javascript.py
+-rw-rw-rw-   0        0        0     2059 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/jmespath.py
+-rw-rw-rw-   0        0        0     3701 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/jslt.py
+-rw-rw-rw-   0        0        0     5635 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/jsonnet.py
+-rw-rw-rw-   0        0        0    11646 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/julia.py
+-rw-rw-rw-   0        0        0    72929 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/jvm.py
+-rw-rw-rw-   0        0        0    11406 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/kuin.py
+-rw-rw-rw-   0        0        0     9753 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/lilypond.py
+-rw-rw-rw-   0        0        0   144039 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/lisp.py
+-rw-rw-rw-   0        0        0    31914 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/macaulay2.py
+-rw-rw-rw-   0        0        0     7618 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/make.py
+-rw-rw-rw-   0        0        0    58129 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/markup.py
+-rw-rw-rw-   0        0        0      676 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/math.py
+-rw-rw-rw-   0        0        0   132852 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/matlab.py
+-rw-rw-rw-   0        0        0     2716 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/maxima.py
+-rw-rw-rw-   0        0        0     4337 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/meson.py
+-rw-rw-rw-   0        0        0     7538 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/mime.py
+-rw-rw-rw-   0        0        0    13846 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/minecraft.py
+-rw-rw-rw-   0        0        0     4604 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/mips.py
+-rw-rw-rw-   0        0        0    35324 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/ml.py
+-rw-rw-rw-   0        0        0    13524 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/modeling.py
+-rw-rw-rw-   0        0        0    53073 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/modula2.py
+-rw-rw-rw-   0        0        0     6290 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/monte.py
+-rw-rw-rw-   0        0        0     9187 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/mosel.py
+-rw-rw-rw-   0        0        0    63962 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/ncl.py
+-rw-rw-rw-   0        0        0     6416 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/nimrod.py
+-rw-rw-rw-   0        0        0     2726 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/nit.py
+-rw-rw-rw-   0        0        0     4015 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/nix.py
+-rw-rw-rw-   0        0        0     4169 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/oberon.py
+-rw-rw-rw-   0        0        0    22961 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/objective.py
+-rw-rw-rw-   0        0        0     2982 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/ooc.py
+-rw-rw-rw-   0        0        0     1744 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/other.py
+-rw-rw-rw-   0        0        0     2720 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/parasail.py
+-rw-rw-rw-   0        0        0    25904 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/parsers.py
+-rw-rw-rw-   0        0        0    30880 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/pascal.py
+-rw-rw-rw-   0        0        0     8146 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/pawn.py
+-rw-rw-rw-   0        0        0    39170 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/perl.py
+-rw-rw-rw-   0        0        0    23252 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/phix.py
+-rw-rw-rw-   0        0        0    13040 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/php.py
+-rw-rw-rw-   0        0        0     1975 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/pointless.py
+-rw-rw-rw-   0        0        0     3244 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/pony.py
+-rw-rw-rw-   0        0        0    12677 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/praat.py
+-rw-rw-rw-   0        0        0     1156 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/procfile.py
+-rw-rw-rw-   0        0        0    12351 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/prolog.py
+-rw-rw-rw-   0        0        0     4715 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/promql.py
+-rw-rw-rw-   0        0        0    53376 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/python.py
+-rw-rw-rw-   0        0        0     6932 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/q.py
+-rw-rw-rw-   0        0        0     3665 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/qlik.py
+-rw-rw-rw-   0        0        0     6072 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/qvt.py
+-rw-rw-rw-   0        0        0     6185 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/r.py
+-rw-rw-rw-   0        0        0    15790 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/rdf.py
+-rw-rw-rw-   0        0        0    18248 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/rebol.py
+-rw-rw-rw-   0        0        0     2902 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/resource.py
+-rw-rw-rw-   0        0        0     5056 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/ride.py
+-rw-rw-rw-   0        0        0     1128 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/rita.py
+-rw-rw-rw-   0        0        0     1973 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/rnc.py
+-rw-rw-rw-   0        0        0     1962 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/roboconf.py
+-rw-rw-rw-   0        0        0    18449 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/robotframework.py
+-rw-rw-rw-   0        0        0    22775 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/ruby.py
+-rw-rw-rw-   0        0        0     8216 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/rust.py
+-rw-rw-rw-   0        0        0     9400 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/sas.py
+-rw-rw-rw-   0        0        0     4645 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/savi.py
+-rw-rw-rw-   0        0        0     2239 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/scdoc.py
+-rw-rw-rw-   0        0        0    70014 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/scripting.py
+-rw-rw-rw-   0        0        0     1986 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/sgf.py
+-rw-rw-rw-   0        0        0    36466 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/shell.py
+-rw-rw-rw-   0        0        0     2441 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/sieve.py
+-rw-rw-rw-   0        0        0     8482 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/slash.py
+-rw-rw-rw-   0        0        0     7206 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/smalltalk.py
+-rw-rw-rw-   0        0        0     2660 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/smithy.py
+-rw-rw-rw-   0        0        0     2773 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/smv.py
+-rw-rw-rw-   0        0        0     2732 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/snobol.py
+-rw-rw-rw-   0        0        0     3127 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/solidity.py
+-rw-rw-rw-   0        0        0     3330 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/sophia.py
+-rw-rw-rw-   0        0        0     3414 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/special.py
+-rw-rw-rw-   0        0        0     2733 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/spice.py
+-rw-rw-rw-   0        0        0    42086 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/sql.py
+-rw-rw-rw-   0        0        0     1693 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/srcinfo.py
+-rw-rw-rw-   0        0        0     6416 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/stata.py
+-rw-rw-rw-   0        0        0     3698 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/supercollider.py
+-rw-rw-rw-   0        0        0     2639 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/tal.py
+-rw-rw-rw-   0        0        0     5513 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/tcl.py
+-rw-rw-rw-   0        0        0     3523 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/teal.py
+-rw-rw-rw-   0        0        0    72610 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/templates.py
+-rw-rw-rw-   0        0        0     9719 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/teraterm.py
+-rw-rw-rw-   0        0        0    10767 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/testing.py
+-rw-rw-rw-   0        0        0     1029 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/text.py
+-rw-rw-rw-   0        0        0     7609 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/textedit.py
+-rw-rw-rw-   0        0        0    15192 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/textfmts.py
+-rw-rw-rw-   0        0        0    20157 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/theorem.py
+-rw-rw-rw-   0        0        0     4228 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/thingsdb.py
+-rw-rw-rw-   0        0        0     1377 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/tlb.py
+-rw-rw-rw-   0        0        0    10457 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/tnt.py
+-rw-rw-rw-   0        0        0     1474 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/trafficscript.py
+-rw-rw-rw-   0        0        0     8207 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/typoscript.py
+-rw-rw-rw-   0        0        0     8956 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/ul4.py
+-rw-rw-rw-   0        0        0    18512 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/unicon.py
+-rw-rw-rw-   0        0        0     6037 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/urbi.py
+-rw-rw-rw-   0        0        0     3513 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/usd.py
+-rw-rw-rw-   0        0        0     7273 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/varnish.py
+-rw-rw-rw-   0        0        0     3885 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/verification.py
+-rw-rw-rw-   0        0        0      894 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/web.py
+-rw-rw-rw-   0        0        0     5699 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/webassembly.py
+-rw-rw-rw-   0        0        0    10517 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/webidl.py
+-rw-rw-rw-   0        0        0    40549 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/webmisc.py
+-rw-rw-rw-   0        0        0    11920 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/wgsl.py
+-rw-rw-rw-   0        0        0     4018 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/whiley.py
+-rw-rw-rw-   0        0        0     4021 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/wowtoc.py
+-rw-rw-rw-   0        0        0     3239 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/wren.py
+-rw-rw-rw-   0        0        0     1920 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/x10.py
+-rw-rw-rw-   0        0        0      902 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/xorg.py
+-rw-rw-rw-   0        0        0     4500 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/yang.py
+-rw-rw-rw-   0        0        0     3953 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/zig.py
+-rw-rw-rw-   0        0        0      986 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/modeline.py
+-rw-rw-rw-   0        0        0     2579 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/plugin.py
+-rw-rw-rw-   0        0        0     3072 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/regexopt.py
+-rw-rw-rw-   0        0        0     3092 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/scanner.py
+-rw-rw-rw-   0        0        0     6816 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/sphinxext.py
+-rw-rw-rw-   0        0        0     6245 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/style.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.846029 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/
+-rw-rw-rw-   0        0        0     3676 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/__init__.py
+-rw-rw-rw-   0        0        0      705 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/abap.py
+-rw-rw-rw-   0        0        0     2216 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/algol.py
+-rw-rw-rw-   0        0        0     2231 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/algol_nu.py
+-rw-rw-rw-   0        0        0     4443 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/arduino.py
+-rw-rw-rw-   0        0        0     2096 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/autumn.py
+-rw-rw-rw-   0        0        0     1514 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/borland.py
+-rw-rw-rw-   0        0        0     1308 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/bw.py
+-rw-rw-rw-   0        0        0     2730 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/colorful.py
+-rw-rw-rw-   0        0        0     2488 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/default.py
+-rw-rw-rw-   0        0        0     3314 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/dracula.py
+-rw-rw-rw-   0        0        0     2439 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/emacs.py
+-rw-rw-rw-   0        0        0     2502 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/friendly.py
+-rw-rw-rw-   0        0        0     2707 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/friendly_grayscale.py
+-rw-rw-rw-   0        0        0     1274 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/fruity.py
+-rw-rw-rw-   0        0        0     3481 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/gh_dark.py
+-rw-rw-rw-   0        0        0     3230 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/gruvbox.py
+-rw-rw-rw-   0        0        0      692 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/igor.py
+-rw-rw-rw-   0        0        0     2302 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/inkpot.py
+-rw-rw-rw-   0        0        0     2016 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/lilypond.py
+-rw-rw-rw-   0        0        0     3117 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/lovelace.py
+-rw-rw-rw-   0        0        0     2350 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/manni.py
+-rw-rw-rw-   0        0        0     4083 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/material.py
+-rw-rw-rw-   0        0        0     5063 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/monokai.py
+-rw-rw-rw-   0        0        0     2703 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/murphy.py
+-rw-rw-rw-   0        0        0     1948 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/native.py
+-rw-rw-rw-   0        0        0     5244 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/nord.py
+-rw-rw-rw-   0        0        0     1664 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/onedark.py
+-rw-rw-rw-   0        0        0     5526 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/paraiso_dark.py
+-rw-rw-rw-   0        0        0     5530 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/paraiso_light.py
+-rw-rw-rw-   0        0        0     2425 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/pastie.py
+-rw-rw-rw-   0        0        0     2128 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/perldoc.py
+-rw-rw-rw-   0        0        0     2432 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/rainbow_dash.py
+-rw-rw-rw-   0        0        0      874 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/rrt.py
+-rw-rw-rw-   0        0        0     1393 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/sas.py
+-rw-rw-rw-   0        0        0     4078 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/solarized.py
+-rw-rw-rw-   0        0        0      770 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/staroffice.py
+-rw-rw-rw-   0        0        0     1198 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/stata_dark.py
+-rw-rw-rw-   0        0        0     1227 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/stata_light.py
+-rw-rw-rw-   0        0        0     7039 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/tango.py
+-rw-rw-rw-   0        0        0     1885 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/trac.py
+-rw-rw-rw-   0        0        0     1922 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/vim.py
+-rw-rw-rw-   0        0        0     1026 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/vs.py
+-rw-rw-rw-   0        0        0     1453 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/xcode.py
+-rw-rw-rw-   0        0        0     2148 2023-07-26 08:05:58.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/styles/zenburn.py
+-rw-rw-rw-   0        0        0     6184 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/token.py
+-rw-rw-rw-   0        0        0    63223 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/unistring.py
+-rw-rw-rw-   0        0        0    10230 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pygments/util.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.848022 mylove-1.0.0/venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/
+-rw-rw-rw-   0        0        0     1616 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/LICENSE.txt
+-rw-rw-rw-   0        0        0       12 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.853005 mylove-1.0.0/venv/Lib/site-packages/readme_renderer/
+-rw-rw-rw-   0        0        0     1119 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/readme_renderer/__about__.py
+-rw-rw-rw-   0        0        0      573 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/readme_renderer/__init__.py
+-rw-rw-rw-   0        0        0     2622 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/readme_renderer/__main__.py
+-rw-rw-rw-   0        0        0     4290 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/readme_renderer/clean.py
+-rw-rw-rw-   0        0        0     3595 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/readme_renderer/markdown.py
+-rw-rw-rw-   0        0        0     4460 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/readme_renderer/rst.py
+-rw-rw-rw-   0        0        0      823 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/readme_renderer/txt.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.854434 mylove-1.0.0/venv/Lib/site-packages/readme_renderer-40.0.dist-info/
+-rw-rw-rw-   0        0        0       16 2023-07-26 08:06:14.000000 mylove-1.0.0/venv/Lib/site-packages/readme_renderer-40.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.869389 mylove-1.0.0/venv/Lib/site-packages/requests/
+-rw-rw-rw-   0        0        0     4963 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/requests/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/requests/__version__.py
+-rw-rw-rw-   0        0        0     1495 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/requests/_internal_utils.py
+-rw-rw-rw-   0        0        0    19553 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/requests/adapters.py
+-rw-rw-rw-   0        0        0     6449 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/requests/api.py
+-rw-rw-rw-   0        0        0    10187 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/requests/auth.py
+-rw-rw-rw-   0        0        0      429 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/requests/certs.py
+-rw-rw-rw-   0        0        0     1451 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/requests/compat.py
+-rw-rw-rw-   0        0        0    18560 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/requests/cookies.py
+-rw-rw-rw-   0        0        0     3811 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/requests/exceptions.py
+-rw-rw-rw-   0        0        0     3875 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/requests/help.py
+-rw-rw-rw-   0        0        0      733 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/requests/hooks.py
+-rw-rw-rw-   0        0        0    35223 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/requests/models.py
+-rw-rw-rw-   0        0        0      957 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/requests/packages.py
+-rw-rw-rw-   0        0        0    30373 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/requests/sessions.py
+-rw-rw-rw-   0        0        0     4235 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/requests/status_codes.py
+-rw-rw-rw-   0        0        0     2912 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/requests/structures.py
+-rw-rw-rw-   0        0        0    33448 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/requests/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.870385 mylove-1.0.0/venv/Lib/site-packages/requests-2.31.0.dist-info/
+-rw-rw-rw-   0        0        0        9 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/requests-2.31.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.874373 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/
+-rw-rw-rw-   0        0        0     1188 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/__init__.py
+-rw-rw-rw-   0        0        0     9260 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/_compat.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.883376 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/adapters/
+-rw-rw-rw-   0        0        0      370 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/adapters/__init__.py
+-rw-rw-rw-   0        0        0     7539 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/adapters/appengine.py
+-rw-rw-rw-   0        0        0     1404 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/adapters/fingerprint.py
+-rw-rw-rw-   0        0        0     1396 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/adapters/host_header_ssl.py
+-rw-rw-rw-   0        0        0     4789 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/adapters/socket_options.py
+-rw-rw-rw-   0        0        0     2608 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/adapters/source.py
+-rw-rw-rw-   0        0        0     2399 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/adapters/ssl.py
+-rw-rw-rw-   0        0        0     7854 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/adapters/x509.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.887364 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/auth/
+-rw-rw-rw-   0        0        0        0 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/auth/__init__.py
+-rw-rw-rw-   0        0        0      910 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/auth/_digest_auth_compat.py
+-rw-rw-rw-   0        0        0     4944 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/auth/guess.py
+-rw-rw-rw-   0        0        0     4407 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/auth/handler.py
+-rw-rw-rw-   0        0        0     3706 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/auth/http_proxy_digest.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.889358 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/cookies/
+-rw-rw-rw-   0        0        0        0 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/cookies/__init__.py
+-rw-rw-rw-   0        0        0      213 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/cookies/forgetful.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.891396 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/downloadutils/
+-rw-rw-rw-   0        0        0        0 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/downloadutils/__init__.py
+-rw-rw-rw-   0        0        0     6024 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/downloadutils/stream.py
+-rw-rw-rw-   0        0        0     4365 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/downloadutils/tee.py
+-rw-rw-rw-   0        0        0      695 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.893393 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/multipart/
+-rw-rw-rw-   0        0        0      854 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/multipart/__init__.py
+-rw-rw-rw-   0        0        0     4861 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/multipart/decoder.py
+-rw-rw-rw-   0        0        0    20769 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/multipart/encoder.py
+-rw-rw-rw-   0        0        0     3102 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/sessions.py
+-rw-rw-rw-   0        0        0     4044 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/streaming_iterator.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.897381 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/threaded/
+-rw-rw-rw-   0        0        0     3213 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/threaded/__init__.py
+-rw-rw-rw-   0        0        0     6628 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/threaded/pool.py
+-rw-rw-rw-   0        0        0     1465 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/threaded/thread.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.901366 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/utils/__init__.py
+-rw-rw-rw-   0        0        0     2558 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/utils/deprecated.py
+-rw-rw-rw-   0        0        0     6522 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/utils/dump.py
+-rw-rw-rw-   0        0        0     3233 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/utils/formdata.py
+-rw-rw-rw-   0        0        0     4524 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/utils/user_agent.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.875369 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/
+-rw-rw-rw-   0        0        0       18 2023-07-26 08:06:09.000000 mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.909339 mylove-1.0.0/venv/Lib/site-packages/rfc3986/
+-rw-rw-rw-   0        0        0     1565 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/rfc3986/__init__.py
+-rw-rw-rw-   0        0        0    13297 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/rfc3986/_mixin.py
+-rw-rw-rw-   0        0        0     9048 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/rfc3986/abnf_regexp.py
+-rw-rw-rw-   0        0        0     3862 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/rfc3986/api.py
+-rw-rw-rw-   0        0        0    12709 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/rfc3986/builder.py
+-rw-rw-rw-   0        0        0     1620 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/rfc3986/compat.py
+-rw-rw-rw-   0        0        0     3614 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/rfc3986/exceptions.py
+-rw-rw-rw-   0        0        0     5477 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/rfc3986/iri.py
+-rw-rw-rw-   0        0        0     4114 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/rfc3986/misc.py
+-rw-rw-rw-   0        0        0     5261 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/rfc3986/normalizers.py
+-rw-rw-rw-   0        0        0    14599 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/rfc3986/parseresult.py
+-rw-rw-rw-   0        0        0     5183 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/rfc3986/uri.py
+-rw-rw-rw-   0        0        0    13676 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/rfc3986/validators.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.910336 mylove-1.0.0/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/
+-rw-rw-rw-   0        0        0        8 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:34.974337 mylove-1.0.0/venv/Lib/site-packages/rich/
+-rw-rw-rw-   0        0        0     6066 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/__init__.py
+-rw-rw-rw-   0        0        0     8334 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/__main__.py
+-rw-rw-rw-   0        0        0    10096 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/_cell_widths.py
+-rw-rw-rw-   0        0        0   140235 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/_emoji_codes.py
+-rw-rw-rw-   0        0        0     1064 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/_emoji_replace.py
+-rw-rw-rw-   0        0        0     2100 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/_export_format.py
+-rw-rw-rw-   0        0        0      241 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/_extension.py
+-rw-rw-rw-   0        0        0      799 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/_fileno.py
+-rw-rw-rw-   0        0        0     9695 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/_inspect.py
+-rw-rw-rw-   0        0        0     3213 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/_log_render.py
+-rw-rw-rw-   0        0        0     1236 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/_loop.py
+-rw-rw-rw-   0        0        0     1387 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/_null_file.py
+-rw-rw-rw-   0        0        0     7063 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/_palettes.py
+-rw-rw-rw-   0        0        0      423 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/_pick.py
+-rw-rw-rw-   0        0        0     5460 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/_ratio.py
+-rw-rw-rw-   0        0        0    19919 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/_spinners.py
+-rw-rw-rw-   0        0        0      351 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/_stack.py
+-rw-rw-rw-   0        0        0      417 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/_timer.py
+-rw-rw-rw-   0        0        0    22784 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/_win32_console.py
+-rw-rw-rw-   0        0        0     1902 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/_windows.py
+-rw-rw-rw-   0        0        0     2759 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/_windows_renderer.py
+-rw-rw-rw-   0        0        0     1840 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/_wrap.py
+-rw-rw-rw-   0        0        0      878 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/abc.py
+-rw-rw-rw-   0        0        0    10320 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/align.py
+-rw-rw-rw-   0        0        0     6906 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/ansi.py
+-rw-rw-rw-   0        0        0     3264 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/bar.py
+-rw-rw-rw-   0        0        0     9794 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/box.py
+-rw-rw-rw-   0        0        0     4509 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/cells.py
+-rw-rw-rw-   0        0        0    18224 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/color.py
+-rw-rw-rw-   0        0        0     1054 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/color_triplet.py
+-rw-rw-rw-   0        0        0     7131 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/columns.py
+-rw-rw-rw-   0        0        0    99146 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/console.py
+-rw-rw-rw-   0        0        0     1288 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/constrain.py
+-rw-rw-rw-   0        0        0     5497 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/containers.py
+-rw-rw-rw-   0        0        0     6606 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/control.py
+-rw-rw-rw-   0        0        0     8046 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/default_styles.py
+-rw-rw-rw-   0        0        0      924 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/diagnose.py
+-rw-rw-rw-   0        0        0     2465 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/emoji.py
+-rw-rw-rw-   0        0        0      642 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/errors.py
+-rw-rw-rw-   0        0        0     1683 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/file_proxy.py
+-rw-rw-rw-   0        0        0     2508 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/filesize.py
+-rw-rw-rw-   0        0        0     9584 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/highlighter.py
+-rw-rw-rw-   0        0        0     5020 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/json.py
+-rw-rw-rw-   0        0        0     3228 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/jupyter.py
+-rw-rw-rw-   0        0        0    13947 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/layout.py
+-rw-rw-rw-   0        0        0    14273 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/live.py
+-rw-rw-rw-   0        0        0     3655 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/live_render.py
+-rw-rw-rw-   0        0        0    11891 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/logging.py
+-rw-rw-rw-   0        0        0    26245 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/markdown.py
+-rw-rw-rw-   0        0        0     8174 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/markup.py
+-rw-rw-rw-   0        0        0     5305 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/measure.py
+-rw-rw-rw-   0        0        0     4958 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/padding.py
+-rw-rw-rw-   0        0        0      828 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/pager.py
+-rw-rw-rw-   0        0        0     3288 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/palette.py
+-rw-rw-rw-   0        0        0    10574 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/panel.py
+-rw-rw-rw-   0        0        0    35816 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/pretty.py
+-rw-rw-rw-   0        0        0    59694 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/progress.py
+-rw-rw-rw-   0        0        0     8165 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/progress_bar.py
+-rw-rw-rw-   0        0        0    11291 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/prompt.py
+-rw-rw-rw-   0        0        0     1367 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/protocol.py
+-rw-rw-rw-   0        0        0      166 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/region.py
+-rw-rw-rw-   0        0        0     4419 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/repr.py
+-rw-rw-rw-   0        0        0     4590 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/rule.py
+-rw-rw-rw-   0        0        0     2831 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/scope.py
+-rw-rw-rw-   0        0        0     1579 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/screen.py
+-rw-rw-rw-   0        0        0    24211 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/segment.py
+-rw-rw-rw-   0        0        0     4339 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/spinner.py
+-rw-rw-rw-   0        0        0     4425 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/status.py
+-rw-rw-rw-   0        0        0    27073 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/style.py
+-rw-rw-rw-   0        0        0     1234 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/styled.py
+-rw-rw-rw-   0        0        0    35065 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/syntax.py
+-rw-rw-rw-   0        0        0    39648 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/table.py
+-rw-rw-rw-   0        0        0     3370 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/terminal_theme.py
+-rw-rw-rw-   0        0        0    45513 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/text.py
+-rw-rw-rw-   0        0        0     3777 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/theme.py
+-rw-rw-rw-   0        0        0      102 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/themes.py
+-rw-rw-rw-   0        0        0    29532 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/traceback.py
+-rw-rw-rw-   0        0        0     9109 2023-07-26 08:06:12.000000 mylove-1.0.0/venv/Lib/site-packages/rich/tree.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.000251 mylove-1.0.0/venv/Lib/site-packages/setuptools/
+-rw-rw-rw-   0        0        0     8429 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/__init__.py
+-rw-rw-rw-   0        0        0      218 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_deprecation_warning.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.027160 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/
+-rw-rw-rw-   0        0        0      537 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/__init__.py
+-rw-rw-rw-   0        0        0     1330 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/_collections.py
+-rw-rw-rw-   0        0        0      411 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/_functools.py
+-rw-rw-rw-   0        0        0      239 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/_macos_compat.py
+-rw-rw-rw-   0        0        0    19672 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-rw-rw-   0        0        0     8603 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/archive_util.py
+-rw-rw-rw-   0        0        0    14789 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-rw-rw-   0        0        0    47369 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py
+-rw-rw-rw-   0        0        0    17973 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/cmd.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.047752 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/
+-rw-rw-rw-   0        0        0      430 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/__init__.py
+-rw-rw-rw-   0        0        0     1614 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py
+-rw-rw-rw-   0        0        0     5441 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py
+-rw-rw-rw-   0        0        0     4701 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-rw-rw-   0        0        0    22051 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-rw-rw-   0        0        0     5617 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/build.py
+-rw-rw-rw-   0        0        0     7728 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-rw-rw-   0        0        0    31558 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-rw-rw-   0        0        0    16568 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py
+-rw-rw-rw-   0        0        0     5624 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-rw-rw-   0        0        0     4888 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/check.py
+-rw-rw-rw-   0        0        0     2603 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/clean.py
+-rw-rw-rw-   0        0        0    13137 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/config.py
+-rw-rw-rw-   0        0        0    30221 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/install.py
+-rw-rw-rw-   0        0        0     2779 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py
+-rw-rw-rw-   0        0        0     2785 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-rw-rw-   0        0        0     1189 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-rw-rw-   0        0        0     8434 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-rw-rw-   0        0        0     1936 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-rw-rw-   0        0        0      672 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-rw-rw-   0        0        0    11765 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/register.py
+-rw-rw-rw-   0        0        0    19241 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py
+-rw-rw-rw-   0        0        0     7477 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/upload.py
+-rw-rw-rw-   0        0        0     4920 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/config.py
+-rw-rw-rw-   0        0        0     9451 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/core.py
+-rw-rw-rw-   0        0        0    12537 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-rw-rw-   0        0        0      139 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/debug.py
+-rw-rw-rw-   0        0        0     3423 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/dep_util.py
+-rw-rw-rw-   0        0        0     8082 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/dir_util.py
+-rw-rw-rw-   0        0        0    50186 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/dist.py
+-rw-rw-rw-   0        0        0     3589 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/errors.py
+-rw-rw-rw-   0        0        0    10270 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/extension.py
+-rw-rw-rw-   0        0        0    17910 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-rw-rw-   0        0        0     8226 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/file_util.py
+-rw-rw-rw-   0        0        0    13713 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/filelist.py
+-rw-rw-rw-   0        0        0     1972 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/log.py
+-rw-rw-rw-   0        0        0    30235 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-rw-rw-   0        0        0    23602 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-rw-rw-   0        0        0      217 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/py38compat.py
+-rw-rw-rw-   0        0        0      639 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/py39compat.py
+-rw-rw-rw-   0        0        0     3517 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/spawn.py
+-rw-rw-rw-   0        0        0    18858 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py
+-rw-rw-rw-   0        0        0    12096 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/text_file.py
+-rw-rw-rw-   0        0        0    15641 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-rw-rw-   0        0        0    18128 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/util.py
+-rw-rw-rw-   0        0        0    12952 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/version.py
+-rw-rw-rw-   0        0        0     5248 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-rw-rw-   0        0        0     1972 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_entry_points.py
+-rw-rw-rw-   0        0        0     2392 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_imp.py
+-rw-rw-rw-   0        0        0     1311 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_importlib.py
+-rw-rw-rw-   0        0        0      675 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_itertools.py
+-rw-rw-rw-   0        0        0      749 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_path.py
+-rw-rw-rw-   0        0        0      501 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_reqs.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.050742 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.057718 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-rw-rw-   0        0        0    30130 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
+-rw-rw-rw-   0        0        0     1862 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
+-rw-rw-rw-   0        0        0      743 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
+-rw-rw-rw-   0        0        0     1828 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
+-rw-rw-rw-   0        0        0     2895 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
+-rw-rw-rw-   0        0        0     2068 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
+-rw-rw-rw-   0        0        0     1154 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
+-rw-rw-rw-   0        0        0     2166 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.067187 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/
+-rw-rw-rw-   0        0        0      506 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/__init__.py
+-rw-rw-rw-   0        0        0     4504 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
+-rw-rw-rw-   0        0        0     2741 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py
+-rw-rw-rw-   0        0        0     2706 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py
+-rw-rw-rw-   0        0        0      884 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
+-rw-rw-rw-   0        0        0     3494 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
+-rw-rw-rw-   0        0        0     3886 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py
+-rw-rw-rw-   0        0        0     3566 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py
+-rw-rw-rw-   0        0        0     2836 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.069181 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/__init__.py
+-rw-rw-rw-   0        0        0     5420 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py
+-rw-rw-rw-   0        0        0    13512 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.069181 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/
+-rw-rw-rw-   0        0        0    15517 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.072170 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/
+-rw-rw-rw-   0        0        0       82 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-rw-rw-   0        0        0   117959 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-rw-rw-   0        0        0    16256 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-rw-rw-   0        0        0    15130 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.081179 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/packaging/
+-rw-rw-rw-   0        0        0      661 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py
+-rw-rw-rw-   0        0        0      497 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0    11488 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     4378 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     1431 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     8493 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     4700 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    30110 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    15699 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4200 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    14665 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.091120 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/
+-rw-rw-rw-   0        0        0     9159 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/__init__.py
+-rw-rw-rw-   0        0        0     6426 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/actions.py
+-rw-rw-rw-   0        0        0    12936 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/common.py
+-rw-rw-rw-   0        0        0   213310 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/core.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.091657 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/
+-rw-rw-rw-   0        0        0    23668 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
+-rw-rw-rw-   0        0        0     9023 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py
+-rw-rw-rw-   0        0        0    39129 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/helpers.py
+-rw-rw-rw-   0        0        0    25341 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/results.py
+-rw-rw-rw-   0        0        0    13402 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/testing.py
+-rw-rw-rw-   0        0        0    10787 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/unicode.py
+-rw-rw-rw-   0        0        0     6805 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/util.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.095649 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/tomli/
+-rw-rw-rw-   0        0        0      396 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/tomli/__init__.py
+-rw-rw-rw-   0        0        0    22633 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py
+-rw-rw-rw-   0        0        0     2943 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py
+-rw-rw-rw-   0        0        0      254 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/tomli/_types.py
+-rw-rw-rw-   0        0        0    87149 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py
+-rw-rw-rw-   0        0        0     8425 2023-07-26 07:30:17.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/zipp.py
+-rw-rw-rw-   0        0        0     7346 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/archive_util.py
+-rw-rw-rw-   0        0        0    19539 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/build_meta.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.119570 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/
+-rw-rw-rw-   0        0        0      396 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/__init__.py
+-rw-rw-rw-   0        0        0     2381 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/alias.py
+-rw-rw-rw-   0        0        0    16623 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/bdist_egg.py
+-rw-rw-rw-   0        0        0     1182 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/bdist_rpm.py
+-rw-rw-rw-   0        0        0     6589 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/build.py
+-rw-rw-rw-   0        0        0     4415 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/build_clib.py
+-rw-rw-rw-   0        0        0    15821 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/build_ext.py
+-rw-rw-rw-   0        0        0    14115 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/build_py.py
+-rw-rw-rw-   0        0        0     7012 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/develop.py
+-rw-rw-rw-   0        0        0     4800 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/dist_info.py
+-rw-rw-rw-   0        0        0    85662 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/easy_install.py
+-rw-rw-rw-   0        0        0    31188 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/editable_wheel.py
+-rw-rw-rw-   0        0        0    26795 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/egg_info.py
+-rw-rw-rw-   0        0        0     5163 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/install.py
+-rw-rw-rw-   0        0        0     2226 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/install_egg_info.py
+-rw-rw-rw-   0        0        0     3875 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/install_lib.py
+-rw-rw-rw-   0        0        0     2612 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/install_scripts.py
+-rw-rw-rw-   0        0        0     4946 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/py36compat.py
+-rw-rw-rw-   0        0        0      468 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/register.py
+-rw-rw-rw-   0        0        0     2128 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/rotate.py
+-rw-rw-rw-   0        0        0      658 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/saveopts.py
+-rw-rw-rw-   0        0        0     7071 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/sdist.py
+-rw-rw-rw-   0        0        0     5086 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/setopt.py
+-rw-rw-rw-   0        0        0     8102 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/test.py
+-rw-rw-rw-   0        0        0      462 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/upload.py
+-rw-rw-rw-   0        0        0     7494 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/command/upload_docs.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.124672 mylove-1.0.0/venv/Lib/site-packages/setuptools/config/
+-rw-rw-rw-   0        0        0     1121 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/config/__init__.py
+-rw-rw-rw-   0        0        0    13398 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.130666 mylove-1.0.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/
+-rw-rw-rw-   0        0        0     1038 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py
+-rw-rw-rw-   0        0        0    11266 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
+-rw-rw-rw-   0        0        0     1153 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
+-rw-rw-rw-   0        0        0     1612 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
+-rw-rw-rw-   0        0        0   269900 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
+-rw-rw-rw-   0        0        0     8736 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py
+-rw-rw-rw-   0        0        0    16319 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/config/expand.py
+-rw-rw-rw-   0        0        0    19304 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/config/pyprojecttoml.py
+-rw-rw-rw-   0        0        0    25198 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/config/setupcfg.py
+-rw-rw-rw-   0        0        0      949 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/dep_util.py
+-rw-rw-rw-   0        0        0     5499 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/depends.py
+-rw-rw-rw-   0        0        0    20799 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/discovery.py
+-rw-rw-rw-   0        0        0    45578 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/dist.py
+-rw-rw-rw-   0        0        0     2464 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/errors.py
+-rw-rw-rw-   0        0        0     5591 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/extension.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.131649 mylove-1.0.0/venv/Lib/site-packages/setuptools/extern/
+-rw-rw-rw-   0        0        0     2512 2023-07-26 07:30:16.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/extern/__init__.py
+-rw-rw-rw-   0        0        0     4873 2023-07-26 07:30:14.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/glob.py
+-rw-rw-rw-   0        0        0     3824 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/installer.py
+-rw-rw-rw-   0        0        0      812 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/launch.py
+-rw-rw-rw-   0        0        0     1210 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/logging.py
+-rw-rw-rw-   0        0        0     4857 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/monkey.py
+-rw-rw-rw-   0        0        0    47724 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/msvc.py
+-rw-rw-rw-   0        0        0     3093 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/namespaces.py
+-rw-rw-rw-   0        0        0    40329 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/package_index.py
+-rw-rw-rw-   0        0        0      245 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/py34compat.py
+-rw-rw-rw-   0        0        0    14348 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/sandbox.py
+-rw-rw-rw-   0        0        0      941 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/unicode_utils.py
+-rw-rw-rw-   0        0        0      144 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/version.py
+-rw-rw-rw-   0        0        0     8376 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/wheel.py
+-rw-rw-rw-   0        0        0      718 2023-07-26 07:30:15.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools/windows_support.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.001247 mylove-1.0.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/
+-rw-rw-rw-   0        0        0     2740 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0       41 2023-07-26 07:30:18.000000 mylove-1.0.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.132646 mylove-1.0.0/venv/Lib/site-packages/six-1.16.0.dist-info/
+-rw-rw-rw-   0        0        0        4 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/six-1.16.0.dist-info/top_level.txt
+-rw-rw-rw-   0        0        0    34549 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/six.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.135766 mylove-1.0.0/venv/Lib/site-packages/speech_recognition/
+-rw-rw-rw-   0        0        0    94078 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/speech_recognition/__init__.py
+-rw-rw-rw-   0        0        0      833 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/speech_recognition/__main__.py
+-rw-rw-rw-   0        0        0    14807 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/speech_recognition/audio.py
+-rw-rw-rw-   0        0        0      273 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/speech_recognition/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.645743 mylove-1.0.0/venv/Lib/site-packages/speech_recognition/pocketsphinx-data/
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.136762 mylove-1.0.0/venv/Lib/site-packages/speech_recognition/pocketsphinx-data/en-US/
+-rw-rw-rw-   0        0        0     1537 2023-07-26 07:38:30.000000 mylove-1.0.0/venv/Lib/site-packages/speech_recognition/pocketsphinx-data/en-US/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.138266 mylove-1.0.0/venv/Lib/site-packages/speech_recognition/recognizers/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:38:31.000000 mylove-1.0.0/venv/Lib/site-packages/speech_recognition/recognizers/__init__.py
+-rw-rw-rw-   0        0        0     1492 2023-07-26 07:38:31.000000 mylove-1.0.0/venv/Lib/site-packages/speech_recognition/recognizers/whisper.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.149229 mylove-1.0.0/venv/Lib/site-packages/twine/
+-rw-rw-rw-   0        0        0     1343 2023-07-26 08:06:15.000000 mylove-1.0.0/venv/Lib/site-packages/twine/__init__.py
+-rw-rw-rw-   0        0        0     1475 2023-07-26 08:06:15.000000 mylove-1.0.0/venv/Lib/site-packages/twine/__main__.py
+-rw-rw-rw-   0        0        0     3129 2023-07-26 08:06:15.000000 mylove-1.0.0/venv/Lib/site-packages/twine/auth.py
+-rw-rw-rw-   0        0        0     3738 2023-07-26 08:06:15.000000 mylove-1.0.0/venv/Lib/site-packages/twine/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.153214 mylove-1.0.0/venv/Lib/site-packages/twine/commands/
+-rw-rw-rw-   0        0        0     1802 2023-07-26 08:06:15.000000 mylove-1.0.0/venv/Lib/site-packages/twine/commands/__init__.py
+-rw-rw-rw-   0        0        0     5727 2023-07-26 08:06:15.000000 mylove-1.0.0/venv/Lib/site-packages/twine/commands/check.py
+-rw-rw-rw-   0        0        0     2904 2023-07-26 08:06:15.000000 mylove-1.0.0/venv/Lib/site-packages/twine/commands/register.py
+-rw-rw-rw-   0        0        0     7469 2023-07-26 08:06:15.000000 mylove-1.0.0/venv/Lib/site-packages/twine/commands/upload.py
+-rw-rw-rw-   0        0        0     3814 2023-07-26 08:06:15.000000 mylove-1.0.0/venv/Lib/site-packages/twine/exceptions.py
+-rw-rw-rw-   0        0        0    11024 2023-07-26 08:06:15.000000 mylove-1.0.0/venv/Lib/site-packages/twine/package.py
+-rw-rw-rw-   0        0        0     8713 2023-07-26 08:06:15.000000 mylove-1.0.0/venv/Lib/site-packages/twine/repository.py
+-rw-rw-rw-   0        0        0    12269 2023-07-26 08:06:15.000000 mylove-1.0.0/venv/Lib/site-packages/twine/settings.py
+-rw-rw-rw-   0        0        0    10867 2023-07-26 08:06:15.000000 mylove-1.0.0/venv/Lib/site-packages/twine/utils.py
+-rw-rw-rw-   0        0        0     3049 2023-07-26 08:06:15.000000 mylove-1.0.0/venv/Lib/site-packages/twine/wheel.py
+-rw-rw-rw-   0        0        0     1795 2023-07-26 08:06:15.000000 mylove-1.0.0/venv/Lib/site-packages/twine/wininst.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.150225 mylove-1.0.0/venv/Lib/site-packages/twine-4.0.2.dist-info/
+-rw-rw-rw-   0        0        0      185 2023-07-26 08:06:15.000000 mylove-1.0.0/venv/Lib/site-packages/twine-4.0.2.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-26 08:06:15.000000 mylove-1.0.0/venv/Lib/site-packages/twine-4.0.2.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.162186 mylove-1.0.0/venv/Lib/site-packages/urllib3/
+-rw-rw-rw-   0        0        0     5283 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/__init__.py
+-rw-rw-rw-   0        0        0     5651 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/_base_connection.py
+-rw-rw-rw-   0        0        0    15561 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/_collections.py
+-rw-rw-rw-   0        0        0     7756 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/_request_methods.py
+-rw-rw-rw-   0        0        0       98 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/_version.py
+-rw-rw-rw-   0        0        0    33622 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/connection.py
+-rw-rw-rw-   0        0        0    42961 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/connectionpool.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.168165 mylove-1.0.0/venv/Lib/site-packages/urllib3/contrib/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/contrib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.170159 mylove-1.0.0/venv/Lib/site-packages/urllib3/contrib/_securetransport/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/contrib/_securetransport/__init__.py
+-rw-rw-rw-   0        0        0    14452 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/contrib/_securetransport/bindings.py
+-rw-rw-rw-   0        0        0    16220 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/contrib/_securetransport/low_level.py
+-rw-rw-rw-   0        0        0    19437 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/contrib/pyopenssl.py
+-rw-rw-rw-   0        0        0    34121 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/contrib/securetransport.py
+-rw-rw-rw-   0        0        0     7715 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/contrib/socks.py
+-rw-rw-rw-   0        0        0     9385 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/exceptions.py
+-rw-rw-rw-   0        0        0    11026 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/fields.py
+-rw-rw-rw-   0        0        0     2395 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/filepost.py
+-rw-rw-rw-   0        0        0    22648 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/poolmanager.py
+-rw-rw-rw-   0        0        0    40092 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/response.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.178187 mylove-1.0.0/venv/Lib/site-packages/urllib3/util/
+-rw-rw-rw-   0        0        0     1051 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/util/__init__.py
+-rw-rw-rw-   0        0        0     4462 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/util/connection.py
+-rw-rw-rw-   0        0        0     1148 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/util/proxy.py
+-rw-rw-rw-   0        0        0     8111 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/util/request.py
+-rw-rw-rw-   0        0        0     3374 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/util/response.py
+-rw-rw-rw-   0        0        0    18374 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/util/retry.py
+-rw-rw-rw-   0        0        0    18860 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/util/ssl_.py
+-rw-rw-rw-   0        0        0     5812 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/util/ssl_match_hostname.py
+-rw-rw-rw-   0        0        0     9045 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/util/ssltransport.py
+-rw-rw-rw-   0        0        0    10529 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/util/timeout.py
+-rw-rw-rw-   0        0        0    15213 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/util/url.py
+-rw-rw-rw-   0        0        0     1146 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/util/util.py
+-rw-rw-rw-   0        0        0     4423 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3/util/wait.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:33.648733 mylove-1.0.0/venv/Lib/site-packages/urllib3-2.0.3.dist-info/
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.164179 mylove-1.0.0/venv/Lib/site-packages/urllib3-2.0.3.dist-info/licenses/
+-rw-rw-rw-   0        0        0     1093 2023-07-26 07:38:25.000000 mylove-1.0.0/venv/Lib/site-packages/urllib3-2.0.3.dist-info/licenses/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.182346 mylove-1.0.0/venv/Lib/site-packages/webencodings/
+-rw-rw-rw-   0        0        0    10579 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/webencodings/__init__.py
+-rw-rw-rw-   0        0        0     8979 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/webencodings/labels.py
+-rw-rw-rw-   0        0        0     1305 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/webencodings/mklabels.py
+-rw-rw-rw-   0        0        0     6563 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/webencodings/tests.py
+-rw-rw-rw-   0        0        0     4307 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/webencodings/x_user_defined.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.183341 mylove-1.0.0/venv/Lib/site-packages/webencodings-0.5.1.dist-info/
+-rw-rw-rw-   0        0        0       13 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/webencodings-0.5.1.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.190359 mylove-1.0.0/venv/Lib/site-packages/wheel/
+-rw-rw-rw-   0        0        0       59 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/wheel/__init__.py
+-rw-rw-rw-   0        0        0      455 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/wheel/__main__.py
+-rw-rw-rw-   0        0        0      746 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/wheel/_setuptools_logging.py
+-rw-rw-rw-   0        0        0    19293 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/wheel/bdist_wheel.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.195346 mylove-1.0.0/venv/Lib/site-packages/wheel/cli/
+-rw-rw-rw-   0        0        0     2384 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/wheel/cli/__init__.py
+-rw-rw-rw-   0        0        0     9427 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/wheel/cli/convert.py
+-rw-rw-rw-   0        0        0     3383 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/wheel/cli/pack.py
+-rw-rw-rw-   0        0        0      659 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/wheel/cli/unpack.py
+-rw-rw-rw-   0        0        0    16145 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/wheel/macosx_libfile.py
+-rw-rw-rw-   0        0        0     3727 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/wheel/metadata.py
+-rw-rw-rw-   0        0        0      621 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/wheel/util.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.196343 mylove-1.0.0/venv/Lib/site-packages/wheel/vendored/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/wheel/vendored/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.199331 mylove-1.0.0/venv/Lib/site-packages/wheel/vendored/packaging/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/wheel/vendored/packaging/__init__.py
+-rw-rw-rw-   0        0        0    11489 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/wheel/vendored/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     4374 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/wheel/vendored/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0    15612 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/wheel/vendored/packaging/tags.py
+-rw-rw-rw-   0        0        0     7536 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/wheel/wheelfile.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.192357 mylove-1.0.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/
+-rw-rw-rw-   0        0        0     1107 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/LICENSE.txt
+-rw-rw-rw-   0        0        0      107 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-26 07:30:13.000000 mylove-1.0.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.202828 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/
+-rw-rw-rw-   0        0        0      206 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.205817 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/
+-rw-rw-rw-   0        0        0     1564 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/__init__.py
+-rw-rw-rw-   0        0        0      190 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/_winerrors.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.214980 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/cffi/
+-rw-rw-rw-   0        0        0      259 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/cffi/__init__.py
+-rw-rw-rw-   0        0        0     5161 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/cffi/_authentication.py
+-rw-rw-rw-   0        0        0      547 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/cffi/_common.py
+-rw-rw-rw-   0        0        0      741 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/cffi/_dll.py
+-rw-rw-rw-   0        0        0      295 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/cffi/_nl_support.py
+-rw-rw-rw-   0        0        0     4423 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/cffi/_resource.py
+-rw-rw-rw-   0        0        0      840 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/cffi/_system_information.py
+-rw-rw-rw-   0        0        0      314 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/cffi/_time.py
+-rw-rw-rw-   0        0        0     2557 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/cffi/_util.py
+-rw-rw-rw-   0        0        0      148 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/compat.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.221958 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/ctypes/
+-rw-rw-rw-   0        0        0      261 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/ctypes/__init__.py
+-rw-rw-rw-   0        0        0     3700 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/ctypes/_authentication.py
+-rw-rw-rw-   0        0        0     1170 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/ctypes/_common.py
+-rw-rw-rw-   0        0        0      531 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/ctypes/_dll.py
+-rw-rw-rw-   0        0        0      303 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/ctypes/_nl_support.py
+-rw-rw-rw-   0        0        0     4116 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/ctypes/_resource.py
+-rw-rw-rw-   0        0        0      905 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/ctypes/_system_information.py
+-rw-rw-rw-   0        0        0      327 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/ctypes/_time.py
+-rw-rw-rw-   0        0        0     1952 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/ctypes/_util.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.227353 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/pywin32/
+-rw-rw-rw-   0        0        0      342 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/pywin32/__init__.py
+-rw-rw-rw-   0        0        0      967 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/pywin32/pywintypes.py
+-rw-rw-rw-   0        0        0     7430 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/pywin32/win32api.py
+-rw-rw-rw-   0        0        0     4656 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/pywin32/win32cred.py
+-rw-rw-rw-   0        0        0      337 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/pywintypes.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.233349 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/tests/
+-rw-rw-rw-   0        0        0      672 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/tests/__init__.py
+-rw-rw-rw-   0        0        0     1017 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/tests/test_backends.py
+-rw-rw-rw-   0        0        0    11383 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/tests/test_win32api.py
+-rw-rw-rw-   0        0        0     7718 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/tests/test_win32cred.py
+-rw-rw-rw-   0        0        0       22 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/version.py
+-rw-rw-rw-   0        0        0      333 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/win32api.py
+-rw-rw-rw-   0        0        0      335 2023-07-26 08:05:57.000000 mylove-1.0.0/venv/Lib/site-packages/win32ctypes/win32cred.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.236334 mylove-1.0.0/venv/Lib/site-packages/zipp/
+-rw-rw-rw-   0        0        0    10453 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/zipp/__init__.py
+-rw-rw-rw-   0        0        0      893 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/zipp/glob.py
+-rw-rw-rw-   0        0        0      219 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/zipp/py310compat.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.237331 mylove-1.0.0/venv/Lib/site-packages/zipp-3.16.2.dist-info/
+-rw-rw-rw-   0        0        0        5 2023-07-26 08:05:56.000000 mylove-1.0.0/venv/Lib/site-packages/zipp-3.16.2.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:34:35.255189 mylove-1.0.0/venv/Scripts/
+-rw-rw-rw-   0        0        0     1169 2023-07-26 07:30:22.000000 mylove-1.0.0/venv/Scripts/activate_this.py
+-rw-rw-rw-   0        0        0      657 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Scripts/rst2html.py
+-rw-rw-rw-   0        0        0      779 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Scripts/rst2html4.py
+-rw-rw-rw-   0        0        0     1114 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Scripts/rst2html5.py
+-rw-rw-rw-   0        0        0      856 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Scripts/rst2latex.py
+-rw-rw-rw-   0        0        0      679 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Scripts/rst2man.py
+-rw-rw-rw-   0        0        0      845 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Scripts/rst2odt.py
+-rw-rw-rw-   0        0        0      651 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Scripts/rst2odt_prepstyles.py
+-rw-rw-rw-   0        0        0      664 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Scripts/rst2pseudoxml.py
+-rw-rw-rw-   0        0        0      700 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Scripts/rst2s5.py
+-rw-rw-rw-   0        0        0      936 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Scripts/rst2xetex.py
+-rw-rw-rw-   0        0        0      665 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Scripts/rst2xml.py
+-rw-rw-rw-   0        0        0      733 2023-07-26 08:06:06.000000 mylove-1.0.0/venv/Scripts/rstpep2html.py
```

### Comparing `mylove-0.0.2/LICENCE.txt` & `mylove-1.0.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/PKG-INFO` & `mylove-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mylove
-Version: 0.0.2
+Version: 1.0.0
 Summary: Drawing picture for loves
 Home-page: 
 Author: Umidyor
 Author-email: umidyor007@gmail.com
 License: MIT
 Keywords: drawing love,love picture
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mylove-0.0.2/mylove/__init__.py` & `mylove-1.0.0/mylove/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import turtle
 from PIL import Image, ImageTk
 import tempfile
-
+import pkg_resources
 
 
 def love(girlfriendname,text):
 
 
 # Set up the turtle screen
     screen = turtle.Screen()
     screen.setup(width=800, height=600)  # Adjust the screen size as desired
 
     # Load the background image and resize it
+    image_path = pkg_resources.resource_filename(__name__, 'data/h.jpg')
     bg_image = Image.open("h.jpg")
     bg_image = bg_image.resize((800, 600))  # Adjust the size to match the screen size
 
     # Save the resized image as a temporary file
     temp_filename = tempfile.NamedTemporaryFile(suffix=".png", delete=False)
     temp_filename.close()
     bg_image.save(temp_filename.name)
```

### Comparing `mylove-0.0.2/mylove/h.jpg` & `mylove-1.0.0/mylove/h.jpg`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/mylove.egg-info/PKG-INFO` & `mylove-1.0.0/mylove.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mylove
-Version: 0.0.2
+Version: 1.0.0
 Summary: Drawing picture for loves
 Home-page: 
 Author: Umidyor
 Author-email: umidyor007@gmail.com
 License: MIT
 Keywords: drawing love,love picture
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mylove-0.0.2/mylove.egg-info/SOURCES.txt` & `mylove-1.0.0/mylove.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/setup.py` & `mylove-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='mylove',
-    version='0.0.2',
+    version='1.0.0',
     description='Drawing picture for loves',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Umidyor',
     author_email='umidyor007@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/BdfFontFile.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/BdfFontFile.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/BlpImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/BlpImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/BmpImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/BmpImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/BufrStubImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/BufrStubImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ContainerIO.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ContainerIO.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/CurImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/CurImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/DcxImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/DcxImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/DdsImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/DdsImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/EpsImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/EpsImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ExifTags.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ExifTags.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/FitsImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/FitsImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/FliImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/FliImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/FontFile.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/FontFile.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/FpxImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/FpxImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/FtexImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/FtexImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/GbrImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/GbrImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/GdImageFile.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/GdImageFile.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/GifImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/GifImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/GimpGradientFile.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/GimpGradientFile.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/GimpPaletteFile.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/GimpPaletteFile.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/GribStubImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/GribStubImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/Hdf5StubImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/Hdf5StubImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/IcnsImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/IcnsImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/IcoImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/IcoImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/Image.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/Image.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImageChops.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImageChops.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImageCms.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImageCms.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImageColor.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImageColor.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImageDraw.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImageDraw.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImageDraw2.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImageDraw2.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImageEnhance.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImageEnhance.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImageFile.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImageFile.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImageFilter.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImageFilter.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImageFont.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImageFont.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImageGrab.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImageGrab.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImageMath.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImageMath.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImageMode.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImageMode.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImageMorph.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImageMorph.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImageOps.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImageOps.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImagePalette.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImagePalette.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImageQt.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImageQt.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImageSequence.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImageSequence.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImageShow.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImageShow.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImageStat.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImageStat.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImageTk.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImageTk.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImageTransform.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImageTransform.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImageWin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImageWin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/ImtImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/ImtImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/IptcImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/IptcImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/Jpeg2KImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/Jpeg2KImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/JpegImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/JpegImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/JpegPresets.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/JpegPresets.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/McIdasImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/McIdasImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/MicImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/MicImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/MpegImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/MpegImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/MpoImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/MpoImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/MspImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/MspImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/PSDraw.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/PSDraw.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/PaletteFile.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/PaletteFile.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/PalmImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/PalmImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/PcdImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/PcdImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/PcfFontFile.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/PcfFontFile.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/PcxImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/PcxImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/PdfImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/PdfImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/PdfParser.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/PdfParser.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/PixarImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/PixarImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/PngImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/PngImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/PpmImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/PpmImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/PsdImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/PsdImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/PyAccess.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/PyAccess.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/QoiImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/QoiImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/SgiImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/SgiImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/SpiderImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/SpiderImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/SunImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/SunImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/TarIO.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/TarIO.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/TgaImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/TgaImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/TiffImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/TiffImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/TiffTags.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/TiffTags.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/WalImageFile.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/WalImageFile.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/WebPImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/WebPImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/WmfImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/WmfImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/XVThumbImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/XVThumbImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/XbmImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/XbmImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/XpmImagePlugin.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/XpmImagePlugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/_binary.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/_binary.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/_deprecate.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/_deprecate.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/_tkinter_finder.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/_tkinter_finder.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/PIL/features.py` & `mylove-1.0.0/venv/Lib/site-packages/PIL/features.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/SpeechRecognition-3.10.0.dist-info/LICENSE-FLAC.txt` & `mylove-1.0.0/venv/Lib/site-packages/SpeechRecognition-3.10.0.dist-info/LICENSE-FLAC.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/SpeechRecognition-3.10.0.dist-info/LICENSE.txt` & `mylove-1.0.0/venv/Lib/site-packages/SpeechRecognition-3.10.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/_distutils_hack/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/_distutils_hack/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/_virtualenv.py` & `mylove-1.0.0/venv/Lib/site-packages/_virtualenv.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_ihatexml.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/_ihatexml.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_inputstream.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/_inputstream.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_tokenizer.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/_base.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/_base.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/py.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/py.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_utils.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/_utils.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/constants.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/constants.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/alphabeticalattributes.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/alphabeticalattributes.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/inject_meta_charset.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/inject_meta_charset.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/lint.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/lint.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/optionaltags.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/optionaltags.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/sanitizer.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/sanitizer.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/whitespace.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/whitespace.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/html5parser.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/html5parser.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/serializer.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/serializer.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/genshi.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/genshi.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/sax.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/sax.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/base.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/base.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/dom.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/dom.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/etree.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/etree.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/etree_lxml.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/etree_lxml.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/base.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/base.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/dom.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/dom.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/etree.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/etree.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/etree_lxml.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/etree_lxml.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/genshi.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/genshi.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/_vendor/parse.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/_vendor/parse.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/callbacks.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/callbacks.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/css_sanitizer.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/css_sanitizer.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/html5lib_shim.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/html5lib_shim.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/linkifier.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/linkifier.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/bleach/sanitizer.py` & `mylove-1.0.0/venv/Lib/site-packages/bleach/sanitizer.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/certifi/core.py` & `mylove-1.0.0/venv/Lib/site-packages/certifi/core.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/api.py` & `mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/api.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/assets/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/cd.py` & `mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/cd.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/cli/normalizer.py` & `mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/cli/normalizer.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/constant.py` & `mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/constant.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/legacy.py` & `mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/legacy.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/md.py` & `mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/md.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/models.py` & `mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/models.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/charset_normalizer/utils.py` & `mylove-1.0.0/venv/Lib/site-packages/charset_normalizer/utils.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/__main__.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/__main__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/core.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/core.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/examples.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/examples.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/frontend.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/frontend.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/io.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/io.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/af.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/af.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/ar.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/ar.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/ca.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/ca.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/cs.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/cs.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/da.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/da.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/de.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/de.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/en.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/en.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/eo.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/eo.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/es.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/es.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/fa.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/fa.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/fi.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/fi.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/fr.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/fr.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/gl.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/gl.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/he.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/he.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/it.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/it.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/ja.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/ja.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/ko.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/ko.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/lt.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/lt.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/lv.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/lv.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/nl.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/nl.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/pl.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/pl.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/pt_br.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/pt_br.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/ru.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/ru.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/sk.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/sk.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/sv.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/sv.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/uk.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/uk.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/zh_cn.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/zh_cn.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/languages/zh_tw.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/languages/zh_tw.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/nodes.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/nodes.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/commonmark_wrapper.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/commonmark_wrapper.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/recommonmark_wrapper.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/recommonmark_wrapper.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/directives/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/admonitions.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/directives/admonitions.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/body.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/directives/body.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/html.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/directives/html.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/images.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/directives/images.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/misc.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/directives/misc.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/parts.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/directives/parts.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/references.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/directives/references.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/directives/tables.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/directives/tables.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/README.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/README.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsa.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsa.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsb.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsb.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsc.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsc.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsn.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsn.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamso.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isoamso.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsr.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsr.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isobox.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isobox.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isocyr1.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isocyr1.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isocyr2.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isocyr2.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isodia.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isodia.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk1.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk1.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk2.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk2.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk3.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk3.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk4-wide.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk4-wide.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isolat1.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isolat1.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isolat2.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isolat2.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk-wide.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk-wide.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomopf-wide.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isomopf-wide.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomopf.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isomopf.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomscr-wide.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isomscr-wide.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomscr.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isomscr.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isonum.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isonum.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isopub.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isopub.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/isotech.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/isotech.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/mmlalias.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/mmlalias.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra-wide.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra-wide.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/s5defs.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/s5defs.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-lat1.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-lat1.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-special.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-special.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-symbol.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-symbol.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/af.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/af.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ar.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/ar.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ca.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/ca.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/cs.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/cs.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/da.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/da.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/de.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/de.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/en.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/en.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/eo.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/eo.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/es.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/es.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/fa.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/fa.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/fi.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/fi.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/fr.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/fr.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/gl.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/gl.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/he.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/he.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/it.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/it.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ja.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/ja.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ko.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/ko.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/lt.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/lt.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/lv.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/lv.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/nl.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/nl.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/pl.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/pl.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/pt_br.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/pt_br.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ru.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/ru.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/sk.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/sk.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/sv.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/sv.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/uk.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/uk.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/zh_cn.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/zh_cn.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/languages/zh_tw.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/languages/zh_tw.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/roles.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/roles.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/states.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/states.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/parsers/rst/tableparser.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/parsers/rst/tableparser.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/readers/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/readers/doctree.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/readers/doctree.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/readers/pep.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/readers/pep.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/readers/standalone.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/readers/standalone.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/statemachine.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/statemachine.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/transforms/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/transforms/components.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/transforms/components.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/transforms/frontmatter.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/transforms/frontmatter.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/transforms/misc.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/transforms/misc.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/transforms/parts.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/transforms/parts.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/transforms/peps.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/transforms/peps.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/transforms/references.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/transforms/references.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/transforms/universal.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/transforms/universal.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/transforms/writer_aux.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/transforms/writer_aux.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/utils/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/utils/code_analyzer.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/utils/code_analyzer.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/utils/error_reporting.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/utils/error_reporting.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/utils/math/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/utils/math/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/utils/math/latex2mathml.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/utils/math/latex2mathml.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/utils/math/math2html.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/utils/math/math2html.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/utils/math/tex2mathml_extern.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/utils/math/tex2mathml_extern.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/utils/math/tex2unichar.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/utils/math/tex2unichar.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/utils/math/unichar2tex.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/utils/math/unichar2tex.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/utils/punctuation_chars.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/utils/punctuation_chars.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/utils/roman.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/utils/roman.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/utils/smartquotes.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/utils/smartquotes.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/utils/urischemes.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/utils/urischemes.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/writers/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/writers/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/writers/_html_base.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/writers/_html_base.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/writers/docutils_xml.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/writers/docutils_xml.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/writers/html4css1/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/writers/html4css1/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/writers/html5_polyglot/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/writers/latex2e/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/writers/latex2e/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/writers/manpage.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/writers/manpage.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/writers/null.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/writers/null.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/writers/odf_odt/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/writers/odf_odt/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/writers/odf_odt/prepstyles.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/writers/odf_odt/prepstyles.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/writers/odf_odt/pygmentsformatter.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/writers/odf_odt/pygmentsformatter.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/writers/pep_html/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/writers/pep_html/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/writers/pep_html/template.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils/writers/pep_html/template.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/writers/pseudoxml.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/writers/pseudoxml.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/writers/s5_html/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/writers/s5_html/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils/writers/xetex/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/docutils/writers/xetex/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/docutils-0.20.1.dist-info/COPYING.txt` & `mylove-1.0.0/venv/Lib/site-packages/docutils-0.20.1.dist-info/COPYING.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/idna/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/idna/codec.py` & `mylove-1.0.0/venv/Lib/site-packages/idna/codec.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/idna/core.py` & `mylove-1.0.0/venv/Lib/site-packages/idna/core.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/idna/idnadata.py` & `mylove-1.0.0/venv/Lib/site-packages/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/idna/intranges.py` & `mylove-1.0.0/venv/Lib/site-packages/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/idna/uts46data.py` & `mylove-1.0.0/venv/Lib/site-packages/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/importlib_metadata/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/importlib_metadata/_adapters.py` & `mylove-1.0.0/venv/Lib/site-packages/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/importlib_metadata/_collections.py` & `mylove-1.0.0/venv/Lib/site-packages/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/importlib_metadata/_compat.py` & `mylove-1.0.0/venv/Lib/site-packages/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/importlib_metadata/_functools.py` & `mylove-1.0.0/venv/Lib/site-packages/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/importlib_metadata/_itertools.py` & `mylove-1.0.0/venv/Lib/site-packages/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/importlib_metadata/_meta.py` & `mylove-1.0.0/venv/Lib/site-packages/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/importlib_metadata/_py39compat.py` & `mylove-1.0.0/venv/Lib/site-packages/importlib_metadata/_py39compat.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/importlib_metadata/_text.py` & `mylove-1.0.0/venv/Lib/site-packages/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/jaraco/classes/ancestry.py` & `mylove-1.0.0/venv/Lib/site-packages/jaraco/classes/ancestry.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/jaraco/classes/meta.py` & `mylove-1.0.0/venv/Lib/site-packages/jaraco/classes/meta.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/jaraco/classes/properties.py` & `mylove-1.0.0/venv/Lib/site-packages/jaraco/classes/properties.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/keyring/_properties_compat.py` & `mylove-1.0.0/venv/Lib/site-packages/keyring/_properties_compat.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/keyring/backend.py` & `mylove-1.0.0/venv/Lib/site-packages/keyring/backend.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/keyring/backends/SecretService.py` & `mylove-1.0.0/venv/Lib/site-packages/keyring/backends/SecretService.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/keyring/backends/Windows.py` & `mylove-1.0.0/venv/Lib/site-packages/keyring/backends/Windows.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/keyring/backends/chainer.py` & `mylove-1.0.0/venv/Lib/site-packages/keyring/backends/chainer.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/keyring/backends/fail.py` & `mylove-1.0.0/venv/Lib/site-packages/keyring/backends/fail.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/keyring/backends/kwallet.py` & `mylove-1.0.0/venv/Lib/site-packages/keyring/backends/kwallet.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/keyring/backends/libsecret.py` & `mylove-1.0.0/venv/Lib/site-packages/keyring/backends/libsecret.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/keyring/backends/macOS/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/keyring/backends/macOS/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/keyring/backends/macOS/api.py` & `mylove-1.0.0/venv/Lib/site-packages/keyring/backends/macOS/api.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/keyring/cli.py` & `mylove-1.0.0/venv/Lib/site-packages/keyring/cli.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/keyring/completion.py` & `mylove-1.0.0/venv/Lib/site-packages/keyring/completion.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/keyring/core.py` & `mylove-1.0.0/venv/Lib/site-packages/keyring/core.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/keyring/credentials.py` & `mylove-1.0.0/venv/Lib/site-packages/keyring/credentials.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/keyring/devpi_client.py` & `mylove-1.0.0/venv/Lib/site-packages/keyring/devpi_client.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/keyring/errors.py` & `mylove-1.0.0/venv/Lib/site-packages/keyring/errors.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/keyring/http.py` & `mylove-1.0.0/venv/Lib/site-packages/keyring/http.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/keyring/testing/backend.py` & `mylove-1.0.0/venv/Lib/site-packages/keyring/testing/backend.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/keyring/testing/util.py` & `mylove-1.0.0/venv/Lib/site-packages/keyring/testing/util.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/keyring/util/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/keyring/util/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/keyring/util/platform_.py` & `mylove-1.0.0/venv/Lib/site-packages/keyring/util/platform_.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/_punycode.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/_punycode.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/cli/parse.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/cli/parse.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/common/html_blocks.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/common/html_blocks.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/common/html_re.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/common/html_re.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/common/normalize_url.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/common/normalize_url.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/common/utils.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/common/utils.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/helpers/parse_link_destination.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/helpers/parse_link_destination.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/helpers/parse_link_label.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/helpers/parse_link_label.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/helpers/parse_link_title.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/helpers/parse_link_title.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/main.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/main.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/parser_block.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/parser_block.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/parser_core.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/parser_core.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/parser_inline.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/parser_inline.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/presets/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/presets/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/presets/commonmark.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/presets/commonmark.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/presets/default.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/presets/default.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/presets/zero.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/presets/zero.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/renderer.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/renderer.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/ruler.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/ruler.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/blockquote.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/blockquote.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/code.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/code.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/fence.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/fence.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/heading.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/heading.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/hr.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/hr.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/html_block.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/html_block.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/lheading.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/lheading.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/list.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/list.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/paragraph.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/paragraph.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/reference.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/reference.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/state_block.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/state_block.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_block/table.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_block/table.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_core/linkify.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_core/linkify.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_core/replacements.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_core/replacements.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_core/smartquotes.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_core/smartquotes.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_core/state_core.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_core/state_core.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_core/text_join.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_core/text_join.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/autolink.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/autolink.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/backticks.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/backticks.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/balance_pairs.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/balance_pairs.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/emphasis.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/emphasis.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/entity.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/entity.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/escape.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/escape.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/fragments_join.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/fragments_join.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/html_inline.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/html_inline.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/image.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/image.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/link.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/link.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/linkify.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/linkify.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/newline.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/newline.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/state_inline.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/state_inline.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/strikethrough.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/strikethrough.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/rules_inline/text.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/rules_inline/text.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/token.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/token.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/tree.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/tree.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/markdown_it/utils.py` & `mylove-1.0.0/venv/Lib/site-packages/markdown_it/utils.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/mdurl/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/mdurl/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/mdurl/_decode.py` & `mylove-1.0.0/venv/Lib/site-packages/mdurl/_decode.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/mdurl/_encode.py` & `mylove-1.0.0/venv/Lib/site-packages/mdurl/_encode.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/mdurl/_format.py` & `mylove-1.0.0/venv/Lib/site-packages/mdurl/_format.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/mdurl/_parse.py` & `mylove-1.0.0/venv/Lib/site-packages/mdurl/_parse.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/more_itertools/more.py` & `mylove-1.0.0/venv/Lib/site-packages/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/more_itertools/recipes.py` & `mylove-1.0.0/venv/Lib/site-packages/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/__main__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/__pip-runner__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/build_env.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cache.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cli/base_command.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cli/command_context.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cli/main.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cli/main_parser.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cli/parser.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cli/req_command.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/cli/spinners.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/cache.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/check.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/completion.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/configuration.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/debug.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/download.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/freeze.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/hash.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/help.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/index.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/inspect.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/install.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/list.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/search.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/show.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/uninstall.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/commands/wheel.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/configuration.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/distributions/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/distributions/base.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/distributions/installed.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/distributions/sdist.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/distributions/wheel.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/exceptions.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/index/collector.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/index/package_finder.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/index/sources.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/locations/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/locations/_distutils.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/locations/base.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/metadata/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/metadata/_json.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/metadata/base.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/candidate.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/direct_url.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/format_control.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/index.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/installation_report.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/link.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/scheme.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/search_scope.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/target_python.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/models/wheel.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/network/auth.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/network/cache.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/network/download.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/network/session.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/network/utils.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/check.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/freeze.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/operations/prepare.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/pyproject.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/req/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/req/constructors.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/req/req_file.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/req/req_install.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/req/req_set.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/base.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/self_outdated_check.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/_log.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/appdirs.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/compat.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/deprecation.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/egg_link.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/encoding.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/filesystem.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/filetypes.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/glibc.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/hashes.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/logging.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/misc.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/models.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/packaging.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/subprocess.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/unpacking.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/urls.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/utils/wheel.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/vcs/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/vcs/git.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/vcs/subversion.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_internal/wheel_builder.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/certifi/core.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/enums.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/colorama/win32.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/compat.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/database.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/index.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/locators.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/markers.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/resources.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/util.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/version.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distro/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/distro/distro.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/idna/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/idna/codec.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/idna/core.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/idna/intranges.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/packaging/markers.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/packaging/tags.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/packaging/utils.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/packaging/version.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pep517/build.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pep517/build.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pep517/check.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pep517/check.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pep517/colorlog.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pep517/colorlog.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pep517/dirtools.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pep517/dirtools.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pep517/envbuild.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pep517/envbuild.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pep517/in_process/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pep517/in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pep517/in_process/_in_process.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pep517/in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pep517/meta.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pep517/meta.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pep517/wrappers.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pep517/wrappers.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/console.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/filter.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/style.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/token.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pygments/util.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/adapters.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/api.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/auth.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/certs.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/compat.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/cookies.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/help.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/hooks.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/models.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/packages.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/sessions.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/structures.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/requests/utils.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/__main__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_loop.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_windows.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/abc.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/align.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/ansi.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/bar.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/box.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/cells.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/color.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/columns.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/console.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/constrain.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/containers.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/control.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/emoji.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/errors.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/filesize.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/json.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/layout.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/live.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/live_render.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/logging.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/markup.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/measure.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/padding.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/pager.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/palette.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/panel.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/pretty.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/progress.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/prompt.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/protocol.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/repr.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/rule.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/scope.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/screen.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/segment.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/spinner.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/status.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/style.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/styled.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/syntax.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/table.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/text.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/theme.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/traceback.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/rich/tree.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/six.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/after.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/before.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/tomli/_re.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/typing_extensions.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/request.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/response.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `mylove-1.0.0/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pip-22.3.1.dist-info/LICENSE.txt` & `mylove-1.0.0/venv/Lib/site-packages/pip-22.3.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/common.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/core.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/results.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/util.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/_vendor/zipp.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkg_resources/extern/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkginfo/bdist.py` & `mylove-1.0.0/venv/Lib/site-packages/pkginfo/bdist.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkginfo/commandline.py` & `mylove-1.0.0/venv/Lib/site-packages/pkginfo/commandline.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkginfo/develop.py` & `mylove-1.0.0/venv/Lib/site-packages/pkginfo/develop.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkginfo/distribution.py` & `mylove-1.0.0/venv/Lib/site-packages/pkginfo/distribution.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkginfo/index.py` & `mylove-1.0.0/venv/Lib/site-packages/pkginfo/index.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkginfo/installed.py` & `mylove-1.0.0/venv/Lib/site-packages/pkginfo/installed.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkginfo/sdist.py` & `mylove-1.0.0/venv/Lib/site-packages/pkginfo/sdist.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkginfo/tests/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pkginfo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkginfo/tests/test_bdist.py` & `mylove-1.0.0/venv/Lib/site-packages/pkginfo/tests/test_bdist.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkginfo/tests/test_commandline.py` & `mylove-1.0.0/venv/Lib/site-packages/pkginfo/tests/test_commandline.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkginfo/tests/test_develop.py` & `mylove-1.0.0/venv/Lib/site-packages/pkginfo/tests/test_develop.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkginfo/tests/test_distribution.py` & `mylove-1.0.0/venv/Lib/site-packages/pkginfo/tests/test_distribution.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkginfo/tests/test_index.py` & `mylove-1.0.0/venv/Lib/site-packages/pkginfo/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkginfo/tests/test_installed.py` & `mylove-1.0.0/venv/Lib/site-packages/pkginfo/tests/test_installed.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkginfo/tests/test_sdist.py` & `mylove-1.0.0/venv/Lib/site-packages/pkginfo/tests/test_sdist.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkginfo/tests/test_utils.py` & `mylove-1.0.0/venv/Lib/site-packages/pkginfo/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkginfo/tests/test_wheel.py` & `mylove-1.0.0/venv/Lib/site-packages/pkginfo/tests/test_wheel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkginfo/utils.py` & `mylove-1.0.0/venv/Lib/site-packages/pkginfo/utils.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkginfo/wheel.py` & `mylove-1.0.0/venv/Lib/site-packages/pkginfo/wheel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/LICENSE.txt` & `mylove-1.0.0/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/cmdline.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/console.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/console.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/filter.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/filters/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/formatter.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/_mapping.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/bbcode.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/groff.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/html.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/img.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/irc.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/latex.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/other.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/pangomarkup.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/rtf.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/svg.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/terminal.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/formatters/terminal256.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexer.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_ada_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_ada_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_asy_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_asy_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_cl_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_cl_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_cocoa_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_cocoa_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_csound_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_csound_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_css_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_css_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_julia_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_julia_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_lasso_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_lasso_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_lilypond_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_lilypond_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_lua_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_lua_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_mapping.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_mql_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_mql_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_mysql_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_mysql_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_openedge_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_openedge_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_php_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_php_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_postgres_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_postgres_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_qlik_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_qlik_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_scheme_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_scheme_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_scilab_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_scilab_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_sourcemod_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_sourcemod_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_stan_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_stan_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_stata_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_stata_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_tsql_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_tsql_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_usd_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_usd_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_vbscript_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_vbscript_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/_vim_builtins.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/_vim_builtins.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/actionscript.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/actionscript.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/ada.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/ada.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/agile.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/agile.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/algebra.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/algebra.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/ambient.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/ambient.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/amdgpu.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/amdgpu.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/ampl.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/ampl.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/apdlexer.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/apdlexer.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/apl.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/apl.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/archetype.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/archetype.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/arrow.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/arrow.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/arturo.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/arturo.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/asc.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/asc.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/asm.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/asm.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/automation.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/automation.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/bare.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/bare.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/basic.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/basic.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/bdd.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/bdd.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/berry.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/berry.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/bibtex.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/bibtex.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/boa.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/boa.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/business.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/business.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/c_cpp.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/c_cpp.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/c_like.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/c_like.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/capnproto.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/capnproto.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/carbon.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/carbon.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/cddl.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/cddl.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/chapel.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/chapel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/clean.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/clean.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/comal.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/comal.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/compiled.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/compiled.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/configs.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/configs.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/console.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/console.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/cplint.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/cplint.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/crystal.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/crystal.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/csound.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/csound.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/css.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/css.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/d.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/d.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/dalvik.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/dalvik.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/data.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/data.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/dax.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/dax.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/devicetree.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/devicetree.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/diff.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/diff.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/dotnet.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/dotnet.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/dsls.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/dsls.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/dylan.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/dylan.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/ecl.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/ecl.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/eiffel.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/eiffel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/elm.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/elm.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/elpi.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/elpi.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/email.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/email.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/erlang.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/erlang.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/esoteric.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/esoteric.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/ezhil.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/ezhil.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/factor.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/factor.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/fantom.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/fantom.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/felix.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/felix.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/fift.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/fift.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/floscript.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/floscript.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/forth.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/forth.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/fortran.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/fortran.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/foxpro.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/foxpro.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/freefem.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/freefem.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/func.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/func.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/functional.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/functional.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/futhark.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/futhark.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/gcodelexer.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/gcodelexer.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/gdscript.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/gdscript.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/go.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/go.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/grammar_notation.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/grammar_notation.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/graph.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/graph.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/graphics.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/graphics.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/graphviz.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/graphviz.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/gsql.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/gsql.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/haskell.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/haskell.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/haxe.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/haxe.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/hdl.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/hdl.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/hexdump.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/hexdump.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/html.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/html.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/idl.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/idl.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/igor.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/igor.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/inferno.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/inferno.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/installers.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/installers.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/int_fiction.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/int_fiction.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/iolang.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/iolang.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/j.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/j.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/javascript.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/javascript.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/jmespath.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/jmespath.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/jslt.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/jslt.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/jsonnet.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/jsonnet.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/julia.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/julia.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/jvm.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/jvm.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/kuin.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/kuin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/lilypond.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/lilypond.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/lisp.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/lisp.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/macaulay2.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/macaulay2.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/make.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/make.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/markup.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/markup.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/math.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/math.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/matlab.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/matlab.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/maxima.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/maxima.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/meson.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/meson.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/mime.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/mime.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/minecraft.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/minecraft.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/mips.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/mips.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/ml.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/ml.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/modeling.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/modeling.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/modula2.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/modula2.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/monte.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/monte.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/mosel.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/mosel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/ncl.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/ncl.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/nimrod.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/nimrod.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/nit.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/nit.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/nix.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/nix.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/oberon.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/oberon.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/objective.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/objective.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/ooc.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/ooc.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/other.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/other.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/parasail.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/parasail.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/parsers.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/parsers.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/pascal.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/pascal.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/pawn.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/pawn.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/perl.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/perl.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/phix.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/phix.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/php.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/php.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/pointless.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/pointless.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/pony.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/pony.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/praat.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/praat.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/procfile.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/procfile.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/prolog.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/prolog.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/promql.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/promql.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/python.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/q.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/q.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/qlik.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/qlik.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/qvt.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/qvt.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/r.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/r.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/rdf.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/rdf.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/rebol.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/rebol.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/resource.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/resource.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/ride.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/ride.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/rita.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/rita.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/rnc.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/rnc.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/roboconf.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/roboconf.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/robotframework.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/robotframework.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/ruby.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/ruby.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/rust.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/rust.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/sas.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/sas.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/savi.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/savi.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/scdoc.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/scdoc.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/scripting.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/scripting.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/sgf.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/sgf.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/shell.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/shell.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/sieve.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/sieve.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/slash.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/slash.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/smalltalk.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/smalltalk.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/smithy.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/smithy.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/smv.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/smv.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/snobol.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/snobol.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/solidity.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/solidity.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/sophia.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/sophia.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/special.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/special.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/spice.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/spice.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/sql.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/sql.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/srcinfo.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/srcinfo.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/stata.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/stata.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/supercollider.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/supercollider.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/tal.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/tal.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/tcl.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/tcl.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/teal.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/teal.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/templates.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/templates.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/teraterm.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/teraterm.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/testing.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/testing.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/text.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/text.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/textedit.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/textedit.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/textfmts.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/textfmts.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/theorem.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/theorem.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/thingsdb.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/thingsdb.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/tlb.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/tlb.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/tnt.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/tnt.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/trafficscript.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/trafficscript.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/typoscript.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/typoscript.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/ul4.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/ul4.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/unicon.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/unicon.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/urbi.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/urbi.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/usd.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/usd.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/varnish.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/varnish.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/verification.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/verification.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/web.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/web.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/webassembly.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/webassembly.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/webidl.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/webidl.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/webmisc.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/webmisc.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/wgsl.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/wgsl.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/whiley.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/whiley.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/wowtoc.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/wowtoc.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/wren.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/wren.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/x10.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/x10.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/xorg.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/xorg.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/yang.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/yang.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/lexers/zig.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/lexers/zig.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/modeline.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/plugin.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/regexopt.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/scanner.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/sphinxext.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/style.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/style.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/abap.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/abap.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/algol.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/algol.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/algol_nu.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/algol_nu.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/arduino.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/arduino.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/autumn.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/autumn.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/borland.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/borland.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/bw.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/bw.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/colorful.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/colorful.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/default.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/default.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/dracula.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/dracula.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/emacs.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/emacs.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/friendly.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/friendly.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/friendly_grayscale.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/friendly_grayscale.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/fruity.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/fruity.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/gh_dark.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/gh_dark.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/gruvbox.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/gruvbox.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/igor.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/igor.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/inkpot.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/inkpot.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/lilypond.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/lilypond.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/lovelace.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/lovelace.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/manni.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/manni.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/material.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/material.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/monokai.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/monokai.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/murphy.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/murphy.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/native.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/native.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/nord.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/nord.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/onedark.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/onedark.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/paraiso_dark.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/paraiso_dark.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/paraiso_light.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/paraiso_light.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/pastie.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/pastie.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/perldoc.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/perldoc.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/rainbow_dash.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/rainbow_dash.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/rrt.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/rrt.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/sas.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/sas.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/solarized.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/solarized.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/staroffice.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/staroffice.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/stata_dark.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/stata_dark.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/stata_light.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/stata_light.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/tango.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/tango.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/trac.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/trac.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/vim.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/vim.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/vs.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/vs.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/xcode.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/xcode.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/styles/zenburn.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/styles/zenburn.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/token.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/token.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/unistring.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pygments/util.py` & `mylove-1.0.0/venv/Lib/site-packages/pygments/util.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/LICENSE.txt` & `mylove-1.0.0/venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/readme_renderer/__about__.py` & `mylove-1.0.0/venv/Lib/site-packages/readme_renderer/__about__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/readme_renderer/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/readme_renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/readme_renderer/__main__.py` & `mylove-1.0.0/venv/Lib/site-packages/readme_renderer/__main__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/readme_renderer/clean.py` & `mylove-1.0.0/venv/Lib/site-packages/readme_renderer/clean.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/readme_renderer/markdown.py` & `mylove-1.0.0/venv/Lib/site-packages/readme_renderer/markdown.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/readme_renderer/rst.py` & `mylove-1.0.0/venv/Lib/site-packages/readme_renderer/rst.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/readme_renderer/txt.py` & `mylove-1.0.0/venv/Lib/site-packages/readme_renderer/txt.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests/_internal_utils.py` & `mylove-1.0.0/venv/Lib/site-packages/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests/adapters.py` & `mylove-1.0.0/venv/Lib/site-packages/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests/api.py` & `mylove-1.0.0/venv/Lib/site-packages/requests/api.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests/auth.py` & `mylove-1.0.0/venv/Lib/site-packages/requests/auth.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests/compat.py` & `mylove-1.0.0/venv/Lib/site-packages/requests/compat.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests/cookies.py` & `mylove-1.0.0/venv/Lib/site-packages/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests/exceptions.py` & `mylove-1.0.0/venv/Lib/site-packages/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests/help.py` & `mylove-1.0.0/venv/Lib/site-packages/requests/help.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests/hooks.py` & `mylove-1.0.0/venv/Lib/site-packages/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests/models.py` & `mylove-1.0.0/venv/Lib/site-packages/requests/models.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests/packages.py` & `mylove-1.0.0/venv/Lib/site-packages/requests/packages.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests/sessions.py` & `mylove-1.0.0/venv/Lib/site-packages/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests/status_codes.py` & `mylove-1.0.0/venv/Lib/site-packages/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests/structures.py` & `mylove-1.0.0/venv/Lib/site-packages/requests/structures.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests/utils.py` & `mylove-1.0.0/venv/Lib/site-packages/requests/utils.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/_compat.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/_compat.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/appengine.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/adapters/appengine.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/fingerprint.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/adapters/fingerprint.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/host_header_ssl.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/adapters/host_header_ssl.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/socket_options.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/adapters/socket_options.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/source.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/adapters/source.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/ssl.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/adapters/ssl.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/adapters/x509.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/adapters/x509.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/auth/_digest_auth_compat.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/auth/_digest_auth_compat.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/auth/guess.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/auth/guess.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/auth/handler.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/auth/handler.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/auth/http_proxy_digest.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/auth/http_proxy_digest.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/downloadutils/stream.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/downloadutils/stream.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/downloadutils/tee.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/downloadutils/tee.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/exceptions.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/exceptions.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/multipart/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/multipart/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/multipart/decoder.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/multipart/decoder.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/multipart/encoder.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/multipart/encoder.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/sessions.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/sessions.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/streaming_iterator.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/streaming_iterator.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/threaded/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/threaded/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/threaded/pool.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/threaded/pool.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/threaded/thread.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/threaded/thread.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/utils/deprecated.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/utils/dump.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/utils/dump.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/utils/formdata.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/utils/formdata.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/requests_toolbelt/utils/user_agent.py` & `mylove-1.0.0/venv/Lib/site-packages/requests_toolbelt/utils/user_agent.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rfc3986/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/rfc3986/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rfc3986/_mixin.py` & `mylove-1.0.0/venv/Lib/site-packages/rfc3986/_mixin.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rfc3986/abnf_regexp.py` & `mylove-1.0.0/venv/Lib/site-packages/rfc3986/abnf_regexp.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rfc3986/api.py` & `mylove-1.0.0/venv/Lib/site-packages/rfc3986/api.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rfc3986/builder.py` & `mylove-1.0.0/venv/Lib/site-packages/rfc3986/builder.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rfc3986/compat.py` & `mylove-1.0.0/venv/Lib/site-packages/rfc3986/compat.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rfc3986/exceptions.py` & `mylove-1.0.0/venv/Lib/site-packages/rfc3986/exceptions.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rfc3986/iri.py` & `mylove-1.0.0/venv/Lib/site-packages/rfc3986/iri.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rfc3986/misc.py` & `mylove-1.0.0/venv/Lib/site-packages/rfc3986/misc.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rfc3986/normalizers.py` & `mylove-1.0.0/venv/Lib/site-packages/rfc3986/normalizers.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rfc3986/parseresult.py` & `mylove-1.0.0/venv/Lib/site-packages/rfc3986/parseresult.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rfc3986/uri.py` & `mylove-1.0.0/venv/Lib/site-packages/rfc3986/uri.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rfc3986/validators.py` & `mylove-1.0.0/venv/Lib/site-packages/rfc3986/validators.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/__main__.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/_cell_widths.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/_emoji_codes.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/_emoji_replace.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/_export_format.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/_fileno.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/_fileno.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/_inspect.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/_log_render.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/_loop.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/_null_file.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/_palettes.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/_ratio.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/_spinners.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/_win32_console.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/_windows.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/_windows_renderer.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/_wrap.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/abc.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/abc.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/align.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/align.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/ansi.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/bar.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/bar.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/box.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/box.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/cells.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/cells.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/color.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/color.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/color_triplet.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/columns.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/columns.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/console.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/console.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/constrain.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/containers.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/containers.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/control.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/control.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/default_styles.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/diagnose.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/emoji.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/errors.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/errors.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/file_proxy.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/filesize.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/highlighter.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/json.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/json.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/jupyter.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/layout.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/layout.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/live.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/live.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/live_render.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/logging.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/logging.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/markdown.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/markdown.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/markup.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/markup.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/measure.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/measure.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/padding.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/padding.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/pager.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/pager.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/palette.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/palette.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/panel.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/panel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/pretty.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/progress.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/progress.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/progress_bar.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/prompt.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/protocol.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/repr.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/repr.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/rule.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/rule.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/scope.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/scope.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/screen.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/screen.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/segment.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/segment.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/spinner.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/status.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/status.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/style.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/style.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/styled.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/styled.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/syntax.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/table.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/table.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/terminal_theme.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/text.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/text.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/theme.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/theme.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/traceback.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/rich/tree.py` & `mylove-1.0.0/venv/Lib/site-packages/rich/tree.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/_collections.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/_collections.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/archive_util.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/archive_util.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/cmd.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/cmd.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/build.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/check.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/check.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/clean.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/clean.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/config.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/config.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/install.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/install.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/register.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/register.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/command/upload.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/command/upload.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/config.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/config.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/core.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/core.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/dep_util.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/dep_util.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/dir_util.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/dir_util.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/dist.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/dist.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/errors.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/errors.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/extension.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/extension.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/file_util.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/file_util.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/filelist.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/filelist.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/log.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/log.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/py39compat.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/py39compat.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/spawn.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/spawn.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/text_file.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/text_file.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/util.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/util.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/version.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/version.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_entry_points.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_entry_points.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_imp.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_importlib.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_importlib.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_itertools.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_itertools.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_path.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_path.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/actions.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/common.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/core.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/helpers.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/results.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/testing.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/unicode.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing/util.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/_vendor/zipp.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/archive_util.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/build_meta.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/command/alias.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/command/bdist_egg.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/command/bdist_rpm.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/command/build.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/command/build.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/command/build_clib.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/command/build_ext.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/command/build_py.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/command/develop.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/command/dist_info.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/command/easy_install.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/command/editable_wheel.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/command/editable_wheel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/command/egg_info.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/command/install.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/command/install_egg_info.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/command/install_lib.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/command/install_scripts.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/command/py36compat.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/command/py36compat.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/command/rotate.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/command/saveopts.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/command/sdist.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/command/setopt.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/command/test.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/command/test.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/command/upload_docs.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/config/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/config/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/config/expand.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/config/expand.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/config/pyprojecttoml.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/config/pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/config/setupcfg.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/config/setupcfg.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/dep_util.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/depends.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/discovery.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/discovery.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/dist.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/errors.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/extension.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/extern/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/glob.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/installer.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/installer.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/launch.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/logging.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/logging.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/monkey.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/msvc.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/namespaces.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/package_index.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/sandbox.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/unicode_utils.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/wheel.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools/windows_support.py` & `mylove-1.0.0/venv/Lib/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/setuptools-65.5.1.dist-info/entry_points.txt` & `mylove-1.0.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/six.py` & `mylove-1.0.0/venv/Lib/site-packages/six.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/speech_recognition/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/speech_recognition/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/speech_recognition/__main__.py` & `mylove-1.0.0/venv/Lib/site-packages/speech_recognition/__main__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/speech_recognition/audio.py` & `mylove-1.0.0/venv/Lib/site-packages/speech_recognition/audio.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/speech_recognition/pocketsphinx-data/en-US/LICENSE.txt` & `mylove-1.0.0/venv/Lib/site-packages/speech_recognition/pocketsphinx-data/en-US/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/speech_recognition/recognizers/whisper.py` & `mylove-1.0.0/venv/Lib/site-packages/speech_recognition/recognizers/whisper.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/twine/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/twine/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/twine/__main__.py` & `mylove-1.0.0/venv/Lib/site-packages/twine/__main__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/twine/auth.py` & `mylove-1.0.0/venv/Lib/site-packages/twine/auth.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/twine/cli.py` & `mylove-1.0.0/venv/Lib/site-packages/twine/cli.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/twine/commands/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/twine/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/twine/commands/check.py` & `mylove-1.0.0/venv/Lib/site-packages/twine/commands/check.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/twine/commands/register.py` & `mylove-1.0.0/venv/Lib/site-packages/twine/commands/register.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/twine/commands/upload.py` & `mylove-1.0.0/venv/Lib/site-packages/twine/commands/upload.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/twine/exceptions.py` & `mylove-1.0.0/venv/Lib/site-packages/twine/exceptions.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/twine/package.py` & `mylove-1.0.0/venv/Lib/site-packages/twine/package.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/twine/repository.py` & `mylove-1.0.0/venv/Lib/site-packages/twine/repository.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/twine/settings.py` & `mylove-1.0.0/venv/Lib/site-packages/twine/settings.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/twine/utils.py` & `mylove-1.0.0/venv/Lib/site-packages/twine/utils.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/twine/wheel.py` & `mylove-1.0.0/venv/Lib/site-packages/twine/wheel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/twine/wininst.py` & `mylove-1.0.0/venv/Lib/site-packages/twine/wininst.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/_base_connection.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/_base_connection.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/_collections.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/_request_methods.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/_request_methods.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/connection.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/connectionpool.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/contrib/_securetransport/bindings.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/contrib/_securetransport/low_level.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/contrib/pyopenssl.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/contrib/securetransport.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/contrib/socks.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/exceptions.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/fields.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/filepost.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/poolmanager.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/response.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/util/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/util/connection.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/util/proxy.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/util/request.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/util/response.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/util/retry.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/util/ssl_.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/util/ssl_match_hostname.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/util/ssltransport.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/util/timeout.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/util/url.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/util/util.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/util/util.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3/util/wait.py` & `mylove-1.0.0/venv/Lib/site-packages/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/urllib3-2.0.3.dist-info/licenses/LICENSE.txt` & `mylove-1.0.0/venv/Lib/site-packages/urllib3-2.0.3.dist-info/licenses/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/webencodings/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/webencodings/labels.py` & `mylove-1.0.0/venv/Lib/site-packages/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/webencodings/mklabels.py` & `mylove-1.0.0/venv/Lib/site-packages/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/webencodings/tests.py` & `mylove-1.0.0/venv/Lib/site-packages/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/webencodings/x_user_defined.py` & `mylove-1.0.0/venv/Lib/site-packages/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/wheel/_setuptools_logging.py` & `mylove-1.0.0/venv/Lib/site-packages/wheel/_setuptools_logging.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/wheel/bdist_wheel.py` & `mylove-1.0.0/venv/Lib/site-packages/wheel/bdist_wheel.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/wheel/cli/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/wheel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/wheel/cli/convert.py` & `mylove-1.0.0/venv/Lib/site-packages/wheel/cli/convert.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/wheel/cli/pack.py` & `mylove-1.0.0/venv/Lib/site-packages/wheel/cli/pack.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/wheel/cli/unpack.py` & `mylove-1.0.0/venv/Lib/site-packages/wheel/cli/unpack.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/wheel/macosx_libfile.py` & `mylove-1.0.0/venv/Lib/site-packages/wheel/macosx_libfile.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/wheel/metadata.py` & `mylove-1.0.0/venv/Lib/site-packages/wheel/metadata.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/wheel/util.py` & `mylove-1.0.0/venv/Lib/site-packages/wheel/util.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/wheel/vendored/packaging/_manylinux.py` & `mylove-1.0.0/venv/Lib/site-packages/wheel/vendored/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/wheel/vendored/packaging/_musllinux.py` & `mylove-1.0.0/venv/Lib/site-packages/wheel/vendored/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/wheel/vendored/packaging/tags.py` & `mylove-1.0.0/venv/Lib/site-packages/wheel/vendored/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/wheel/wheelfile.py` & `mylove-1.0.0/venv/Lib/site-packages/wheel/wheelfile.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/wheel-0.38.4.dist-info/LICENSE.txt` & `mylove-1.0.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/_authentication.py` & `mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/cffi/_authentication.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/_common.py` & `mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/cffi/_common.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/_dll.py` & `mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/cffi/_dll.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/_resource.py` & `mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/cffi/_resource.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/_system_information.py` & `mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/cffi/_system_information.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/cffi/_util.py` & `mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/cffi/_util.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_authentication.py` & `mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/ctypes/_authentication.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_common.py` & `mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/ctypes/_common.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_dll.py` & `mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/ctypes/_dll.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_resource.py` & `mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/ctypes/_resource.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_system_information.py` & `mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/ctypes/_system_information.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_util.py` & `mylove-1.0.0/venv/Lib/site-packages/win32ctypes/core/ctypes/_util.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/win32ctypes/pywin32/pywintypes.py` & `mylove-1.0.0/venv/Lib/site-packages/win32ctypes/pywin32/pywintypes.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/win32ctypes/pywin32/win32api.py` & `mylove-1.0.0/venv/Lib/site-packages/win32ctypes/pywin32/win32api.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/win32ctypes/pywin32/win32cred.py` & `mylove-1.0.0/venv/Lib/site-packages/win32ctypes/pywin32/win32cred.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/win32ctypes/tests/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/win32ctypes/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/win32ctypes/tests/test_backends.py` & `mylove-1.0.0/venv/Lib/site-packages/win32ctypes/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/win32ctypes/tests/test_win32api.py` & `mylove-1.0.0/venv/Lib/site-packages/win32ctypes/tests/test_win32api.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/win32ctypes/tests/test_win32cred.py` & `mylove-1.0.0/venv/Lib/site-packages/win32ctypes/tests/test_win32cred.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/zipp/__init__.py` & `mylove-1.0.0/venv/Lib/site-packages/zipp/__init__.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Lib/site-packages/zipp/glob.py` & `mylove-1.0.0/venv/Lib/site-packages/zipp/glob.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Scripts/activate_this.py` & `mylove-1.0.0/venv/Scripts/activate_this.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Scripts/rst2html.py` & `mylove-1.0.0/venv/Scripts/rst2html.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Scripts/rst2html4.py` & `mylove-1.0.0/venv/Scripts/rst2html4.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Scripts/rst2html5.py` & `mylove-1.0.0/venv/Scripts/rst2html5.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Scripts/rst2latex.py` & `mylove-1.0.0/venv/Scripts/rst2latex.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Scripts/rst2man.py` & `mylove-1.0.0/venv/Scripts/rst2man.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Scripts/rst2odt.py` & `mylove-1.0.0/venv/Scripts/rst2odt.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Scripts/rst2odt_prepstyles.py` & `mylove-1.0.0/venv/Scripts/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Scripts/rst2pseudoxml.py` & `mylove-1.0.0/venv/Scripts/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Scripts/rst2s5.py` & `mylove-1.0.0/venv/Scripts/rst2s5.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Scripts/rst2xetex.py` & `mylove-1.0.0/venv/Scripts/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Scripts/rst2xml.py` & `mylove-1.0.0/venv/Scripts/rst2xml.py`

 * *Files identical despite different names*

### Comparing `mylove-0.0.2/venv/Scripts/rstpep2html.py` & `mylove-1.0.0/venv/Scripts/rstpep2html.py`

 * *Files identical despite different names*

