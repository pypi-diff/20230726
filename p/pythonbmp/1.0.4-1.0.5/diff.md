# Comparing `tmp/pythonbmp-1.0.4.tar.gz` & `tmp/pythonbmp-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonbmp-1.0.4.tar", last modified: Tue Jul 25 04:49:51 2023, max compression
+gzip compressed data, was "pythonbmp-1.0.5.tar", last modified: Wed Jul 26 08:27:33 2023, max compression
```

## Comparing `pythonbmp-1.0.4.tar` & `pythonbmp-1.0.5.tar`

### file list

```diff
@@ -1,240 +1,294 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 04:49:51.364934 pythonbmp-1.0.4/
--rw-rw-rw-   0        0        0     1090 2022-04-13 00:20:29.000000 pythonbmp-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      139 2023-07-25 04:30:25.000000 pythonbmp-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     4149 2023-07-25 04:49:51.362948 pythonbmp-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2187 2023-07-25 04:47:21.000000 pythonbmp-1.0.4/README.md
--rw-rw-rw-   0        0        0      896 2023-07-25 04:31:47.000000 pythonbmp-1.0.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-25 04:49:50.186403 pythonbmp-1.0.4/pythonbmp/
--rw-rw-rw-   0        0        0   449728 2023-03-06 17:05:20.000000 pythonbmp-1.0.4/pythonbmp/BITMAPlib.py
--rw-rw-rw-   0        0        0    66015 2022-06-25 10:49:24.000000 pythonbmp-1.0.4/pythonbmp/X11colordict.py
--rw-rw-rw-   0        0        0    91943 2022-05-29 23:32:29.000000 pythonbmp-1.0.4/pythonbmp/XKCDcolordict.py
--rw-rw-rw-   0        0        0        0 2022-04-13 00:20:29.000000 pythonbmp-1.0.4/pythonbmp/__init__.py
--rw-rw-rw-   0        0        0      783 2022-09-04 13:43:04.000000 pythonbmp-1.0.4/pythonbmp/bmpconstants.py
--rw-rw-rw-   0        0        0     8335 2022-05-29 18:00:32.000000 pythonbmp-1.0.4/pythonbmp/bmppal.py
--rw-rw-rw-   0        0        0     1885 2022-05-29 18:03:32.000000 pythonbmp-1.0.4/pythonbmp/bufferflip.py
--rw-rw-rw-   0        0        0     1877 2022-05-31 12:10:53.000000 pythonbmp-1.0.4/pythonbmp/buffersplit.py
--rw-rw-rw-   0        0        0     6634 2022-05-31 12:10:53.000000 pythonbmp-1.0.4/pythonbmp/bufresize.py
--rw-rw-rw-   0        0        0     1401 2022-05-31 12:10:53.000000 pythonbmp-1.0.4/pythonbmp/chartools.py
--rw-rw-rw-   0        0        0     1422 2022-05-31 12:10:53.000000 pythonbmp-1.0.4/pythonbmp/charts.py
--rw-rw-rw-   0        0        0     4603 2022-05-29 22:58:36.000000 pythonbmp-1.0.4/pythonbmp/colordict.py
--rw-rw-rw-   0        0        0    28282 2022-09-19 08:21:23.000000 pythonbmp-1.0.4/pythonbmp/colors.py
--rw-rw-rw-   0        0        0     1575 2022-05-29 19:14:32.000000 pythonbmp-1.0.4/pythonbmp/conditionaltools.py
--rw-rw-rw-   0        0        0      853 2022-05-31 12:10:53.000000 pythonbmp-1.0.4/pythonbmp/dicttools.py
--rw-rw-rw-   0        0        0     1637 2022-06-05 11:41:44.000000 pythonbmp-1.0.4/pythonbmp/fileutils.py
--rw-rw-rw-   0        0        0   113333 2023-02-21 07:03:50.000000 pythonbmp-1.0.4/pythonbmp/fonts.py
--rw-rw-rw-   0        0        0    57313 2023-07-12 05:53:17.000000 pythonbmp-1.0.4/pythonbmp/fractals.py
--rw-rw-rw-   0        0        0      346 2022-06-09 11:01:53.000000 pythonbmp-1.0.4/pythonbmp/funcmeta.py
--rw-rw-rw-   0        0        0     2380 2022-08-27 08:50:11.000000 pythonbmp-1.0.4/pythonbmp/inttools.py
--rw-rw-rw-   0        0        0    44529 2022-10-04 08:21:21.000000 pythonbmp-1.0.4/pythonbmp/mathlib.py
--rw-rw-rw-   0        0        0     2498 2022-09-14 06:02:31.000000 pythonbmp-1.0.4/pythonbmp/messages.py
--rw-rw-rw-   0        0        0     9821 2022-08-30 02:29:48.000000 pythonbmp-1.0.4/pythonbmp/paramchecks.py
--rw-rw-rw-   0        0        0    40078 2022-09-07 22:46:41.000000 pythonbmp-1.0.4/pythonbmp/primitives2D.py
--rw-rw-rw-   0        0        0     1860 2022-06-05 03:55:11.000000 pythonbmp-1.0.4/pythonbmp/proctimer.py
--rw-rw-rw-   0        0        0      818 2022-08-30 12:38:45.000000 pythonbmp-1.0.4/pythonbmp/shims.py
--rw-rw-rw-   0        0        0    19674 2022-09-07 20:14:18.000000 pythonbmp-1.0.4/pythonbmp/solids3D.py
--rw-rw-rw-   0        0        0     1869 2022-07-21 16:34:56.000000 pythonbmp-1.0.4/pythonbmp/textgraphics.py
-drwxrwxrwx   0        0        0        0 2023-07-25 04:49:50.217405 pythonbmp-1.0.4/pythonbmp.egg-info/
--rw-rw-rw-   0        0        0     4149 2023-07-25 04:49:49.000000 pythonbmp-1.0.4/pythonbmp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9494 2023-07-25 04:49:49.000000 pythonbmp-1.0.4/pythonbmp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 04:49:49.000000 pythonbmp-1.0.4/pythonbmp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-25 04:49:49.000000 pythonbmp-1.0.4/pythonbmp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-25 04:49:50.236406 pythonbmp-1.0.4/samples/
-drwxrwxrwx   0        0        0        0 2023-07-25 04:49:50.333403 pythonbmp-1.0.4/samples/3d/
--rw-rw-rw-   0        0        0     4170 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_3D.py
--rw-rw-rw-   0        0        0     1853 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_3D_surfaceplot.py
--rw-rw-rw-   0        0        0     1898 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_Benzene.py
--rw-rw-rw-   0        0        0     2350 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_Coin.py
--rw-rw-rw-   0        0        0     2298 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_Cone.py
--rw-rw-rw-   0        0        0     2105 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_Cube.py
--rw-rw-rw-   0        0        0     2033 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_Decahedron.py
--rw-rw-rw-   0        0        0     2046 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_DiscoBall.py
--rw-rw-rw-   0        0        0     1793 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_Globe.py
--rw-rw-rw-   0        0        0     1886 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_Icosahedron.py
--rw-rw-rw-   0        0        0     2006 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_Icosahedron_Outline.py
--rw-rw-rw-   0        0        0     2348 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_Octahedron.py
--rw-rw-rw-   0        0        0     1497 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/3d/Hello_Sphere.py
--rw-rw-rw-   0        0        0     2330 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/3d/Hello_Tetrahedron.py
--rw-rw-rw-   0        0        0     3679 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/Hello_APP_Github_ID.py
--rw-rw-rw-   0        0        0     1210 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/Hello_Darkness.py
-drwxrwxrwx   0        0        0        0 2023-07-25 04:49:50.570497 pythonbmp-1.0.4/samples/colorgradients/
--rw-rw-rw-   0        0        0     1603 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Circular_Gradient.py
--rw-rw-rw-   0        0        0     1467 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Dichromic_Circular_Gradient.py
--rw-rw-rw-   0        0        0     1507 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Dichromic_Circular_Gradient_smoothstep.py
--rw-rw-rw-   0        0        0     1539 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Elliptical_Gradient.py
--rw-rw-rw-   0        0        0     1514 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromatichoriGradRect.py
--rw-rw-rw-   0        0        0     1562 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromatichoriGradRectsmootherstep.py
--rw-rw-rw-   0        0        0     1565 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromatichoriGradRectsmootheststep.py
--rw-rw-rw-   0        0        0     1556 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromatichoriGradRectsmoothstep.py
--rw-rw-rw-   0        0        0     1510 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromaticvertGradRect.py
--rw-rw-rw-   0        0        0     1558 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromaticvertGradRectsmootherstep.py
--rw-rw-rw-   0        0        0     1561 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromaticvertGradRectsmootheststep.py
--rw-rw-rw-   0        0        0     1552 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromaticvertGradRectsmoothstep.py
--rw-rw-rw-   0        0        0     1480 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilledhoriGradRect.py
--rw-rw-rw-   0        0        0     1531 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilledhoriGradRectsmootherstep.py
--rw-rw-rw-   0        0        0     1534 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilledhoriGradRectsmootheststep.py
--rw-rw-rw-   0        0        0     1525 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilledhoriGradRectsmoothstep.py
--rw-rw-rw-   0        0        0     1476 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilledvertGradRect.py
--rw-rw-rw-   0        0        0     1527 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilledvertGradRectsmootherstep.py
--rw-rw-rw-   0        0        0     1530 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilledvertGradRectsmootheststep.py
--rw-rw-rw-   0        0        0     1521 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilledvertGradRectsmoothstep.py
--rw-rw-rw-   0        0        0     1401 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Linear_Gradient.py
--rw-rw-rw-   0        0        0     1856 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_NonLinearRadialMultichannel_Gradients.py
--rw-rw-rw-   0        0        0     1758 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_NonLinearRadial_Gradients.py
--rw-rw-rw-   0        0        0     1466 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Orb.py
--rw-rw-rw-   0        0        0     1870 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_RadialMultichannel_Gradients.py
--rw-rw-rw-   0        0        0     1884 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Radial_Gradients.py
--rw-rw-rw-   0        0        0     1530 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Sphere_dichromic.py
--rw-rw-rw-   0        0        0     1578 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Sphere_dichromic_smootherstep.py
--rw-rw-rw-   0        0        0     1581 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Sphere_dichromic_smootheststep.py
--rw-rw-rw-   0        0        0     1573 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Sphere_dichromic_smoothstep.py
--rw-rw-rw-   0        0        0     1524 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Sphere_smootherstep.py
--rw-rw-rw-   0        0        0     1527 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Sphere_smootheststep.py
--rw-rw-rw-   0        0        0     1519 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Sphere_smoothstep.py
--rw-rw-rw-   0        0        0  1440054 2023-07-25 04:28:42.000000 pythonbmp-1.0.4/samples/colorgradients/HellodistcentercoordplotRGBxybit1.bmp
-drwxrwxrwx   0        0        0        0 2023-07-25 04:49:50.598510 pythonbmp-1.0.4/samples/colornames/
--rw-rw-rw-   0        0        0     1701 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colornames/Hello_ColorNames.py
--rw-rw-rw-   0        0        0     1710 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/colornames/Hello_X11ColorNames.py
--rw-rw-rw-   0        0        0     1754 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/colornames/Hello_XKCDColorNames.py
-drwxrwxrwx   0        0        0        0 2023-07-25 04:49:50.681495 pythonbmp-1.0.4/samples/curves/
--rw-rw-rw-   0        0        0     1645 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/curves/Hello_Cardioid.py
--rw-rw-rw-   0        0        0     1456 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/curves/Hello_CornuSpiral.py
--rw-rw-rw-   0        0        0     1506 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/curves/Hello_EggCurve.py
--rw-rw-rw-   0        0        0     1760 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/curves/Hello_Epicycloid.py
--rw-rw-rw-   0        0        0     1679 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/curves/Hello_Flower.py
--rw-rw-rw-   0        0        0     1551 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/curves/Hello_GearCurve.py
--rw-rw-rw-   0        0        0     1475 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/curves/Hello_HeartCurve.py
--rw-rw-rw-   0        0        0     1807 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/curves/Hello_Hypotrochoid.py
--rw-rw-rw-   0        0        0     1658 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/curves/Hello_InvoluteofaCircle.py
--rw-rw-rw-   0        0        0     1621 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/curves/Hello_Octopetala.py
--rw-rw-rw-   0        0        0     1688 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/curves/Hello_SquareSpiral.py
--rw-rw-rw-   0        0        0     1542 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/curves/Hello_Squircles.py
--rw-rw-rw-   0        0        0     1672 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/curves/Hello_Superellipse.py
--rw-rw-rw-   0        0        0     2133 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/curves/Hello_Thick_Exponential_Spiral_Gradient.py
-drwxrwxrwx   0        0        0        0 2023-07-25 04:49:50.854116 pythonbmp-1.0.4/samples/fonts/
--rw-rw-rw-   0        0        0     1760 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_WorId_Italic_RainbowSideway.py
--rw-rw-rw-   0        0        0     1505 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World.py
--rw-rw-rw-   0        0        0     1558 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots.py
--rw-rw-rw-   0        0        0     1580 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_Italicupsidedown.py
--rw-rw-rw-   0        0        0     1779 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_Rainbow_vertical.py
--rw-rw-rw-   0        0        0     1775 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_italic_rainbowsideway.py
--rw-rw-rw-   0        0        0     1577 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_italicsideway.py
--rw-rw-rw-   0        0        0     1575 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_italicvertical.py
--rw-rw-rw-   0        0        0     1777 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_italicvertical_rainbow.py
--rw-rw-rw-   0        0        0     1788 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_rainbowItalicupsidedown.py
--rw-rw-rw-   0        0        0     1792 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_rainbowreversedItalic.py
--rw-rw-rw-   0        0        0     1779 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_rainbowsideway.py
--rw-rw-rw-   0        0        0     1785 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_rainbowupsidedown.py
--rw-rw-rw-   0        0        0     1569 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_reversed.py
--rw-rw-rw-   0        0        0     1578 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_reversedItalic.py
--rw-rw-rw-   0        0        0     1563 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_sideway.py
--rw-rw-rw-   0        0        0     1572 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_upsidedown.py
--rw-rw-rw-   0        0        0     1569 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_vertical.py
--rw-rw-rw-   0        0        0     1414 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Italic.py
--rw-rw-rw-   0        0        0     1417 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Italicdots.py
--rw-rw-rw-   0        0        0     1572 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Italicupsidedown.py
--rw-rw-rw-   0        0        0     1768 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Rainbow_Dots.py
--rw-rw-rw-   0        0        0     1584 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Rainbow_Italic.py
--rw-rw-rw-   0        0        0     1773 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Rainbow_Italic_Dots.py
--rw-rw-rw-   0        0        0     1770 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Rainbow_vertical.py
--rw-rw-rw-   0        0        0     1568 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_italicsideway.py
--rw-rw-rw-   0        0        0     1568 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_italicvertical.py
--rw-rw-rw-   0        0        0     1774 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_italicvertical_rainbow.py
--rw-rw-rw-   0        0        0     1771 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_rainbowItalicupsidedown.py
--rw-rw-rw-   0        0        0     1766 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_rainbowreversedItalic.py
--rw-rw-rw-   0        0        0     1770 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_rainbowsideway.py
--rw-rw-rw-   0        0        0     1761 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_rainbowupsidedown.py
--rw-rw-rw-   0        0        0     1514 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_reversedItalic.py
-drwxrwxrwx   0        0        0        0 2023-07-25 04:49:51.222936 pythonbmp-1.0.4/samples/fractals/
--rw-rw-rw-   0        0        0     1307 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Astroidfractal.py
--rw-rw-rw-   0        0        0     1466 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_BarnsleyTree.py
--rw-rw-rw-   0        0        0     1431 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_CatPaws.py
--rw-rw-rw-   0        0        0     1262 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_CliffordAttractor.py
--rw-rw-rw-   0        0        0     1474 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_CosJulia_Set.py
--rw-rw-rw-   0        0        0     1259 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_DuffingAttractor.py
--rw-rw-rw-   0        0        0     1238 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Fern.py
--rw-rw-rw-   0        0        0     1287 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_FractalDreamAttractor.py
--rw-rw-rw-   0        0        0     1267 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Gumowski-Mira_attractor.py
--rw-rw-rw-   0        0        0     1266 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Gumowski-Mira_attractor_1.py
--rw-rw-rw-   0        0        0     1161 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_HilbertCurve.py
--rw-rw-rw-   0        0        0     1260 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_HopalongAttractor.py
--rw-rw-rw-   0        0        0     1261 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Ikedaattractor.py
--rw-rw-rw-   0        0        0     1497 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Julia_Set.py
--rw-rw-rw-   0        0        0     1585 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_KochCurve.py
--rw-rw-rw-   0        0        0     1627 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_KochSnowflake.py
--rw-rw-rw-   0        0        0     1379 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Lambdafractal.py
--rw-rw-rw-   0        0        0     1308 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Lemniscatefractal.py
--rw-rw-rw-   0        0        0     1732 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_LissajousCurve.py
--rw-rw-rw-   0        0        0     1354 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Mandelbrot_Set.py
--rw-rw-rw-   0        0        0     1388 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Mandelbrot_Set_dichromatic.py
--rw-rw-rw-   0        0        0     1431 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MarekDragon.py
--rw-rw-rw-   0        0        0     1437 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MarekDragon_4bit.py
--rw-rw-rw-   0        0        0     1504 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Multi2ndtetrationBiomorphfractal.py
--rw-rw-rw-   0        0        0     1523 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiBiomorphfractal.py
--rw-rw-rw-   0        0        0     1554 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiBiomorphphasevariantfractal.py
--rw-rw-rw-   0        0        0     1498 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiBiomorphvariantfractal.py
--rw-rw-rw-   0        0        0     1501 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiBiomorphvariantfractal1.py
--rw-rw-rw-   0        0        0     1531 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiCosBiomorphfractal.py
--rw-rw-rw-   0        0        0     1504 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiCoshBiomorphfractal.py
--rw-rw-rw-   0        0        0     1494 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiSinBiomorphfractal.py
--rw-rw-rw-   0        0        0     1508 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiSinhBiomorphfractal.py
--rw-rw-rw-   0        0        0     1502 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiTanBiomorphfractal.py
--rw-rw-rw-   0        0        0     1531 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiTanBiomorphfractal_dichromatic.py
--rw-rw-rw-   0        0        0     1504 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiTanhBiomorphfractal.py
--rw-rw-rw-   0        0        0     1433 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Multibrot_Set.py
--rw-rw-rw-   0        0        0     1426 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Multicircle.py
--rw-rw-rw-   0        0        0     1461 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Multicircle_dichromatic.py
--rw-rw-rw-   0        0        0     1413 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Multicorn_Set.py
--rw-rw-rw-   0        0        0     1494 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiexpBiomorphfractal.py
--rw-rw-rw-   0        0        0     1414 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Multihyperbola.py
--rw-rw-rw-   0        0        0     1497 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Multijulia_Set.py
--rw-rw-rw-   0        0        0     1315 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Multisuperellipse.py
--rw-rw-rw-   0        0        0     1501 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultizconjugateBiomorphfractal.py
--rw-rw-rw-   0        0        0     1528 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal.py
--rw-rw-rw-   0        0        0     1551 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal4.py
--rw-rw-rw-   0        0        0     1552 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal4_1.py
--rw-rw-rw-   0        0        0     1575 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal5.py
--rw-rw-rw-   0        0        0     1577 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal5_1.py
--rw-rw-rw-   0        0        0     1578 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal5_3.py
--rw-rw-rw-   0        0        0     1627 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal6.py
--rw-rw-rw-   0        0        0     1629 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal6_3.py
--rw-rw-rw-   0        0        0     1272 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_PeterdeJongAttractor.py
--rw-rw-rw-   0        0        0     1474 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fractals/Hello_SinJulia_Set.py
--rw-rw-rw-   0        0        0     1472 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fractals/Hello_SinJulia_Set_1bit.py
--rw-rw-rw-   0        0        0     1487 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fractals/Hello_SinJulia_Set_4bit.py
--rw-rw-rw-   0        0        0     1489 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fractals/Hello_SpiralJulia_Set.py
--rw-rw-rw-   0        0        0     1314 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fractals/Hello_Symmetric_Icon_Attractor.py
--rw-rw-rw-   0        0        0     1294 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fractals/Hello_Tetration_Fractal.py
--rw-rw-rw-   0        0        0     1783 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fractals/Hello_ThickGradHilbertCurve.py
--rw-rw-rw-   0        0        0     1279 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fractals/Hello_ThickHilbertCurve.py
--rw-rw-rw-   0        0        0     1401 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fractals/Hello_Tricorn_Set.py
--rw-rw-rw-   0        0        0     1416 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fractals/Hello_Xordivfractal.py
--rw-rw-rw-   0        0        0     1329 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fractals/Hello_Xorfractal.py
--rw-rw-rw-   0        0        0     1262 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_nattractor.py
--rw-rw-rw-   0        0        0     1472 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_ngonfractal.py
-drwxrwxrwx   0        0        0        0 2023-07-25 04:49:51.228931 pythonbmp-1.0.4/samples/graphs/
--rw-rw-rw-   0        0        0     2230 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/graphs/Hello_XYScatterplot.py
-drwxrwxrwx   0        0        0        0 2023-07-25 04:49:51.336931 pythonbmp-1.0.4/samples/primitives2d/
--rw-rw-rw-   0        0        0     1711 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_BezierCurve.py
--rw-rw-rw-   0        0        0     1943 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Bspline.py
--rw-rw-rw-   0        0        0     1544 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Circles.py
--rw-rw-rw-   0        0        0     1415 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Ellipse.py
--rw-rw-rw-   0        0        0     1713 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_FilledCircle.py
--rw-rw-rw-   0        0        0     1677 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_FilledEllipse.py
--rw-rw-rw-   0        0        0     1679 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_FilledRectangle.py
--rw-rw-rw-   0        0        0     1868 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Gradient_Thick_Regular_Polygon.py
--rw-rw-rw-   0        0        0     1485 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Lines.py
--rw-rw-rw-   0        0        0     1550 2023-07-21 14:08:45.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Rectangle.py
--rw-rw-rw-   0        0        0     1672 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Regular_Polygon.py
--rw-rw-rw-   0        0        0     1699 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Thick_Circle.py
--rw-rw-rw-   0        0        0     1709 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Thick_Gradient_Circle.py
--rw-rw-rw-   0        0        0     1721 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Thick_Gradient_Ellipse_Rotated.py
--rw-rw-rw-   0        0        0     1479 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Thick_Regular_Polygon.py
--rw-rw-rw-   0        0        0     1665 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Thick_Round_Gradient_Line.py
--rw-rw-rw-   0        0        0     1772 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Thick_Round_Line.py
--rw-rw-rw-   0        0        0     1461 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Vector.py
-drwxrwxrwx   0        0        0        0 2023-07-25 04:49:51.356930 pythonbmp-1.0.4/samples/spirographs/
--rw-rw-rw-   0        0        0     1759 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/spirographs/Hello_Spirograph.py
--rw-rw-rw-   0        0        0     1856 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/spirographs/Hello_Spirograph_1.py
--rw-rw-rw-   0        0        0     1772 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/spirographs/Hello_Spirograph_2.py
--rw-rw-rw-   0        0        0     1639 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/spirographs/Hello_Spirograph_Record.py
--rw-rw-rw-   0        0        0       42 2023-07-25 04:49:51.365930 pythonbmp-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 08:27:33.335472 pythonbmp-1.0.5/
+-rw-rw-rw-   0        0        0     1090 2022-04-13 00:20:29.000000 pythonbmp-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      139 2023-07-26 08:23:32.000000 pythonbmp-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4157 2023-07-26 08:27:33.288470 pythonbmp-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2195 2023-07-25 15:21:08.000000 pythonbmp-1.0.5/README.md
+-rw-rw-rw-   0        0        0      896 2023-07-26 08:12:11.000000 pythonbmp-1.0.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-26 08:27:16.804466 pythonbmp-1.0.5/pythonbmp/
+-rw-rw-rw-   0        0        0   449728 2023-03-06 17:05:20.000000 pythonbmp-1.0.5/pythonbmp/BITMAPlib.py
+-rw-rw-rw-   0        0        0    66015 2022-06-25 10:49:24.000000 pythonbmp-1.0.5/pythonbmp/X11colordict.py
+-rw-rw-rw-   0        0        0    91943 2022-05-29 23:32:29.000000 pythonbmp-1.0.5/pythonbmp/XKCDcolordict.py
+-rw-rw-rw-   0        0        0        0 2022-04-13 00:20:29.000000 pythonbmp-1.0.5/pythonbmp/__init__.py
+-rw-rw-rw-   0        0        0      783 2022-09-04 13:43:04.000000 pythonbmp-1.0.5/pythonbmp/bmpconstants.py
+-rw-rw-rw-   0        0        0     8335 2022-05-29 18:00:32.000000 pythonbmp-1.0.5/pythonbmp/bmppal.py
+-rw-rw-rw-   0        0        0     1885 2022-05-29 18:03:32.000000 pythonbmp-1.0.5/pythonbmp/bufferflip.py
+-rw-rw-rw-   0        0        0     1877 2022-05-31 12:10:53.000000 pythonbmp-1.0.5/pythonbmp/buffersplit.py
+-rw-rw-rw-   0        0        0     6634 2022-05-31 12:10:53.000000 pythonbmp-1.0.5/pythonbmp/bufresize.py
+-rw-rw-rw-   0        0        0     1401 2022-05-31 12:10:53.000000 pythonbmp-1.0.5/pythonbmp/chartools.py
+-rw-rw-rw-   0        0        0     1422 2022-05-31 12:10:53.000000 pythonbmp-1.0.5/pythonbmp/charts.py
+-rw-rw-rw-   0        0        0     4603 2022-05-29 22:58:36.000000 pythonbmp-1.0.5/pythonbmp/colordict.py
+-rw-rw-rw-   0        0        0    28282 2022-09-19 08:21:23.000000 pythonbmp-1.0.5/pythonbmp/colors.py
+-rw-rw-rw-   0        0        0     1575 2022-05-29 19:14:32.000000 pythonbmp-1.0.5/pythonbmp/conditionaltools.py
+-rw-rw-rw-   0        0        0      853 2022-05-31 12:10:53.000000 pythonbmp-1.0.5/pythonbmp/dicttools.py
+-rw-rw-rw-   0        0        0     1637 2022-06-05 11:41:44.000000 pythonbmp-1.0.5/pythonbmp/fileutils.py
+-rw-rw-rw-   0        0        0   113333 2023-02-21 07:03:50.000000 pythonbmp-1.0.5/pythonbmp/fonts.py
+-rw-rw-rw-   0        0        0    57313 2023-07-12 05:53:17.000000 pythonbmp-1.0.5/pythonbmp/fractals.py
+-rw-rw-rw-   0        0        0      346 2022-06-09 11:01:53.000000 pythonbmp-1.0.5/pythonbmp/funcmeta.py
+-rw-rw-rw-   0        0        0     2380 2022-08-27 08:50:11.000000 pythonbmp-1.0.5/pythonbmp/inttools.py
+-rw-rw-rw-   0        0        0    44529 2022-10-04 08:21:21.000000 pythonbmp-1.0.5/pythonbmp/mathlib.py
+-rw-rw-rw-   0        0        0     2498 2022-09-14 06:02:31.000000 pythonbmp-1.0.5/pythonbmp/messages.py
+-rw-rw-rw-   0        0        0     9821 2022-08-30 02:29:48.000000 pythonbmp-1.0.5/pythonbmp/paramchecks.py
+-rw-rw-rw-   0        0        0    40078 2022-09-07 22:46:41.000000 pythonbmp-1.0.5/pythonbmp/primitives2D.py
+-rw-rw-rw-   0        0        0     1860 2022-06-05 03:55:11.000000 pythonbmp-1.0.5/pythonbmp/proctimer.py
+-rw-rw-rw-   0        0        0      818 2022-08-30 12:38:45.000000 pythonbmp-1.0.5/pythonbmp/shims.py
+-rw-rw-rw-   0        0        0    19674 2022-09-07 20:14:18.000000 pythonbmp-1.0.5/pythonbmp/solids3D.py
+-rw-rw-rw-   0        0        0     1869 2022-07-21 16:34:56.000000 pythonbmp-1.0.5/pythonbmp/textgraphics.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:27:17.022469 pythonbmp-1.0.5/pythonbmp.egg-info/
+-rw-rw-rw-   0        0        0     4157 2023-07-26 08:27:13.000000 pythonbmp-1.0.5/pythonbmp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11646 2023-07-26 08:27:15.000000 pythonbmp-1.0.5/pythonbmp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 08:27:13.000000 pythonbmp-1.0.5/pythonbmp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-26 08:27:13.000000 pythonbmp-1.0.5/pythonbmp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:27:17.547470 pythonbmp-1.0.5/samples/
+drwxrwxrwx   0        0        0        0 2023-07-26 08:27:19.423469 pythonbmp-1.0.5/samples/3d/
+-rw-rw-rw-   0        0        0     4170 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/3d/Hello_3D.py
+-rw-rw-rw-   0        0        0     1853 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/3d/Hello_3D_surfaceplot.py
+-rw-rw-rw-   0        0        0     1898 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/3d/Hello_Benzene.py
+-rw-rw-rw-   0        0        0     2350 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/3d/Hello_Coin.py
+-rw-rw-rw-   0        0        0     2298 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/3d/Hello_Cone.py
+-rw-rw-rw-   0        0        0     2105 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/3d/Hello_Cube.py
+-rw-rw-rw-   0        0        0     2033 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/3d/Hello_Decahedron.py
+-rw-rw-rw-   0        0        0     2046 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/3d/Hello_DiscoBall.py
+-rw-rw-rw-   0        0        0     1793 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/3d/Hello_Globe.py
+-rw-rw-rw-   0        0        0     1886 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/3d/Hello_Icosahedron.py
+-rw-rw-rw-   0        0        0     2006 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/3d/Hello_Icosahedron_Outline.py
+-rw-rw-rw-   0        0        0     2348 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/3d/Hello_Octahedron.py
+-rw-rw-rw-   0        0        0     1497 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/3d/Hello_Sphere.py
+-rw-rw-rw-   0        0        0     2330 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/3d/Hello_Tetrahedron.py
+-rw-rw-rw-   0        0        0    14983 2023-07-25 15:18:53.000000 pythonbmp-1.0.5/samples/Features_Speedtest.py
+-rw-rw-rw-   0        0        0     3679 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/Hello_APP_Github_ID.py
+-rw-rw-rw-   0        0        0     1210 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/Hello_Darkness.py
+-rw-rw-rw-   0        0        0  2457654 2023-07-25 05:13:33.000000 pythonbmp-1.0.5/samples/Hello_GithubID.bmp
+drwxrwxrwx   0        0        0        0 2023-07-26 08:27:19.989471 pythonbmp-1.0.5/samples/assets/
+-rw-rw-rw-   0        0        0    87038 2022-04-13 00:20:33.000000 pythonbmp-1.0.5/samples/assets/Earth.bmp
+-rw-rw-rw-   0        0        0    32886 2022-08-26 10:22:08.000000 pythonbmp-1.0.5/samples/assets/biomorph.bmp
+-rw-rw-rw-   0        0        0    14726 2022-06-29 14:46:16.000000 pythonbmp-1.0.5/samples/assets/earth-4bit.bmp
+-rw-rw-rw-   0        0        0   172854 2022-04-13 00:20:33.000000 pythonbmp-1.0.5/samples/assets/somebody.bmp
+-rw-rw-rw-   0        0        0   606670 2022-04-17 05:47:11.000000 pythonbmp-1.0.5/samples/assets/tanuki.bmp
+drwxrwxrwx   0        0        0        0 2023-07-26 08:27:23.721470 pythonbmp-1.0.5/samples/colorgradients/
+-rw-rw-rw-   0        0        0     1603 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_Circular_Gradient.py
+-rw-rw-rw-   0        0        0     1467 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_Dichromic_Circular_Gradient.py
+-rw-rw-rw-   0        0        0     1507 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_Dichromic_Circular_Gradient_smoothstep.py
+-rw-rw-rw-   0        0        0     1539 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_Elliptical_Gradient.py
+-rw-rw-rw-   0        0        0     1514 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_FilleddichromatichoriGradRect.py
+-rw-rw-rw-   0        0        0     1562 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_FilleddichromatichoriGradRectsmootherstep.py
+-rw-rw-rw-   0        0        0     1565 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_FilleddichromatichoriGradRectsmootheststep.py
+-rw-rw-rw-   0        0        0     1556 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_FilleddichromatichoriGradRectsmoothstep.py
+-rw-rw-rw-   0        0        0     1510 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_FilleddichromaticvertGradRect.py
+-rw-rw-rw-   0        0        0     1558 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_FilleddichromaticvertGradRectsmootherstep.py
+-rw-rw-rw-   0        0        0     1561 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_FilleddichromaticvertGradRectsmootheststep.py
+-rw-rw-rw-   0        0        0     1552 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_FilleddichromaticvertGradRectsmoothstep.py
+-rw-rw-rw-   0        0        0     1480 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_FilledhoriGradRect.py
+-rw-rw-rw-   0        0        0     1531 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_FilledhoriGradRectsmootherstep.py
+-rw-rw-rw-   0        0        0     1534 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_FilledhoriGradRectsmootheststep.py
+-rw-rw-rw-   0        0        0     1525 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_FilledhoriGradRectsmoothstep.py
+-rw-rw-rw-   0        0        0     1476 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_FilledvertGradRect.py
+-rw-rw-rw-   0        0        0     1527 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_FilledvertGradRectsmootherstep.py
+-rw-rw-rw-   0        0        0     1530 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_FilledvertGradRectsmootheststep.py
+-rw-rw-rw-   0        0        0     1521 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_FilledvertGradRectsmoothstep.py
+-rw-rw-rw-   0        0        0     1401 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_Linear_Gradient.py
+-rw-rw-rw-   0        0        0     1856 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_NonLinearRadialMultichannel_Gradients.py
+-rw-rw-rw-   0        0        0     1758 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_NonLinearRadial_Gradients.py
+-rw-rw-rw-   0        0        0     1466 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_Orb.py
+-rw-rw-rw-   0        0        0     1870 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_RadialMultichannel_Gradients.py
+-rw-rw-rw-   0        0        0     1884 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_Radial_Gradients.py
+-rw-rw-rw-   0        0        0     1530 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_Sphere_dichromic.py
+-rw-rw-rw-   0        0        0     1578 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_Sphere_dichromic_smootherstep.py
+-rw-rw-rw-   0        0        0     1581 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_Sphere_dichromic_smootheststep.py
+-rw-rw-rw-   0        0        0     1573 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_Sphere_dichromic_smoothstep.py
+-rw-rw-rw-   0        0        0     1524 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_Sphere_smootherstep.py
+-rw-rw-rw-   0        0        0     1527 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_Sphere_smootheststep.py
+-rw-rw-rw-   0        0        0     1519 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/colorgradients/Hello_Sphere_smoothstep.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:27:23.973482 pythonbmp-1.0.5/samples/colornames/
+-rw-rw-rw-   0        0        0     1701 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/colornames/Hello_ColorNames.py
+-rw-rw-rw-   0        0        0     1710 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/colornames/Hello_X11ColorNames.py
+-rw-rw-rw-   0        0        0     1754 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/colornames/Hello_XKCDColorNames.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:27:25.784473 pythonbmp-1.0.5/samples/curves/
+-rw-rw-rw-   0        0        0     1645 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/curves/Hello_Cardioid.py
+-rw-rw-rw-   0        0        0     1456 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/curves/Hello_CornuSpiral.py
+-rw-rw-rw-   0        0        0     1506 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/curves/Hello_EggCurve.py
+-rw-rw-rw-   0        0        0     1760 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/curves/Hello_Epicycloid.py
+-rw-rw-rw-   0        0        0     1679 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/curves/Hello_Flower.py
+-rw-rw-rw-   0        0        0     1551 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/curves/Hello_GearCurve.py
+-rw-rw-rw-   0        0        0     1475 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/curves/Hello_HeartCurve.py
+-rw-rw-rw-   0        0        0     1807 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/curves/Hello_Hypotrochoid.py
+-rw-rw-rw-   0        0        0     1658 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/curves/Hello_InvoluteofaCircle.py
+-rw-rw-rw-   0        0        0     1621 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/curves/Hello_Octopetala.py
+-rw-rw-rw-   0        0        0     1688 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/curves/Hello_SquareSpiral.py
+-rw-rw-rw-   0        0        0     1542 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/curves/Hello_Squircles.py
+-rw-rw-rw-   0        0        0     1672 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/curves/Hello_Superellipse.py
+-rw-rw-rw-   0        0        0     2133 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/curves/Hello_Thick_Exponential_Spiral_Gradient.py
+-rw-rw-rw-   0        0        0     1450 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/curves/Hello_Thick_Spiral_Gradient.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:27:29.417466 pythonbmp-1.0.5/samples/fonts/
+-rw-rw-rw-   0        0        0     1735 2023-07-26 05:17:49.000000 pythonbmp-1.0.5/samples/fonts/Hello_Earth.py
+-rw-rw-rw-   0        0        0     1790 2023-07-26 05:27:06.000000 pythonbmp-1.0.5/samples/fonts/Hello_Earth_Reverse_text.py
+-rw-rw-rw-   0        0        0     1812 2023-07-26 05:28:57.000000 pythonbmp-1.0.5/samples/fonts/Hello_Earth_Sideways_text.py
+-rw-rw-rw-   0        0        0     1859 2023-07-26 05:29:34.000000 pythonbmp-1.0.5/samples/fonts/Hello_Earth_Upsidedown_text.py
+-rw-rw-rw-   0        0        0     2108 2023-07-26 05:30:01.000000 pythonbmp-1.0.5/samples/fonts/Hello_Earth_Vertical_text.py
+-rw-rw-rw-   0        0        0     1755 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fonts/Hello_Rainbow.py
+-rw-rw-rw-   0        0        0     1760 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_WorId_Italic_RainbowSideway.py
+-rw-rw-rw-   0        0        0     1505 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World.py
+-rw-rw-rw-   0        0        0     1558 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_Dots.py
+-rw-rw-rw-   0        0        0     1580 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_Italicupsidedown.py
+-rw-rw-rw-   0        0        0     1779 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_Rainbow_vertical.py
+-rw-rw-rw-   0        0        0     1775 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_italic_rainbowsideway.py
+-rw-rw-rw-   0        0        0     1577 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_italicsideway.py
+-rw-rw-rw-   0        0        0     1575 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_italicvertical.py
+-rw-rw-rw-   0        0        0     1777 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_italicvertical_rainbow.py
+-rw-rw-rw-   0        0        0     1788 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_rainbowItalicupsidedown.py
+-rw-rw-rw-   0        0        0     1792 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_rainbowreversedItalic.py
+-rw-rw-rw-   0        0        0     1779 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_rainbowsideway.py
+-rw-rw-rw-   0        0        0     1785 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_rainbowupsidedown.py
+-rw-rw-rw-   0        0        0     1569 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_reversed.py
+-rw-rw-rw-   0        0        0     1578 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_reversedItalic.py
+-rw-rw-rw-   0        0        0     1563 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_sideway.py
+-rw-rw-rw-   0        0        0     1572 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_upsidedown.py
+-rw-rw-rw-   0        0        0     1569 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_vertical.py
+-rw-rw-rw-   0        0        0     1414 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_Italic.py
+-rw-rw-rw-   0        0        0     1417 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_Italicdots.py
+-rw-rw-rw-   0        0        0     1572 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_Italicupsidedown.py
+-rw-rw-rw-   0        0        0     1768 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_Rainbow_Dots.py
+-rw-rw-rw-   0        0        0     1584 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_Rainbow_Italic.py
+-rw-rw-rw-   0        0        0     1773 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_Rainbow_Italic_Dots.py
+-rw-rw-rw-   0        0        0     1770 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_Rainbow_vertical.py
+-rw-rw-rw-   0        0        0     1568 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_italicsideway.py
+-rw-rw-rw-   0        0        0     1568 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_italicvertical.py
+-rw-rw-rw-   0        0        0     1774 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_italicvertical_rainbow.py
+-rw-rw-rw-   0        0        0     1771 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_rainbowItalicupsidedown.py
+-rw-rw-rw-   0        0        0     1766 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_rainbowreversedItalic.py
+-rw-rw-rw-   0        0        0     1770 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_rainbowsideway.py
+-rw-rw-rw-   0        0        0     1761 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_rainbowupsidedown.py
+-rw-rw-rw-   0        0        0     1514 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/Hello_World_reversedItalic.py
+-rw-rw-rw-   0        0        0     1633 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fonts/TetraPlex_logo.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:27:31.765473 pythonbmp-1.0.5/samples/fractals/
+-rw-rw-rw-   0        0        0     1307 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Astroidfractal.py
+-rw-rw-rw-   0        0        0     1466 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_BarnsleyTree.py
+-rw-rw-rw-   0        0        0     1431 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_CatPaws.py
+-rw-rw-rw-   0        0        0     1262 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_CliffordAttractor.py
+-rw-rw-rw-   0        0        0     1474 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_CosJulia_Set.py
+-rw-rw-rw-   0        0        0     1259 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_DuffingAttractor.py
+-rw-rw-rw-   0        0        0     1238 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Fern.py
+-rw-rw-rw-   0        0        0     1287 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_FractalDreamAttractor.py
+-rw-rw-rw-   0        0        0     1267 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Gumowski-Mira_attractor.py
+-rw-rw-rw-   0        0        0     1266 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Gumowski-Mira_attractor_1.py
+-rw-rw-rw-   0        0        0     1161 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_HilbertCurve.py
+-rw-rw-rw-   0        0        0     1260 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_HopalongAttractor.py
+-rw-rw-rw-   0        0        0     1261 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Ikedaattractor.py
+-rw-rw-rw-   0        0        0     1497 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Julia_Set.py
+-rw-rw-rw-   0        0        0     1585 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_KochCurve.py
+-rw-rw-rw-   0        0        0     1627 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_KochSnowflake.py
+-rw-rw-rw-   0        0        0     1379 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Lambdafractal.py
+-rw-rw-rw-   0        0        0     1308 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Lemniscatefractal.py
+-rw-rw-rw-   0        0        0     1732 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_LissajousCurve.py
+-rw-rw-rw-   0        0        0     1354 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Mandelbrot_Set.py
+-rw-rw-rw-   0        0        0     1388 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Mandelbrot_Set_dichromatic.py
+-rw-rw-rw-   0        0        0     1431 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_MarekDragon.py
+-rw-rw-rw-   0        0        0     1437 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_MarekDragon_4bit.py
+-rw-rw-rw-   0        0        0     1504 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Multi2ndtetrationBiomorphfractal.py
+-rw-rw-rw-   0        0        0     1523 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_MultiBiomorphfractal.py
+-rw-rw-rw-   0        0        0     1554 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_MultiBiomorphphasevariantfractal.py
+-rw-rw-rw-   0        0        0     1498 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_MultiBiomorphvariantfractal.py
+-rw-rw-rw-   0        0        0     1501 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_MultiBiomorphvariantfractal1.py
+-rw-rw-rw-   0        0        0     1531 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_MultiCosBiomorphfractal.py
+-rw-rw-rw-   0        0        0     1504 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_MultiCoshBiomorphfractal.py
+-rw-rw-rw-   0        0        0     1494 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_MultiSinBiomorphfractal.py
+-rw-rw-rw-   0        0        0     1508 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_MultiSinhBiomorphfractal.py
+-rw-rw-rw-   0        0        0     1502 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_MultiTanBiomorphfractal.py
+-rw-rw-rw-   0        0        0     1531 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_MultiTanBiomorphfractal_dichromatic.py
+-rw-rw-rw-   0        0        0     1504 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_MultiTanhBiomorphfractal.py
+-rw-rw-rw-   0        0        0     1433 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Multibrot_Set.py
+-rw-rw-rw-   0        0        0     1426 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Multicircle.py
+-rw-rw-rw-   0        0        0     1461 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Multicircle_dichromatic.py
+-rw-rw-rw-   0        0        0     1413 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Multicorn_Set.py
+-rw-rw-rw-   0        0        0     1494 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_MultiexpBiomorphfractal.py
+-rw-rw-rw-   0        0        0     1414 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Multihyperbola.py
+-rw-rw-rw-   0        0        0     1497 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Multijulia_Set.py
+-rw-rw-rw-   0        0        0     1315 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Multisuperellipse.py
+-rw-rw-rw-   0        0        0     1501 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_MultizconjugateBiomorphfractal.py
+-rw-rw-rw-   0        0        0     1528 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Newtons_fractal.py
+-rw-rw-rw-   0        0        0     1551 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Newtons_fractal4.py
+-rw-rw-rw-   0        0        0     1552 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Newtons_fractal4_1.py
+-rw-rw-rw-   0        0        0     1575 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Newtons_fractal5.py
+-rw-rw-rw-   0        0        0     1577 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Newtons_fractal5_1.py
+-rw-rw-rw-   0        0        0     1578 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Newtons_fractal5_3.py
+-rw-rw-rw-   0        0        0     1627 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Newtons_fractal6.py
+-rw-rw-rw-   0        0        0     1629 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_Newtons_fractal6_3.py
+-rw-rw-rw-   0        0        0     1272 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_PeterdeJongAttractor.py
+-rw-rw-rw-   0        0        0     1474 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fractals/Hello_SinJulia_Set.py
+-rw-rw-rw-   0        0        0     1472 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fractals/Hello_SinJulia_Set_1bit.py
+-rw-rw-rw-   0        0        0     1487 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fractals/Hello_SinJulia_Set_4bit.py
+-rw-rw-rw-   0        0        0     1489 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fractals/Hello_SpiralJulia_Set.py
+-rw-rw-rw-   0        0        0     1314 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fractals/Hello_Symmetric_Icon_Attractor.py
+-rw-rw-rw-   0        0        0     1294 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fractals/Hello_Tetration_Fractal.py
+-rw-rw-rw-   0        0        0     1783 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fractals/Hello_ThickGradHilbertCurve.py
+-rw-rw-rw-   0        0        0     1279 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fractals/Hello_ThickHilbertCurve.py
+-rw-rw-rw-   0        0        0     1401 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fractals/Hello_Tricorn_Set.py
+-rw-rw-rw-   0        0        0     1416 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fractals/Hello_Xordivfractal.py
+-rw-rw-rw-   0        0        0     1329 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/fractals/Hello_Xorfractal.py
+-rw-rw-rw-   0        0        0     1262 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_nattractor.py
+-rw-rw-rw-   0        0        0     1472 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/fractals/Hello_ngonfractal.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:27:31.772471 pythonbmp-1.0.5/samples/graphs/
+-rw-rw-rw-   0        0        0     2230 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/graphs/Hello_XYScatterplot.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:27:32.669471 pythonbmp-1.0.5/samples/imageproc/
+-rw-rw-rw-   0        0        0     1269 2023-07-26 04:38:38.000000 pythonbmp-1.0.5/samples/imageproc/Hello_1bitBMP_Downscale.py
+-rw-rw-rw-   0        0        0     1268 2023-07-26 04:47:11.000000 pythonbmp-1.0.5/samples/imageproc/Hello_4bitBMP_Downscale.py
+-rw-rw-rw-   0        0        0     1266 2023-07-26 04:49:42.000000 pythonbmp-1.0.5/samples/imageproc/Hello_8bitBMP_Downscale.py
+-rw-rw-rw-   0        0        0     1258 2023-07-26 04:54:04.000000 pythonbmp-1.0.5/samples/imageproc/Hello_BrightnessAdj.py
+-rw-rw-rw-   0        0        0     1348 2023-07-26 04:54:25.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Circular_Color_Filter.py
+-rw-rw-rw-   0        0        0     1270 2023-07-26 04:54:56.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Circular_Mono_Filter.py
+-rw-rw-rw-   0        0        0     1343 2023-07-26 04:57:16.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Circular_Pixellate.py
+-rw-rw-rw-   0        0        0     1610 2023-07-26 04:57:44.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Circular_Region_BrightnessAdj.py
+-rw-rw-rw-   0        0        0     1471 2023-07-26 04:58:09.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Circular_Region_GammaAdj.py
+-rw-rw-rw-   0        0        0     1177 2023-07-26 05:02:26.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Color_Filter.py
+-rw-rw-rw-   0        0        0     1391 2023-07-26 05:11:57.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Copy_Paste_Earth.py
+-rw-rw-rw-   0        0        0     1202 2023-07-26 05:17:18.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Crop_Earth.py
+-rw-rw-rw-   0        0        0     1243 2023-07-26 06:56:31.000000 pythonbmp-1.0.5/samples/imageproc/Hello_FlipXY.py
+-rw-rw-rw-   0        0        0     1226 2023-07-26 06:37:28.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Flip_Horizontal.py
+-rw-rw-rw-   0        0        0     1251 2023-07-26 06:54:45.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Flip_Vertical.py
+-rw-rw-rw-   0        0        0     1180 2023-07-26 06:57:53.000000 pythonbmp-1.0.5/samples/imageproc/Hello_GammaAdj.py
+-rw-rw-rw-   0        0        0     1172 2023-07-26 07:01:31.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Invert_Colors.py
+-rw-rw-rw-   0        0        0     1176 2023-07-26 07:02:43.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Mirror_Bottom.py
+-rw-rw-rw-   0        0        0     1183 2023-07-26 07:03:16.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Mirror_BottomLeft.py
+-rw-rw-rw-   0        0        0     1153 2023-07-26 07:04:05.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Mirror_BottomRight.py
+-rw-rw-rw-   0        0        0     1168 2023-07-26 07:04:37.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Mirror_Top.py
+-rw-rw-rw-   0        0        0     1176 2023-07-26 07:06:03.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Mirror_TopLeft.py
+-rw-rw-rw-   0        0        0     1188 2023-07-26 07:06:32.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Mirror_TopRight.py
+-rw-rw-rw-   0        0        0     1178 2023-07-26 07:07:23.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Monochrome.py
+-rw-rw-rw-   0        0        0     1161 2023-07-26 07:07:56.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Outline.py
+-rw-rw-rw-   0        0        0     1132 2023-07-26 07:00:11.000000 pythonbmp-1.0.5/samples/imageproc/Hello_PaletteShift.py
+-rw-rw-rw-   0        0        0     1190 2023-07-26 07:08:38.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Pixellate_the_Earth.py
+-rw-rw-rw-   0        0        0     1449 2023-07-26 07:11:45.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Rectangular_BrightnessAdj.py
+-rw-rw-rw-   0        0        0     1424 2023-07-26 07:12:21.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Rectangular_Color_Filter.py
+-rw-rw-rw-   0        0        0     1403 2023-07-26 07:13:11.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Rectangular_GammaAdj.py
+-rw-rw-rw-   0        0        0     1345 2023-07-26 07:13:47.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Rectangular_Mono_Filter.py
+-rw-rw-rw-   0        0        0     1154 2023-07-26 07:14:30.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Resize_Larger_by_n.py
+-rw-rw-rw-   0        0        0     1166 2023-07-26 07:15:16.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Resize_Smaller_by_n.py
+-rw-rw-rw-   0        0        0     1371 2023-07-26 07:15:55.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Save_Selection.py
+-rw-rw-rw-   0        0        0     1214 2023-07-26 07:16:20.000000 pythonbmp-1.0.5/samples/imageproc/Hello_TV_Scanlines.py
+-rw-rw-rw-   0        0        0     1310 2023-07-26 07:16:48.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Vertical_Brightness_Gradient.py
+-rw-rw-rw-   0        0        0     1476 2023-07-26 07:17:16.000000 pythonbmp-1.0.5/samples/imageproc/Hello_Vertical_Brightness_Gradient_Circular_Region.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:27:33.238470 pythonbmp-1.0.5/samples/primitives2d/
+-rw-rw-rw-   0        0        0     1376 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/primitives2d/Hello_8bitPixels.py
+-rw-rw-rw-   0        0        0     1711 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/primitives2d/Hello_BezierCurve.py
+-rw-rw-rw-   0        0        0     1943 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/primitives2d/Hello_Bspline.py
+-rw-rw-rw-   0        0        0     1544 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/primitives2d/Hello_Circles.py
+-rw-rw-rw-   0        0        0     1415 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/primitives2d/Hello_Ellipse.py
+-rw-rw-rw-   0        0        0     1713 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/primitives2d/Hello_FilledCircle.py
+-rw-rw-rw-   0        0        0     1677 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/primitives2d/Hello_FilledEllipse.py
+-rw-rw-rw-   0        0        0     1679 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/primitives2d/Hello_FilledRectangle.py
+-rw-rw-rw-   0        0        0     1868 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/primitives2d/Hello_Gradient_Thick_Regular_Polygon.py
+-rw-rw-rw-   0        0        0     1485 2023-07-21 14:08:49.000000 pythonbmp-1.0.5/samples/primitives2d/Hello_Lines.py
+-rw-rw-rw-   0        0        0     1550 2023-07-21 14:08:45.000000 pythonbmp-1.0.5/samples/primitives2d/Hello_Rectangle.py
+-rw-rw-rw-   0        0        0     1672 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/primitives2d/Hello_Regular_Polygon.py
+-rw-rw-rw-   0        0        0     1699 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/primitives2d/Hello_Thick_Circle.py
+-rw-rw-rw-   0        0        0     1709 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/primitives2d/Hello_Thick_Gradient_Circle.py
+-rw-rw-rw-   0        0        0     1721 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/primitives2d/Hello_Thick_Gradient_Ellipse_Rotated.py
+-rw-rw-rw-   0        0        0     1479 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/primitives2d/Hello_Thick_Regular_Polygon.py
+-rw-rw-rw-   0        0        0     1665 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/primitives2d/Hello_Thick_Round_Gradient_Line.py
+-rw-rw-rw-   0        0        0     1772 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/primitives2d/Hello_Thick_Round_Line.py
+-rw-rw-rw-   0        0        0     1461 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/primitives2d/Hello_Vector.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:27:33.262472 pythonbmp-1.0.5/samples/spirographs/
+-rw-rw-rw-   0        0        0     1759 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/spirographs/Hello_Spirograph.py
+-rw-rw-rw-   0        0        0     1856 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/spirographs/Hello_Spirograph_1.py
+-rw-rw-rw-   0        0        0     1772 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/spirographs/Hello_Spirograph_2.py
+-rw-rw-rw-   0        0        0     1639 2023-07-21 14:08:42.000000 pythonbmp-1.0.5/samples/spirographs/Hello_Spirograph_Record.py
+-rw-rw-rw-   0        0        0       42 2023-07-26 08:27:33.336471 pythonbmp-1.0.5/setup.cfg
```

### Comparing `pythonbmp-1.0.4/LICENSE` & `pythonbmp-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/PKG-INFO` & `pythonbmp-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonbmp
-Version: 1.0.4
+Version: 1.0.5
 Summary: A pure Python 2D/3D graphics library that outputs to windows bitmap format
 Author-email: Joel Alcarez <joelalcarez1975@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 TechnoTanuki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -49,15 +49,15 @@
 
 Run Hello_somestring_here.py
 
 This will show minimum code to accomplish certain tasks
 
 * ![Hello_Darkness.py](https://github.com/TechnoTanuki/Python_BMP/blob/main/samples/Hello_Darkness.py) (my old friend) is a minimum template
 
-Run ![Features_Speedtest.py](https://github.com/TechnoTanuki/Python_BMP/blob/main/Features_Speedtest.py)
+Run ![Features_Speedtest.py](https://github.com/TechnoTanuki/Python_BMP/blob/main/samples/Features_Speedtest.py)
 
 * It should generate a bitmap and open MS Paint under windows to show output...
 * Close the MS Paint window to execute another script
 
 # Unit tests (images are links to test)
 
 [![Picmanip](https://github.com/TechnoTanuki/Python_BMP/blob/main/assets/test_images/raccoon-flipXYcircregion.bmp)](https://github.com/TechnoTanuki/Python_BMP/blob/main/test_picturemanipulation.py)
```

### Comparing `pythonbmp-1.0.4/README.md` & `pythonbmp-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 Run Hello_somestring_here.py
 
 This will show minimum code to accomplish certain tasks
 
 * ![Hello_Darkness.py](https://github.com/TechnoTanuki/Python_BMP/blob/main/samples/Hello_Darkness.py) (my old friend) is a minimum template
 
-Run ![Features_Speedtest.py](https://github.com/TechnoTanuki/Python_BMP/blob/main/Features_Speedtest.py)
+Run ![Features_Speedtest.py](https://github.com/TechnoTanuki/Python_BMP/blob/main/samples/Features_Speedtest.py)
 
 * It should generate a bitmap and open MS Paint under windows to show output...
 * Close the MS Paint window to execute another script
 
 # Unit tests (images are links to test)
 
 [![Picmanip](https://github.com/TechnoTanuki/Python_BMP/blob/main/assets/test_images/raccoon-flipXYcircregion.bmp)](https://github.com/TechnoTanuki/Python_BMP/blob/main/test_picturemanipulation.py)
```

### Comparing `pythonbmp-1.0.4/pyproject.toml` & `pythonbmp-1.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "pythonbmp"
 description = "A pure Python 2D/3D graphics library that outputs to windows bitmap format"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
     { name = "Joel Alcarez", email = "joelalcarez1975@gmail.com" }
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python"
 ]
```

### Comparing `pythonbmp-1.0.4/pythonbmp/BITMAPlib.py` & `pythonbmp-1.0.5/pythonbmp/BITMAPlib.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/X11colordict.py` & `pythonbmp-1.0.5/pythonbmp/X11colordict.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/XKCDcolordict.py` & `pythonbmp-1.0.5/pythonbmp/XKCDcolordict.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/bmpconstants.py` & `pythonbmp-1.0.5/pythonbmp/bmpconstants.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/bmppal.py` & `pythonbmp-1.0.5/pythonbmp/bmppal.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/bufferflip.py` & `pythonbmp-1.0.5/pythonbmp/bufferflip.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/buffersplit.py` & `pythonbmp-1.0.5/pythonbmp/buffersplit.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/bufresize.py` & `pythonbmp-1.0.5/pythonbmp/bufresize.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/chartools.py` & `pythonbmp-1.0.5/pythonbmp/chartools.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/charts.py` & `pythonbmp-1.0.5/pythonbmp/charts.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/colordict.py` & `pythonbmp-1.0.5/pythonbmp/colordict.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/colors.py` & `pythonbmp-1.0.5/pythonbmp/colors.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/conditionaltools.py` & `pythonbmp-1.0.5/pythonbmp/conditionaltools.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/dicttools.py` & `pythonbmp-1.0.5/pythonbmp/dicttools.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/fileutils.py` & `pythonbmp-1.0.5/pythonbmp/fileutils.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/fonts.py` & `pythonbmp-1.0.5/pythonbmp/fonts.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/fractals.py` & `pythonbmp-1.0.5/pythonbmp/fractals.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/inttools.py` & `pythonbmp-1.0.5/pythonbmp/inttools.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/mathlib.py` & `pythonbmp-1.0.5/pythonbmp/mathlib.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/messages.py` & `pythonbmp-1.0.5/pythonbmp/messages.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/paramchecks.py` & `pythonbmp-1.0.5/pythonbmp/paramchecks.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/primitives2D.py` & `pythonbmp-1.0.5/pythonbmp/primitives2D.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/proctimer.py` & `pythonbmp-1.0.5/pythonbmp/proctimer.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/shims.py` & `pythonbmp-1.0.5/pythonbmp/shims.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/solids3D.py` & `pythonbmp-1.0.5/pythonbmp/solids3D.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp/textgraphics.py` & `pythonbmp-1.0.5/pythonbmp/textgraphics.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/pythonbmp.egg-info/PKG-INFO` & `pythonbmp-1.0.5/pythonbmp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonbmp
-Version: 1.0.4
+Version: 1.0.5
 Summary: A pure Python 2D/3D graphics library that outputs to windows bitmap format
 Author-email: Joel Alcarez <joelalcarez1975@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 TechnoTanuki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -49,15 +49,15 @@
 
 Run Hello_somestring_here.py
 
 This will show minimum code to accomplish certain tasks
 
 * ![Hello_Darkness.py](https://github.com/TechnoTanuki/Python_BMP/blob/main/samples/Hello_Darkness.py) (my old friend) is a minimum template
 
-Run ![Features_Speedtest.py](https://github.com/TechnoTanuki/Python_BMP/blob/main/Features_Speedtest.py)
+Run ![Features_Speedtest.py](https://github.com/TechnoTanuki/Python_BMP/blob/main/samples/Features_Speedtest.py)
 
 * It should generate a bitmap and open MS Paint under windows to show output...
 * Close the MS Paint window to execute another script
 
 # Unit tests (images are links to test)
 
 [![Picmanip](https://github.com/TechnoTanuki/Python_BMP/blob/main/assets/test_images/raccoon-flipXYcircregion.bmp)](https://github.com/TechnoTanuki/Python_BMP/blob/main/test_picturemanipulation.py)
```

### Comparing `pythonbmp-1.0.4/pythonbmp.egg-info/SOURCES.txt` & `pythonbmp-1.0.5/pythonbmp.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -30,30 +30,37 @@
 pythonbmp/shims.py
 pythonbmp/solids3D.py
 pythonbmp/textgraphics.py
 pythonbmp.egg-info/PKG-INFO
 pythonbmp.egg-info/SOURCES.txt
 pythonbmp.egg-info/dependency_links.txt
 pythonbmp.egg-info/top_level.txt
+samples/Features_Speedtest.py
 samples/Hello_APP_Github_ID.py
 samples/Hello_Darkness.py
+samples/Hello_GithubID.bmp
 samples/3d/Hello_3D.py
 samples/3d/Hello_3D_surfaceplot.py
 samples/3d/Hello_Benzene.py
 samples/3d/Hello_Coin.py
 samples/3d/Hello_Cone.py
 samples/3d/Hello_Cube.py
 samples/3d/Hello_Decahedron.py
 samples/3d/Hello_DiscoBall.py
 samples/3d/Hello_Globe.py
 samples/3d/Hello_Icosahedron.py
 samples/3d/Hello_Icosahedron_Outline.py
 samples/3d/Hello_Octahedron.py
 samples/3d/Hello_Sphere.py
 samples/3d/Hello_Tetrahedron.py
+samples/assets/Earth.bmp
+samples/assets/biomorph.bmp
+samples/assets/earth-4bit.bmp
+samples/assets/somebody.bmp
+samples/assets/tanuki.bmp
 samples/colorgradients/Hello_Circular_Gradient.py
 samples/colorgradients/Hello_Dichromic_Circular_Gradient.py
 samples/colorgradients/Hello_Dichromic_Circular_Gradient_smoothstep.py
 samples/colorgradients/Hello_Elliptical_Gradient.py
 samples/colorgradients/Hello_FilleddichromatichoriGradRect.py
 samples/colorgradients/Hello_FilleddichromatichoriGradRectsmootherstep.py
 samples/colorgradients/Hello_FilleddichromatichoriGradRectsmootheststep.py
@@ -79,15 +86,14 @@
 samples/colorgradients/Hello_Sphere_dichromic.py
 samples/colorgradients/Hello_Sphere_dichromic_smootherstep.py
 samples/colorgradients/Hello_Sphere_dichromic_smootheststep.py
 samples/colorgradients/Hello_Sphere_dichromic_smoothstep.py
 samples/colorgradients/Hello_Sphere_smootherstep.py
 samples/colorgradients/Hello_Sphere_smootheststep.py
 samples/colorgradients/Hello_Sphere_smoothstep.py
-samples/colorgradients/HellodistcentercoordplotRGBxybit1.bmp
 samples/colornames/Hello_ColorNames.py
 samples/colornames/Hello_X11ColorNames.py
 samples/colornames/Hello_XKCDColorNames.py
 samples/curves/Hello_Cardioid.py
 samples/curves/Hello_CornuSpiral.py
 samples/curves/Hello_EggCurve.py
 samples/curves/Hello_Epicycloid.py
@@ -97,14 +103,21 @@
 samples/curves/Hello_Hypotrochoid.py
 samples/curves/Hello_InvoluteofaCircle.py
 samples/curves/Hello_Octopetala.py
 samples/curves/Hello_SquareSpiral.py
 samples/curves/Hello_Squircles.py
 samples/curves/Hello_Superellipse.py
 samples/curves/Hello_Thick_Exponential_Spiral_Gradient.py
+samples/curves/Hello_Thick_Spiral_Gradient.py
+samples/fonts/Hello_Earth.py
+samples/fonts/Hello_Earth_Reverse_text.py
+samples/fonts/Hello_Earth_Sideways_text.py
+samples/fonts/Hello_Earth_Upsidedown_text.py
+samples/fonts/Hello_Earth_Vertical_text.py
+samples/fonts/Hello_Rainbow.py
 samples/fonts/Hello_WorId_Italic_RainbowSideway.py
 samples/fonts/Hello_World.py
 samples/fonts/Hello_World_Dots.py
 samples/fonts/Hello_World_Dots_Italicupsidedown.py
 samples/fonts/Hello_World_Dots_Rainbow_vertical.py
 samples/fonts/Hello_World_Dots_italic_rainbowsideway.py
 samples/fonts/Hello_World_Dots_italicsideway.py
@@ -130,14 +143,15 @@
 samples/fonts/Hello_World_italicvertical.py
 samples/fonts/Hello_World_italicvertical_rainbow.py
 samples/fonts/Hello_World_rainbowItalicupsidedown.py
 samples/fonts/Hello_World_rainbowreversedItalic.py
 samples/fonts/Hello_World_rainbowsideway.py
 samples/fonts/Hello_World_rainbowupsidedown.py
 samples/fonts/Hello_World_reversedItalic.py
+samples/fonts/TetraPlex_logo.py
 samples/fractals/Hello_Astroidfractal.py
 samples/fractals/Hello_BarnsleyTree.py
 samples/fractals/Hello_CatPaws.py
 samples/fractals/Hello_CliffordAttractor.py
 samples/fractals/Hello_CosJulia_Set.py
 samples/fractals/Hello_DuffingAttractor.py
 samples/fractals/Hello_Fern.py
@@ -197,14 +211,52 @@
 samples/fractals/Hello_ThickHilbertCurve.py
 samples/fractals/Hello_Tricorn_Set.py
 samples/fractals/Hello_Xordivfractal.py
 samples/fractals/Hello_Xorfractal.py
 samples/fractals/Hello_nattractor.py
 samples/fractals/Hello_ngonfractal.py
 samples/graphs/Hello_XYScatterplot.py
+samples/imageproc/Hello_1bitBMP_Downscale.py
+samples/imageproc/Hello_4bitBMP_Downscale.py
+samples/imageproc/Hello_8bitBMP_Downscale.py
+samples/imageproc/Hello_BrightnessAdj.py
+samples/imageproc/Hello_Circular_Color_Filter.py
+samples/imageproc/Hello_Circular_Mono_Filter.py
+samples/imageproc/Hello_Circular_Pixellate.py
+samples/imageproc/Hello_Circular_Region_BrightnessAdj.py
+samples/imageproc/Hello_Circular_Region_GammaAdj.py
+samples/imageproc/Hello_Color_Filter.py
+samples/imageproc/Hello_Copy_Paste_Earth.py
+samples/imageproc/Hello_Crop_Earth.py
+samples/imageproc/Hello_FlipXY.py
+samples/imageproc/Hello_Flip_Horizontal.py
+samples/imageproc/Hello_Flip_Vertical.py
+samples/imageproc/Hello_GammaAdj.py
+samples/imageproc/Hello_Invert_Colors.py
+samples/imageproc/Hello_Mirror_Bottom.py
+samples/imageproc/Hello_Mirror_BottomLeft.py
+samples/imageproc/Hello_Mirror_BottomRight.py
+samples/imageproc/Hello_Mirror_Top.py
+samples/imageproc/Hello_Mirror_TopLeft.py
+samples/imageproc/Hello_Mirror_TopRight.py
+samples/imageproc/Hello_Monochrome.py
+samples/imageproc/Hello_Outline.py
+samples/imageproc/Hello_PaletteShift.py
+samples/imageproc/Hello_Pixellate_the_Earth.py
+samples/imageproc/Hello_Rectangular_BrightnessAdj.py
+samples/imageproc/Hello_Rectangular_Color_Filter.py
+samples/imageproc/Hello_Rectangular_GammaAdj.py
+samples/imageproc/Hello_Rectangular_Mono_Filter.py
+samples/imageproc/Hello_Resize_Larger_by_n.py
+samples/imageproc/Hello_Resize_Smaller_by_n.py
+samples/imageproc/Hello_Save_Selection.py
+samples/imageproc/Hello_TV_Scanlines.py
+samples/imageproc/Hello_Vertical_Brightness_Gradient.py
+samples/imageproc/Hello_Vertical_Brightness_Gradient_Circular_Region.py
+samples/primitives2d/Hello_8bitPixels.py
 samples/primitives2d/Hello_BezierCurve.py
 samples/primitives2d/Hello_Bspline.py
 samples/primitives2d/Hello_Circles.py
 samples/primitives2d/Hello_Ellipse.py
 samples/primitives2d/Hello_FilledCircle.py
 samples/primitives2d/Hello_FilledEllipse.py
 samples/primitives2d/Hello_FilledRectangle.py
```

### Comparing `pythonbmp-1.0.4/samples/3d/Hello_3D.py` & `pythonbmp-1.0.5/samples/3d/Hello_3D.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/3d/Hello_3D_surfaceplot.py` & `pythonbmp-1.0.5/samples/3d/Hello_3D_surfaceplot.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/3d/Hello_Benzene.py` & `pythonbmp-1.0.5/samples/3d/Hello_Benzene.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/3d/Hello_Coin.py` & `pythonbmp-1.0.5/samples/3d/Hello_Coin.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/3d/Hello_Cone.py` & `pythonbmp-1.0.5/samples/3d/Hello_Cone.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/3d/Hello_Cube.py` & `pythonbmp-1.0.5/samples/3d/Hello_Cube.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/3d/Hello_Decahedron.py` & `pythonbmp-1.0.5/samples/3d/Hello_Decahedron.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/3d/Hello_DiscoBall.py` & `pythonbmp-1.0.5/samples/3d/Hello_DiscoBall.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/3d/Hello_Globe.py` & `pythonbmp-1.0.5/samples/3d/Hello_Globe.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/3d/Hello_Icosahedron.py` & `pythonbmp-1.0.5/samples/3d/Hello_Icosahedron.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/3d/Hello_Icosahedron_Outline.py` & `pythonbmp-1.0.5/samples/3d/Hello_Icosahedron_Outline.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/3d/Hello_Octahedron.py` & `pythonbmp-1.0.5/samples/3d/Hello_Octahedron.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/3d/Hello_Sphere.py` & `pythonbmp-1.0.5/samples/3d/Hello_Sphere.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/3d/Hello_Tetrahedron.py` & `pythonbmp-1.0.5/samples/3d/Hello_Tetrahedron.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/Hello_APP_Github_ID.py` & `pythonbmp-1.0.5/samples/Hello_APP_Github_ID.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/Hello_Darkness.py` & `pythonbmp-1.0.5/samples/Hello_Darkness.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_Circular_Gradient.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_Circular_Gradient.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_Dichromic_Circular_Gradient.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_Dichromic_Circular_Gradient.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_Dichromic_Circular_Gradient_smoothstep.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_Dichromic_Circular_Gradient_smoothstep.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_Elliptical_Gradient.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_Elliptical_Gradient.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromatichoriGradRect.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_FilleddichromatichoriGradRect.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromatichoriGradRectsmootherstep.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_FilleddichromatichoriGradRectsmootherstep.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromatichoriGradRectsmootheststep.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_FilleddichromatichoriGradRectsmootheststep.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromatichoriGradRectsmoothstep.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_FilleddichromatichoriGradRectsmoothstep.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromaticvertGradRect.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_FilleddichromaticvertGradRect.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromaticvertGradRectsmootherstep.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_FilleddichromaticvertGradRectsmootherstep.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromaticvertGradRectsmootheststep.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_FilleddichromaticvertGradRectsmootheststep.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromaticvertGradRectsmoothstep.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_FilleddichromaticvertGradRectsmoothstep.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_FilledhoriGradRect.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_FilledhoriGradRect.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_FilledhoriGradRectsmootherstep.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_FilledhoriGradRectsmootherstep.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_FilledhoriGradRectsmootheststep.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_FilledhoriGradRectsmootheststep.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_FilledhoriGradRectsmoothstep.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_FilledhoriGradRectsmoothstep.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_FilledvertGradRect.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_FilledvertGradRect.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_FilledvertGradRectsmootherstep.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_FilledvertGradRectsmootherstep.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_FilledvertGradRectsmootheststep.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_FilledvertGradRectsmootheststep.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_FilledvertGradRectsmoothstep.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_FilledvertGradRectsmoothstep.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_Linear_Gradient.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_Linear_Gradient.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_NonLinearRadialMultichannel_Gradients.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_NonLinearRadialMultichannel_Gradients.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_NonLinearRadial_Gradients.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_NonLinearRadial_Gradients.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_Orb.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_Orb.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_RadialMultichannel_Gradients.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_RadialMultichannel_Gradients.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_Radial_Gradients.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_Radial_Gradients.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_Sphere_dichromic.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_Sphere_dichromic.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_Sphere_dichromic_smootherstep.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_Sphere_dichromic_smootherstep.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_Sphere_dichromic_smootheststep.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_Sphere_dichromic_smootheststep.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_Sphere_dichromic_smoothstep.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_Sphere_dichromic_smoothstep.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_Sphere_smootherstep.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_Sphere_smootherstep.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_Sphere_smootheststep.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_Sphere_smootheststep.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colorgradients/Hello_Sphere_smoothstep.py` & `pythonbmp-1.0.5/samples/colorgradients/Hello_Sphere_smoothstep.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colornames/Hello_ColorNames.py` & `pythonbmp-1.0.5/samples/colornames/Hello_ColorNames.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colornames/Hello_X11ColorNames.py` & `pythonbmp-1.0.5/samples/colornames/Hello_X11ColorNames.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/colornames/Hello_XKCDColorNames.py` & `pythonbmp-1.0.5/samples/colornames/Hello_XKCDColorNames.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/curves/Hello_Cardioid.py` & `pythonbmp-1.0.5/samples/curves/Hello_Cardioid.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/curves/Hello_CornuSpiral.py` & `pythonbmp-1.0.5/samples/curves/Hello_CornuSpiral.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/curves/Hello_EggCurve.py` & `pythonbmp-1.0.5/samples/curves/Hello_EggCurve.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/curves/Hello_Epicycloid.py` & `pythonbmp-1.0.5/samples/curves/Hello_Epicycloid.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/curves/Hello_Flower.py` & `pythonbmp-1.0.5/samples/curves/Hello_Flower.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/curves/Hello_GearCurve.py` & `pythonbmp-1.0.5/samples/curves/Hello_GearCurve.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/curves/Hello_HeartCurve.py` & `pythonbmp-1.0.5/samples/curves/Hello_HeartCurve.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/curves/Hello_Hypotrochoid.py` & `pythonbmp-1.0.5/samples/curves/Hello_Hypotrochoid.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/curves/Hello_InvoluteofaCircle.py` & `pythonbmp-1.0.5/samples/curves/Hello_InvoluteofaCircle.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/curves/Hello_Octopetala.py` & `pythonbmp-1.0.5/samples/curves/Hello_Octopetala.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/curves/Hello_SquareSpiral.py` & `pythonbmp-1.0.5/samples/curves/Hello_SquareSpiral.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/curves/Hello_Squircles.py` & `pythonbmp-1.0.5/samples/curves/Hello_Squircles.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/curves/Hello_Superellipse.py` & `pythonbmp-1.0.5/samples/curves/Hello_Superellipse.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/curves/Hello_Thick_Exponential_Spiral_Gradient.py` & `pythonbmp-1.0.5/samples/curves/Hello_Thick_Exponential_Spiral_Gradient.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_WorId_Italic_RainbowSideway.py` & `pythonbmp-1.0.5/samples/fonts/Hello_WorId_Italic_RainbowSideway.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_Dots.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_Dots.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_Italicupsidedown.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_Italicupsidedown.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_Rainbow_vertical.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_Rainbow_vertical.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_italic_rainbowsideway.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_italic_rainbowsideway.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_italicsideway.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_italicsideway.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_italicvertical.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_italicvertical.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_italicvertical_rainbow.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_italicvertical_rainbow.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_rainbowItalicupsidedown.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_rainbowItalicupsidedown.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_rainbowreversedItalic.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_rainbowreversedItalic.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_rainbowsideway.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_rainbowsideway.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_rainbowupsidedown.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_rainbowupsidedown.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_reversed.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_reversed.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_reversedItalic.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_reversedItalic.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_sideway.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_sideway.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_upsidedown.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_upsidedown.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_vertical.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_Dots_vertical.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_Italic.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_Italic.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_Italicdots.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_Italicdots.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_Italicupsidedown.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_Italicupsidedown.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_Rainbow_Dots.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_Rainbow_Dots.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_Rainbow_Italic.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_Rainbow_Italic.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_Rainbow_Italic_Dots.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_Rainbow_Italic_Dots.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_Rainbow_vertical.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_Rainbow_vertical.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_italicsideway.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_italicsideway.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_italicvertical.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_italicvertical.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_italicvertical_rainbow.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_italicvertical_rainbow.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_rainbowItalicupsidedown.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_rainbowItalicupsidedown.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_rainbowreversedItalic.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_rainbowreversedItalic.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_rainbowsideway.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_rainbowsideway.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_rainbowupsidedown.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_rainbowupsidedown.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fonts/Hello_World_reversedItalic.py` & `pythonbmp-1.0.5/samples/fonts/Hello_World_reversedItalic.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Astroidfractal.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Astroidfractal.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_BarnsleyTree.py` & `pythonbmp-1.0.5/samples/fractals/Hello_BarnsleyTree.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_CatPaws.py` & `pythonbmp-1.0.5/samples/fractals/Hello_CatPaws.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_CliffordAttractor.py` & `pythonbmp-1.0.5/samples/fractals/Hello_CliffordAttractor.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_CosJulia_Set.py` & `pythonbmp-1.0.5/samples/fractals/Hello_CosJulia_Set.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_DuffingAttractor.py` & `pythonbmp-1.0.5/samples/fractals/Hello_DuffingAttractor.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Fern.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Fern.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_FractalDreamAttractor.py` & `pythonbmp-1.0.5/samples/fractals/Hello_FractalDreamAttractor.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Gumowski-Mira_attractor.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Gumowski-Mira_attractor.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Gumowski-Mira_attractor_1.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Gumowski-Mira_attractor_1.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_HilbertCurve.py` & `pythonbmp-1.0.5/samples/fractals/Hello_HilbertCurve.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_HopalongAttractor.py` & `pythonbmp-1.0.5/samples/fractals/Hello_HopalongAttractor.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Ikedaattractor.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Ikedaattractor.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Julia_Set.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Julia_Set.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_KochCurve.py` & `pythonbmp-1.0.5/samples/fractals/Hello_KochCurve.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_KochSnowflake.py` & `pythonbmp-1.0.5/samples/fractals/Hello_KochSnowflake.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Lambdafractal.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Lambdafractal.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Lemniscatefractal.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Lemniscatefractal.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_LissajousCurve.py` & `pythonbmp-1.0.5/samples/fractals/Hello_LissajousCurve.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Mandelbrot_Set.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Mandelbrot_Set.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Mandelbrot_Set_dichromatic.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Mandelbrot_Set_dichromatic.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_MarekDragon.py` & `pythonbmp-1.0.5/samples/fractals/Hello_MarekDragon.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_MarekDragon_4bit.py` & `pythonbmp-1.0.5/samples/fractals/Hello_MarekDragon_4bit.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Multi2ndtetrationBiomorphfractal.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Multi2ndtetrationBiomorphfractal.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_MultiBiomorphfractal.py` & `pythonbmp-1.0.5/samples/fractals/Hello_MultiBiomorphfractal.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_MultiBiomorphphasevariantfractal.py` & `pythonbmp-1.0.5/samples/fractals/Hello_MultiBiomorphphasevariantfractal.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_MultiBiomorphvariantfractal.py` & `pythonbmp-1.0.5/samples/fractals/Hello_MultiBiomorphvariantfractal.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_MultiBiomorphvariantfractal1.py` & `pythonbmp-1.0.5/samples/fractals/Hello_MultiBiomorphvariantfractal1.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_MultiCosBiomorphfractal.py` & `pythonbmp-1.0.5/samples/fractals/Hello_MultiCosBiomorphfractal.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_MultiCoshBiomorphfractal.py` & `pythonbmp-1.0.5/samples/fractals/Hello_MultiCoshBiomorphfractal.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_MultiSinBiomorphfractal.py` & `pythonbmp-1.0.5/samples/fractals/Hello_MultiSinBiomorphfractal.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_MultiSinhBiomorphfractal.py` & `pythonbmp-1.0.5/samples/fractals/Hello_MultiSinhBiomorphfractal.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_MultiTanBiomorphfractal.py` & `pythonbmp-1.0.5/samples/fractals/Hello_MultiTanBiomorphfractal.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_MultiTanBiomorphfractal_dichromatic.py` & `pythonbmp-1.0.5/samples/fractals/Hello_MultiTanBiomorphfractal_dichromatic.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_MultiTanhBiomorphfractal.py` & `pythonbmp-1.0.5/samples/fractals/Hello_MultiTanhBiomorphfractal.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Multibrot_Set.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Multibrot_Set.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Multicircle.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Multicircle.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Multicircle_dichromatic.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Multicircle_dichromatic.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Multicorn_Set.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Multicorn_Set.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_MultiexpBiomorphfractal.py` & `pythonbmp-1.0.5/samples/fractals/Hello_MultiexpBiomorphfractal.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Multihyperbola.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Multihyperbola.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Multijulia_Set.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Multijulia_Set.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Multisuperellipse.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Multisuperellipse.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_MultizconjugateBiomorphfractal.py` & `pythonbmp-1.0.5/samples/fractals/Hello_MultizconjugateBiomorphfractal.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Newtons_fractal.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal4.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Newtons_fractal4.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal4_1.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Newtons_fractal4_1.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal5.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Newtons_fractal5.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal5_1.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Newtons_fractal5_1.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal5_3.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Newtons_fractal5_3.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal6.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Newtons_fractal6.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal6_3.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Newtons_fractal6_3.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_PeterdeJongAttractor.py` & `pythonbmp-1.0.5/samples/fractals/Hello_PeterdeJongAttractor.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_SinJulia_Set.py` & `pythonbmp-1.0.5/samples/fractals/Hello_SinJulia_Set.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_SinJulia_Set_1bit.py` & `pythonbmp-1.0.5/samples/fractals/Hello_SinJulia_Set_1bit.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_SinJulia_Set_4bit.py` & `pythonbmp-1.0.5/samples/fractals/Hello_SinJulia_Set_4bit.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_SpiralJulia_Set.py` & `pythonbmp-1.0.5/samples/fractals/Hello_SpiralJulia_Set.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Symmetric_Icon_Attractor.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Symmetric_Icon_Attractor.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Tetration_Fractal.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Tetration_Fractal.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_ThickGradHilbertCurve.py` & `pythonbmp-1.0.5/samples/fractals/Hello_ThickGradHilbertCurve.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_ThickHilbertCurve.py` & `pythonbmp-1.0.5/samples/fractals/Hello_ThickHilbertCurve.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Tricorn_Set.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Tricorn_Set.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Xordivfractal.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Xordivfractal.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_Xorfractal.py` & `pythonbmp-1.0.5/samples/fractals/Hello_Xorfractal.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_nattractor.py` & `pythonbmp-1.0.5/samples/fractals/Hello_nattractor.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/fractals/Hello_ngonfractal.py` & `pythonbmp-1.0.5/samples/fractals/Hello_ngonfractal.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/graphs/Hello_XYScatterplot.py` & `pythonbmp-1.0.5/samples/graphs/Hello_XYScatterplot.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/primitives2d/Hello_BezierCurve.py` & `pythonbmp-1.0.5/samples/primitives2d/Hello_BezierCurve.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/primitives2d/Hello_Bspline.py` & `pythonbmp-1.0.5/samples/primitives2d/Hello_Bspline.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/primitives2d/Hello_Circles.py` & `pythonbmp-1.0.5/samples/primitives2d/Hello_Circles.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/primitives2d/Hello_Ellipse.py` & `pythonbmp-1.0.5/samples/primitives2d/Hello_Ellipse.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/primitives2d/Hello_FilledCircle.py` & `pythonbmp-1.0.5/samples/primitives2d/Hello_FilledCircle.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/primitives2d/Hello_FilledEllipse.py` & `pythonbmp-1.0.5/samples/primitives2d/Hello_FilledEllipse.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/primitives2d/Hello_FilledRectangle.py` & `pythonbmp-1.0.5/samples/primitives2d/Hello_FilledRectangle.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/primitives2d/Hello_Gradient_Thick_Regular_Polygon.py` & `pythonbmp-1.0.5/samples/primitives2d/Hello_Gradient_Thick_Regular_Polygon.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/primitives2d/Hello_Lines.py` & `pythonbmp-1.0.5/samples/primitives2d/Hello_Lines.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/primitives2d/Hello_Rectangle.py` & `pythonbmp-1.0.5/samples/primitives2d/Hello_Rectangle.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/primitives2d/Hello_Regular_Polygon.py` & `pythonbmp-1.0.5/samples/primitives2d/Hello_Regular_Polygon.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/primitives2d/Hello_Thick_Circle.py` & `pythonbmp-1.0.5/samples/primitives2d/Hello_Thick_Circle.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/primitives2d/Hello_Thick_Gradient_Circle.py` & `pythonbmp-1.0.5/samples/primitives2d/Hello_Thick_Gradient_Circle.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/primitives2d/Hello_Thick_Gradient_Ellipse_Rotated.py` & `pythonbmp-1.0.5/samples/primitives2d/Hello_Thick_Gradient_Ellipse_Rotated.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/primitives2d/Hello_Thick_Regular_Polygon.py` & `pythonbmp-1.0.5/samples/primitives2d/Hello_Thick_Regular_Polygon.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/primitives2d/Hello_Thick_Round_Gradient_Line.py` & `pythonbmp-1.0.5/samples/primitives2d/Hello_Thick_Round_Gradient_Line.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/primitives2d/Hello_Thick_Round_Line.py` & `pythonbmp-1.0.5/samples/primitives2d/Hello_Thick_Round_Line.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/primitives2d/Hello_Vector.py` & `pythonbmp-1.0.5/samples/primitives2d/Hello_Vector.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/spirographs/Hello_Spirograph.py` & `pythonbmp-1.0.5/samples/spirographs/Hello_Spirograph.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/spirographs/Hello_Spirograph_1.py` & `pythonbmp-1.0.5/samples/spirographs/Hello_Spirograph_1.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/spirographs/Hello_Spirograph_2.py` & `pythonbmp-1.0.5/samples/spirographs/Hello_Spirograph_2.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.4/samples/spirographs/Hello_Spirograph_Record.py` & `pythonbmp-1.0.5/samples/spirographs/Hello_Spirograph_Record.py`

 * *Files identical despite different names*

