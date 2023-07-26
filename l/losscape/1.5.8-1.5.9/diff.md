# Comparing `tmp/losscape-1.5.8.tar.gz` & `tmp/losscape-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "losscape-1.5.8.tar", last modified: Tue Jul 25 08:19:53 2023, max compression
+gzip compressed data, was "losscape-1.5.9.tar", last modified: Wed Jul 26 08:49:04 2023, max compression
```

## Comparing `losscape-1.5.8.tar` & `losscape-1.5.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-25 08:19:53.844528 losscape-1.5.8/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-25 08:19:53.844528 losscape-1.5.8/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3312 2023-07-21 13:44:05.000000 losscape-1.5.8/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-25 08:19:53.844528 losscape-1.5.8/losscape/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-18 12:39:49.000000 losscape-1.5.8/losscape/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1715 2023-07-22 18:00:07.000000 losscape-1.5.8/losscape/compute_loss.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1816 2023-07-18 09:41:21.000000 losscape-1.5.8/losscape/create_directions.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    16336 2023-07-25 08:19:17.000000 losscape-1.5.8/losscape/create_landscape.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2099 2023-07-21 07:07:54.000000 losscape-1.5.8/losscape/train.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-25 08:19:53.844528 losscape-1.5.8/losscape.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-25 08:19:53.000000 losscape-1.5.8/losscape.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      300 2023-07-25 08:19:53.000000 losscape-1.5.8/losscape.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-25 08:19:53.000000 losscape-1.5.8/losscape.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       41 2023-07-25 08:19:53.000000 losscape-1.5.8/losscape.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-25 08:19:53.000000 losscape-1.5.8/losscape.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-25 08:19:53.844528 losscape-1.5.8/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)      596 2023-07-25 08:19:45.000000 losscape-1.5.8/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-26 08:49:04.401615 losscape-1.5.9/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-26 08:49:04.401615 losscape-1.5.9/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3312 2023-07-21 13:44:05.000000 losscape-1.5.9/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-26 08:49:04.401615 losscape-1.5.9/losscape/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-18 12:39:49.000000 losscape-1.5.9/losscape/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1715 2023-07-22 18:00:07.000000 losscape-1.5.9/losscape/compute_loss.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1816 2023-07-18 09:41:21.000000 losscape-1.5.9/losscape/create_directions.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16336 2023-07-25 11:10:20.000000 losscape-1.5.9/losscape/create_landscape.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2331 2023-07-26 08:48:31.000000 losscape-1.5.9/losscape/train.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-26 08:49:04.401615 losscape-1.5.9/losscape.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-26 08:49:04.000000 losscape-1.5.9/losscape.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      300 2023-07-26 08:49:04.000000 losscape-1.5.9/losscape.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-26 08:49:04.000000 losscape-1.5.9/losscape.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       41 2023-07-26 08:49:04.000000 losscape-1.5.9/losscape.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-26 08:49:04.000000 losscape-1.5.9/losscape.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-26 08:49:04.401615 losscape-1.5.9/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)      596 2023-07-26 08:48:43.000000 losscape-1.5.9/setup.py
```

### Comparing `losscape-1.5.8/PKG-INFO` & `losscape-1.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: losscape
-Version: 1.5.8
+Version: 1.5.9
 Summary: Visualize easily the loss landscape of your neural networks
 Home-page: https://github.com/Procuste34/losscape
 Author: Alexandre TL
 Author-email: alexandretl3434@gmail.com
 Description-Content-Type: text/markdown
 
 # loss + landscape = `losscape` 🌄
```

### Comparing `losscape-1.5.8/README.md` & `losscape-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `losscape-1.5.8/losscape/compute_loss.py` & `losscape-1.5.9/losscape/compute_loss.py`

 * *Files identical despite different names*

### Comparing `losscape-1.5.8/losscape/create_directions.py` & `losscape-1.5.9/losscape/create_directions.py`

 * *Files identical despite different names*

### Comparing `losscape-1.5.8/losscape/create_landscape.py` & `losscape-1.5.9/losscape/create_landscape.py`

 * *Files identical despite different names*

### Comparing `losscape-1.5.8/losscape/train.py` & `losscape-1.5.9/losscape/train.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,18 +41,26 @@
 
             logits = model(Xb)
             loss = criterion(logits, Yb)
             optimizer.zero_grad()
             loss.backward()
             optimizer.step()
 
+        """
         if epoch%decay_lr_epochs == 0:
             lr = 0.1 * lr
             for param_group in optimizer.param_groups:
-                param_group['lr'] = lr
+                param_group['lr'] = lr OUPSSSS
+        """
+        
+        if int(epoch) == 150 or int(epoch) == 225 or int(epoch) == 275:
+            lr *= 0.1
+            for param_group in optimizer.param_groups:
+                param_group['lr'] *= 0.1
+
 
         if verbose == 2:
             print("Epoch {}/{}. Loss={}".format(epoch, epochs, loss.item()))
 
         if verbose == 1 and (epoch%(epochs/4) == 0):
             print("Epoch {}/{}. Loss={}".format(epoch, epochs, loss.item()))
```

### Comparing `losscape-1.5.8/losscape.egg-info/PKG-INFO` & `losscape-1.5.9/losscape.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: losscape
-Version: 1.5.8
+Version: 1.5.9
 Summary: Visualize easily the loss landscape of your neural networks
 Home-page: https://github.com/Procuste34/losscape
 Author: Alexandre TL
 Author-email: alexandretl3434@gmail.com
 Description-Content-Type: text/markdown
 
 # loss + landscape = `losscape` 🌄
```

### Comparing `losscape-1.5.8/setup.py` & `losscape-1.5.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 current_dir = Path(__file__).parent
 desc = (current_dir / "README.md").read_text()
 
 setup(
     name='losscape',
-    version='1.5.8',
+    version='1.5.9',
     url='https://github.com/Procuste34/losscape',
     author='Alexandre TL',
     author_email='alexandretl3434@gmail.com',
     description='Visualize easily the loss landscape of your neural networks',
     long_description=desc,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

