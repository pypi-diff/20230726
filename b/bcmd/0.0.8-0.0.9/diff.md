# Comparing `tmp/bcmd-0.0.8.tar.gz` & `tmp/bcmd-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcmd-0.0.8.tar", last modified: Mon Jul 24 06:41:18 2023, max compression
+gzip compressed data, was "bcmd-0.0.9.tar", last modified: Wed Jul 26 03:53:08 2023, max compression
```

## Comparing `bcmd-0.0.8.tar` & `bcmd-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 06:41:18.798607 bcmd-0.0.8/
--rw-rw-rw-   0        0        0      233 2023-07-24 06:41:18.798607 bcmd-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-24 06:41:18.784828 bcmd-0.0.8/bcmd/
--rw-rw-rw-   0        0        0        0 2023-07-21 02:19:54.000000 bcmd-0.0.8/bcmd/__init__.py
--rw-rw-rw-   0        0        0      473 2023-07-24 03:57:58.000000 bcmd-0.0.8/bcmd/dev.py
--rw-rw-rw-   0        0        0      259 2023-07-24 01:26:53.000000 bcmd-0.0.8/bcmd/main.py
-drwxrwxrwx   0        0        0        0 2023-07-24 06:41:18.797608 bcmd-0.0.8/bcmd/tasks/
--rw-rw-rw-   0        0        0        0 2023-07-20 07:37:38.000000 bcmd-0.0.8/bcmd/tasks/__init__.py
--rw-rw-rw-   0        0        0     1394 2023-07-24 03:16:35.000000 bcmd-0.0.8/bcmd/tasks/bin.py
--rw-rw-rw-   0        0        0      451 2023-07-24 02:24:56.000000 bcmd-0.0.8/bcmd/tasks/json.py
--rw-rw-rw-   0        0        0     1328 2023-07-24 01:44:47.000000 bcmd-0.0.8/bcmd/tasks/mirrors.py
--rw-rw-rw-   0        0        0      598 2023-07-24 01:55:47.000000 bcmd-0.0.8/bcmd/tasks/proxy.py
--rw-rw-rw-   0        0        0     2368 2023-07-22 09:34:39.000000 bcmd-0.0.8/bcmd/tasks/time.py
--rw-rw-rw-   0        0        0     2292 2023-07-22 10:03:50.000000 bcmd-0.0.8/bcmd/tasks/venv.py
-drwxrwxrwx   0        0        0        0 2023-07-24 06:41:18.791606 bcmd-0.0.8/bcmd.egg-info/
--rw-rw-rw-   0        0        0      233 2023-07-24 06:41:18.000000 bcmd-0.0.8/bcmd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-07-24 06:41:18.000000 bcmd-0.0.8/bcmd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 06:41:18.000000 bcmd-0.0.8/bcmd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-24 06:41:18.000000 bcmd-0.0.8/bcmd.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      149 2023-07-24 06:41:18.000000 bcmd-0.0.8/bcmd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-24 06:41:18.000000 bcmd-0.0.8/bcmd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      617 2023-07-24 06:39:06.000000 bcmd-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-24 06:41:18.799608 bcmd-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 03:53:08.963889 bcmd-0.0.9/
+-rw-rw-rw-   0        0        0      233 2023-07-26 03:53:08.963889 bcmd-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 03:53:08.949885 bcmd-0.0.9/bcmd/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:19:54.000000 bcmd-0.0.9/bcmd/__init__.py
+-rw-rw-rw-   0        0        0      163 2023-07-26 03:14:56.000000 bcmd-0.0.9/bcmd/dev.py
+-rw-rw-rw-   0        0        0      259 2023-07-26 02:55:56.000000 bcmd-0.0.9/bcmd/main.py
+drwxrwxrwx   0        0        0        0 2023-07-26 03:53:08.962889 bcmd-0.0.9/bcmd/tasks/
+-rw-rw-rw-   0        0        0        0 2023-07-20 07:37:38.000000 bcmd-0.0.9/bcmd/tasks/__init__.py
+-rw-rw-rw-   0        0        0     1674 2023-07-26 03:52:09.000000 bcmd-0.0.9/bcmd/tasks/bin.py
+-rw-rw-rw-   0        0        0      447 2023-07-24 06:53:08.000000 bcmd-0.0.9/bcmd/tasks/json.py
+-rw-rw-rw-   0        0        0     1342 2023-07-25 09:30:03.000000 bcmd-0.0.9/bcmd/tasks/mirrors.py
+-rw-rw-rw-   0        0        0      598 2023-07-24 01:55:47.000000 bcmd-0.0.9/bcmd/tasks/proxy.py
+-rw-rw-rw-   0        0        0     3763 2023-07-26 03:31:36.000000 bcmd-0.0.9/bcmd/tasks/task.py
+-rw-rw-rw-   0        0        0     2365 2023-07-25 09:30:10.000000 bcmd-0.0.9/bcmd/tasks/time.py
+-rw-rw-rw-   0        0        0     3022 2023-07-26 03:31:02.000000 bcmd-0.0.9/bcmd/tasks/venv.py
+drwxrwxrwx   0        0        0        0 2023-07-26 03:53:08.954886 bcmd-0.0.9/bcmd.egg-info/
+-rw-rw-rw-   0        0        0      233 2023-07-26 03:53:08.000000 bcmd-0.0.9/bcmd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-07-26 03:53:08.000000 bcmd-0.0.9/bcmd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 03:53:08.000000 bcmd-0.0.9/bcmd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-26 03:53:08.000000 bcmd-0.0.9/bcmd.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      149 2023-07-26 03:53:08.000000 bcmd-0.0.9/bcmd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-26 03:53:08.000000 bcmd-0.0.9/bcmd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      617 2023-07-26 03:52:51.000000 bcmd-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 03:53:08.963889 bcmd-0.0.9/setup.cfg
```

### Comparing `bcmd-0.0.8/bcmd/tasks/bin.py` & `bcmd-0.0.9/bcmd/tasks/bin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 import os
 from pathlib import Path
-from typing import Optional
+from typing import Final, Optional
 
 import typer
-from beni import bcolor, bfile, bfunc, btask
+from beni import bcolor, bfile, bfunc, bstore
 from beni.bqiniu import QiniuBucket
 
+app: Final = typer.Typer(help='bin 工具')
 
-@btask.app.command()
+
+@app.command()
 @bfunc.syncCall
-async def bin(
-    names: str = typer.Argument(None, help="如果有多个使用,分割"),
-    file: Path = typer.Option(None, help="文件形式指定参数，行为单位"),
+async def init(
     ak: str = typer.Option(..., help="七牛云账号AK"),
     sk: str = typer.Option(..., help="七牛云账号SK"),
+):
+    await bstore.set(__file__, (ak, sk))
+
+
+@app.command()
+@bfunc.syncCall
+async def download(
+    names: str = typer.Argument(None, help="如果有多个使用,分割"),
+    file: Path = typer.Option(None, help="文件形式指定参数，行为单位"),
     output: Optional[Path] = typer.Option(None, help="本地保存路径"),
 ):
     '从七牛云下载执行文件'
+    try:
+        (ak, sk) = await bstore.get(__file__)
+    except:
+        return bcolor.printRed('请先执行 init 进行初始化')
     bucketName = 'pytask'
     bucketUrl = 'http://qiniu-cdn.pytask.com'
     if output is None:
         output = Path(os.curdir)
     bucket = QiniuBucket(bucketName, bucketUrl, ak, sk)
     targetList: list[str] = []
     if names:
```

### Comparing `bcmd-0.0.8/bcmd/tasks/mirrors.py` & `bcmd-0.0.9/bcmd/tasks/mirrors.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from beni import bcolor, bfile, bfunc, bpath, btask
 
 
 @btask.app.command()
 @bfunc.syncCall
 async def mirrors(
     types: list[_MirrorsType] = typer.Argument(None, help="镜像的类型"),
-    disabled: bool = typer.Option(False, help="是否禁用"),
+    disabled: bool = typer.Option(False, '--disabled', '-d', help="是否禁用"),
 ):
     '设置镜像'
     if not types:
         types = [_MirrorsType.pip, _MirrorsType.npm]
     for targetType in types:
         data = _mirrorsFiles[targetType]
         for file, msgAry in data.items():
@@ -32,19 +32,19 @@
 class _MirrorsType(StrEnum):
     pip = 'pip'
     npm = 'npm'
 
 
 _mirrorsFiles = {
     _MirrorsType.pip: {
-        bpath.getUser('pip/pip.ini'): [
+        bpath.user('pip/pip.ini'): [
             '[global]',
             'index-url = https://mirrors.aliyun.com/pypi/simple',
         ],
     },
     _MirrorsType.npm: {
-        bpath.getUser('.bashrc'): [
+        bpath.user('.bashrc'): [
             'registry=https://registry.npm.taobao.org/',
             'electron_mirror=https://npm.taobao.org/mirrors/electron/',
         ],
     },
 }
```

### Comparing `bcmd-0.0.8/bcmd/tasks/proxy.py` & `bcmd-0.0.9/bcmd/tasks/proxy.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.8/bcmd/tasks/time.py` & `bcmd-0.0.9/bcmd/tasks/time.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         typer.secho('\n'.join(msg_ary), fg=color)
         raise typer.Abort()
     print()
     print(timestamp)
     print()
     localtime = time.localtime(timestamp)
     tzname = time.tzname[(time.daylight and localtime.tm_isdst) and 1 or 0]
-    bcolor.printx(time.strftime('%Y-%m-%d %H:%M:%S %z', localtime), tzname, colorList=[Fore.YELLOW])
+    bcolor.printx(time.strftime('%Y-%m-%d %H:%M:%S %z', localtime), tzname, colors=[Fore.YELLOW])
     print()
     datetime_utc = Datetime.fromtimestamp(timestamp, tz=timezone.utc)
     tzname_list = [
         'Australia/Sydney',
         'Asia/Tokyo',
         'Asia/Kolkata',
         'Africa/Cairo',
```

### Comparing `bcmd-0.0.8/bcmd/tasks/venv.py` & `bcmd-0.0.9/bcmd/tasks/venv.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,39 +5,50 @@
 from beni import bexecute, bfile, bfunc, binput, bpath, btask
 
 
 @btask.app.command()
 @bfunc.syncCall
 async def venv(
     packages: list[str] = typer.Argument(None),
-    path: Path = typer.Option(None, help="指定路径，默认当前目录"),
+    path: Path = typer.Option(None, '--path', '-p', help='指定路径，默认当前目录'),
+    noMirrors: bool = typer.Option(False, '--no-mirrors', '-n', help='是否禁用镜像'),
+    quiet: bool = typer.Option(False, '--quiet', '-q', help='是否安静模式'),
 ):
     'python 虚拟环境配置'
-    path = path or Path(os.getcwd())
-    venvPath = bpath.get(path, 'venv')
-    assertPath(venvPath)
-    if not venvPath.exists():
-        await binput.confirm('指定目录为非venv目录，是否确认新创建？')
-    if not venvPath.exists():
-        await bexecute.run(f'python.exe -m venv {venvPath}')
-    venvLockFile = bpath.get(path, 'venv.lock')
-    assertFile(venvLockFile)
-    venvListFile = bpath.get(path, 'venv.list')
-    assertFile(venvListFile)
-    if not venvListFile.exists():
-        await bfile.writeText(venvListFile, '')
-    await tidyVenvFile(venvListFile, packages)
-    if venvLockFile.exists():
-        await tidyVenvFile(venvLockFile, packages)
-        targetFile = venvLockFile
-    else:
-        targetFile = venvListFile
-    pip = bpath.get(venvPath, 'Scripts/pip.exe')
-    await pipInstall(pip, targetFile)
-    await bexecute.run(f'{pip} freeze > {venvLockFile}')
+    packages = packages or []
+    async with bpath.useTempFile() as tempFile:
+        pipIniFile = bpath.user('pip/pip.ini')
+        if noMirrors and pipIniFile.is_file():
+            await bpath.move(pipIniFile, tempFile)
+        try:
+            path = path or Path(os.getcwd())
+            venvPath = bpath.get(path, 'venv')
+            assertPath(venvPath)
+            if not venvPath.exists() and not quiet:
+                await binput.confirm('指定目录为非venv目录，是否确认新创建？')
+            if not venvPath.exists():
+                await bexecute.run(f'python.exe -m venv {venvPath}')
+            venvLockFile = bpath.get(path, 'venv.lock')
+            assertFile(venvLockFile)
+            venvListFile = bpath.get(path, 'venv.list')
+            assertFile(venvListFile)
+            if not venvListFile.exists():
+                await bfile.writeText(venvListFile, '')
+            await tidyVenvFile(venvListFile, packages)
+            if venvLockFile.exists():
+                await tidyVenvFile(venvLockFile, packages)
+                targetFile = venvLockFile
+            else:
+                targetFile = venvListFile
+            pip = bpath.get(venvPath, 'Scripts/pip.exe')
+            await pipInstall(pip, targetFile)
+            await bexecute.run(f'{pip} freeze > {venvLockFile}')
+        finally:
+            if tempFile.is_file():
+                await bpath.move(tempFile, pipIniFile, True)
 
 
 async def pipInstall(pip: Path, file: Path):
     python = pip.with_name('python.exe')
     assert python.is_file()
     assert pip.is_file()
     assert not await bexecute.run(f'{python} -m pip install --upgrade pip'), '更新 pip 失败'
```

### Comparing `bcmd-0.0.8/pyproject.toml` & `bcmd-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # https://peps.python.org/pep-0621/#example
 
 [project]
 name = "bcmd"
-version = "0.0.8"
+version = "0.0.9"
 description = "Commands for Beni"
 requires-python = ">=3.10"
 keywords = ["benimang", "beni", "bcmd"]
 authors = [
   {email = "benimang@126.com"},
   {name = "Beni Mang"},
 ]
```

