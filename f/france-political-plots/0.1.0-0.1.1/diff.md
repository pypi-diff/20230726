# Comparing `tmp/france_political_plots-0.1.0.tar.gz` & `tmp/france_political_plots-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "france_political_plots-0.1.0.tar", max compression
+gzip compressed data, was "france_political_plots-0.1.1.tar", max compression
```

## Comparing `france_political_plots-0.1.0.tar` & `france_political_plots-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0        0 2023-07-22 04:52:35.441958 france_political_plots-0.1.0/README.md
--rw-r--r--   0        0        0      199 2023-07-22 04:52:35.440957 france_political_plots-0.1.0/france_political_plots/__init__.py
--rw-r--r--   0        0        0     2302 2023-07-22 04:52:35.440957 france_political_plots-0.1.0/france_political_plots/cli.py
--rw-r--r--   0        0        0      195 2023-07-22 04:52:35.440957 france_political_plots-0.1.0/france_political_plots/config.toml
--rw-r--r--   0        0        0       51 2023-07-22 04:52:35.440957 france_political_plots-0.1.0/france_political_plots/data/__init__.py
--rw-r--r--   0        0        0     6158 2023-07-22 04:52:35.441958 france_political_plots-0.1.0/france_political_plots/data/government_spending.py
--rw-r--r--   0        0        0       42 2023-07-22 04:52:35.441958 france_political_plots-0.1.0/france_political_plots/server/__init__.py
--rw-r--r--   0        0        0    11931 2023-07-22 04:52:35.441958 france_political_plots-0.1.0/france_political_plots/server/assets/volt-data-250x250.jpeg
--rw-r--r--   0        0        0     6999 2023-07-22 04:52:35.441958 france_political_plots-0.1.0/france_political_plots/server/assets/volt-data-250x250.png
--rw-r--r--   0        0        0     9052 2023-07-22 04:52:35.441958 france_political_plots-0.1.0/france_political_plots/server/assets/volt-data-250x250.webp
--rw-r--r--   0        0        0    26953 2023-07-22 04:52:35.441958 france_political_plots-0.1.0/france_political_plots/server/assets/volt-data-500x500.jpeg
--rw-r--r--   0        0        0    13710 2023-07-22 04:52:35.441958 france_political_plots-0.1.0/france_political_plots/server/assets/volt-data-500x500.png
--rw-r--r--   0        0        0    18246 2023-07-22 04:52:35.441958 france_political_plots-0.1.0/france_political_plots/server/assets/volt-data-500x500.webp
--rw-r--r--   0        0        0    43428 2023-07-22 04:52:35.441958 france_political_plots-0.1.0/france_political_plots/server/assets/volt-data-750x750.jpeg
--rw-r--r--   0        0        0    21728 2023-07-22 04:52:35.441958 france_political_plots-0.1.0/france_political_plots/server/assets/volt-data-750x750.png
--rw-r--r--   0        0        0    27108 2023-07-22 04:52:35.441958 france_political_plots-0.1.0/france_political_plots/server/assets/volt-data-750x750.webp
--rw-r--r--   0        0        0    50672 2023-07-22 04:52:35.441958 france_political_plots-0.1.0/france_political_plots/server/assets/volt-data.ico
--rw-r--r--   0        0        0   333343 2023-07-22 04:52:35.441958 france_political_plots-0.1.0/france_political_plots/server/assets/volt-data.svg
--rw-r--r--   0        0        0     6205 2023-07-22 04:52:35.441958 france_political_plots-0.1.0/france_political_plots/server/government_spending.py
--rw-r--r--   0        0        0     7334 2023-07-22 04:52:35.441958 france_political_plots-0.1.0/france_political_plots/server/tools.py
--rw-r--r--   0        0        0     1995 2023-07-22 04:52:35.441958 france_political_plots-0.1.0/france_political_plots/utils.py
--rw-r--r--   0        0        0      704 2023-07-22 04:52:35.441958 france_political_plots-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 france_political_plots-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-26 01:23:12.017611 france_political_plots-0.1.1/README.md
+-rw-r--r--   0        0        0      257 2023-07-26 01:34:58.084806 france_political_plots-0.1.1/france_political_plots/__init__.py
+-rw-r--r--   0        0        0     2479 2023-07-26 01:55:54.846706 france_political_plots-0.1.1/france_political_plots/cli.py
+-rw-r--r--   0        0        0      315 2023-07-26 01:54:59.952324 france_political_plots-0.1.1/france_political_plots/config.toml
+-rw-r--r--   0        0        0       51 2023-07-26 01:23:12.017611 france_political_plots-0.1.1/france_political_plots/data/__init__.py
+-rw-r--r--   0        0        0     6158 2023-07-26 01:23:12.017611 france_political_plots-0.1.1/france_political_plots/data/government_spending.py
+-rw-r--r--   0        0        0       42 2023-07-26 01:23:12.017611 france_political_plots-0.1.1/france_political_plots/server/__init__.py
+-rw-r--r--   0        0        0    11931 2023-07-26 01:23:12.017611 france_political_plots-0.1.1/france_political_plots/server/assets/volt-data-250x250.jpeg
+-rw-r--r--   0        0        0     6999 2023-07-26 01:23:12.017611 france_political_plots-0.1.1/france_political_plots/server/assets/volt-data-250x250.png
+-rw-r--r--   0        0        0     9052 2023-07-26 01:23:12.017611 france_political_plots-0.1.1/france_political_plots/server/assets/volt-data-250x250.webp
+-rw-r--r--   0        0        0    26953 2023-07-26 01:23:12.017611 france_political_plots-0.1.1/france_political_plots/server/assets/volt-data-500x500.jpeg
+-rw-r--r--   0        0        0    13710 2023-07-26 01:23:12.017611 france_political_plots-0.1.1/france_political_plots/server/assets/volt-data-500x500.png
+-rw-r--r--   0        0        0    18246 2023-07-26 01:23:12.017611 france_political_plots-0.1.1/france_political_plots/server/assets/volt-data-500x500.webp
+-rw-r--r--   0        0        0    43428 2023-07-26 01:23:12.017611 france_political_plots-0.1.1/france_political_plots/server/assets/volt-data-750x750.jpeg
+-rw-r--r--   0        0        0    21728 2023-07-26 01:23:12.017611 france_political_plots-0.1.1/france_political_plots/server/assets/volt-data-750x750.png
+-rw-r--r--   0        0        0    27108 2023-07-26 01:23:12.017611 france_political_plots-0.1.1/france_political_plots/server/assets/volt-data-750x750.webp
+-rw-r--r--   0        0        0    50672 2023-07-26 01:23:12.018611 france_political_plots-0.1.1/france_political_plots/server/assets/volt-data.ico
+-rw-r--r--   0        0        0   333343 2023-07-26 01:23:12.018611 france_political_plots-0.1.1/france_political_plots/server/assets/volt-data.svg
+-rw-r--r--   0        0        0     6112 2023-07-26 01:23:12.018611 france_political_plots-0.1.1/france_political_plots/server/government_spending.py
+-rw-r--r--   0        0        0     6063 2023-07-26 03:17:48.375857 france_political_plots-0.1.1/france_political_plots/server/polling_stations.py
+-rw-r--r--   0        0        0     5438 2023-07-26 03:14:04.322526 france_political_plots-0.1.1/france_political_plots/utils.py
+-rw-r--r--   0        0        0      762 2023-07-26 03:24:08.166241 france_political_plots-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 france_political_plots-0.1.1/PKG-INFO
```

### Comparing `france_political_plots-0.1.0/france_political_plots/cli.py` & `france_political_plots-0.1.1/france_political_plots/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import typer
 import sys
 import os
 
 
 from .server.government_spending import Dashboard as gvt_spend
-from .utils import Config, Pkg, Root, Path, error, log, powershell
+from .server.polling_stations import Dashboard as pollstat
+from .utils import Config, Pkg, Root, Path, error, log, powershell, cout
 
 cli = typer.Typer(
     name='fr-pol-plots',
     help='Make interactive plots about french politics.',
     no_args_is_help=True
     )
 
@@ -20,17 +21,21 @@
     host: str = typer.Option("127.0.0.1", '-h', '--host', help='Dash server host'),
     port: str = typer.Option("8050", '-p', '--port', help='Dash server port')
     ):
     config = Config()
 
     name = config.find_project(project)
     
+    cout.log(f"Found: {project} --> {name}")
+    
     match name:
         case 'lfi-spending':
             app = gvt_spend.make()
+        case 'volt-scores':
+            app = pollstat.make()
         case _:
             app = gvt_spend.make()
             
             
     app.run(port=port, host=host, debug=debug)
     
 @cli.command("ls", help="List project names.")
```

### Comparing `france_political_plots-0.1.0/france_political_plots/data/government_spending.py` & `france_political_plots-0.1.1/france_political_plots/data/government_spending.py`

 * *Files identical despite different names*

### Comparing `france_political_plots-0.1.0/france_political_plots/server/assets/volt-data-250x250.jpeg` & `france_political_plots-0.1.1/france_political_plots/server/assets/volt-data-250x250.jpeg`

 * *Files identical despite different names*

### Comparing `france_political_plots-0.1.0/france_political_plots/server/assets/volt-data-250x250.png` & `france_political_plots-0.1.1/france_political_plots/server/assets/volt-data-250x250.png`

 * *Files identical despite different names*

### Comparing `france_political_plots-0.1.0/france_political_plots/server/assets/volt-data-250x250.webp` & `france_political_plots-0.1.1/france_political_plots/server/assets/volt-data-250x250.webp`

 * *Files identical despite different names*

### Comparing `france_political_plots-0.1.0/france_political_plots/server/assets/volt-data-500x500.jpeg` & `france_political_plots-0.1.1/france_political_plots/server/assets/volt-data-500x500.jpeg`

 * *Files identical despite different names*

### Comparing `france_political_plots-0.1.0/france_political_plots/server/assets/volt-data-500x500.png` & `france_political_plots-0.1.1/france_political_plots/server/assets/volt-data-500x500.png`

 * *Files identical despite different names*

### Comparing `france_political_plots-0.1.0/france_political_plots/server/assets/volt-data-500x500.webp` & `france_political_plots-0.1.1/france_political_plots/server/assets/volt-data-500x500.webp`

 * *Files identical despite different names*

### Comparing `france_political_plots-0.1.0/france_political_plots/server/assets/volt-data-750x750.jpeg` & `france_political_plots-0.1.1/france_political_plots/server/assets/volt-data-750x750.jpeg`

 * *Files identical despite different names*

### Comparing `france_political_plots-0.1.0/france_political_plots/server/assets/volt-data-750x750.png` & `france_political_plots-0.1.1/france_political_plots/server/assets/volt-data-750x750.png`

 * *Files identical despite different names*

### Comparing `france_political_plots-0.1.0/france_political_plots/server/assets/volt-data-750x750.webp` & `france_political_plots-0.1.1/france_political_plots/server/assets/volt-data-750x750.webp`

 * *Files identical despite different names*

### Comparing `france_political_plots-0.1.0/france_political_plots/server/assets/volt-data.ico` & `france_political_plots-0.1.1/france_political_plots/server/assets/volt-data.ico`

 * *Files identical despite different names*

### Comparing `france_political_plots-0.1.0/france_political_plots/server/assets/volt-data.svg` & `france_political_plots-0.1.1/france_political_plots/server/assets/volt-data.svg`

 * *Files identical despite different names*

### Comparing `france_political_plots-0.1.0/france_political_plots/server/government_spending.py` & `france_political_plots-0.1.1/france_political_plots/server/government_spending.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,167 +1,187 @@
 from dash import Dash, dcc, html, Input, Output, callback
 from typing import Self, List, Dict, Any
 import dash_ag_grid as dag
 import dash_mantine_components as dmc
 import dash_iconify as dic
-
-from .tools import AGGrid
 from ..data.government_spending import GovernmentSpending
 from ..utils import Pkg, Assets
 
-FULL_SIZE_STYLE = {"width": "100vw", "height": "90vh"}
-
-CONFIG = {"displayModeBar": False, "responsive": True}
+FULL_SIZE_STYLE = {
+    'width':'100vw',
+    'height':'90vh'
+}
 
+CONFIG = {'displayModeBar': False, 'responsive': True}
 
 class Dashboard:
     def __new__(cls) -> Self:
         cls.server = None
         cls.app = None
         return cls
-
+    
     @classmethod
     def make(cls):
         data = GovernmentSpending()
-        before, after = data.spending_change(kind="scatter")
-        line_before, line_after = data.spending_change(kind="line")
-        df = data.df.dropna(subset=["spending"])
-
+        before, after = data.spending_change(kind='scatter')
+        line_before, line_after = data.spending_change(kind='line')
+        df = data.df.dropna(subset=['spending'])
+        
         external_stylesheets = [
-            "https://codepen.io/chriddyp/pen/bWLwgP.css",
+            'https://codepen.io/chriddyp/pen/bWLwgP.css',
             "https://fonts.googleapis.com/css2?family=Fira+Sans:wght@300;400;500;600;700&display=swap",
-        ]
-
-        app = Dash(
-            __name__,
-            external_stylesheets=external_stylesheets,
-            title="LFI 2022 Spending",
-        )
+            ]
 
-        grid = AGGrid(df, app).make()
+        app = Dash(__name__, external_stylesheets=external_stylesheets, title="LFI 2022 Spending")
 
-        components = html.Div(
-            [
-                dcc.Tabs(
-                    [
-                        dcc.Tab(
-                            label="Usual Spending",
-                            children=[
-                                html.Div(
-                                    [
-                                        dcc.Graph(
-                                            figure=before,
-                                            style=FULL_SIZE_STYLE,
-                                            config=CONFIG,
-                                        )
-                                    ],
-                                    style=FULL_SIZE_STYLE,
-                                )
-                            ],
-                        ),
-                        dcc.Tab(
-                            label="Comparison LFI 2022",
-                            children=[
-                                html.Div(
-                                    [
-                                        dcc.Graph(
-                                            figure=after,
-                                            style=FULL_SIZE_STYLE,
-                                            config=CONFIG,
-                                        )
-                                    ],
-                                    style=FULL_SIZE_STYLE,
-                                )
-                            ],
-                        ),
-                        dcc.Tab(
-                            label="Usual Spending per Year",
-                            children=[
-                                html.Div(
-                                    [
-                                        dcc.Graph(
-                                            figure=line_before,
-                                            style=FULL_SIZE_STYLE,
-                                            config=CONFIG,
-                                        )
-                                    ],
-                                    style=FULL_SIZE_STYLE,
-                                )
-                            ],
-                        ),
-                        dcc.Tab(
-                            label="Spending per Year LFI 2022",
-                            children=[
-                                html.Div(
-                                    [
-                                        dcc.Graph(
-                                            figure=line_after,
-                                            style=FULL_SIZE_STYLE,
-                                            config=CONFIG,
-                                        )
-                                    ],
-                                    style=FULL_SIZE_STYLE,
-                                )
-                            ],
-                        ),
-                        dcc.Tab(label="Data", children=grid, style=FULL_SIZE_STYLE),
-                    ]
-                )
-            ],
+        textFilterOpts = {
+            "filterOptions": ["contains", "notContains"],
+            "debounceMs": 200,
+            "suppressAndOrCondition": True,
+        }
+        
+        defaultColDef = {
+            "flex": 1,
+            "sortable": True,
+            "filter": True,
+            'floatingFilter': True,
+            
+        }
+        
+        columnDefs = [
+            {
+                'field': col, 
+                'filter': 'agTextColumnFilter',
+                'filterParams': textFilterOpts,
+                'sortable': True, 
+                'headerName': col
+                } 
+            for col in df.columns
+        ]
+        
+        
+        
+        grid = dag.AgGrid(
+            columnDefs=columnDefs,
+            rowData=df.to_dict('records'),
+            className='ag-theme-material',
+            defaultColDef=defaultColDef,
+            columnSize="sizeToFit",
+            style= FULL_SIZE_STYLE,
         )
 
+        
+        @callback(
+            Output("download-dataframe-csv", "data", allow_duplicate=True),
+            Input("btn_csv", "n_clicks"),
+            prevent_initial_call=True,
+            
+        )
+        def func(n_clicks):
+            return dcc.send_data_frame(df.to_csv, "government-spending.csv")
+        
+        components = html.Div([
+            dcc.Tabs([
+                dcc.Tab(label='Usual Spending', children=[
+                    html.Div([
+                        dcc.Graph(
+                        figure=before,
+                        style=FULL_SIZE_STYLE,
+                        config=CONFIG
+                    )
+                    ],
+                    style=FULL_SIZE_STYLE
+                    )
+                ]),
+                dcc.Tab(label='Comparison LFI 2022', children=[
+                    html.Div([
+                        dcc.Graph(
+                        figure=after,
+                        style=FULL_SIZE_STYLE,
+                        config=CONFIG
+                    )
+                    ],
+                    style=FULL_SIZE_STYLE
+                    )
+                ]),
+                dcc.Tab(label='Usual Spending per Year', children=[
+                    html.Div([
+                        dcc.Graph(
+                        figure=line_before,
+                        style=FULL_SIZE_STYLE,
+                        config=CONFIG
+                    )
+                    ],
+                    style=FULL_SIZE_STYLE
+                    )
+                ]),
+                dcc.Tab(label='Spending per Year LFI 2022', children=[
+                    html.Div([
+                        dcc.Graph(
+                        figure=line_after,
+                        style=FULL_SIZE_STYLE,
+                        config=CONFIG
+                    )
+                    ],
+                    style=FULL_SIZE_STYLE
+                    )
+                ]),
+                dcc.Tab(label='Data', children=[
+                    html.Div([
+                        grid,
+                        dmc.Button("Download as CSV", variant="gradient", id="btn_csv", leftIcon=dic.DashIconify(icon="ic:baseline-download")),
+                        dcc.Download(id="download-dataframe-csv"),
+                    ],
+                    style=FULL_SIZE_STYLE,
+                    )
+                ]),
+            ])
+        ],
+        style=FULL_SIZE_STYLE
+        )
+        
         app.layout = dmc.MantineProvider(
             theme={
                 "fontFamily": "'Fira Sans', sans-serif",
                 "primaryColor": "violet",
                 "components": {
                     "Button": {"styles": {"root": {"fontWeight": 400, "fontSize": 22}}},
                     "Alert": {"styles": {"title": {"fontWeight": 500}}},
                     "AvatarGroup": {"styles": {"truncated": {"fontWeight": 500}}},
                 },
             },
             inherit=True,
             withGlobalStyles=True,
             withNormalizeCSS=True,
             children=[
-                dmc.Stack(
-                    [
+                    dmc.Stack([
                         dmc.Header(
                             height=110,
                             style={"backgroundColor": "#82D0F4"},
                             children=[
-                                dmc.Grid(
-                                    [
-                                        dmc.Center(
-                                            [
-                                                dmc.Image(
-                                                    width=100,
-                                                    height=100,
-                                                    src="/assets/volt-data.svg",
-                                                ),
-                                                dmc.Space(w=50),
-                                                dmc.Title("France Political Data"),
-                                            ]
-                                        )
-                                    ],
-                                    align="left",
-                                    gutter="xs",
-                                )
+                            dmc.Grid([
+                                dmc.Center([
+                                        dmc.Image(width=100, height=100, src="/assets/volt-data.svg"),
+                                        dmc.Space(w=50),
+                                        dmc.Title("France Political Data")
+                                    ])
                             ],
-                        ),
-                        components,
-                    ]
-                )
-            ],
+                            align='left',
+                            gutter='xs',
+                            )
+                        ]),
+                        components
+                    ])
+                    
+                ],
         )
-
+        
         app._favicon = "volt-data.ico"
-
+        
         cls.server = app.server
         cls.app = app
-
+        
         return app
-
-
+        
 dash = Dashboard()
 dash.make()
-server = dash.app.server
+server = dash.app.server
```

### Comparing `france_political_plots-0.1.0/pyproject.toml` & `france_political_plots-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "france-political-plots"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 packages = [{include = "france_political_plots"}]
 
 
 [tool.poetry.scripts]
@@ -22,10 +22,13 @@
 typer = {extras = ["all"], version = "^0.9.0"}
 dash-iconify = "^0.1.2"
 dash-mantine-components = "^0.12.1"
 statsmodels = "^0.14.0"
 waitress = "^2.1.2"
 
 
+[tool.poetry.group.dev.dependencies]
+ipython = "^8.14.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `france_political_plots-0.1.0/PKG-INFO` & `france_political_plots-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: france-political-plots
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dash (>=2.11.1,<3.0.0)
```

