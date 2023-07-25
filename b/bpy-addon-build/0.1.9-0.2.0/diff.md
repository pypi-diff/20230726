# Comparing `tmp/bpy_addon_build-0.1.9.tar.gz` & `tmp/bpy_addon_build-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpy_addon_build-0.1.9.tar", max compression
+gzip compressed data, was "bpy_addon_build-0.2.0.tar", max compression
```

## Comparing `bpy_addon_build-0.1.9.tar` & `bpy_addon_build-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     5458 2023-07-23 18:36:24.734437 bpy_addon_build-0.1.9/bpy_addon_build/__init__.py
--rw-r--r--   0        0        0     1644 2023-07-23 18:35:35.169888 bpy_addon_build-0.1.9/bpy_addon_build/actions.py
--rw-r--r--   0        0        0     1021 2023-06-26 06:24:00.000000 bpy_addon_build-0.1.9/bpy_addon_build/yaml_conf.py
--rw-r--r--   0        0        0      548 2023-07-23 18:42:36.848348 bpy_addon_build-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 bpy_addon_build-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     5351 2023-07-25 22:14:33.854613 bpy_addon_build-0.2.0/bpy_addon_build/__init__.py
+-rw-r--r--   0        0        0     1644 2023-07-24 22:05:51.530691 bpy_addon_build-0.2.0/bpy_addon_build/actions.py
+-rw-r--r--   0        0        0     1021 2023-07-24 22:05:51.530691 bpy_addon_build-0.2.0/bpy_addon_build/yaml_conf.py
+-rw-r--r--   0        0        0      548 2023-07-25 22:16:13.648344 bpy_addon_build-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 bpy_addon_build-0.2.0/PKG-INFO
```

### Comparing `bpy_addon_build-0.1.9/bpy_addon_build/__init__.py` & `bpy_addon_build-0.2.0/bpy_addon_build/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,25 +39,27 @@
 
 # Parse a file from a Path
 def parse_file(file: Path) -> yaml_conf.BpyBuildYaml:
     with open(file, "r") as f:
         yaml_config: yaml_conf.BpyBuildYaml = yaml_conf.BpyBuildYaml(f, file)
         return yaml_config
 
+
 # Main function
 def main():
     args = docopt(USAGE)
     bpy_build_yaml: Path = WORKING_DIR / Path("bpy-build.yaml")
 
     if not args["<file>"]:
         if bpy_build_yaml.exists():
             pass
         else:
-            console.print("Can't find bpy-build.yaml, maybe pass it directly?",
-                          style="bold red")
+            console.print(
+                "Can't find bpy-build.yaml, maybe pass it directly?", style="bold red"
+            )
             return
     else:
         bpy_build_yaml = Path(args["<file>"]).resolve()
 
     yaml_conf = parse_file(bpy_build_yaml)
     build_dir = bpy_build_yaml.parents[0] / Path("build")
     copy_dir = build_dir / Path(yaml_conf.build_name + "subfolder")
@@ -100,26 +102,23 @@
                     actions.execute_action(action, inter_dir, console)
         # Rebuild
         if copy_dir.exists():
             shutil.rmtree(copy_dir)
         copy_dir.mkdir()
         shutil.copytree(inter_dir, copy_dir / Path(yaml_conf.build_name))
         with console.status("[bold green]Building...") as _:
-            time.sleep(2)
-            shutil.make_archive(str(build_dir / yaml_conf.build_name), "zip", copy_dir )
+            shutil.make_archive(str(build_dir / yaml_conf.build_name), "zip", copy_dir)
     else:
         # Build addon
         if copy_dir.exists():
             shutil.rmtree(copy_dir)
         copy_dir.mkdir()
         shutil.copytree(yaml_conf.addon_folder, copy_dir / Path(yaml_conf.build_name))
         with console.status("[bold green]Building...") as _:
-            shutil.make_archive(
-                str(build_dir / yaml_conf.build_name), "zip", copy_dir
-            )
+            shutil.make_archive(str(build_dir / yaml_conf.build_name), "zip", copy_dir)
 
     # Install addon
     with console.status("[bold green] Installing...") as _:
         versions_list = yaml_conf.install_versions
         if len(args["<versions>"]):
             versions_list = args["<versions>"]
         for path in map(Path, versions_list):
@@ -138,17 +137,16 @@
                     path = found
                 else:
                     console.print(
                         f"Path {str(path)} doesn't exist, skipping...",
                         style="bold yellow",
                     )
                     continue
-            edited_path: Path = path / Path(yaml_conf.build_name)
+            addon_path: Path = path / Path(yaml_conf.build_name)
             console.print(f"Installing in {str(path)}", style="bold green")
-            shutil.rmtree(edited_path, ignore_errors=True)
-            edited_path.mkdir(exist_ok=True)
-            shutil.unpack_archive(built_zip, edited_path)
-            console.print(f"Installed to {edited_path}")
+            shutil.rmtree(addon_path, ignore_errors=True)
+            shutil.unpack_archive(built_zip, path)
+            console.print(f"Installed to {addon_path}")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `bpy_addon_build-0.1.9/bpy_addon_build/actions.py` & `bpy_addon_build-0.2.0/bpy_addon_build/actions.py`

 * *Files identical despite different names*

### Comparing `bpy_addon_build-0.1.9/bpy_addon_build/yaml_conf.py` & `bpy_addon_build-0.2.0/bpy_addon_build/yaml_conf.py`

 * *Files identical despite different names*

### Comparing `bpy_addon_build-0.1.9/pyproject.toml` & `bpy_addon_build-0.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpy-addon-build"
-version = "0.1.9"
+version = "0.2.0"
 description = "A build system to make building and testing Blender addons 10 times easier"
 authors = ["StandingPad"]
 license = "MIT"
 homepage = "https://github.com/StandingPadAnimations/bpy-build"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `bpy_addon_build-0.1.9/PKG-INFO` & `bpy_addon_build-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpy-addon-build
-Version: 0.1.9
+Version: 0.2.0
 Summary: A build system to make building and testing Blender addons 10 times easier
 Home-page: https://github.com/StandingPadAnimations/bpy-build
 License: MIT
 Author: StandingPad
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

