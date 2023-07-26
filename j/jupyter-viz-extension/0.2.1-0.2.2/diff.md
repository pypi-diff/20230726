# Comparing `tmp/jupyter_viz_extension-0.2.1.tar.gz` & `tmp/jupyter_viz_extension-0.2.2.tar.gz`

## Comparing `jupyter_viz_extension-0.2.1.tar` & `jupyter_viz_extension-0.2.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/.yarnrc.yml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/install.json
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/tsconfig.json
--rw-r--r--   0        0        0   231366 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/yarn.lock
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter-config/nb-config/jupyter_viz_extension.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter-config/server-config/jupyter_viz_extension.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/_version.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/handlers/__init__.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/handlers/cmd.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/handlers/paraview.py
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/handlers/trame.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/handlers/user.py
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/package.json
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/package.json.orig
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/plugin.json
--rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/187.f44cc496302e8c70c5db.js
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/747.9c4710b3d6c36a34214f.js
--rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/759.6e640b9e09625b3f48df.js
--rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/893.b4c09f80424627b87fe3.js
--rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/remoteEntry.5dcc448ea4f84de302ab.js
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/style.js
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/share/launch_paraview.in
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/schema/plugin.json
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/src/components.tsx
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/src/dialogs.tsx
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/src/handler.ts
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/src/index.tsx
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/src/paraview.tsx
--rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/src/trame.tsx
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/style/base.css
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/style/collapsible.css
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/style/index.js
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/.gitignore
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/LICENSE
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/README.md
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/.yarnrc.yml
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/install.json
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/tsconfig.json
+-rw-r--r--   0        0        0   231366 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/yarn.lock
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter-config/nb-config/jupyter_viz_extension.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter-config/server-config/jupyter_viz_extension.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/_version.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/handlers/__init__.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/handlers/cmd.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/handlers/paraview.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/handlers/trame.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/handlers/user.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/package.json
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/package.json.orig
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/plugin.json
+-rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/187.f44cc496302e8c70c5db.js
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/747.9c4710b3d6c36a34214f.js
+-rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/759.6e640b9e09625b3f48df.js
+-rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/893.b4c09f80424627b87fe3.js
+-rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/remoteEntry.027b522a580a66176974.js
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/share/launch_paraview.in
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/schema/plugin.json
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/src/components.tsx
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/src/dialogs.tsx
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/src/handler.ts
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/src/index.tsx
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/src/paraview.tsx
+-rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/src/trame.tsx
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/style/base.css
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/style/collapsible.css
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/style/index.js
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/README.md
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/PKG-INFO
```

### Comparing `jupyter_viz_extension-0.2.1/package.json` & `jupyter_viz_extension-0.2.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.2.2'"}*

```diff
@@ -178,9 +178,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `jupyter_viz_extension-0.2.1/tsconfig.json` & `jupyter_viz_extension-0.2.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.1/yarn.lock` & `jupyter_viz_extension-0.2.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.1/jupyter_viz_extension/__init__.py` & `jupyter_viz_extension-0.2.2/jupyter_viz_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.1/jupyter_viz_extension/handlers/cmd.py` & `jupyter_viz_extension-0.2.2/jupyter_viz_extension/handlers/cmd.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import asyncio
 
 
-async def run(programm: str, *args: list[str], **kwargs):
+async def run(programm: str, *args: str, logger=None, **kwargs):
     command = " ".join([programm, *args])
     
     proccess = await asyncio.create_subprocess_shell(
         command,
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.PIPE,
         **kwargs
     )
 
     stdout, stderr = await proccess.communicate()
 
-    print(f'{command!r} exited with {proccess.returncode}')
-    if stdout:
-        print(f'[stdout]\n{stdout.decode()}')
-    if stderr:
-        print(f'[stderr]\n{stderr.decode()}')
+    if logger:
+        logger.info(f"{command!r} exited with {proccess.returncode}")
+        if stdout:
+            logger.info(f"[stdout]\n{stdout.decode()}")
+        if stderr:
+            logger.info(f"[stderr]\n{stderr.decode()}")
     
     return proccess.returncode
 
 
-async def output(programm: str, *args: list[str], **kwargs):
+async def output(programm: str, *args: str, **kwargs):
     command = " ".join([programm, *args])
     
     proccess = await asyncio.create_subprocess_shell(
         command,
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.STDOUT,
         **kwargs
```

### Comparing `jupyter_viz_extension-0.2.1/jupyter_viz_extension/handlers/paraview.py` & `jupyter_viz_extension-0.2.2/jupyter_viz_extension/handlers/paraview.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,58 +3,57 @@
 from tempfile import NamedTemporaryFile
 from jinja2 import Template
 from jupyter_server.base.handlers import APIHandler
 from tornado.web import authenticated
 from .cmd import run, output
 
 
-async def _get_running_servers():
-    out = await output("squeue", "--me", "--noheader", "--Format='Partition,Account,NumNodes,TimeUsed,TimeLimit,State,NodeList'")
-    
-    servers = []
-    for server in out.splitlines():
-        print(server)
-        partition, account, nodes, timeUsed, timeLimit, state, *nodelist = server.split()
-        servers.append({
-            "partition": partition,
-            "account": account,
-            "nodes": int(nodes),
-            "timeUsed": timeUsed,
-            "timeLimit": timeLimit,
-            "state": state,
-            "url": f"jwb{nodelist[4:8]}i.juwels:11111" if state == "RUNNING" else None
-        })
-        
-    return servers
-
+class ParaViewHandler(APIHandler):
+    async def get_running_servers(self):
+        out = await output("squeue", "--me", "--noheader", "--Format='Partition,Account,NumNodes,TimeUsed,TimeLimit,State,NodeList'")
 
-async def _launch_paraview(options):
-    print("Launching: ", options)
-    input_file = Path(__file__).parent / ".." / "share" / "launch_paraview.in"
-    template = Template(input_file.read_text())
-    
-    # Create a tempfile and write the SLURM Config into it
-    with NamedTemporaryFile("w", delete=False) as tmp:
-        path = tmp.name
-        tmp.write(template.render(options))
-    
-    print(f"{path = }")
-    await run("sbatch", path)
+        servers = []
+        for server in out.splitlines():
+            self.log.info(f"Found Server: {server}")
+            partition, account, nodes, time_used, time_limit, state, *nodelist = server.split()
+            servers.append({
+                "partition": partition,
+                "account": account,
+                "nodes": int(nodes),
+                "timeUsed": time_used,
+                "timeLimit": time_limit,
+                "state": state,
+                "url": f"jwb{nodelist[4:8]}i.juwels:11111" if state == "RUNNING" else None
+            })
+
+        return servers
+
+    async def launch_paraview(self, options):
+        self.log.info(f"Launching ParaView with Options {options!r}")
+
+        input_file = Path(__file__).parent / ".." / "share" / "launch_paraview.in"
+        template = Template(input_file.read_text())
+
+        # Create a tempfile and write the SLURM Config into it
+        with NamedTemporaryFile("w", delete=False) as tmp:
+            path = tmp.name
+            tmp.write(template.render(options))
 
+        self.log.info(f"Job script in {path!r}")
+        await run("sbatch", path, logger=self.log)
 
-class ParaViewHandler(APIHandler):
     @authenticated
     async def get(self):
-        servers = await _get_running_servers()
+        servers = await self.get_running_servers()
         await self.finish(json.dumps(servers))
         
     @authenticated
     async def post(self):
         try:
-            await _launch_paraview(json.loads(self.request.body))
+            await self.launch_paraview(json.loads(self.request.body))
             self.set_status(200)
             await self.finish()
             
         except Exception as e:
-            print(e)
+            self.log.error(str(e))
             self.set_status(400)
             await self.finish(str(e))
```

### Comparing `jupyter_viz_extension-0.2.1/jupyter_viz_extension/handlers/trame.py` & `jupyter_viz_extension-0.2.2/jupyter_viz_extension/handlers/trame.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,90 +5,89 @@
 from subprocess import Popen
 from pathlib import Path
 
 from jupyter_server.base.handlers import APIHandler
 from tornado.web import authenticated
 
 
-trame_apps = dict()
-processes = []
-
-
 def _next_open_port() -> int:
     # We let socket determine an available open port
     with socket.socket() as s:
         s.bind(("", 0))
         return s.getsockname()[1]
 
 
-def _discover_apps():
-    # We use JUPYTER_PATH to discover Apps
-    paths = os.getenv("JUPYTER_PATH")
-    paths = paths.split(os.pathsep) if paths else []
-    print(f"Searching for trame apps in {paths!r}")
-
-    for path in paths:
-        path = Path(path) / "trame"
-        for short_name in path.iterdir():
-            # Open Config
-            config_file = short_name / "app.yml"
-            if not config_file.exists():
-                raise AttributeError(f"trame app at {short_name.resolve()} does not have a app.yml file")
+class TrameHandler(APIHandler):
+    trame_apps = dict()
+    processes = []
 
-            print(f"Found config at {config_file.resolve()!r}")
+    def discover_apps(self):
+        # We use JUPYTER_PATH to discover Apps
+        paths = os.getenv("JUPYTER_PATH")
+        paths = paths.split(os.pathsep) if paths else []
+        self.log.info(f"Searching for trame apps in {paths!r}")
 
-            config = yaml.safe_load(config_file.read_text())
-            config["path"] = short_name.resolve()
+        for path in paths:
+            path = Path(path) / "trame"
+            if not path.exists():
+                continue
 
-            trame_apps[short_name.name] = config
+            for short_name in path.iterdir():
+                # Open Config
+                config_file = short_name / "app.yml"
+                if not config_file.exists():
+                    raise AttributeError(f"trame app at {short_name.resolve()} does not have a app.yml file")
 
-        
-async def _launch_trame(app_name: str) -> int:
-    config = trame_apps[app_name]
+                self.log.info(f"Found app config at {config_file.resolve()!r}")
 
-    # Determine Port
-    port = _next_open_port()
+                config = yaml.safe_load(config_file.read_text())
+                config["path"] = short_name.resolve()
 
-    # Prepare Environment
-    env = os.environ.copy()
-    env["JUVIZ_ARGS"] = f"--port={port} --server"
+                self.trame_apps[short_name.name] = config
 
-    print(f"Starting {app_name} on port {port}")
-    process = Popen(config["command"], shell=True, env=env, cwd=config.get("working_directory", None))
-    processes.append(process)
+    async def launch_trame(self, app_name: str) -> int:
+        config = self.trame_apps[app_name]
 
-    return port
+        # Determine Port
+        port = _next_open_port()
 
+        # Prepare Environment
+        env = os.environ.copy()
+        env["JUVIZ_ARGS"] = f"--port={port} --server"
+
+        self.log.info(f"Starting {app_name} on port {port}")
+        process = Popen(config["command"], shell=True, env=env, cwd=config.get("working_directory", None))
+        self.processes.append(process)
+
+        return port
 
-class TrameHandler(APIHandler):
     @authenticated
     async def get(self):
-        if not trame_apps:
-            _discover_apps()
-
-        print(trame_apps)
+        if not self.trame_apps:
+            self.discover_apps()
+            self.log.debug(f"Trame Apps: {self.trame_apps}")
 
         await self.finish(json.dumps([
             {
                 "name": name,
                 "displayName": config["name"],
                 "path": str(config["path"].resolve()),
                 "instances": []
             }
-            for name, config in trame_apps.items()
+            for name, config in self.trame_apps.items()
         ]))
     
     @authenticated
     async def post(self):
         app_name = self.get_argument("app_name", "juviz")
         
-        print(f"Launching new trame instance '{app_name}'")
+        self.log.info(f"Launching new trame instance {app_name!r}")
 
         try:
-            port = await _launch_trame(app_name)
+            port = await self.launch_trame(app_name)
             self.set_status(200)
             await self.finish({"port": port})
             
         except Exception as e:
-            print(e)
+            self.log.error(str(e))
             self.set_status(400)
             await self.finish(str(e))
```

### Comparing `jupyter_viz_extension-0.2.1/jupyter_viz_extension/handlers/user.py` & `jupyter_viz_extension-0.2.2/jupyter_viz_extension/handlers/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 from tornado.web import authenticated
 from .cmd import output
 
 
 async def _get_accounts():
     out = await output("jutil", "user", "projects", "--format='json'")
     return [group["unixgroup"] for group in json.loads(out)] if out else []
-    
+
 
 async def _get_partitions():
     return ["booster", "develbooster"]
-    
-    
+
+
 class UserHandler(APIHandler):
     @authenticated
     async def get(self):
         username, accounts, partitions = await asyncio.gather(
             output("whoami"),
             _get_accounts(),
             _get_partitions()
         )
-        
+
+        self.log.debug(f"User: {username!r} - Accounts: {accounts!r} - Partitions: {partitions!r}")
+
         await self.finish({
             "user": username,
             "accounts": accounts,
             "partitions": partitions
         })
```

### Comparing `jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/package.json` & `jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788194444444445%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.027b522a580a66176974.js'}}",*

 * * "'version'": "'0.2.2'"}*

```diff
@@ -106,15 +106,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/github_username/jupyter-viz-extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.5dcc448ea4f84de302ab.js",
+            "load": "static/remoteEntry.027b522a580a66176974.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_viz_extension"
                 },
@@ -183,9 +183,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/package.json.orig` & `jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.2.2'"}*

```diff
@@ -178,9 +178,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/187.f44cc496302e8c70c5db.js` & `jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/187.f44cc496302e8c70c5db.js`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/747.9c4710b3d6c36a34214f.js` & `jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/747.9c4710b3d6c36a34214f.js`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/759.6e640b9e09625b3f48df.js` & `jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/759.6e640b9e09625b3f48df.js`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/893.b4c09f80424627b87fe3.js` & `jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/893.b4c09f80424627b87fe3.js`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/remoteEntry.5dcc448ea4f84de302ab.js` & `jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/remoteEntry.027b522a580a66176974.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -113,15 +113,15 @@
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("jupyter-viz-extension", "0.2.1", (() => Promise.all([j.e(271), j.e(759)]).then((() => () => j(759))))), u("react-collapsible", "2.10.0", (() => Promise.all([j.e(271), j.e(893)]).then((() => () => j(893)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("jupyter-viz-extension", "0.2.2", (() => Promise.all([j.e(271), j.e(759)]).then((() => () => j(759))))), u("react-collapsible", "2.10.0", (() => Promise.all([j.e(271), j.e(893)]).then((() => () => j(893)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/third-party-licenses.json` & `jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.1/jupyter_viz_extension/share/launch_paraview.in` & `jupyter_viz_extension-0.2.2/jupyter_viz_extension/share/launch_paraview.in`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.1/src/dialogs.tsx` & `jupyter_viz_extension-0.2.2/src/dialogs.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.1/src/handler.ts` & `jupyter_viz_extension-0.2.2/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.1/src/index.tsx` & `jupyter_viz_extension-0.2.2/src/index.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.1/src/paraview.tsx` & `jupyter_viz_extension-0.2.2/src/paraview.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.1/src/trame.tsx` & `jupyter_viz_extension-0.2.2/src/trame.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.1/style/collapsible.css` & `jupyter_viz_extension-0.2.2/style/collapsible.css`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.1/.gitignore` & `jupyter_viz_extension-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.1/LICENSE` & `jupyter_viz_extension-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.1/README.md` & `jupyter_viz_extension-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.1/pyproject.toml` & `jupyter_viz_extension-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.1/PKG-INFO` & `jupyter_viz_extension-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_viz_extension
-Version: 0.2.1
+Version: 0.2.2
 Summary: A JupyterLab extension.
 Project-URL: Homepage, https://github.com/github_username/jupyter-viz-extension
 Project-URL: Bug Tracker, https://github.com/github_username/jupyter-viz-extension/issues
 Project-URL: Repository, https://github.com/github_username/jupyter-viz-extension.git
 Author-email: Jonathan Windgassen <j.windgassen@fz-juelich.de>
 License: BSD 3-Clause License
```

