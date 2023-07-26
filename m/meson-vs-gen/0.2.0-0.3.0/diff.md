# Comparing `tmp/meson_vs_gen-0.2.0.tar.gz` & `tmp/meson_vs_gen-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meson_vs_gen-0.2.0.tar", max compression
+gzip compressed data, was "meson_vs_gen-0.3.0.tar", max compression
```

## Comparing `meson_vs_gen-0.2.0.tar` & `meson_vs_gen-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1067 2023-07-25 11:54:34.935475 meson_vs_gen-0.2.0/LICENSE
--rw-r--r--   0        0        0     9649 2023-07-25 11:54:34.935475 meson_vs_gen-0.2.0/README.md
--rw-r--r--   0        0        0     1440 2023-07-25 11:54:34.936475 meson_vs_gen-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-25 11:54:34.959475 meson_vs_gen-0.2.0/vsgen/__init__.py
--rw-r--r--   0        0        0       71 2023-07-25 11:54:34.936475 meson_vs_gen-0.2.0/vsgen/__main__.py
--rw-r--r--   0        0        0     4213 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/api.py
--rw-r--r--   0        0        0      440 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/cli/__init__.py
--rw-r--r--   0        0        0     2380 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/cli/_pathconfig.py
--rw-r--r--   0        0        0     1573 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/cli/generate.py
--rw-r--r--   0        0        0     1221 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/cli/project.py
--rw-r--r--   0        0        0     2776 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/cli/solution.py
--rw-r--r--   0        0        0    10848 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/configfile.py
--rw-r--r--   0        0        0     1043 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/configuration.py
--rw-r--r--   0        0        0     8807 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/introspector.py
--rw-r--r--   0        0        0     3358 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/runsettings.py
--rw-r--r--   0        0        0     6010 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/sln.py
--rw-r--r--   0        0        0    12465 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/vcxproj.py
--rw-r--r--   0        0        0    10837 1970-01-01 00:00:00.000000 meson_vs_gen-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-26 20:11:03.322478 meson_vs_gen-0.3.0/LICENSE
+-rw-r--r--   0        0        0     9649 2023-07-26 20:11:03.322478 meson_vs_gen-0.3.0/README.md
+-rw-r--r--   0        0        0     1440 2023-07-26 20:11:03.323479 meson_vs_gen-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-26 20:11:03.348478 meson_vs_gen-0.3.0/vsgen/__init__.py
+-rw-r--r--   0        0        0       71 2023-07-26 20:11:03.323479 meson_vs_gen-0.3.0/vsgen/__main__.py
+-rw-r--r--   0        0        0     4344 2023-07-26 20:11:03.323479 meson_vs_gen-0.3.0/vsgen/api.py
+-rw-r--r--   0        0        0      440 2023-07-26 20:11:03.323479 meson_vs_gen-0.3.0/vsgen/cli/__init__.py
+-rw-r--r--   0        0        0     2380 2023-07-26 20:11:03.323479 meson_vs_gen-0.3.0/vsgen/cli/_pathconfig.py
+-rw-r--r--   0        0        0     1573 2023-07-26 20:11:03.323479 meson_vs_gen-0.3.0/vsgen/cli/generate.py
+-rw-r--r--   0        0        0     1221 2023-07-26 20:11:03.323479 meson_vs_gen-0.3.0/vsgen/cli/project.py
+-rw-r--r--   0        0        0     2776 2023-07-26 20:11:03.323479 meson_vs_gen-0.3.0/vsgen/cli/solution.py
+-rw-r--r--   0        0        0    10959 2023-07-26 20:11:03.324478 meson_vs_gen-0.3.0/vsgen/configfile.py
+-rw-r--r--   0        0        0     1043 2023-07-26 20:11:03.324478 meson_vs_gen-0.3.0/vsgen/configuration.py
+-rw-r--r--   0        0        0     8818 2023-07-26 20:11:03.324478 meson_vs_gen-0.3.0/vsgen/introspector.py
+-rw-r--r--   0        0        0     3358 2023-07-26 20:11:03.324478 meson_vs_gen-0.3.0/vsgen/runsettings.py
+-rw-r--r--   0        0        0     7261 2023-07-26 20:11:03.324478 meson_vs_gen-0.3.0/vsgen/sln.py
+-rw-r--r--   0        0        0    12465 2023-07-26 20:11:03.324478 meson_vs_gen-0.3.0/vsgen/vcxproj.py
+-rw-r--r--   0        0        0    10837 1970-01-01 00:00:00.000000 meson_vs_gen-0.3.0/PKG-INFO
```

### Comparing `meson_vs_gen-0.2.0/LICENSE` & `meson_vs_gen-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.2.0/README.md` & `meson_vs_gen-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.2.0/pyproject.toml` & `meson_vs_gen-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "meson-vs-gen"
-version = "0.2.0"
+version = "0.3.0"
 description = "Generates Visual Studio solutions and projects for meson projects"
 authors = ["Charles Brunet <charles.brunet@optelgroup.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://gitlab.com/optelgroup-public/meson-vs-gen"
 keywords = ["visualstudio", "meson"]
 classifiers = [
```

### Comparing `meson_vs_gen-0.2.0/vsgen/api.py` & `meson_vs_gen-0.3.0/vsgen/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
     def all_targets(self) -> list[str]:
         return self.introspector.all_targets()
 
     def project(
         self,
         name: str,
-        target: Union[str, bool, None] = None,
+        target: Union[str, bool, None] = True,
         subdir: Union[PathOrStr, bool] = False,
         update: bool = True,
         only_relative_files: bool = False
     ) -> VcxProj:
         project_path = self.projectdir
         if subdir is True:
             project_path /= name
@@ -87,20 +87,24 @@
         if update:
             vcxproj.load_configs()
         else:
             vcxproj.remove_user_file()
 
         vcxproj.add_config(self.config)
 
-        if target is True or not target:
-            target = name
-        output = self.introspector.get_target_filename(target)
-        extra_paths = self.introspector.get_target_extra_paths(target)
-
-        if target.startswith('dep:'):
+        if target:
+            if target is True:
+                target = name
+
+            output = self.introspector.get_target_filename(target)
+            extra_paths = self.introspector.get_target_extra_paths(target)
+
+        if not target:
+            build_params = BuildParams()
+        elif target.startswith('dep:'):
             build_params = BuildParams(
                 None,
                 *self.introspector.get_target_params(target)
             )
         elif output:
             output = Path(output).relative_to(self.builddir)
 
@@ -110,20 +114,21 @@
                 extra_paths,
             )
         else:
             build_params = BuildParams(output=target)
 
         vcxproj.add_build_params(str(self.config), build_params)
 
-        if output or target.startswith('dep:'):
-            vcxproj.add_sources(self.introspector.get_target_sources(target, only_relative_files))
-            vcxproj.add_headers(self.introspector.get_target_headers(target, only_relative_files))
-            vcxproj.add_extra_files(self.introspector.get_target_extra_files(target, self.basedir, only_relative_files))
-        elif target == 'all':
-            vcxproj.add_extra_files(self.introspector.get_build_files())
+        if target:
+            if output or target.startswith('dep:'):
+                vcxproj.add_sources(self.introspector.get_target_sources(target, only_relative_files))
+                vcxproj.add_headers(self.introspector.get_target_headers(target, only_relative_files))
+                vcxproj.add_extra_files(self.introspector.get_target_extra_files(target, self.basedir, only_relative_files))
+            elif target == 'all':
+                vcxproj.add_extra_files(self.introspector.get_build_files())
 
         return vcxproj
 
     def solution(self, name: str, update: bool = True) -> SolutionFile:
         sln = SolutionFile(self.outputdir / name)
 
         if update:
```

### Comparing `meson_vs_gen-0.2.0/vsgen/cli/_pathconfig.py` & `meson_vs_gen-0.3.0/vsgen/cli/_pathconfig.py`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.2.0/vsgen/cli/generate.py` & `meson_vs_gen-0.3.0/vsgen/cli/generate.py`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.2.0/vsgen/cli/project.py` & `meson_vs_gen-0.3.0/vsgen/cli/project.py`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.2.0/vsgen/cli/solution.py` & `meson_vs_gen-0.3.0/vsgen/cli/solution.py`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.2.0/vsgen/configfile.py` & `meson_vs_gen-0.3.0/vsgen/configfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,25 +57,27 @@
 
         if not outputpath:
             outputpath = Path(self.data.get('outputdir', '.'))
 
         gen = Generator(outputpath, basepath, self.data.get('projectdir', ''))
         gen.cpu_arch = self.data.get('archs', {})
 
-        projects = []
+        all_projects = {}
         solutions = {}
         for config_path, config_name in self.data.get('configs', {}).items():
             if not gen.set_config(config_path, config_name, use_include_from_env):
                 continue
 
             projects = self._generate_projects(gen, update)
+            for p in projects:
+                all_projects[p.uuid] = p
             solutions = self._generate_solutions(gen, projects, update)
             update = True
 
-        self._generate_runsettings(gen, solutions, projects)
+        self._generate_runsettings(gen, solutions, all_projects.values())
 
     def _analyse_targets(self, targets: set[str]) -> dict:
         listed_targets = set()
         for project_name, target in self.data['projects'].items():
             if project_name == '*':
                 continue
             if isinstance(target, bool):
@@ -170,15 +172,15 @@
 
                 target = " ".join(target)
 
             else:
                 if target in all_targets:
                     all_targets.remove(target)
                 elif target not in self.SPECIAL_TARGETS:
-                    continue
+                    target = False  # dummy target
 
             project = gen.project(name, target, config['subdir'], update, orf).write()
             projects.append(project)
 
         if self.data.get('projects', {}).get('*'):
             for target in all_targets:
                 if target.startswith('dep:'):
```

### Comparing `meson_vs_gen-0.2.0/vsgen/configuration.py` & `meson_vs_gen-0.3.0/vsgen/configuration.py`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.2.0/vsgen/introspector.py` & `meson_vs_gen-0.3.0/vsgen/introspector.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,30 +175,30 @@
         return headers
 
     def get_target_extra_files(self, target: str, sources_root: Path, only_relative_files: bool = False) -> list[Path]:
         data = self._target_data(target)
         if not data:
             return []
         
-        if not target.startswith('dep:'):
-            source_dir = Path(data['defined_in']).parent
+        source_dir = Path(data['defined_in']).parent if 'defined_in' in data else None
 
         extras = set()
         for s in data['extra_files']:
             if not s.endswith(self.HEADER_SUFFIXES):
                 s = Path(s)
                 if target.startswith('dep:') or not only_relative_files or s.is_relative_to(source_dir):
                     extras.add(s)
 
-        if not target.startswith('dep:'):
+        if source_dir:
             # meson.build files
             for m in self.intro_data['buildsystem_files']:
                 if (e := Path(m)).is_relative_to(source_dir):
                     extras.add(e)
 
+        if not target.startswith('dep:'):
             if def_file := data.get('vs_module_defs'):
                 def_file = (sources_root / def_file).resolve()
                 extras.add(def_file)
 
         return list(sorted(extras))
 
     def get_target_extra_paths(self, target: str) -> list[Path]:
```

### Comparing `meson_vs_gen-0.2.0/vsgen/runsettings.py` & `meson_vs_gen-0.3.0/vsgen/runsettings.py`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.2.0/vsgen/sln.py` & `meson_vs_gen-0.3.0/vsgen/sln.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,23 +30,25 @@
 
 
 class SolutionFile:
 
     VCXPROJ_UUID = "{8BC9CEB8-8B4A-11D0-8D11-00A0C91BC942}"
     SUBDIR_UUID = "{2150E333-8FDC-42A3-9474-1A3956D46DE8}"
 
+    UUID_RE = r'\{[A-F0-9]{8}-[A-F0-9]{4}-[A-F0-9]{4}-[A-F0-9]{4}-[A-F0-9]{12}\}'
+
     def __init__(self, solution_path: Path):
         self.path = solution_path.with_suffix('.sln')
 
         self.projects: dict[str, ProjectData] = {}
 
-        self._subdirs: dict[str, str] = {}
+        self._subdirs: dict[str, str] = {}  # map path to uuid
         self.uuid = f"{{{str(uuid.uuid4())}}}".upper()
 
-    def add_project(self, project: VcxProj, subdir: Optinoal[str] = None, build_solution_target: bool = False) -> None:
+    def add_project(self, project: VcxProj, subdir: Optional[str] = None, build_solution_target: bool = False) -> None:
         project_path = project.filepath
         if project_path.is_relative_to(self.path.parent):
             project_path = project_path.relative_to(self.path.parent)
 
         project_data = ProjectData(
             project.uuid, project.name, project_path, subdir=subdir, build_solution_target=build_solution_target
         )
@@ -66,25 +68,53 @@
             parts.pop(-1)
 
     def load_configs(self) -> None:
         if not self.path.exists():
             return
 
         contents = self.path.read_text(encoding='utf-8')
-        m = re.search(r'SolutionGuid = (\{[0-9A-F-]+\})', contents)
+        m = re.search(f'SolutionGuid = ({self.UUID_RE})', contents)
         self.uuid = m[1]
 
-        for m in re.finditer(rf'Project\("{self.VCXPROJ_UUID}"\) = "(.*)", "(.*)", "(.*)"', contents):
+        for m in re.finditer(rf'Project\("{self.VCXPROJ_UUID}"\) = "(.*)", "(.*)", "({self.UUID_RE})"', contents):
             project_path = Path(m[2])
             if (self.path.parent / project_path).with_suffix(VcxProj.EXT).exists():
                 project_data = ProjectData(m[3], m[1], project_path)
                 self.projects[project_data.uuid] = project_data
 
-        for m in re.finditer(rf'Project\("{self.SUBDIR_UUID}"\) = "(.*)", "(.*)", "(.*)"', contents):
-            self._subdirs[m[2]] = m[3]
+        sln_subdirs = {}  # map subdir uuid to subdir name
+        for m in re.finditer(rf'Project\("{self.SUBDIR_UUID}"\) = "(.*)", "(.*)", "({self.UUID_RE})"', contents):
+            sln_subdirs[m[3]] = m[1]
+
+        # rebuild solution hieararchy...
+        sln_subdirs_parents = {}
+        prj_subdirs = {}  # map project uuid to subdir uuid
+        for m in re.finditer(f'({self.UUID_RE}) = ({self.UUID_RE})', contents):
+            if m[1] in sln_subdirs:
+                sln_subdirs_parents[m[1]] = m[2]
+            elif m[1] in self.projects:
+                prj_subdirs[m[1]] = m[2]
+
+        while sln_subdirs:
+            top_level = {u for u in sln_subdirs if u not in sln_subdirs_parents}
+
+            for u, p in list(sln_subdirs_parents.items()):
+                if p in top_level:
+                    sln_subdirs[u] = sln_subdirs[p] + '/' + sln_subdirs[u]
+                    del sln_subdirs_parents[u]
+
+            for t in top_level:
+                sd = sln_subdirs.pop(t)
+                self._subdirs[sd] = t
+                
+                for p, u in list(prj_subdirs.items()):
+                    if u == t:
+                        self.projects[p].subdir = sd
+                        del prj_subdirs[p]
+        assert not sln_subdirs_parents
 
         for m in re.finditer(r'(\{[0-9A-F-]+\}).([\w-]+\|[\w]+)\.ActiveCfg', contents):
             self.projects[m[1]].configurations.add(BaseConfig.from_str(m[2]))
         for m in re.finditer(r'(\{[0-9A-F-]+\}).([\w-]+\|[\w]+)\.Build\.0', contents):
             self.projects[m[1]].build_solution_target = True
 
     def write(self) -> None:
@@ -100,15 +130,15 @@
         for project in sorted(self.projects.values()):
             contents.append(f'Project("{self.VCXPROJ_UUID}") = "{project.name}", "{project.path}", "{project.uuid}"')
             contents.append('EndProject')
             configurations.update(project.configurations)
         for subdir in sorted(self._subdirs):
             subdir_uuid = self._subdirs[subdir]
             parts = subdir.split('/')
-            contents.append(f'Project("{self.SUBDIR_UUID}") = "{parts[-1]}", "{subdir}", "{subdir_uuid}"')
+            contents.append(f'Project("{self.SUBDIR_UUID}") = "{parts[-1]}", "{parts[-1]}", "{subdir_uuid}"')
             contents.append('EndProject')
 
         contents.append('Global')
 
         contents.append('	GlobalSection(SolutionConfigurationPlatforms) = preSolution')
         for config in sorted(configurations):
             contents.append(f'		{config} = {config}')
@@ -125,24 +155,24 @@
         contents.append('	GlobalSection(SolutionProperties) = preSolution')
         contents.append('		HideSolutionNode = FALSE')
         contents.append('	EndGlobalSection')
 
         if self._subdirs:
             contents.append('	GlobalSection(NestedProjects) = preSolution')
 
-            for subdir_name, subdir_uuid in self._subdirs.items():
-                if '/' in subdir_name:
-                    parent, _ = subdir_name.rsplit('/', maxsplit=1)
-                    parent_uuid = self._subdirs[parent]
-                    contents.append(f'		{subdir_uuid} = {parent_uuid}')
-
             for project in sorted(self.projects.values()):
                 if project.subdir:
                     subdir_uuid = self._subdirs[project.subdir]
                     contents.append(f'		{project.uuid} = {subdir_uuid}')
+
+            for subdir_name, subdir_uuid in sorted(self._subdirs.items()):
+                if '/' in subdir_name:
+                    parent, _ = subdir_name.rsplit('/', maxsplit=1)
+                    parent_uuid = self._subdirs[parent]
+                    contents.append(f'		{subdir_uuid} = {parent_uuid}')
             contents.append('	EndGlobalSection')
 
         contents.append('	GlobalSection(ExtensibilityGlobals) = postSolution')
         contents.append(f'		SolutionGuid = {self.uuid}')
         contents.append('	EndGlobalSection')
 
         contents.append('EndGlobal')
```

### Comparing `meson_vs_gen-0.2.0/vsgen/vcxproj.py` & `meson_vs_gen-0.3.0/vsgen/vcxproj.py`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.2.0/PKG-INFO` & `meson_vs_gen-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meson-vs-gen
-Version: 0.2.0
+Version: 0.3.0
 Summary: Generates Visual Studio solutions and projects for meson projects
 Home-page: https://gitlab.com/optelgroup-public/meson-vs-gen
 License: MIT
 Keywords: visualstudio,meson
 Author: Charles Brunet
 Author-email: charles.brunet@optelgroup.com
 Requires-Python: >=3.9,<4.0
```

