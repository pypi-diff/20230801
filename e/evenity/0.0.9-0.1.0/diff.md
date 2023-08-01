# Comparing `tmp/evenity-0.0.9.tar.gz` & `tmp/evenity-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evenity-0.0.9.tar", last modified: Mon Jul 31 22:11:33 2023, max compression
+gzip compressed data, was "evenity-0.1.0.tar", last modified: Tue Aug  1 00:13:56 2023, max compression
```

## Comparing `evenity-0.0.9.tar` & `evenity-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-31 22:11:33.722782 evenity-0.0.9/
--rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 21:02:20.000000 evenity-0.0.9/LICENSE
--rw-r--r--   0 localghost  (1000) localghost  (1000)     7703 2023-07-31 22:11:33.722782 evenity-0.0.9/PKG-INFO
--rw-r--r--   0 localghost  (1000) localghost  (1000)     7248 2023-07-31 21:11:07.000000 evenity-0.0.9/README.md
--rw-r--r--   0 localghost  (1000) localghost  (1000)      532 2023-07-31 22:11:24.000000 evenity-0.0.9/pyproject.toml
--rw-r--r--   0 localghost  (1000) localghost  (1000)       38 2023-07-31 22:11:33.722782 evenity-0.0.9/setup.cfg
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-31 22:11:33.719449 evenity-0.0.9/src/
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-31 22:11:33.719449 evenity-0.0.9/src/evenity/
--rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:22:35.000000 evenity-0.0.9/src/evenity/__init__.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      528 2023-07-31 22:09:35.000000 evenity-0.0.9/src/evenity/observable.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      919 2023-07-31 22:09:35.000000 evenity-0.0.9/src/evenity/observer.py
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-31 22:11:33.722782 evenity-0.0.9/src/evenity/plugins/
--rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:22:35.000000 evenity-0.0.9/src/evenity/plugins/__init__.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)     1451 2023-07-31 21:11:07.000000 evenity-0.0.9/src/evenity/plugins/ftp.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      714 2023-07-28 23:22:35.000000 evenity-0.0.9/src/evenity/plugins/kafka.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      632 2023-07-28 23:22:35.000000 evenity-0.0.9/src/evenity/plugins/shell.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      742 2023-07-31 21:11:07.000000 evenity-0.0.9/src/evenity/plugins/telegram.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)     1741 2023-07-30 17:27:26.000000 evenity-0.0.9/src/evenity/plugins/websocket.py
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-31 22:11:33.719449 evenity-0.0.9/src/evenity.egg-info/
--rw-r--r--   0 localghost  (1000) localghost  (1000)     7703 2023-07-31 22:11:33.000000 evenity-0.0.9/src/evenity.egg-info/PKG-INFO
--rw-r--r--   0 localghost  (1000) localghost  (1000)      449 2023-07-31 22:11:33.000000 evenity-0.0.9/src/evenity.egg-info/SOURCES.txt
--rw-r--r--   0 localghost  (1000) localghost  (1000)        1 2023-07-31 22:11:33.000000 evenity-0.0.9/src/evenity.egg-info/dependency_links.txt
--rw-r--r--   0 localghost  (1000) localghost  (1000)        8 2023-07-31 22:11:33.000000 evenity-0.0.9/src/evenity.egg-info/top_level.txt
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-31 22:11:33.722782 evenity-0.0.9/tests/
--rw-r--r--   0 localghost  (1000) localghost  (1000)     1105 2023-07-31 21:38:27.000000 evenity-0.0.9/tests/test_simple.py
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-08-01 00:13:56.809421 evenity-0.1.0/
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 21:02:20.000000 evenity-0.1.0/LICENSE
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     8566 2023-08-01 00:13:56.809421 evenity-0.1.0/PKG-INFO
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     8111 2023-08-01 00:13:38.000000 evenity-0.1.0/README.md
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      532 2023-08-01 00:13:38.000000 evenity-0.1.0/pyproject.toml
+-rw-r--r--   0 localghost  (1000) localghost  (1000)       38 2023-08-01 00:13:56.809421 evenity-0.1.0/setup.cfg
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-08-01 00:13:56.806088 evenity-0.1.0/src/
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-08-01 00:13:56.806088 evenity-0.1.0/src/evenity/
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:22:35.000000 evenity-0.1.0/src/evenity/__init__.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      598 2023-08-01 00:13:38.000000 evenity-0.1.0/src/evenity/observable.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      845 2023-08-01 00:13:38.000000 evenity-0.1.0/src/evenity/observer.py
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-08-01 00:13:56.806088 evenity-0.1.0/src/evenity/plugins/
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:22:35.000000 evenity-0.1.0/src/evenity/plugins/__init__.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     1451 2023-07-31 21:11:07.000000 evenity-0.1.0/src/evenity/plugins/ftp.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      714 2023-07-28 23:22:35.000000 evenity-0.1.0/src/evenity/plugins/kafka.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      632 2023-07-28 23:22:35.000000 evenity-0.1.0/src/evenity/plugins/shell.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      742 2023-07-31 21:11:07.000000 evenity-0.1.0/src/evenity/plugins/telegram.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     1741 2023-07-30 17:27:26.000000 evenity-0.1.0/src/evenity/plugins/websocket.py
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-08-01 00:13:56.806088 evenity-0.1.0/src/evenity.egg-info/
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     8566 2023-08-01 00:13:56.000000 evenity-0.1.0/src/evenity.egg-info/PKG-INFO
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      487 2023-08-01 00:13:56.000000 evenity-0.1.0/src/evenity.egg-info/SOURCES.txt
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        1 2023-08-01 00:13:56.000000 evenity-0.1.0/src/evenity.egg-info/dependency_links.txt
+-rw-r--r--   0 localghost  (1000) localghost  (1000)       13 2023-08-01 00:13:56.000000 evenity-0.1.0/src/evenity.egg-info/top_level.txt
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      963 2023-08-01 00:13:38.000000 evenity-0.1.0/src/main.py
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-08-01 00:13:56.809421 evenity-0.1.0/tests/
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     1149 2023-08-01 00:13:38.000000 evenity-0.1.0/tests/test_memory_leak.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     1136 2023-08-01 00:13:38.000000 evenity-0.1.0/tests/test_simple.py
```

### Comparing `evenity-0.0.9/PKG-INFO` & `evenity-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evenity
-Version: 0.0.9
+Version: 0.1.0
 Summary: Pluggable event hooks library
 Author-email: Mario Baldi <mariobaldi.py@gmail.com>
 Project-URL: Homepage, https://github.com/baldimario/evenity
 Project-URL: Bug Tracker, https://github.com/baldimario/evenity/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
@@ -14,14 +14,22 @@
 # Evenity - Pluggable event hook libary
 
 ## Installation
 ```sh
 pip install evenity
 ```
 
+## Important Notes!
+Observables tracks observers with a weakref, if the reference to the observable is lost the observer automatically does not track the object anymore.
+So keep track of the observers in a variable to keep them receive observable events.
+It could've happened that when you delete an observer, the observable keeping track of the object made the garbage collector not delete it since it still kept its reference. In this case the observer continued to handle the events.
+Currently, however, the reference is maintained through a weakref which is why you need to be careful to keep the observer in a variable otherwise if you lose track of it, the observable will lose track of it and it will die.
+This is a safety measure to avoid memory leaks.
+(Thanks [krow89](https://github.com/krow89))
+
 ## Usage
 See examples folder at [https://github.com/baldimario/evenity](https://github.com/baldimario/evenity)
 
 ```python
 """Example"""
 from evenity.observable import Observable
 from evenity.observer import Observer
@@ -43,23 +51,23 @@
         super().__init__(observable)
         self.listen("test", self.on_test)
         self.listen("foo", self.on_test)
 
     def on_test(self, event):
         """On test event"""
         print(f"1 {event}")
-    
+
     def on_foo(self, event):
         """On test event"""
         print(f"2 {event}")
 
 def main():
     dispatcher = EventDispatcher()
 
-    EventListener(dispatcher)
+    listener = EventListener(dispatcher)
 
     # Simulate dispatching of some events
     events = [
         ["test", "Hello World!"],
         ["foo", "Foo Bar!"],
     ]
 
@@ -69,15 +77,15 @@
 if __name__ == '__main__':
     main()
 
 # 1 Hello World!
 # 2 Foo Bar!
 ```
 
-### simple.py 
+### simple.py
 This file contains an implementation of observers and observable
 It shows how simple is to implement your own observable and register all the observers as you want
 
 ## kafka.py
 This script contains an implementations of some listeners (observers) for the kafka plugin
 
 This subscribe some listeners for the KafkaObservableConsumer listening for events from many topics
@@ -109,15 +117,15 @@
     group="mygroup",
     topics=[
         "topic1",
         "topic2"
     ]
 )
 
-Listener(consumer)
+listener = Listener(consumer)
 
 consumer.consume()
 ```
 
 ## ftp.py 
 ftp.py contains an example listener for the ftp observable
 
@@ -146,15 +154,15 @@
     password=os.environ.get('FTP_PASSWORD'),
     port=os.environ.get('FTP_PORT'),
     path=os.path.join(ABSPATH, os.environ.get('FTP_PATH')),
     host=os.environ.get('FTP_BIND_ADDRESS'),
     on_file_received_event='ftp'
 )
 
-Listener(consumer)
+listener = Listener(consumer)
 
 consumer.consume()
 ```
 
 ## shell.py
 This file contains an example listener for the shell observable
 
@@ -174,15 +182,15 @@
         self.listen('monitor-sensor --accel', self.fetch)
 
     def fetch(self, line):
         """Update method"""
         print(line)
 
 observable = ShellObservableConsumer('monitor-sensor --accel')
-Listener(observable)
+listener = Listener(observable)
 observable.consume()
 ```
 
 ## telegram.py
 This script contains an example listener for telegram bot events (updates, texts and commands)
 
 The observers will be notified for each telegram bot event
@@ -194,15 +202,15 @@
 from evenity.observer import Observer
 from evenity.plugins.telegram import AsyncTelegramaObservableConsumer
 
 class Listener(Observer):
     def __init__(self, observable):
         super().__init__(observable)
         self.listen("telegram", self.on_telegram)
-    
+
     def on_telegram(self, message):
         if 'chat' in message:
             user = message['username']
             chat_id = message['chat']['id']
             text = message['text']
             self.observable.bot.sendMessage(
                 chat_id,
@@ -210,15 +218,15 @@
             )
 
 consumer = AsyncTelegramaObservableConsumer(
     token=os.environ.get('TOKEN'),
     on_message_received_event='telegram'
 )
 
-Listener(consumer)
+listener = Listener(consumer)
 
 consumer.consume()
 
 while True:
     time.sleep(10)
 ```
 
@@ -231,34 +239,34 @@
 
 ```python
 from evenity.plugins.websocket import WebsocketObservable
 from evenity.observer import Observer
 
 class Listener(Observer):
     """Websocket listener."""
-    
+
     def __init__(self, observable):
         super().__init__(observable)
         self.listen("message", self.on_message)
         self.listen("close", self.on_close)
         self.listen("error", self.on_error)
         self.listen("open", self.on_open)
 
     def on_message(self, event):
         """Update websocket listener."""
         websocket = event['websocket']
         message = event['event']
         print(websocket, message)
-    
+
     def on_error(self, event):
         """Update websocket listener."""
         websocket = event['websocket']
         message = event['event']
         print(websocket, message)
-    
+
     def on_open(self, event):
         """Update websocket listener."""
         websocket = event['websocket']
         message = event['event']
         print(websocket, message)
 
     def on_close(self, event):
@@ -271,15 +279,15 @@
     "wss://localhost/foo",
     on_open_event='open',
     on_error_event='error',
     on_close_event='close',
     on_message_event='message'
 )
 
-Listener(consumer)
+listener = Listener(consumer)
 
 consumer.consume()
 ```
 
 ## SimpleObserver
 
 You can use the SimpleObserver to create observers without defining a new class but using callbacks instead
@@ -297,14 +305,14 @@
     ]
 )
 
 def on_topic1(event):
     """On test event"""
     print(event.decode('utf-8'))
 
-SimpleObserver(consumer, {
+listener = SimpleObserver(consumer, {
     'topic1': on_topic1,
     'topic2': lambda event: print(event.decode('utf-8'))
 })
 
 consumer.consume()
 ```
```

### Comparing `evenity-0.0.9/README.md` & `evenity-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # Evenity - Pluggable event hook libary
 
 ## Installation
 ```sh
 pip install evenity
 ```
 
+## Important Notes!
+Observables tracks observers with a weakref, if the reference to the observable is lost the observer automatically does not track the object anymore.
+So keep track of the observers in a variable to keep them receive observable events.
+It could've happened that when you delete an observer, the observable keeping track of the object made the garbage collector not delete it since it still kept its reference. In this case the observer continued to handle the events.
+Currently, however, the reference is maintained through a weakref which is why you need to be careful to keep the observer in a variable otherwise if you lose track of it, the observable will lose track of it and it will die.
+This is a safety measure to avoid memory leaks.
+(Thanks [krow89](https://github.com/krow89))
+
 ## Usage
 See examples folder at [https://github.com/baldimario/evenity](https://github.com/baldimario/evenity)
 
 ```python
 """Example"""
 from evenity.observable import Observable
 from evenity.observer import Observer
@@ -30,23 +38,23 @@
         super().__init__(observable)
         self.listen("test", self.on_test)
         self.listen("foo", self.on_test)
 
     def on_test(self, event):
         """On test event"""
         print(f"1 {event}")
-    
+
     def on_foo(self, event):
         """On test event"""
         print(f"2 {event}")
 
 def main():
     dispatcher = EventDispatcher()
 
-    EventListener(dispatcher)
+    listener = EventListener(dispatcher)
 
     # Simulate dispatching of some events
     events = [
         ["test", "Hello World!"],
         ["foo", "Foo Bar!"],
     ]
 
@@ -56,15 +64,15 @@
 if __name__ == '__main__':
     main()
 
 # 1 Hello World!
 # 2 Foo Bar!
 ```
 
-### simple.py 
+### simple.py
 This file contains an implementation of observers and observable
 It shows how simple is to implement your own observable and register all the observers as you want
 
 ## kafka.py
 This script contains an implementations of some listeners (observers) for the kafka plugin
 
 This subscribe some listeners for the KafkaObservableConsumer listening for events from many topics
@@ -96,15 +104,15 @@
     group="mygroup",
     topics=[
         "topic1",
         "topic2"
     ]
 )
 
-Listener(consumer)
+listener = Listener(consumer)
 
 consumer.consume()
 ```
 
 ## ftp.py 
 ftp.py contains an example listener for the ftp observable
 
@@ -133,15 +141,15 @@
     password=os.environ.get('FTP_PASSWORD'),
     port=os.environ.get('FTP_PORT'),
     path=os.path.join(ABSPATH, os.environ.get('FTP_PATH')),
     host=os.environ.get('FTP_BIND_ADDRESS'),
     on_file_received_event='ftp'
 )
 
-Listener(consumer)
+listener = Listener(consumer)
 
 consumer.consume()
 ```
 
 ## shell.py
 This file contains an example listener for the shell observable
 
@@ -161,15 +169,15 @@
         self.listen('monitor-sensor --accel', self.fetch)
 
     def fetch(self, line):
         """Update method"""
         print(line)
 
 observable = ShellObservableConsumer('monitor-sensor --accel')
-Listener(observable)
+listener = Listener(observable)
 observable.consume()
 ```
 
 ## telegram.py
 This script contains an example listener for telegram bot events (updates, texts and commands)
 
 The observers will be notified for each telegram bot event
@@ -181,15 +189,15 @@
 from evenity.observer import Observer
 from evenity.plugins.telegram import AsyncTelegramaObservableConsumer
 
 class Listener(Observer):
     def __init__(self, observable):
         super().__init__(observable)
         self.listen("telegram", self.on_telegram)
-    
+
     def on_telegram(self, message):
         if 'chat' in message:
             user = message['username']
             chat_id = message['chat']['id']
             text = message['text']
             self.observable.bot.sendMessage(
                 chat_id,
@@ -197,15 +205,15 @@
             )
 
 consumer = AsyncTelegramaObservableConsumer(
     token=os.environ.get('TOKEN'),
     on_message_received_event='telegram'
 )
 
-Listener(consumer)
+listener = Listener(consumer)
 
 consumer.consume()
 
 while True:
     time.sleep(10)
 ```
 
@@ -218,34 +226,34 @@
 
 ```python
 from evenity.plugins.websocket import WebsocketObservable
 from evenity.observer import Observer
 
 class Listener(Observer):
     """Websocket listener."""
-    
+
     def __init__(self, observable):
         super().__init__(observable)
         self.listen("message", self.on_message)
         self.listen("close", self.on_close)
         self.listen("error", self.on_error)
         self.listen("open", self.on_open)
 
     def on_message(self, event):
         """Update websocket listener."""
         websocket = event['websocket']
         message = event['event']
         print(websocket, message)
-    
+
     def on_error(self, event):
         """Update websocket listener."""
         websocket = event['websocket']
         message = event['event']
         print(websocket, message)
-    
+
     def on_open(self, event):
         """Update websocket listener."""
         websocket = event['websocket']
         message = event['event']
         print(websocket, message)
 
     def on_close(self, event):
@@ -258,15 +266,15 @@
     "wss://localhost/foo",
     on_open_event='open',
     on_error_event='error',
     on_close_event='close',
     on_message_event='message'
 )
 
-Listener(consumer)
+listener = Listener(consumer)
 
 consumer.consume()
 ```
 
 ## SimpleObserver
 
 You can use the SimpleObserver to create observers without defining a new class but using callbacks instead
@@ -284,14 +292,14 @@
     ]
 )
 
 def on_topic1(event):
     """On test event"""
     print(event.decode('utf-8'))
 
-SimpleObserver(consumer, {
+listener = SimpleObserver(consumer, {
     'topic1': on_topic1,
     'topic2': lambda event: print(event.decode('utf-8'))
 })
 
 consumer.consume()
 ```
```

### Comparing `evenity-0.0.9/pyproject.toml` & `evenity-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=42"]
 
 [project]
 name = "evenity"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Mario Baldi", email="mariobaldi.py@gmail.com" },
 ]
 description = "Pluggable event hooks library"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
```

### Comparing `evenity-0.0.9/src/evenity/observable.py` & `evenity-0.1.0/src/evenity/observable.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Ovservable class"""
+import weakref
 
 class Observable:
     """Observable class"""
 
     def __init__(self):
-        self._observers = []
+        self._observers = weakref.WeakValueDictionary()
 
     def register_observer(self, observer):
         """Register an observer"""
-        self._observers.append(observer)
-
-    def unregister_observer(self, observer):
-        """Unregister an observer"""
-        self._observers.remove(observer)
+        self._observers[id(observer)] = observer
 
     def notify_observers(self, listener, event):
         """Notify all observers"""
-        for obs in self._observers:
-            obs.notify(listener, event)
+        for oid in self._observers:
+            self._observers[oid].notify(listener, event)
+
+    def deregister_observer(self, observer):
+        """Deregister an observer"""
+        self._observers.remove(id(observer))
```

### Comparing `evenity-0.0.9/src/evenity/observer.py` & `evenity-0.1.0/src/evenity/observer.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,17 +17,14 @@
         if listener in self._listeners:
             self._listeners[listener](event)
 
     def listen(self, event, callback):
         """Listen to an event"""
         self._listeners[event] = callback
 
-    def __del__(self):
-        self.observable.unregister_observer(self)
-
 class SimpleObserver(Observer):
     """SimpleObserver class"""
 
     def __init__(self, observable, callback_lookup):
         super().__init__(observable)
         for event, callback in callback_lookup.items():
             self.listen(event, callback)
```

### Comparing `evenity-0.0.9/src/evenity/plugins/ftp.py` & `evenity-0.1.0/src/evenity/plugins/ftp.py`

 * *Files identical despite different names*

### Comparing `evenity-0.0.9/src/evenity/plugins/kafka.py` & `evenity-0.1.0/src/evenity/plugins/kafka.py`

 * *Files identical despite different names*

### Comparing `evenity-0.0.9/src/evenity/plugins/shell.py` & `evenity-0.1.0/src/evenity/plugins/shell.py`

 * *Files identical despite different names*

### Comparing `evenity-0.0.9/src/evenity/plugins/telegram.py` & `evenity-0.1.0/src/evenity/plugins/telegram.py`

 * *Files identical despite different names*

### Comparing `evenity-0.0.9/src/evenity/plugins/websocket.py` & `evenity-0.1.0/src/evenity/plugins/websocket.py`

 * *Files identical despite different names*

### Comparing `evenity-0.0.9/src/evenity.egg-info/PKG-INFO` & `evenity-0.1.0/src/evenity.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evenity
-Version: 0.0.9
+Version: 0.1.0
 Summary: Pluggable event hooks library
 Author-email: Mario Baldi <mariobaldi.py@gmail.com>
 Project-URL: Homepage, https://github.com/baldimario/evenity
 Project-URL: Bug Tracker, https://github.com/baldimario/evenity/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
@@ -14,14 +14,22 @@
 # Evenity - Pluggable event hook libary
 
 ## Installation
 ```sh
 pip install evenity
 ```
 
+## Important Notes!
+Observables tracks observers with a weakref, if the reference to the observable is lost the observer automatically does not track the object anymore.
+So keep track of the observers in a variable to keep them receive observable events.
+It could've happened that when you delete an observer, the observable keeping track of the object made the garbage collector not delete it since it still kept its reference. In this case the observer continued to handle the events.
+Currently, however, the reference is maintained through a weakref which is why you need to be careful to keep the observer in a variable otherwise if you lose track of it, the observable will lose track of it and it will die.
+This is a safety measure to avoid memory leaks.
+(Thanks [krow89](https://github.com/krow89))
+
 ## Usage
 See examples folder at [https://github.com/baldimario/evenity](https://github.com/baldimario/evenity)
 
 ```python
 """Example"""
 from evenity.observable import Observable
 from evenity.observer import Observer
@@ -43,23 +51,23 @@
         super().__init__(observable)
         self.listen("test", self.on_test)
         self.listen("foo", self.on_test)
 
     def on_test(self, event):
         """On test event"""
         print(f"1 {event}")
-    
+
     def on_foo(self, event):
         """On test event"""
         print(f"2 {event}")
 
 def main():
     dispatcher = EventDispatcher()
 
-    EventListener(dispatcher)
+    listener = EventListener(dispatcher)
 
     # Simulate dispatching of some events
     events = [
         ["test", "Hello World!"],
         ["foo", "Foo Bar!"],
     ]
 
@@ -69,15 +77,15 @@
 if __name__ == '__main__':
     main()
 
 # 1 Hello World!
 # 2 Foo Bar!
 ```
 
-### simple.py 
+### simple.py
 This file contains an implementation of observers and observable
 It shows how simple is to implement your own observable and register all the observers as you want
 
 ## kafka.py
 This script contains an implementations of some listeners (observers) for the kafka plugin
 
 This subscribe some listeners for the KafkaObservableConsumer listening for events from many topics
@@ -109,15 +117,15 @@
     group="mygroup",
     topics=[
         "topic1",
         "topic2"
     ]
 )
 
-Listener(consumer)
+listener = Listener(consumer)
 
 consumer.consume()
 ```
 
 ## ftp.py 
 ftp.py contains an example listener for the ftp observable
 
@@ -146,15 +154,15 @@
     password=os.environ.get('FTP_PASSWORD'),
     port=os.environ.get('FTP_PORT'),
     path=os.path.join(ABSPATH, os.environ.get('FTP_PATH')),
     host=os.environ.get('FTP_BIND_ADDRESS'),
     on_file_received_event='ftp'
 )
 
-Listener(consumer)
+listener = Listener(consumer)
 
 consumer.consume()
 ```
 
 ## shell.py
 This file contains an example listener for the shell observable
 
@@ -174,15 +182,15 @@
         self.listen('monitor-sensor --accel', self.fetch)
 
     def fetch(self, line):
         """Update method"""
         print(line)
 
 observable = ShellObservableConsumer('monitor-sensor --accel')
-Listener(observable)
+listener = Listener(observable)
 observable.consume()
 ```
 
 ## telegram.py
 This script contains an example listener for telegram bot events (updates, texts and commands)
 
 The observers will be notified for each telegram bot event
@@ -194,15 +202,15 @@
 from evenity.observer import Observer
 from evenity.plugins.telegram import AsyncTelegramaObservableConsumer
 
 class Listener(Observer):
     def __init__(self, observable):
         super().__init__(observable)
         self.listen("telegram", self.on_telegram)
-    
+
     def on_telegram(self, message):
         if 'chat' in message:
             user = message['username']
             chat_id = message['chat']['id']
             text = message['text']
             self.observable.bot.sendMessage(
                 chat_id,
@@ -210,15 +218,15 @@
             )
 
 consumer = AsyncTelegramaObservableConsumer(
     token=os.environ.get('TOKEN'),
     on_message_received_event='telegram'
 )
 
-Listener(consumer)
+listener = Listener(consumer)
 
 consumer.consume()
 
 while True:
     time.sleep(10)
 ```
 
@@ -231,34 +239,34 @@
 
 ```python
 from evenity.plugins.websocket import WebsocketObservable
 from evenity.observer import Observer
 
 class Listener(Observer):
     """Websocket listener."""
-    
+
     def __init__(self, observable):
         super().__init__(observable)
         self.listen("message", self.on_message)
         self.listen("close", self.on_close)
         self.listen("error", self.on_error)
         self.listen("open", self.on_open)
 
     def on_message(self, event):
         """Update websocket listener."""
         websocket = event['websocket']
         message = event['event']
         print(websocket, message)
-    
+
     def on_error(self, event):
         """Update websocket listener."""
         websocket = event['websocket']
         message = event['event']
         print(websocket, message)
-    
+
     def on_open(self, event):
         """Update websocket listener."""
         websocket = event['websocket']
         message = event['event']
         print(websocket, message)
 
     def on_close(self, event):
@@ -271,15 +279,15 @@
     "wss://localhost/foo",
     on_open_event='open',
     on_error_event='error',
     on_close_event='close',
     on_message_event='message'
 )
 
-Listener(consumer)
+listener = Listener(consumer)
 
 consumer.consume()
 ```
 
 ## SimpleObserver
 
 You can use the SimpleObserver to create observers without defining a new class but using callbacks instead
@@ -297,14 +305,14 @@
     ]
 )
 
 def on_topic1(event):
     """On test event"""
     print(event.decode('utf-8'))
 
-SimpleObserver(consumer, {
+listener = SimpleObserver(consumer, {
     'topic1': on_topic1,
     'topic2': lambda event: print(event.decode('utf-8'))
 })
 
 consumer.consume()
 ```
```

### Comparing `evenity-0.0.9/tests/test_simple.py` & `evenity-0.1.0/src/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-import unittest
+
 from evenity.observable import Observable
 from evenity.observer import Observer, SimpleObserver
 
 class EventDispatcher(Observable):
     """EventDispatcher class"""
 
     def __init__(self): # pylint: disable=useless-super-delegation
         super().__init__()
 
     def dispatch(self, topic, event):
         """Consume the observable"""
         self.notify_observers(topic, event)
 
-class TestSimple(unittest.TestCase):
+def main():
+    expected_events = [
+        "1 Hello World!",
+        "2 Foo Bar!",
+    ]
+    received_events = []
+
+    dispatcher = EventDispatcher()
+    observer = SimpleObserver(dispatcher, {
+        'test': lambda event: received_events.append("1 " + event),
+        'foo': lambda event: received_events.append("2 " + event)
+    })
+
+    events = [
+        ["test", "Hello World!"],
+        ["foo", "Foo Bar!"],
+    ]
 
-    def test_upper(self):
-        expected_events = [
-            "1 Hello World!",
-            "2 Foo Bar!",
-        ]
-        received_events = []
-
-        dispatcher = EventDispatcher()
-        SimpleObserver(dispatcher, {
-            'test': lambda event: received_events.append("1 " + event),
-            'foo': lambda event: received_events.append("2 " + event)
-        })
-
-        events = [
-            ["test", "Hello World!"],
-            ["foo", "Foo Bar!"],
-        ]
+    observer = None
 
-        for event in events:
-            dispatcher.dispatch(event[0], event[1])
+    for event in events:
+        dispatcher.dispatch(event[0], event[1])
 
-        self.assertEqual(expected_events, received_events)
+    print(received_events)
 
 if __name__ == '__main__':
-    unittest.main()
-
+    main()
```

