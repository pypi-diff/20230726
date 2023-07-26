# Comparing `tmp/mcptbr-0.1.2.tar.gz` & `tmp/mcptbr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcptbr-0.1.2.tar", last modified: Wed Jul 26 01:25:58 2023, max compression
+gzip compressed data, was "mcptbr-0.1.3.tar", last modified: Wed Jul 26 01:51:59 2023, max compression
```

## Comparing `mcptbr-0.1.2.tar` & `mcptbr-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 01:25:58.791399 mcptbr-0.1.2/
--rw-rw-rw-   0        0        0      176 2023-07-26 01:25:58.789403 mcptbr-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 01:25:58.724577 mcptbr-0.1.2/mcptbr/
--rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.1.2/mcptbr/__init__.py
--rw-rw-rw-   0        0        0      723 2023-07-26 01:24:25.000000 mcptbr-0.1.2/mcptbr/model.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:25:58.787407 mcptbr-0.1.2/mcptbr.egg-info/
--rw-rw-rw-   0        0        0      176 2023-07-26 01:25:58.000000 mcptbr-0.1.2/mcptbr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-07-26 01:25:58.000000 mcptbr-0.1.2/mcptbr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 01:25:58.000000 mcptbr-0.1.2/mcptbr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-26 01:25:58.000000 mcptbr-0.1.2/mcptbr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-26 01:25:58.000000 mcptbr-0.1.2/mcptbr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 01:25:58.791399 mcptbr-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      491 2023-07-26 01:25:18.000000 mcptbr-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 01:51:59.245902 mcptbr-0.1.3/
+-rw-rw-rw-   0        0        0      176 2023-07-26 01:51:59.243905 mcptbr-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 01:51:59.163121 mcptbr-0.1.3/mcptbr/
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.1.3/mcptbr/__init__.py
+-rw-rw-rw-   0        0        0      744 2023-07-26 01:48:09.000000 mcptbr-0.1.3/mcptbr/model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 01:51:59.239914 mcptbr-0.1.3/mcptbr.egg-info/
+-rw-rw-rw-   0        0        0      176 2023-07-26 01:51:58.000000 mcptbr-0.1.3/mcptbr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-07-26 01:51:58.000000 mcptbr-0.1.3/mcptbr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 01:51:58.000000 mcptbr-0.1.3/mcptbr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-26 01:51:58.000000 mcptbr-0.1.3/mcptbr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-26 01:51:58.000000 mcptbr-0.1.3/mcptbr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 01:51:59.245902 mcptbr-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      491 2023-07-26 01:48:54.000000 mcptbr-0.1.3/setup.py
```

### Comparing `mcptbr-0.1.2/mcptbr/model.py` & `mcptbr-0.1.3/mcptbr/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,29 +10,29 @@
     mc.setBlock(x,y,z,id_bloco,estado) 
 
 
 def colocarBlocos(x0,y0,z0,x1,y1,z1,id_bloco,estado):
     mc.setBlocks(x0,y0,z0,x1,y1,z1,id_bloco,estado)
 
 def pegarBloco(x,y,z):
-    mc.getBlock(x,y,z)
+    return mc.getBlock(x,y,z)
 
 
 def mandarMensagem(mensagem):
     mc.postToChat(mensagem)
 
 
 def pegarPosicaoJogador():
-    mc.player.getPos()
+    return mc.player.getPos()
 
 
 def novaPosicaoJogador(x,y,z):
     """
     novaPosicaoJogador(x,y,z)
 
     Coloca o jogador em uma nova posição no mundo do Minecraft.
     """
     mc.player.setPos(x,y,z)
 
 
 def pegarBlocosTocados():
-    mc.events.pollBlockHits()
+    return mc.events.pollBlockHits()
```

