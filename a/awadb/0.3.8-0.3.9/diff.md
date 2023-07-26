# Comparing `tmp/awadb-0.3.8-cp39-cp39-manylinux1_x86_64.whl.zip` & `tmp/awadb-0.3.9-cp39-cp39-macosx_10_13_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,15 @@
-Zip file size: 2525116 bytes, number of entries: 11
--rwxr-xr-x  2.0 unx  7224968 b- defN 23-Jul-21 23:14 awa.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx    45524 b- defN 23-Jul-21 23:07 awadb/__init__.py
--rw-r--r--  2.0 unx       99 b- defN 23-Jul-21 23:07 awadb/punctuation_marks_en.py
--rw-r--r--  2.0 unx    11484 b- defN 23-Jul-21 23:07 awadb/stop_words_en.py
--rw-r--r--  2.0 unx    13236 b- defN 23-Jul-21 23:07 awadb/words_stem_en.py
--rw-r--r--  2.0 unx     1116 b- defN 23-Jul-16 15:11 awadb/llm_embedding/__init__.py
--rw-r--r--  2.0 unx    15759 b- defN 23-Jul-21 23:14 awadb-0.3.8.dist-info/LICENSE
--rw-r--r--  2.0 unx      363 b- defN 23-Jul-21 23:14 awadb-0.3.8.dist-info/METADATA
--rw-r--r--  2.0 unx      108 b- defN 23-Jul-21 23:14 awadb-0.3.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-21 23:14 awadb-0.3.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      878 b- defN 23-Jul-21 23:14 awadb-0.3.8.dist-info/RECORD
-11 files, 7313545 bytes uncompressed, 2523650 bytes compressed:  65.5%
+Zip file size: 2815570 bytes, number of entries: 13
+-rwxr-xr-x  2.0 unx  8174320 b- defN 23-Jul-26 08:04 awa.cpython-39-darwin.so
+-rw-r--r--  2.0 unx    46486 b- defN 23-Jul-26 08:03 awadb/__init__.py
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-21 14:52 awadb/punctuation_marks_en.py
+-rw-r--r--  2.0 unx    11484 b- defN 23-Jul-21 14:52 awadb/stop_words_en.py
+-rw-r--r--  2.0 unx    13236 b- defN 23-Jul-21 14:52 awadb/words_stem_en.py
+-rw-r--r--  2.0 unx     1160 b- defN 23-Jul-26 08:03 awadb/awa_embedding/huggingface.py
+-rw-r--r--  2.0 unx     1268 b- defN 23-Jul-26 08:03 awadb/awa_embedding/openai.py
+-rw-r--r--  2.0 unx     1117 b- defN 23-Jul-21 15:28 awadb/llm_embedding/__init__.py
+-rw-r--r--  2.0 unx    15759 b- defN 23-Jul-26 08:05 awadb-0.3.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      329 b- defN 23-Jul-26 08:05 awadb-0.3.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      109 b- defN 23-Jul-26 08:05 awadb-0.3.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-26 08:05 awadb-0.3.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1045 b- defN 23-Jul-26 08:05 awadb-0.3.9.dist-info/RECORD
+13 files, 8266422 bytes uncompressed, 2813846 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -1,34 +1,40 @@
-Filename: awa.cpython-39-x86_64-linux-gnu.so
+Filename: awa.cpython-39-darwin.so
 Comment: 
 
 Filename: awadb/__init__.py
 Comment: 
 
 Filename: awadb/punctuation_marks_en.py
 Comment: 
 
 Filename: awadb/stop_words_en.py
 Comment: 
 
 Filename: awadb/words_stem_en.py
 Comment: 
 
+Filename: awadb/awa_embedding/huggingface.py
+Comment: 
+
+Filename: awadb/awa_embedding/openai.py
+Comment: 
+
 Filename: awadb/llm_embedding/__init__.py
 Comment: 
 
-Filename: awadb-0.3.8.dist-info/LICENSE
+Filename: awadb-0.3.9.dist-info/LICENSE
 Comment: 
 
-Filename: awadb-0.3.8.dist-info/METADATA
+Filename: awadb-0.3.9.dist-info/METADATA
 Comment: 
 
-Filename: awadb-0.3.8.dist-info/WHEEL
+Filename: awadb-0.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: awadb-0.3.8.dist-info/top_level.txt
+Filename: awadb-0.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: awadb-0.3.8.dist-info/RECORD
+Filename: awadb-0.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## awadb/__init__.py

```diff
@@ -23,14 +23,19 @@
 class FieldDataType(Enum):
     INT = 1
     FLOAT = 2
     STRING = 3
     VECTOR = 4
     ERROR = 5
 
+__all__ = [
+    "OpenAI",
+    "HuggingFace",
+]
+
 
 def typeof(variate):
     v_type = FieldDataType.ERROR
     if isinstance(variate, int):
         v_type = FieldDataType.INT
     elif isinstance(variate, str):
         v_type = FieldDataType.STRING
@@ -54,14 +59,48 @@
     return v_type
 
 
 def md5str(str):
     m = hashlib.md5(str.encode(encoding="utf-8"))
     return m.hexdigest()
 
+class AwaEmbedding:
+    """Embedding models."""
+    def __init__(
+        self, 
+        model_name: Optional[str] = None):
+        if model_name is None:
+            self.model_name = "HuggingFace"
+        else:
+            self.model_name = model_name
+
+        if self.model_name == "OpenAI":
+            from awadb.awa_embedding.openai import OpenAIEmbeddings
+            self.llm = OpenAIEmbeddings()
+        else:
+            from awadb.awa_embedding.huggingface import HuggingFaceEmbeddings
+            self.llm = HuggingFaceEmbeddings()
+
+    #set your own llm
+    def SetModel(self, model_name):
+        self.model = AutoModel.from_pretrained(model_name)
+
+    #set your own tokenizer
+    def SetTokenizer(self, tokenizer_name):
+        self.tokenizer = AutoTokenizer.from_pretrained(tokenizer_name)
+
+    def Embedding(self, sentence):
+        return self.llm.Embedding(sentence)
+    
+    def EmbeddingBatch(
+        self,
+        texts: Iterable[str],
+        **kwargs: Any,
+    ) -> List[List[float]]:
+        return self.llm.EmbeddingBatch(texts, **kwargs)
 
 class Client:
     def __init__(self, root_dir="."):
         self.root_dir = root_dir
         log_dir = root_dir + "/log"
         data_dir = root_dir + "/data"
         if not os.path.isdir(log_dir):
@@ -88,14 +127,15 @@
 
         existed_meta_file = data_dir + "/tables.meta"
         if os.path.isfile(existed_meta_file):
             self.Read()
 
         self.llm = None
         self.is_duplicate_texts = True
+        self.model_name = "HuggingFace"
 
     def Write(self):
         tables_meta = {}
         tables_meta["fields_check"] = self.tables_fields_check
         tables_types = {}
         for table_name in self.tables_fields_type:
             fields_type_list = []
@@ -241,15 +281,18 @@
                     table_info.AddVectorInfo(vec_info)
 
                 table_info.SetIndexingSize(10000)
                 table_info.SetRetrievalType("IVFPQ")
                 table_info.SetRetrievalParam('{"ncentroids" : 256, "nsubvector" : 16}')
                 self.tables_attr[table_name] = table_info
 
-    def Create(self, table_name):
+    def Create(self, table_name, model_name="HuggingFace"):
+        if model_name not in __all__:
+            raise NameError("Could not find this model: ", model_name)
+
         if table_name in self.tables:
             print("Table %s exist! Please directly Use(%s)" % (table_name, table_name))
             return False
         log_dir = self.root_dir + "/log/"
         log_dir = log_dir + table_name
         data_dir = self.root_dir + "/data/"
         data_dir = data_dir + table_name
@@ -257,14 +300,16 @@
         self.tables[table_name] = new_table
         self.using_table_name = table_name
         self.using_table_engine = new_table
         self.tables_fields_check[table_name] = False
         self.tables_have_obvious_primary_key[table_name] = False
         self.tables_primary_key_fid_no[table_name] = None
         self.tables_doc_count[table_name] = 0
+        self.model_name = model_name
+        self.llm = AwaEmbedding(self.model_name)
         return True
 
     def Close(self, table_name: Optional[str] = None):
         if table_name is None:
             if self.using_table_engine is None:
                 return False
             if awa.Close(self.using_table_engine) == 0:
@@ -526,23 +571,24 @@
                 fvec_names.append(field_name)
 
             ret = awa.DoSearch(self.using_table_engine, req, response)
             response.PackResults(fvec_names)
 
             search_result_vec = response.Results()
             search_result_index = 0
+            # the usage of iterator pybind11 struct may cause crash in MacOSX x86 environment
             while search_result_index < search_result_vec.__len__():
                 search_result = search_result_vec[search_result_index]
-            #for search_result in search_result_vec:
+                # for search_result in search_result_vec:
                 items = search_result.result_items
                 item_index = 0
-                #for item in items:
+                # for item in items:
                 while item_index < items.__len__():
                     i = 0
-                    item = items[item_index] 
+                    item = items[item_index]
                     l = item.names.__len__()
                     item_detail = {}
                     while i < l:
                         name = item.names[i]
                         if (
                             not_include_fields is not None
                             and name in not_include_fields
@@ -563,15 +609,15 @@
                         elif f_type == FieldDataType.VECTOR:
                             vec_data = awa.FloatVec()
                             item.GetVecData(name, vec_data)
                             vec_result = []
                             vec_index = 0
                             while vec_index < vec_data.__len__():
                                 each_vec_data = vec_data[vec_index]
-                            #for each_vec_data in vec_data:
+                                # for each_vec_data in vec_data:
                                 vec_result.append(each_vec_data)
                                 vec_index = vec_index + 1
                             item_detail[name] = vec_result
                         i = i + 1
                     docs_detail.append(item_detail)
                     item_index = item_index + 1
                 search_result_index = search_result_index + 1
@@ -589,73 +635,55 @@
             if doc_results[key_id].Key() == "-1":
                 continue
 
             doc_detail = {}
             field_index = 0
             while field_index < doc_results[key_id].TableFields().__len__():
                 field = doc_results[key_id].TableFields()[field_index]
-            #for field in doc_results[key_id].TableFields():
+                # for field in doc_results[key_id].TableFields():
                 if not_include_fields is not None and field.name in not_include_fields:
-                    field_index = field_index + 1 
+                    field_index = field_index + 1
                     continue
                 if field.datatype == awa.DataType.INT:
                     int_value = int(field.value)
                     doc_detail[field.name] = int_value
                 elif field.datatype == awa.DataType.FLOAT:
                     float_value = float(field.value)
                     doc_detail[field.name] = float_value
                 elif field.datatype == awa.DataType.STRING:
                     doc_detail[field.name] = field.value
                 field_index = field_index + 1
 
             field_index = 0
             while field_index < doc_results[key_id].VectorFields().__len__():
                 field = doc_results[key_id].VectorFields()[field_index]
-            #for field in doc_results[key_id].VectorFields():
+                # for field in doc_results[key_id].VectorFields():
                 if not_include_fields is not None and field.name in not_include_fields:
-                    field_index = field_index + 1 
+                    field_index = field_index + 1
                     continue
                 if field.datatype == awa.DataType.VECTOR:
                     vec_data = awa.FloatVec()
                     ret = field.GetVecData(vec_data)
                     if vec_data.__len__() == 0:
                         print("Get vector data error!")
                         break
 
                     vec_result = []
                     vec_index = 0
                     while vec_index < vec_data.__len__():
                         each_vec_data = vec_data[vec_index]
-                    #for each_vec_data in vec_data:
+                        # for each_vec_data in vec_data:
                         vec_result.append(each_vec_data)
                         vec_index = vec_index + 1
                     doc_detail[field.name] = vec_result
                 field_index = field_index + 1
 
             docs_detail.append(doc_detail)
         return docs_detail
 
-    def EmbedQuery(
-        self,
-        text: str,
-        **kwargs: Any,
-    ):
-        #print('enter EmbedQuery....') 
-        #texts = []
-        #texts.append(text)
-        if self.llm is None: 
-            from awadb import llm_embedding
-            self.llm = llm_embedding.LLMEmbedding()
-        #print(text) 
-        return self.llm.Embedding(text)
-
-        #embeddings = self.llm.EmbeddingQuery(text)
-        #print(embeddings)
-        #return embeddings
-
     def __TextPreprocess(
         self,
         text: str,
         **kwargs: Any,
     ) -> Dict[str, int]:
         words = text.split()  # now just support english
         words_count_dict: Dict[str, int] = {}
@@ -684,17 +712,15 @@
         field_no = 0
         for field in doc:
             if (not self.tables_fields_check[self.using_table_name]) and type(
                 field
             ).__name__ == "dict":
                 for key in field:
                     if key == "embedding_text":
-                        from awadb import llm_embedding
-
-                        self.llm = llm_embedding.LLMEmbedding()
+                        self.llm = AwaEmbedding(self.model_name)
 
                         doc.append(self.llm.Embedding(field[key]))
                         self.tables_embedding_text_fid_no[
                             self.using_table_name
                         ] = field_no
             else:
                 if (
@@ -732,18 +758,17 @@
             self.tables_attr[self.using_table_name] = awa.TableInfo()
             self.tables_attr[self.using_table_name].SetName(self.using_table_name)
 
         if is_duplicate_texts is not None:
             self.is_duplicate_texts = is_duplicate_texts
 
         if embeddings is None:
-            if self.llm is None:
-                from awadb import llm_embedding
-
-                self.llm = llm_embedding.LLMEmbedding()
+            if self.llm is None:                
+                # Set llm
+                self.llm = AwaEmbedding(self.model_name)
             embeddings = self.llm.EmbeddingBatch(texts)
 
         awa_docs = awa.DocsVec()
         words_in_docs = awa.WordsCount()
 
         adding_docs_no = 0
         for text in texts:
@@ -1073,29 +1098,29 @@
         for field_name in self.tables_fields_names[self.using_table_name]:
             if field_name == "_id" or (
                 not_include_fields is not None and field_name in not_include_fields
             ):
                 continue
 
             fvec_names.append(field_name)
- 
+
         ret = awa.DoSearch(self.using_table_engine, req, response)
         response.PackResults(fvec_names)
 
         search_result_vec = response.Results()
-        search_result_index = 0 
+        search_result_index = 0
         while search_result_index < search_result_vec.__len__():
             search_result = search_result_vec[search_result_index]
             result_per_request = {}
             result_per_request["ResultSize"] = search_result.result_items.__len__()
 
             result_items_list = []
             items = search_result.result_items
-            item_index = 0 
-            #for item in items:
+            item_index = 0
+            # for item in items:
             while item_index < items.__len__():
                 item = items[item_index]
                 i = 0
                 l = item.names.__len__()
                 item_detail = {}
                 while i < l:
                     name = item.names[i]
```

## awadb/llm_embedding/__init__.py

```diff
@@ -4,15 +4,15 @@
 from sentence_transformers import SentenceTransformer
 from transformers import AutoModel
 from transformers import AutoTokenizer
 from typing import Iterable, Any, List
 
 class LLMEmbedding:
     def __init__(self):
-        self.model = SentenceTransformer('all-MiniLM-L6-v2')
+        self.model = SentenceTransformer('all-mpnet-base-v2')
         self.tokenizer = None 
 
 
     def Embedding(self, sentence):
         tokens = []
         if self.tokenizer != None:
             tokens = self.tokenizer.tokenize(sentence)
```

## Comparing `awadb-0.3.8.dist-info/LICENSE` & `awadb-0.3.9.dist-info/LICENSE`

 * *Files identical despite different names*

