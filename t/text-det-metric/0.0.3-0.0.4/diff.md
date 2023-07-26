# Comparing `tmp/text_det_metric-0.0.3-py3-none-any.whl.zip` & `tmp/text_det_metric-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9052 bytes, number of entries: 8
--rw-r--r--  2.0 unx      151 b- defN 23-Jul-23 02:09 text_det_metric/__init__.py
--rw-r--r--  2.0 unx     7298 b- defN 23-Jul-23 02:09 text_det_metric/main.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-23 02:09 text_det_metric-0.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     2954 b- defN 23-Jul-23 02:09 text_det_metric-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-23 02:09 text_det_metric-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       63 b- defN 23-Jul-23 02:09 text_det_metric-0.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 23-Jul-23 02:09 text_det_metric-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      693 b- defN 23-Jul-23 02:09 text_det_metric-0.0.3.dist-info/RECORD
-8 files, 22624 bytes uncompressed, 7828 bytes compressed:  65.4%
+Zip file size: 9050 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      151 b- defN 23-Jul-26 00:53 text_det_metric/__init__.py
+-rw-r--r--  2.0 unx     7298 b- defN 23-Jul-26 00:53 text_det_metric/main.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-26 00:53 text_det_metric-0.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2957 b- defN 23-Jul-26 00:53 text_det_metric-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-26 00:53 text_det_metric-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       63 b- defN 23-Jul-26 00:53 text_det_metric-0.0.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-26 00:53 text_det_metric-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      693 b- defN 23-Jul-26 00:53 text_det_metric-0.0.4.dist-info/RECORD
+8 files, 22627 bytes uncompressed, 7826 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: text_det_metric/__init__.py
 Comment: 
 
 Filename: text_det_metric/main.py
 Comment: 
 
-Filename: text_det_metric-0.0.3.dist-info/LICENSE
+Filename: text_det_metric-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: text_det_metric-0.0.3.dist-info/METADATA
+Filename: text_det_metric-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: text_det_metric-0.0.3.dist-info/WHEEL
+Filename: text_det_metric-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: text_det_metric-0.0.3.dist-info/entry_points.txt
+Filename: text_det_metric-0.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: text_det_metric-0.0.3.dist-info/top_level.txt
+Filename: text_det_metric-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: text_det_metric-0.0.3.dist-info/RECORD
+Filename: text_det_metric-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `text_det_metric-0.0.3.dist-info/LICENSE` & `text_det_metric-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `text_det_metric-0.0.3.dist-info/METADATA` & `text_det_metric-0.0.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text-det-metric
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tool of computing the metric of text detection
 Home-page: https://github.com/SWHL/TextDetMetric
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: ocr, text-det, hmean
 Platform: Any
@@ -72,15 +72,15 @@
 2. Run `compute_metric.py` to get the metrics on the dataset
     ```python
     from text_det_metric import DetectionIoUEvaluator
 
     metric = DetectionIoUEvaluator()
 
     # pred_path
-    pred_path = "1.txt"
+    pred_path = "pred.txt"
     mertric = metric(pred_path)
     print(mertric)
     ```
 
 ### See details for [TextDetMetric](https://github.com/SWHL/TextDetMetric).
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: text-det-metric Version: 0.0.3 Summary: Tool of
+Metadata-Version: 2.1 Name: text-det-metric Version: 0.0.4 Summary: Tool of
 computing the metric of text detection Home-page: https://github.com/SWHL/
 TextDetMetric Author: SWHL Author-email: liekkaskono@163.com License: Apache-
 2.0 Keywords: ocr, text-det, hmean Platform: Any Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.6,<3.12
@@ -25,9 +25,9 @@
 split="test", ) text_detector = TextDetector() content = [] for one_data in
 test_data: img_path = one_data.get("image:FILE") print(img_path) img =
 cv2.imread(str(img_path)) dt_boxes, scores, _ = text_detector(img)
 content.append(f"{img_path}\t{dt_boxes.tolist()}\t{scores}") with open
 ("pred.txt", "w", encoding="utf-8") as f: for v in content: f.write(f"{v}\n")
 ``` 2. Run `compute_metric.py` to get the metrics on the dataset ```python from
 text_det_metric import DetectionIoUEvaluator metric = DetectionIoUEvaluator() #
-pred_path pred_path = "1.txt" mertric = metric(pred_path) print(mertric) ```
+pred_path pred_path = "pred.txt" mertric = metric(pred_path) print(mertric) ```
 ### See details for [TextDetMetric](https://github.com/SWHL/TextDetMetric).
```

## Comparing `text_det_metric-0.0.3.dist-info/RECORD` & `text_det_metric-0.0.4.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 text_det_metric/__init__.py,sha256=K1TeK28y90XdOksdLCixf5d--5KXgzpsD1s6108yA1g,151
 text_det_metric/main.py,sha256=2JUlNkEZzxGfAPp77K5bz5Re92g9TOWGwi2SVAbP0ok,7298
-text_det_metric-0.0.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-text_det_metric-0.0.3.dist-info/METADATA,sha256=V9_4FT3zMrkQgZR8GWgWuUcSvZJSc-rhaPx6OKVkDSA,2954
-text_det_metric-0.0.3.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-text_det_metric-0.0.3.dist-info/entry_points.txt,sha256=gTbVodddXRR93pLeNRW5XXLwlzkYEB295t8Iy1e-N7Y,63
-text_det_metric-0.0.3.dist-info/top_level.txt,sha256=7olohGvTTeSsVHraNv5VoQm1nFkIT3GS3qWCl_Eamoc,16
-text_det_metric-0.0.3.dist-info/RECORD,,
+text_det_metric-0.0.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+text_det_metric-0.0.4.dist-info/METADATA,sha256=3WII6nTlFPb5ne1yPx5HH_HiZA4_zZ-G9Cug2zQ48cw,2957
+text_det_metric-0.0.4.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+text_det_metric-0.0.4.dist-info/entry_points.txt,sha256=gTbVodddXRR93pLeNRW5XXLwlzkYEB295t8Iy1e-N7Y,63
+text_det_metric-0.0.4.dist-info/top_level.txt,sha256=7olohGvTTeSsVHraNv5VoQm1nFkIT3GS3qWCl_Eamoc,16
+text_det_metric-0.0.4.dist-info/RECORD,,
```

