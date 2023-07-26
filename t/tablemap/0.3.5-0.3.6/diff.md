# Comparing `tmp/tablemap-0.3.5.tar.gz` & `tmp/tablemap-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablemap-0.3.5.tar", last modified: Tue Jul 25 09:50:28 2023, max compression
+gzip compressed data, was "tablemap-0.3.6.tar", last modified: Tue Jul 25 15:13:38 2023, max compression
```

## Comparing `tablemap-0.3.5.tar` & `tablemap-0.3.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 09:50:28.006604 tablemap-0.3.5/
--rw-rw-rw-   0        0        0     1085 2023-03-22 11:37:34.000000 tablemap-0.3.5/LICENSE
--rw-rw-rw-   0        0        0      229 2023-07-25 09:50:28.005604 tablemap-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0    15613 2023-07-24 02:28:24.000000 tablemap-0.3.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-25 09:50:28.007605 tablemap-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0      398 2023-07-25 09:49:21.000000 tablemap-0.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 09:50:27.994605 tablemap-0.3.5/tablemap/
--rw-rw-rw-   0        0        0       34 2023-03-22 11:37:34.000000 tablemap-0.3.5/tablemap/__init__.py
--rw-rw-rw-   0        0        0    43031 2023-07-25 09:49:17.000000 tablemap-0.3.5/tablemap/tablemap.py
-drwxrwxrwx   0        0        0        0 2023-07-25 09:50:28.002611 tablemap-0.3.5/tablemap.egg-info/
--rw-rw-rw-   0        0        0      229 2023-07-25 09:50:27.000000 tablemap-0.3.5/tablemap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-07-25 09:50:27.000000 tablemap-0.3.5/tablemap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 09:50:27.000000 tablemap-0.3.5/tablemap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-25 09:50:27.000000 tablemap-0.3.5/tablemap.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-25 09:50:28.004604 tablemap-0.3.5/test/
--rw-rw-rw-   0        0        0        0 2023-03-22 11:37:34.000000 tablemap-0.3.5/test/__init__.py
--rw-rw-rw-   0        0        0    40307 2023-07-24 11:52:31.000000 tablemap-0.3.5/test/test_core.py
+drwxrwxrwx   0        0        0        0 2023-07-25 15:13:38.751248 tablemap-0.3.6/
+-rw-rw-rw-   0        0        0     1085 2022-12-13 18:38:10.000000 tablemap-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0      229 2023-07-25 15:13:38.750245 tablemap-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0    15842 2023-07-25 15:12:29.000000 tablemap-0.3.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 15:13:38.751248 tablemap-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      398 2023-07-25 15:12:29.000000 tablemap-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 15:13:38.735215 tablemap-0.3.6/tablemap/
+-rw-rw-rw-   0        0        0       34 2022-12-13 18:38:10.000000 tablemap-0.3.6/tablemap/__init__.py
+-rw-rw-rw-   0        0        0    43653 2023-07-25 15:12:29.000000 tablemap-0.3.6/tablemap/tablemap.py
+drwxrwxrwx   0        0        0        0 2023-07-25 15:13:38.742243 tablemap-0.3.6/tablemap.egg-info/
+-rw-rw-rw-   0        0        0      229 2023-07-25 15:13:38.000000 tablemap-0.3.6/tablemap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-07-25 15:13:38.000000 tablemap-0.3.6/tablemap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 15:13:38.000000 tablemap-0.3.6/tablemap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-25 15:13:38.000000 tablemap-0.3.6/tablemap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 15:13:38.749215 tablemap-0.3.6/test/
+-rw-rw-rw-   0        0        0        0 2022-12-13 18:38:10.000000 tablemap-0.3.6/test/__init__.py
+-rw-rw-rw-   0        0        0    40347 2023-07-25 15:12:29.000000 tablemap-0.3.6/test/test_core.py
```

### Comparing `tablemap-0.3.5/LICENSE` & `tablemap-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tablemap-0.3.5/README.md` & `tablemap-0.3.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     {'col1': 'b', 'col2': 1},
 ]
 
 conn = Conn('sample.db')
 conn['t1'] = t1
 ```
 
-The right-hand side of the assignment can consist of a list of dictionaries, an iterator that yields dictionaries, or an object fetched from the connection (referred to as the Rows object, which will be introduced shortly). For example, you can use `conn['t1']` and then chain table-manipulating methods such as `map`, `update`, `by`, `chain`, and more.
+The right-hand side of the assignment can consist of a list of dictionaries, an iterator that yields dictionaries, or an object fetched from the connection (referred to as the Rows object, which will be introduced shortly). For example, you can use `conn['t1']` and then chain table-manipulating methods such as `map`, `update`, `by` and more.
 
 In this context, each dictionary represents a row in a table. For instance, `{'col1': 'a', 'col2': 4}` represents a row with two columns, `col1` and `col2`.
 
 The process of opening and closing the database is handled safely in the background.
 
 To browse tables in the database,
 
@@ -80,33 +80,16 @@
 
 Rows objects provide methods that can be chained together to transform a table.
 
 *** 
 
 ## Methods for table manipulation
 
-+ ### `chain`
 
-To concatenate the `t1` table with itself and create a new table called `t1_double` in the database, you can use the `chain` method provided by the `Rows` object. Here are a couple of examples:
-
-```python
-conn['t1_double'] = conn['t1'].chain(conn['t1'])
-```
-
-This code will create a new table called `t1_double` in the database and populate it with the concatenated result of `t1` with itself.
-
-Alternatively, if you already have a list of dictionaries or an iterator that yields dictionaries named `t1`, you can pass it as an argument to the `chain` method:
-
-```python
-conn['t1_double'] = conn['t1'].chain(t1)
-```
-
-Make sure that the tables being concatenated (`t1` and `t1` in this case) have the same columns. The order of the columns does not matter for concatenation to work correctly.
-
-+ #### A few to brag about. 
+<!-- + #### A few to brag about. 
 
     Some of the properties of this module that make data-wrangling easier 
         
     1. All the methods in this section create a new `Rows` object.  
 
         ```python
         rs = conn['t1']
@@ -141,15 +124,15 @@
         ```python
         conn['t1_1'] = rs2
         ```
 
         Now it actually works because you are trying to save the rows `rs2` generates in the table `t1_1`. Still, `tablemap` does not load up all of `rs2` on memory. It loads and saves one-by-one. 
 
     4. Opens and closes the database automatically and safely. Users don't have to worry about it. Even the keyboard interrupts (like ctrl-c) during the table insertion do not corrupt the database.
-
+ -->
  
 
 + ### `filter` and `update`
 
 Each row is simply a dictionary with column names as keys, so you can access a column value by passing a column name to the row (dictionary). To create new columns or update the existing ones,
 
 ```python
@@ -364,14 +347,44 @@
 + ### `split`
  ```python
 # `xs` is a list of `Rows`.
 xs = conn['t1'].by('col1').split()
  ```
 
 
+ + ### `insert`
+ To concatenate the `t1` table with itself,
+
+ ```python
+ conn['t1'].insert(conn['t1'])
+ conn['t1'].insert(t1)
+ ```
+ 
+`insert` is special in that this is the only method that returns None.
+
+<!-- + ### `chain`
+
+To concatenate the `t1` table with itself and create a new table called `t1_double` in the database, you can use the `chain` method provided by the `Rows` object. Here are a couple of examples:
+
+```python
+conn['t1_double'] = conn['t1'].chain(conn['t1'])
+```
+
+This code will create a new table called `t1_double` in the database and populate it with the concatenated result of `t1` with itself.
+
+Alternatively, if you already have a list of dictionaries or an iterator that yields dictionaries named `t1`, you can pass it as an argument to the `chain` method:
+
+```python
+conn['t1_double'] = conn['t1'].chain(t1)
+```
+
+Make sure that the tables being concatenated (`t1` and `t1` in this case) have the same columns. The order of the columns does not matter for concatenation to work correctly.
+ -->
+
+
 ## Some remarks 
 
 - cross-join example
 
     ```python
     # table2 = conn['t1'].list() is not effective.
     # You should convert it to a list.
```

### Comparing `tablemap-0.3.5/tablemap/tablemap.py` & `tablemap-0.3.6/tablemap/tablemap.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,15 +394,16 @@
         newself._history = newself._history + [{
             'cmd': 'zip_longest',
             'genfn': gen_update_row_ver if self._history[0]['cmd'] == 'fetch'
             else gen_new_row_ver
         }]
         return newself
 
-    def chain(self, other):
+    # deprecated
+    def _chain(self, other):
         """Concatenate Rows to the other
 
         Parameters
         ----------
         other: Rows | list[Row] | Iterable[Row]
 
         Returns
@@ -425,15 +426,36 @@
 
         # pylint: disable=protected-access
         newself._history = newself._history + [{
             'cmd': 'chain',
             'genfn': gen
         }]
         return newself
+    
 
+    def insert(self, other):
+        """Concatenate Rows to the other
+
+        Parameters
+        ----------
+        other: Rows | list[Row] | Iterable[Row]
+
+        """
+        if isinstance(other, Rows):
+            _raise_exception_if_preceded_by_grouping_methods(other)
+
+        prev = self._history[-1] 
+        if prev['cmd'] != 'fetch':
+            raise ValueError("Must be applied to a table in the database")
+
+        with _connect(prev['conn']._dbfile) as dbconn:
+            table_name = prev['tname'] 
+            _insert(dbconn, table_name, _rows2iter(other))
+
+ 
     # each column may contain asc or desc
     # ex) 'col1 desc', 'col2 asc'
     def order(self, fields_maybe_with_desc):
         """Sort according to columns
 
         Parameters
         ----------
```

### Comparing `tablemap-0.3.5/test/test_core.py` & `tablemap-0.3.6/test/test_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,18 +35,30 @@
             os.remove(self.dbfile)
         if Path(self.dbfile1).is_file():
             os.remove(self.dbfile1)
     
     def test_list_various_types(self):
         conn = Conn(self.dbfile)
         conn['t2'] = self.t2
+        rs = conn['t2'].list(set)
+        self.assertEqual(type(rs[0]), set)
 
-        print(conn['t2'].list(set))
+        rs = conn['t2'].list(list)
+        self.assertEqual(type(rs[0]), list)
 
+        rs = conn['t2'].list(tuple)
+        self.assertEqual(type(rs[0]), tuple)
 
+    def test_insert(self):
+        conn = Conn(self.dbfile)
+        conn['t2'] = self.t2
+        conn['t2'].insert(self.t2)
+        conn['t2'].insert(self.t2)
+        conn['t2'].insert(conn['t2'])
+        self.assertEqual(len(conn['t2']), len(self.t2) * 6)
 
     def test_group_with_none(self):
         conn = Conn(self.dbfile)
         conn['t2'] = self.t2
 
         def foo(rs):
             return rs
@@ -314,25 +326,25 @@
                           {'col1': 'c', 'col2': 7, 'n': ''},
                           {'col1': 'd', 'col2': 2, 'n': ''}])
 
     def test_tee_n_new(self):
         conn = Conn(self.dbfile)
 
         def tempfn1(rs):
-            return rs.order('col2 desc').chain(rs.order('col2'))
+            return rs.order('col2 desc')._chain(rs.order('col2'))
         conn['t10'] = self.t1
 
         conn['t1_1'] = conn['t10'].by('col1').map(tempfn1)
 
         self.assertEqual(conn['t1_1']['col2'],
                          [5, 4, 4, 5, 1, 1, 7, 4, 3, 3, 4, 7, 2, 2])
 
         def tempfn2(rs):
             rs1 = rs.update(col2=lambda r: r['col2'] + 1)
-            return rs1.order('col2 desc').chain(rs.order('col2'))
+            return rs1.order('col2 desc')._chain(rs.order('col2'))
 
         conn['t1'] = self.t1
         conn['t1_1'] = conn['t1'].by('col1').map(tempfn2)
         self.assertEqual(conn['t1_1']['col2'],
                          [6, 5, 4, 5, 2, 1, 8, 5, 4, 3, 4, 7, 3, 2])
 
     def test_tee_n_new2(self):
@@ -455,25 +467,14 @@
                           {'col1': 'd', 'col2': 2}]
                          )
         conn['t1_sum2'] = conn['t1']\
             .by('col1').map(sum_by_col1)
 
         self.assertEqual(conn['t1_sum'].list(), conn['t1_sum2'].list())
 
-    def test_chain(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-        conn['t1_double'] = conn['t1'].chain(conn['t1'])
-        self.assertEqual(conn['t1'].list() + conn['t1'].list(),
-                         conn['t1_double'].list())
-
-        conn['t1_double'] = conn['t1'].chain(self.t1)
-        self.assertEqual(conn['t1'].list() + conn['t1'].list(),
-                         conn['t1_double'].list())
-
     def test_df(self):
         import pandas as pd
         conn = Conn(self.dbfile)
         conn['t1'] = self.t1
         df = pd.DataFrame(conn['t1']._iter())
         conn['t1_copy'] = df.to_dict('records')
         self.assertEqual(conn['t1'].list(), conn['t1_copy'].list())
@@ -508,17 +509,17 @@
         conn['t1_1'] = conn['t1'].update(col3=1).by('col1, col3')\
             .map(lambda rs: rs)
 
         conn['t1_2'] = conn['t1'].update(col3=1).by('col1').map(lambda rs: rs)
         self.assertEqual(conn['t1_1'].list(), conn['t1_2'].list())
 
         conn['t1_1_double'] = conn['t1_1']\
-            .chain(conn['t1'].update(col3=1).by('col1, col3')
+            ._chain(conn['t1'].update(col3=1).by('col1, col3')
                    .map(lambda rs: rs))
-        conn['t1_1_double2'] = conn['t1_1'].chain(conn['t1_1'])
+        conn['t1_1_double2'] = conn['t1_1']._chain(conn['t1_1'])
 
         self.assertEqual(conn['t1_1_double'].list(),
                          conn['t1_1_double2'].list())
 
     def test_islice_group(self):
         conn = Conn(self.dbfile)
         conn['t1'] = self.t1
@@ -770,23 +771,23 @@
         )
 
     def test_join2(self):
         conn = Conn(self.dbfile)
         conn['t1'] = self.t1
         conn['t2'] = self.t2
 
-        conn['t1_1'] = conn['t1'].chain([{'col1': 'd', 'col2': 9}, {
+        conn['t1_1'] = conn['t1']._chain([{'col1': 'd', 'col2': 9}, {
             'col1': 'd', 'col2': 19}]).by('col1')\
             .join(conn['t2'].by('col1'), 'full')
 
-        conn['t1_1'] = conn['t1'].chain([{'col1': 'd', 'col2': 9}, {
+        conn['t1_1'] = conn['t1']._chain([{'col1': 'd', 'col2': 9}, {
             'col1': 'd', 'col2': 19}]).by('col1')\
             .join(conn['t2'].by('col1'), 'full')
 
-        conn['t1_2'] = conn['t1'].chain([{'col1': 'd', 'col2': 9}, {
+        conn['t1_2'] = conn['t1']._chain([{'col1': 'd', 'col2': 9}, {
             'col1': 'd', 'col2': 19}]).by('col1')\
             .join(conn['t2'].by('col1'), 'full')\
             .update(col4=lambda r: r['col3'] + 1 if r['col3'] else '')
 
         self.assertEqual(conn['t1_1'].list(),
                          [{'col1': 'a', 'col2': 4, 'col3': ''},
                           {'col1': 'a', 'col2': 5, 'col3': ''},
@@ -818,15 +819,15 @@
                           {'col1': 'd', 'col2': 2, 'col3': 2}])
 
         self.assertEqual(rs1.list(), self.t1)
 
     def test_join4(self):
         rs1 = Rows(self.t1)
         rs2 = Rows(self.t2)
-        rs1 = rs1.chain([{'col1': 'f', 'col2': 9},
+        rs1 = rs1._chain([{'col1': 'f', 'col2': 9},
                          {'col1': 'f', 'col2': 8},
                          {'col1': 'd', 'col2': 11},
 
                          ])
         rs1 = rs1.update(col4=lambda r: r['col2'] * 20)
 
         rs2 = rs2.update(col2=lambda r: r['col3'] * 10)
@@ -864,17 +865,17 @@
         rs3 = rs1.by('col1').join(rs2.by('col1'), 'inner')
         conn['t3'] = conn['t1'].by('col1').join(conn['t2'].by('col1'), 'inner')
         self.assertEqual(rs3.list(), conn['t3'].list())
 
     def test_merge(self):
         rs1 = Rows(self.t1)
         rs2 = Rows(self.t2)
-        rs1 = rs1.chain([{'col1': 'f', 'col2': 9},
+        rs1 = rs1._chain([{'col1': 'f', 'col2': 9},
                          {'col1': 'f', 'col2': 8}])
-        rs2 = rs2.chain([{'col1': 'a', 'col3': 91}])
+        rs2 = rs2._chain([{'col1': 'a', 'col3': 91}])
 
         rs1 = rs1.update(col4=lambda r: r['col2'] * 20)
         rs2 = rs2.update(col2=lambda r: r['col3'] * 10)
 
         rs3 = rs1.by('col1').merge(rs2.by('col1'), 'full')
         self.assertEqual(rs3.list(),
                          [{'col1': 'a', 'col2': 910, 'col4': 80, 'col3': 91},
@@ -966,19 +967,19 @@
             .order('col1, col2 desc').group('col1')\
             .fold(col2_sum=lambda rs: sum(rs['col2']))\
             .deselect('col2')
 
         self.assertEqual(conn['t1_col2sum_groupby_col1'].list(),
                          conn['t1_col2sum_groupby_col1_1'].list())
 
-        conn['t1_double'] = conn['t1'].chain(conn['t1'])
+        conn['t1_double'] = conn['t1']._chain(conn['t1'])
         self.assertEqual(len(conn['t1_double'].list()),
                          2 * len(conn['t1'].list()))
 
-        conn['t1_double'] = conn['t1'].chain(t1)
+        conn['t1_double'] = conn['t1']._chain(t1)
 
         self.assertEqual(len(conn['t1_double'].list()),
                          2 * len(conn['t1'].list()))
 
         conn['t1_1'] = conn['t1']\
             .filter(lambda r: r['col2'] > 2)\
             .update(
```

