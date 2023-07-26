# Comparing `tmp/velikafkaclient-1.0.9.tar.gz` & `tmp/velikafkaclient-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velikafkaclient-1.0.9.tar", last modified: Mon Jul 17 15:50:16 2023, max compression
+gzip compressed data, was "velikafkaclient-1.1.0.tar", last modified: Wed Jul 26 15:14:32 2023, max compression
```

## Comparing `velikafkaclient-1.0.9.tar` & `velikafkaclient-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:50:16.325369 velikafkaclient-1.0.9/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-07-05 09:25:18.000000 velikafkaclient-1.0.9/MANIFEST.in
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2973 2023-07-17 15:50:16.325235 velikafkaclient-1.0.9/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2787 2023-07-17 15:45:52.000000 velikafkaclient-1.0.9/readme.md
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-17 15:50:16.325408 velikafkaclient-1.0.9/setup.cfg
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      398 2023-07-17 15:50:07.000000 velikafkaclient-1.0.9/setup.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:50:16.322889 velikafkaclient-1.0.9/velikafkaclient/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      116 2023-07-05 09:25:18.000000 velikafkaclient-1.0.9/velikafkaclient/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2145 2023-07-12 05:57:42.000000 velikafkaclient-1.0.9/velikafkaclient/consumer.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      725 2023-07-12 11:24:44.000000 velikafkaclient-1.0.9/velikafkaclient/decorators.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3489 2023-07-05 09:25:18.000000 velikafkaclient-1.0.9/velikafkaclient/eventregistration.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:50:16.324483 velikafkaclient-1.0.9/velikafkaclient/events/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.9/velikafkaclient/events/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      165 2023-07-12 08:29:23.000000 velikafkaclient-1.0.9/velikafkaclient/events/base.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1923 2023-07-05 09:25:18.000000 velikafkaclient-1.0.9/velikafkaclient/events/triptracker.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      160 2023-07-05 09:25:18.000000 velikafkaclient-1.0.9/velikafkaclient/exceptions.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      392 2023-07-12 05:57:42.000000 velikafkaclient-1.0.9/velikafkaclient/killer.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1260 2023-07-11 11:27:00.000000 velikafkaclient-1.0.9/velikafkaclient/producer.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1243 2023-07-17 15:49:44.000000 velikafkaclient-1.0.9/velikafkaclient/topicmanager.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:50:16.324992 velikafkaclient-1.0.9/velikafkaclient/topics/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.9/velikafkaclient/topics/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-07-05 09:25:18.000000 velikafkaclient-1.0.9/velikafkaclient/topics/topics.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1124 2023-07-05 09:25:18.000000 velikafkaclient-1.0.9/velikafkaclient/topics/triptracker.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:50:16.323547 velikafkaclient-1.0.9/velikafkaclient.egg-info/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2973 2023-07-17 15:50:16.000000 velikafkaclient-1.0.9/velikafkaclient.egg-info/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      635 2023-07-17 15:50:16.000000 velikafkaclient-1.0.9/velikafkaclient.egg-info/SOURCES.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-17 15:50:16.000000 velikafkaclient-1.0.9/velikafkaclient.egg-info/dependency_links.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       16 2023-07-17 15:50:16.000000 velikafkaclient-1.0.9/velikafkaclient.egg-info/top_level.txt
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-26 15:14:32.491444 velikafkaclient-1.1.0/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-07-05 09:25:18.000000 velikafkaclient-1.1.0/MANIFEST.in
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2973 2023-07-26 15:14:32.491282 velikafkaclient-1.1.0/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2787 2023-07-17 15:51:48.000000 velikafkaclient-1.1.0/readme.md
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-26 15:14:32.491498 velikafkaclient-1.1.0/setup.cfg
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      398 2023-07-26 15:14:15.000000 velikafkaclient-1.1.0/setup.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-26 15:14:32.489203 velikafkaclient-1.1.0/velikafkaclient/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      116 2023-07-05 09:25:18.000000 velikafkaclient-1.1.0/velikafkaclient/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2145 2023-07-12 05:57:42.000000 velikafkaclient-1.1.0/velikafkaclient/consumer.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      725 2023-07-12 11:24:44.000000 velikafkaclient-1.1.0/velikafkaclient/decorators.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3489 2023-07-05 09:25:18.000000 velikafkaclient-1.1.0/velikafkaclient/eventregistration.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-26 15:14:32.490600 velikafkaclient-1.1.0/velikafkaclient/events/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.1.0/velikafkaclient/events/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      165 2023-07-12 08:29:23.000000 velikafkaclient-1.1.0/velikafkaclient/events/base.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1923 2023-07-05 09:25:18.000000 velikafkaclient-1.1.0/velikafkaclient/events/triptracker.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      160 2023-07-05 09:25:18.000000 velikafkaclient-1.1.0/velikafkaclient/exceptions.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      392 2023-07-12 05:57:42.000000 velikafkaclient-1.1.0/velikafkaclient/killer.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2343 2023-07-26 15:13:52.000000 velikafkaclient-1.1.0/velikafkaclient/producer.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1243 2023-07-17 15:51:48.000000 velikafkaclient-1.1.0/velikafkaclient/topicmanager.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-26 15:14:32.491061 velikafkaclient-1.1.0/velikafkaclient/topics/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.1.0/velikafkaclient/topics/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-07-05 09:25:18.000000 velikafkaclient-1.1.0/velikafkaclient/topics/topics.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1124 2023-07-05 09:25:18.000000 velikafkaclient-1.1.0/velikafkaclient/topics/triptracker.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-26 15:14:32.489919 velikafkaclient-1.1.0/velikafkaclient.egg-info/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2973 2023-07-26 15:14:32.000000 velikafkaclient-1.1.0/velikafkaclient.egg-info/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      635 2023-07-26 15:14:32.000000 velikafkaclient-1.1.0/velikafkaclient.egg-info/SOURCES.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-26 15:14:32.000000 velikafkaclient-1.1.0/velikafkaclient.egg-info/dependency_links.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       16 2023-07-26 15:14:32.000000 velikafkaclient-1.1.0/velikafkaclient.egg-info/top_level.txt
```

### Comparing `velikafkaclient-1.0.9/PKG-INFO` & `velikafkaclient-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velikafkaclient
-Version: 1.0.9
+Version: 1.1.0
 Summary: Veli Kafka Client
 Author: Konstantine
 Author-email: kdvalishvili@veli.store
 Description-Content-Type: text/markdown
 
 ### Kafka Client for VELI.STORE
```

### Comparing `velikafkaclient-1.0.9/readme.md` & `velikafkaclient-1.1.0/readme.md`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.9/velikafkaclient/consumer.py` & `velikafkaclient-1.1.0/velikafkaclient/consumer.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.9/velikafkaclient/decorators.py` & `velikafkaclient-1.1.0/velikafkaclient/decorators.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.9/velikafkaclient/eventregistration.py` & `velikafkaclient-1.1.0/velikafkaclient/eventregistration.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.9/velikafkaclient/events/triptracker.py` & `velikafkaclient-1.1.0/velikafkaclient/events/triptracker.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.9/velikafkaclient/producer.py` & `velikafkaclient-1.1.0/velikafkaclient/producer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import json
 
 from aiokafka import AIOKafkaProducer
+from confluent_kafka import Producer
 
 from .eventregistration import kafka_topic_events
 from .exceptions import InvalidEventTopicException, InvalidEventModelForTopic
 from .topics.topics import KafkaTopic
 from .events.base import KafkaEvent
 from velilogger import get_tracing_id
 
+
 class AsyncKafkaEventProducer:
 
     def __init__(self, bootstrap_servers):
         self.kafka_topic_events = kafka_topic_events
         self.producer = AIOKafkaProducer(
             bootstrap_servers=bootstrap_servers
         )
@@ -27,7 +29,29 @@
         if topic not in self.kafka_topic_events.topic_event_models:
             raise InvalidEventTopicException(f"Topic {topic} not found")
         topic_event_model = self.kafka_topic_events.topic_event_models[topic]
         if not isinstance(event, topic_event_model):
             raise InvalidEventModelForTopic(f"event: {str(event)} topic model: {str(topic_event_model)}")
         event.tracing_id = get_tracing_id()
         await self.producer.send(topic.value, json.dumps(event.dict()).encode())
+
+    async def produce_easy_event(self, topic_name, event_data):
+        await self.producer.send(topic_name, json.dumps(event_data).encode())
+
+
+class KafkaEventProducer:
+
+    def __init__(self, bootstrap_servers):
+        self.kafka_topic_events = kafka_topic_events
+        self.producer = Producer({'bootstrap.servers': bootstrap_servers})
+
+    def produce_event(self, topic: KafkaTopic, event: KafkaEvent):
+        if topic not in self.kafka_topic_events.topic_event_models:
+            raise InvalidEventTopicException(f"Topic {topic} not found")
+        topic_event_model = self.kafka_topic_events.topic_event_models[topic]
+        if not isinstance(event, topic_event_model):
+            raise InvalidEventModelForTopic(f"event: {str(event)} topic model: {str(topic_event_model)}")
+        event.tracing_id = get_tracing_id()
+        self.producer.produce(topic.value, json.dumps(event.dict()).encode())
+
+    def produce_easy_event(self, topic_name, event_data):
+        self.producer.produce(topic_name, json.dumps(event_data).encode())
```

### Comparing `velikafkaclient-1.0.9/velikafkaclient/topicmanager.py` & `velikafkaclient-1.1.0/velikafkaclient/topicmanager.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.9/velikafkaclient/topics/triptracker.py` & `velikafkaclient-1.1.0/velikafkaclient/topics/triptracker.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.9/velikafkaclient.egg-info/PKG-INFO` & `velikafkaclient-1.1.0/velikafkaclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velikafkaclient
-Version: 1.0.9
+Version: 1.1.0
 Summary: Veli Kafka Client
 Author: Konstantine
 Author-email: kdvalishvili@veli.store
 Description-Content-Type: text/markdown
 
 ### Kafka Client for VELI.STORE
```

### Comparing `velikafkaclient-1.0.9/velikafkaclient.egg-info/SOURCES.txt` & `velikafkaclient-1.1.0/velikafkaclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

