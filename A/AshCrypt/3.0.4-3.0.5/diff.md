# Comparing `tmp/AshCrypt-3.0.4.tar.gz` & `tmp/AshCrypt-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AshCrypt-3.0.4.tar", last modified: Wed Jul 26 12:24:18 2023, max compression
+gzip compressed data, was "dist/AshCrypt-3.0.5.tar", last modified: Wed Jul 26 13:11:04 2023, max compression
```

## Comparing `AshCrypt-3.0.4.tar` & `AshCrypt-3.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:24:18.000000 AshCrypt-3.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:24:18.000000 AshCrypt-3.0.4/AshCrypt/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-26 12:24:01.000000 AshCrypt-3.0.4/AshCrypt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-26 12:24:01.000000 AshCrypt-3.0.4/AshCrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-07-26 12:24:01.000000 AshCrypt-3.0.4/AshCrypt/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-26 12:24:01.000000 AshCrypt-3.0.4/AshCrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-26 12:24:01.000000 AshCrypt-3.0.4/AshCrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-26 12:24:01.000000 AshCrypt-3.0.4/AshCrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    39164 2023-07-26 12:24:01.000000 AshCrypt-3.0.4/AshCrypt/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-26 12:24:01.000000 AshCrypt-3.0.4/AshCrypt/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-26 12:24:01.000000 AshCrypt-3.0.4/AshCrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:24:18.000000 AshCrypt-3.0.4/AshCrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-26 12:24:01.000000 AshCrypt-3.0.4/AshCrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-26 12:24:01.000000 AshCrypt-3.0.4/AshCrypt/unittests/unittest_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:24:18.000000 AshCrypt-3.0.4/AshCrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-26 12:24:18.000000 AshCrypt-3.0.4/AshCrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-26 12:24:18.000000 AshCrypt-3.0.4/AshCrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:24:18.000000 AshCrypt-3.0.4/AshCrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 12:24:18.000000 AshCrypt-3.0.4/AshCrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 12:24:18.000000 AshCrypt-3.0.4/AshCrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-26 12:24:18.000000 AshCrypt-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20174 2023-07-26 12:24:01.000000 AshCrypt-3.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 12:24:18.000000 AshCrypt-3.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-26 12:24:01.000000 AshCrypt-3.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:11:04.000000 AshCrypt-3.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:11:04.000000 AshCrypt-3.0.5/AshCrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/AshCrypt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/AshCrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/AshCrypt/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/AshCrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/AshCrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/AshCrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39164 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/AshCrypt/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/AshCrypt/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/AshCrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:11:04.000000 AshCrypt-3.0.5/AshCrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/AshCrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/AshCrypt/unittests/unittest_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:11:04.000000 AshCrypt-3.0.5/AshCrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-26 13:11:04.000000 AshCrypt-3.0.5/AshCrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-26 13:11:04.000000 AshCrypt-3.0.5/AshCrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:11:04.000000 AshCrypt-3.0.5/AshCrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 13:11:04.000000 AshCrypt-3.0.5/AshCrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 13:11:04.000000 AshCrypt-3.0.5/AshCrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-26 13:11:04.000000 AshCrypt-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20174 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 13:11:04.000000 AshCrypt-3.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/setup.py
```

### Comparing `AshCrypt-3.0.4/AshCrypt/clicrypt.py` & `AshCrypt-3.0.5/AshCrypt/clicrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.4/AshCrypt/crypt.py` & `AshCrypt-3.0.5/AshCrypt/crypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.4/AshCrypt/database.py` & `AshCrypt-3.0.5/AshCrypt/database.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,62 @@
+"""Module to interact with an SQLite database"""
+
 from dataclasses import dataclass, field
 from typing import Union, Generator
 from datetime import datetime
 import sqlite3
 import os
 
 
 @dataclass
 class Database:
+    """
+    Represents a simple SQLite database wrapper with various methods to interact with the database.
+    """
     dbname: str = field()
     tablename: str = field(default='Classified')
     conn: sqlite3.Connection = field(init=False, repr=False)
     c: sqlite3.Cursor = field(init=False, repr=False)
 
     def __post_init__(self):
         self.conn = sqlite3.connect(self.dbname)
         self.c = self.conn.cursor()
 
     @property
-    def size(self) -> Union[int, tuple]:         # Size in MB #
+    def size(self) -> Union[int, tuple]:
+        """Returns the database size in MB"""
         try:
             with self.conn:
                 self.c.execute(
                     'SELECT page_count * page_size FROM pragma_page_count() , pragma_page_size')
                 size_info = self.c.fetchone()
                 size = size_info[0] / 1024 / 1024
                 return size
         except sqlite3.Error as e:
             return -1, e
 
     @property
     def last_mod(self) -> Union[datetime, tuple]:
+        """Returns the last time the Database has been altered with"""
         try:
             time_stat = datetime.fromtimestamp(os.stat(self.dbname).st_mtime)
             return time_stat
 
         except OSError as e:
             return 0, e
 
     @property
     def default_routing(self) -> str:
+        """Get the default routing information of the Database class."""
         return f'DEFAULT ROUTING ALL METHODS TO "{self.tablename}"'
 
     def query(self, *querys: str) -> list:
+        """Executes one or more SQL queries and return the results.
+           Provides feedback on whether each given query ran successfully or not.
+           Also provides where the Error has occurred and what type of Error it is."""
         result = []
         for i, query in enumerate(querys):
             if not isinstance(query, str):
                 result.append({f'query {i}': (-1, TypeError)})
             try:
                 with self.conn:
                     self.c.execute(query)
@@ -57,14 +68,16 @@
                             {f'query {i}': ['SUCCESS', self.c.fetchall()]})
 
             except sqlite3.Error as e:
                 result.append({f'query {i}': ('FAILURE', e.__str__())})
         return result
 
     def addtable(self, optional_tablename=None) -> Union[int, tuple]:
+        """Creates a new table in the database with the given table name.
+        If the table name is not provided, it uses the default table name  : 'Classified'."""
         if optional_tablename is None:
             try:
                 with self.conn:
                     self.c.execute(
                         f"CREATE TABLE IF NOT EXISTS {self.tablename} "
                         "(ID INTEGER PRIMARY KEY, Name Text , Content BLOB ,Key TEXT )")
                 return 11
@@ -84,14 +97,15 @@
                 return 1
 
             except sqlite3.Error as e:
                 return 0, e
 
     def insert(self, name, content, key,
                optional_table_name=None) -> Union[int, tuple]:
+        """Inserts a new row into the specified table or the default table."""
         if optional_table_name is None:
             try:
                 with self.conn:
                     self.c.execute(
                         f"INSERT INTO {self.tablename} (Name , Content ,Key) VALUES (? , ? , ?) ",
                         (name,
                          content,
@@ -115,14 +129,15 @@
 
     def update(
             self,
             column_name: str,
             new_column_val: str,
             idd: int,
             optional_table_name=None) -> Union[int, tuple]:
+        """Updates a specific column of a row based on the given ID in the specified table or the default table."""
         if optional_table_name is None:
             try:
                 with self.conn:
                     self.c.execute(
                         f'UPDATE {self.tablename} SET {column_name} = ? WHERE ID = ? ',
                         (new_column_val,
                          idd))
@@ -140,14 +155,16 @@
                          idd))
                     return 1
 
             except sqlite3.Error as e:
                 return 0, e
 
     def content(self, optional_tablename=None) -> Union[Generator, tuple]:
+        """Yields all rows from the specified table or the default table
+         ( as a Generator object ) ."""
         if optional_tablename is None:
             try:
                 with self.conn:
                     self.c.execute(f'SELECT * FROM {self.tablename} ')
                     for row in self.c.fetchall():
                         yield row
 
@@ -162,14 +179,16 @@
                         yield row
 
             except sqlite3.Error as e:
                 return 0, e
 
     def content_by_id(
             self, idd: int, optional_tablename=None) -> Union[Generator, tuple]:
+        """Yields a specific row from the specified table or the default table based on a given ID.
+        ( Generator object )"""
         if optional_tablename is None:
             try:
                 with self.conn:
                     self.c.execute(
                         f'SELECT * FROM {self.tablename} WHERE ID = ? ', (idd,))
                     for row in self.c.fetchall():
                         yield row
@@ -185,14 +204,16 @@
                     for row in self.c.fetchall():
                         yield row
 
             except sqlite3.Error as e:
                 return 0, e
 
     def show_contents(self, *optional_tablenames) -> Union[Generator, tuple]:
+        """Yields all rows from specified tables or the default table.
+        ( Generator object )"""
         if optional_tablenames:
             try:
                 for arg in optional_tablenames:
                     with self.conn:
                         self.c.execute(f'SELECT * FROM {arg} ')
                         for row in self.c.fetchall():
                             yield {arg: row}
@@ -207,37 +228,40 @@
                     for row in self.c.fetchall():
                         yield {self.tablename: row}
 
             except sqlite3.Error as e:
                 return 0, e
 
     def show_tables(self) -> Union[Generator, tuple]:
+        """Yields the names of all tables in the Database. ( Generator object )"""
         try:
             with self.conn:
                 self.c.execute(
                     "SELECT name FROM sqlite_master WHERE type= 'table' ")
                 for row in self.c.fetchall():
                     yield row
 
         except sqlite3.Error as e:
             return 0, e
 
     def dropall(self) -> Union[int, tuple]:
+        """Drops ALL tables in the Database."""
         try:
             with self.conn:
                 self.c.execute(
                     "SELECT name FROM sqlite_master WHERE type= 'table' ")
                 for table in self.c.fetchall():
                     self.c.execute(f'DROP TABLE {table[0]}')
                 return 1
 
         except sqlite3.Error as e:
             return 0, e
 
     def drop_table(self, *table_names) -> Union[int, tuple]:
+        """Drops a/many specific table(s) in the Database."""
         if table_names:
             try:
                 for arg in table_names:
                     with self.conn:
                         self.c.execute(f"DROP TABLE {arg}")
                 return 1
             except sqlite3.Error as e:
@@ -249,14 +273,15 @@
                     self.c.execute(f'DROP TABLE {self.tablename}')
                     return 1
 
             except sqlite3.Error as e:
                 return 0, e
 
     def drop_content(self, idd, optional_table_name=None) -> Union[int, tuple]:
+        """Deletes a row from the specified table or the default table based on the given ID."""
         if optional_table_name is None:
             try:
                 with self.conn:
                     self.c.execute(
                         f'DELETE FROM {self.tablename} WHERE ID = {idd}')
                 return 11
```

### Comparing `AshCrypt-3.0.4/AshCrypt/filecrypt.py` & `AshCrypt-3.0.5/AshCrypt/filecrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.4/AshCrypt/gui.py` & `AshCrypt-3.0.5/AshCrypt/gui.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.4/AshCrypt/textcrypt.py` & `AshCrypt-3.0.5/AshCrypt/textcrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.4/AshCrypt/unittests/unittest_crypt.py` & `AshCrypt-3.0.5/AshCrypt/unittests/unittest_crypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.4/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-3.0.5/AshCrypt.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 3.0.4
+Version: 3.0.5
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
-Description: # Cryptography App &  Library : AES-256
-        ##  Objective ## 
-        #### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256 With No Unnecessary Complications.
+Description: # Cryptography App & Library For AES-256
         ## Docs ## 
         **Visit The [GitHub](https://github.com/AshGw/AES-256/tree/main) Repository.**
         
         
 Keywords: Cryptography application,cryptography libraryAES-256
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `AshCrypt-3.0.4/PKG-INFO` & `AshCrypt-3.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 3.0.4
+Version: 3.0.5
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
-Description: # Cryptography App &  Library : AES-256
-        ##  Objective ## 
-        #### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256 With No Unnecessary Complications.
+Description: # Cryptography App & Library For AES-256
         ## Docs ## 
         **Visit The [GitHub](https://github.com/AshGw/AES-256/tree/main) Repository.**
         
         
 Keywords: Cryptography application,cryptography libraryAES-256
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `AshCrypt-3.0.4/README.md` & `AshCrypt-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.4/setup.py` & `AshCrypt-3.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('AshCrypt/README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='3.0.4',
+    version='3.0.5',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along"
                 " with a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

