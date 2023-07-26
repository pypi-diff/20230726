# Comparing `tmp/dash-cytoscape-elements-0.0.3.tar.gz` & `tmp/dash-cytoscape-elements-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash-cytoscape-elements-0.0.3.tar", max compression
+gzip compressed data, was "dash-cytoscape-elements-0.0.4.tar", max compression
```

## Comparing `dash-cytoscape-elements-0.0.3.tar` & `dash-cytoscape-elements-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-05-02 15:51:58.105390 dash-cytoscape-elements-0.0.3/LICENSE
--rw-r--r--   0        0        0     4754 2023-05-02 15:51:58.105768 dash-cytoscape-elements-0.0.3/README.md
--rw-r--r--   0        0        0      221 2023-05-28 16:52:24.311252 dash-cytoscape-elements-0.0.3/dash_cytoscape_elements/__init__.py
--rw-r--r--   0        0        0     4973 2023-05-28 16:33:47.805861 dash-cytoscape-elements-0.0.3/dash_cytoscape_elements/element.py
--rw-r--r--   0        0        0    10692 2023-05-08 15:59:42.716960 dash-cytoscape-elements-0.0.3/dash_cytoscape_elements/elements.py
--rw-r--r--   0        0        0      665 2023-05-28 16:52:45.826138 dash-cytoscape-elements-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5636 2023-05-28 16:56:05.860914 dash-cytoscape-elements-0.0.3/setup.py
--rw-r--r--   0        0        0     5487 2023-05-28 16:56:05.861328 dash-cytoscape-elements-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-02 15:51:58.105390 dash-cytoscape-elements-0.0.4/LICENSE
+-rw-r--r--   0        0        0     4754 2023-05-02 15:51:58.105768 dash-cytoscape-elements-0.0.4/README.md
+-rw-r--r--   0        0        0      221 2023-07-26 13:18:08.600103 dash-cytoscape-elements-0.0.4/dash_cytoscape_elements/__init__.py
+-rw-r--r--   0        0        0     6356 2023-07-26 12:57:32.043334 dash-cytoscape-elements-0.0.4/dash_cytoscape_elements/element.py
+-rw-r--r--   0        0        0    12025 2023-07-26 13:16:45.391414 dash-cytoscape-elements-0.0.4/dash_cytoscape_elements/elements.py
+-rw-r--r--   0        0        0      665 2023-07-26 13:18:21.265541 dash-cytoscape-elements-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5636 2023-07-26 13:21:01.973734 dash-cytoscape-elements-0.0.4/setup.py
+-rw-r--r--   0        0        0     5487 2023-07-26 13:21:01.974288 dash-cytoscape-elements-0.0.4/PKG-INFO
```

### Comparing `dash-cytoscape-elements-0.0.3/LICENSE` & `dash-cytoscape-elements-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dash-cytoscape-elements-0.0.3/README.md` & `dash-cytoscape-elements-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dash-cytoscape-elements-0.0.3/dash_cytoscape_elements/element.py` & `dash-cytoscape-elements-0.0.4/dash_cytoscape_elements/element.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The data structures of Dash Cystoscape/Cytoscape.js element."""
+import re
 from typing import Any, Dict, List, Set
 
 from pydantic import BaseModel, Field, validator
 
 __all__ = ["Element", "Edge", "EdgeData", "Node", "NodeData", "Position"]
 
 
@@ -43,14 +44,38 @@
                 return getattr(self, key) == value
         else:
             for v in self.__dict__.values():
                 if isinstance(v, BaseElement):
                     return v.is_match_attribute(key, value)
             return False
 
+    def is_re_match_attribute(self, key: str, pattern: re.Pattern) -> bool:
+        if key in vars(self):
+            if isinstance(getattr(self, key), List):
+                for value in getattr(self, key):
+                    if pattern.search(value):
+                        return True
+            elif isinstance(getattr(self, key), Set):
+                for value in getattr(self, key):
+                    if pattern.search(value):
+                        return True
+            elif isinstance(getattr(self, key), Dict):
+                for value in getattr(self, key):
+                    if pattern.search(value):
+                        return True
+            else:
+                if pattern.search(getattr(self, key)):
+                    return True
+            return False
+        else:
+            for v in self.__dict__.values():
+                if isinstance(v, BaseElement):
+                    return v.is_re_match_attribute(key, pattern)
+            return False
+
     def add_attribute(self, key: str, value: Any):
         if key in vars(self):
             if isinstance(getattr(self, key), List):
                 if isinstance(value, List):
                     for v in value:
                         if not (v in getattr(self, key)):
                             getattr(self, key).append(v)
@@ -109,14 +134,25 @@
         for k, v in kwargs.items():
             if k == "classes":
                 return set(self.classes.split()) >= set(v.split())
             if not (self.is_match_attribute(k, v)):
                 return False
         return True
 
+    def is_re_match(self, **kwargs: Any) -> bool:
+        for k, v in kwargs.items():
+            pattern = re.compile(v)
+            if k == "classes":
+                for c in self.classes.split():
+                    if pattern.search(c):
+                        return True
+            elif self.is_re_match_attribute(k, pattern):
+                return True
+        return False
+
     def _add_classes(self, value: str) -> None:
         classes = self.classes.split()
         for c in value.split():
             if not (c in classes):
                 classes.append(c)
         self.classes = " ".join([c for c in classes])
```

### Comparing `dash-cytoscape-elements-0.0.3/dash_cytoscape_elements/elements.py` & `dash-cytoscape-elements-0.0.4/dash_cytoscape_elements/elements.py`

 * *Files 8% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         """
         if self.__root__:
             return self.json(exclude_defaults=True, indent=4, by_alias=True)
         return ""
 
     def filter(self, **kwargs: Any) -> "GenericElements":
         """Get the `GenericElements` contains Element(`element.Node`/`element.Edge`)
-         objects that match `kwargs`.
+         objects that exact match `kwargs`.
 
         Args:
             **kwargs (Any): no comment
 
         Returns:
             GenericElements: no comment
 
@@ -150,23 +150,58 @@
             >>> print(e.filter(classes="test"))
             [Node(id="node1"), Edge(id="edge2")]
             >>> print(e.filter(parent="p1"))
             [Node(id="node1"), Node(id="node2")]
 
         Note:
             * Match criteria of filter
-                * List/Dict/Set and `classes`: include value or not
+                * List/Dict/Set and `classes`: include exact match value or not
                 * The others Type: exact match value or not
         """
         elements = Elements()
         for e in self:
             if e.is_match(**kwargs):
                 elements._append(e)
         return elements
 
+    def re_filter(self, **kwargs: Any) -> "GenericElements":
+        """Get the `GenericElements` contains Element(`element.Node`/`element.Edge`)
+         objects that regex match `kwargs`.
+
+        Args:
+            **kwargs (Any): no comment
+
+        Returns:
+            GenericElements: no comment
+
+        Examples:
+            >>> e = Elements()
+            >>> e.add(id="node1", parent="p1", classes="test test2")
+            >>> e.add(id="node2", parent="p2")
+            >>> e.add(id="edge1", source="node1", target="node2", classes="abc")
+            >>> e.add(id="edge2", source="node2", target="node1", classes="test")
+            >>>
+            >>> print(e)
+            [Node(id="node1"), Node(id="node2"), Edge(id="edge1"), Edge(id="edge2")]
+            >>> print(e.re_filter(classes="te.*"))
+            [Node(id="node1"), Edge(id="edge2")]
+            >>> print(e.re_filter(parent="p.*"))
+            [Node(id="node1"), Node(id="node2")]
+
+        Note:
+            * Match criteria of filter
+                * List/Dict/Set and `classes`: include regex match value or not
+                * The others Type: regex match value or not
+        """
+        elements = Elements()
+        for e in self:
+            if e.is_re_match(**kwargs):
+                elements._append(e)
+        return elements
+
     def get(self, **kwargs: Any) -> Union[NodeT, EdgeT, None]:
         """Get the Element(`element.Node`/`element.Edge`) object
          in the `GenericElements` matching the `kwargs`.
 
         Get first element if matching multiple elements.
 
         Args:
```

### Comparing `dash-cytoscape-elements-0.0.3/pyproject.toml` & `dash-cytoscape-elements-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dash-cytoscape-elements"
-version = "0.0.3"
+version = "0.0.4"
 description = "Python object for dash-cytoscape elements"
 authors = ["minefuto <minefuto@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/minefuto/dash-cytoscape-elements"
 
 [tool.poetry.dependencies]
```

### Comparing `dash-cytoscape-elements-0.0.3/setup.py` & `dash-cytoscape-elements-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.10.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'dash-cytoscape-elements',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'Python object for dash-cytoscape elements',
     'long_description': '# dash-cytoscape-elements\n[![test](https://github.com/minefuto/dash-cytoscape-elements/actions/workflows/test.yml/badge.svg)](https://github.com/minefuto/dash-cytoscape-elements/actions/workflows/test.yml)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dash-cytoscape-elements)\n![PyPI](https://img.shields.io/pypi/v/dash-cytoscape-elements)\n![GitHub](https://img.shields.io/github/license/minefuto/dash-cytoscape-elements)\n\nThis is a Python object for [Dash Cytoscape](https://github.com/plotly/dash-cytoscape) Elements.\n\n## Features\n- Add/Remove/Get/Filter Element(Node/Edge) on Python object.\n- Convert Python object from/to Dash Cytoscape format \n- Convert Python object from/to json(Cytoscape.js format)\n\n## Install\n```\npip install dash-cytoscape-elements\n```\n\n## Usage\n### Example1\nCreate Elements object & using on Dash Cytoscape  \n```python\nimport dash\nimport dash_cytoscape as cyto\nfrom dash import html\nfrom dash_cytoscape_elements import Elements\n\ne = Elements()\ne.add(id="one", label="Node 1", x=50, y=50)\ne.add(id="two", label="Node 2", x=200, y=200)\ne.add(source="one", target="two", label="Node 1 to 2")\n\napp = dash.Dash(__name__)\napp.layout = html.Div([\n    cyto.Cytoscape(\n        id=\'cytoscape\',\n        elements=e.to_dash(),\n        layout={\'name\': \'preset\'}\n    )\n])\n\nif __name__ == \'__main__\':\n    app.run_server(debug=True)\n```\n### Example2\nEdit json file of Elements.\n```python\nfrom dash_cytoscape_elements import Elements\n\ne = Elements.from_file("elements.json")\ne.remove(id="node2")\ne.remove(source="node1", target="node2")\n\nwith open("elements.json", mode=\'w\') as f:\n    f.write(e.to_json())\n```\n### Supported Parameters\nThis package supports the following parameters of [Dash Cytoscape](https://github.com/plotly/dash-cytoscape) Element.  \n\n| Parameter | Type | Element |\n| --------- | ---- | ------- |\n| id |  str | Node, Edge |\n| parent | str | Node |\n| source | str | Edge |\n| target | str | Edge |\n| label | str | Node, Edge |\n| source_label | str | Edge |\n| target_label | str | Edge |\n| x | float | Node |\n| y | float | Node |\n| classes | str | Node, Edge |\n| selected | str | Node, Edge |\n| selectable | str | Node, Edge |\n| locked | str | Node, Edge |\n| grabbable | str | Node, Edge |\n| pannable | str | Node, Edge |\n| scratch | dict | Node, Edge |\n\nexample output:\n```python\n>>> e = Elements()\n>>> e.add(id="node1", parent="parent1", label="node_label1", x=1, y=1, classes="class1")\n>>> e.add(source="node1", target="node2", label="edge_label1", source_label="source_label1", target_label="target_label1", classes="class1")\n>>> print(e.to_json())\n[\n    {\n        "group": "nodes",\n        "classes": "class1",\n        "data": {\n            "id": "node1",\n            "parent": "parent1",\n            "label": "node_label1"\n        },\n        "position": {\n            "x": 1.0,\n            "y": 1.0\n        }\n    },\n    {\n        "group": "edges",\n        "classes": "class1",\n        "data": {\n            "id": "49082bcd-dcbb-4db7-b369-29e3bf8f74e2",\n            "source": "node1",\n            "target": "node2",\n            "label": "edge_label1",\n            "source-label": "source_label1",\n            "target-label": "target_label1"\n        }\n    }\n]\n```\nHow to add your own parameters:\n```python\nfrom typing import List, Set\nfrom dash_cytoscape_elements import GenericElements\nfrom dash_cytoscape_elements.element import Edge, EdgeData, Node, NodeData\n\n\nclass CustomNodeData(NodeData):\n    custom_str1: str = ""\n\nclass CustomNode(Node):\n    data: CustomNodeData = CustomNodeData()\n    custom_str2: str = ""\n    custom_list: List[str] = []\n\nclass CustomEdgeData(EdgeData):\n    custom_str1: str = ""\n\nclass CustomEdge(Edge):\n    data: CustomEdgeData = CustomEdgeData()\n    custom_str2: str = ""\n    custom_set: Set[str] = set()\n\ne = GenericElements[CustomNode, CustomEdge]()\ne.add(id="node1", custom_str1="str1", custom_str2="str2", custom_list=["list1", "list2"])\ne.add(id="edge1", source="node1", target="node2", custom_str1="str1", custom_str2="str2", custom_set={"set1", "set2"})\n\nprint(e.to_json())\n# [\n#     {\n#         "group": "nodes",\n#         "data": {\n#             "id": "node1",\n#             "custom_str1": "str1"\n#         },\n#         "custom_str2": "str2",\n#         "custom_list": [\n#             "list1",\n#             "list2"\n#         ]\n#     },\n#     {\n#         "group": "edges",\n#         "data": {\n#             "id": "edge1",\n#             "source": "node1",\n#             "target": "node2",\n#             "custom_str1": "str1"\n#         },\n#         "custom_str2": "str2",\n#         "custom_set": [\n#             "set1",\n#             "set2"\n#         ]\n#     }\n# ]\n```\n\nPlease see the [Documentation](https://minefuto.github.io/dash-cytoscape-elements/) for details.\n',
     'author': 'minefuto',
     'author_email': 'minefuto@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/minefuto/dash-cytoscape-elements',
```

### Comparing `dash-cytoscape-elements-0.0.3/PKG-INFO` & `dash-cytoscape-elements-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-cytoscape-elements
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python object for dash-cytoscape elements
 Home-page: https://github.com/minefuto/dash-cytoscape-elements
 License: MIT
 Author: minefuto
 Author-email: minefuto@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

