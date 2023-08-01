# Comparing `tmp/agent_protocol-0.1.1.tar.gz` & `tmp/agent_protocol-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent_protocol-0.1.1.tar", max compression
+gzip compressed data, was "agent_protocol-0.1.2.tar", max compression
```

## Comparing `agent_protocol-0.1.1.tar` & `agent_protocol-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,13 @@
--rw-r--r--   0        0        0     2078 2023-07-23 11:51:55.219507 agent_protocol-0.1.1/README.md
--rw-r--r--   0        0        0       76 2023-07-23 11:51:55.219507 agent_protocol-0.1.1/agent_protocol/__init__.py
--rw-r--r--   0        0        0     4008 2023-07-23 11:51:55.219507 agent_protocol-0.1.1/agent_protocol/agent.py
--rw-r--r--   0        0        0      202 2023-07-23 11:51:55.219507 agent_protocol-0.1.1/agent_protocol/dependencies.py
--rw-r--r--   0        0        0     1683 2023-07-23 11:51:55.219507 agent_protocol-0.1.1/agent_protocol/models.py
--rw-r--r--   0        0        0      329 2023-07-23 11:51:55.219507 agent_protocol-0.1.1/agent_protocol/server.py
--rw-r--r--   0        0        0      692 2023-07-23 11:51:55.223507 agent_protocol-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2908 1970-01-01 00:00:00.000000 agent_protocol-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2398 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/README.md
+-rw-r--r--   0        0        0       76 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/agent_protocol/__init__.py
+-rw-r--r--   0        0        0     4007 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/agent_protocol/agent.py
+-rw-r--r--   0        0        0      600 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/agent_protocol/cli.py
+-rw-r--r--   0        0        0      202 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/agent_protocol/dependencies.py
+-rw-r--r--   0        0        0     1683 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/agent_protocol/models.py
+-rw-r--r--   0        0        0      329 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/agent_protocol/server.py
+-rw-r--r--   0        0        0        0 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/agent_protocol/utils/__init__.py
+-rw-r--r--   0        0        0       35 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/agent_protocol/utils/compliance/__init__.py
+-rw-r--r--   0        0        0      449 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/agent_protocol/utils/compliance/conftest.py
+-rw-r--r--   0        0        0     3426 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/agent_protocol/utils/compliance/main.py
+-rw-r--r--   0        0        0      804 2023-08-01 15:10:22.894513 agent_protocol-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3404 1970-01-01 00:00:00.000000 agent_protocol-0.1.2/PKG-INFO
```

### Comparing `agent_protocol-0.1.1/README.md` & `agent_protocol-0.1.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,101 @@
 # Agent Communication Protocol - Python SDK
 
 This SDK implements the Agent Communication Protocol in Python and allows you to easily wrap your agent in a webserver compatible with the protocol - you only need to define an agent task handler.
 
-
 ## Installation
+
 ```sh
 pip install agent-protocol
 ```
 
 Then add the following code to your agent:
+
 ```python
 from agent_protocol import (
     Agent,
     StepResult,
     StepHandler,
 )
 
 async def task_handler(task_input) -> StepHandler:
     # TODO: Initialize code for the agent task.
     async def step_handler(step_input) -> StepResult:
         # TODO: Execute code for the agent step.
         # The step could for example be a single iteration of a ReAct loop.
-        
+
         # TODO: Return the result of the step.
         return StepResult(
             output=...,
         )
 
     return step_handler
 
 if __name__ == "__main__":
     # Add the task handler and start the server
     Agent.handle_task(task_handler).start()
 ```
 
-
 ## Usage
+
 To start the server run the file where you added the code above:
+
 ```sh
 python file/where/you/added/code.py
 ```
 
 and then you can call the API using the following terminal commands:
 
 To **create a task** run:
+
 ```sh
 curl --request POST \
   --url http://localhost:8000/agent/tasks \
   --header 'Content-Type: application/json' \
   --data '{
 	"input": "task-input-to-your-agent"
 }'
 ```
 
 You will get a response like this:
+
 ```json
-{"input":"task-input-to-your-agent","task_id":"e6d768bb-4c50-4007-9853-aeffb46c77be","artifacts":[]}
+{
+  "input": "task-input-to-your-agent",
+  "task_id": "e6d768bb-4c50-4007-9853-aeffb46c77be",
+  "artifacts": []
+}
 ```
 
 Then to **execute one step of the task** copy the `task_id` you got from the previous request and run:
 
 ```sh
 curl --request POST \
   --url http://localhost:8000/agent/tasks/<task-id>/steps
 ```
 
 To get response like this:
+
 ```json
 {
-	"output":"output-from-the-agent",
-	"artifacts":[],"is_last":false,
-	"input":null,
-	"task_id":"e6d768bb-4c50-4007-9853-aeffb46c77be",
-	"step_id":"8ff8ba39-2c3e-4246-8086-fbd2a897240b"
+  "output": "output-from-the-agent",
+  "artifacts": [],
+  "is_last": false,
+  "input": null,
+  "task_id": "e6d768bb-4c50-4007-9853-aeffb46c77be",
+  "step_id": "8ff8ba39-2c3e-4246-8086-fbd2a897240b"
 }
 ```
 
+## Test compliance
+Part of the package is also a test suite that can be used to test compliance with the protocol. To run the tests, run the following command:
+
+```sh
+agent-protocol test --url <url>
+```
+
+In the background it uses pytest, you can pass any pytest arguments to the command above.
+
 ## Examples
+
 - [Smol Developer integration](./examples/smol_developer.py)
 - [Beebot integration](https://github.com/AutoPackAI/beebot/pull/3)
```

### Comparing `agent_protocol-0.1.1/agent_protocol/agent.py` & `agent_protocol-0.1.2/agent_protocol/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         artifacts=[],
     )
     tasks.append((task, step_handler))
     return task
 
 
 @app.get("/agent/tasks", response_model=List[str], tags=["agent", "tasks"])
-async def list_agent_tasks_i_ds() -> List[str]:
+async def list_agent_tasks_ids() -> List[str]:
     """
     List all tasks that have been created for the agent.
     """
     return [t[0].task_id for t in tasks]
 
 
 @app.get("/agent/tasks/{task_id}", response_model=Task, tags=["agent", "tasks"])
```

### Comparing `agent_protocol-0.1.1/agent_protocol/models.py` & `agent_protocol-0.1.2/agent_protocol/models.py`

 * *Files identical despite different names*

### Comparing `agent_protocol-0.1.1/PKG-INFO` & `agent_protocol-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,104 +1,128 @@
 Metadata-Version: 2.1
 Name: agent-protocol
-Version: 0.1.1
+Version: 0.1.2
 Summary: API for interacting with Agent
 Home-page: https://e2b.dev/
 License: MIT
 Author: e2b
 Author-email: hello@e2b.dev
 Requires-Python: >=3.7,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.6,<9.0.0)
 Requires-Dist: fastapi (>=0.100.0,<0.101.0)
 Requires-Dist: hypercorn (>=0.14.4,<0.15.0)
-Project-URL: Bug Tracker, https://github.com/e2b/sdk/issues
+Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Requires-Dist: pytest (>=7.4.0,<8.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Project-URL: Bug Tracker, https://github.com/e2b-dev/agent-protocol/issues
 Project-URL: Repository, https://github.com/e2b-dev/sdk/tree/main/agent/python/
 Description-Content-Type: text/markdown
 
 # Agent Communication Protocol - Python SDK
 
 This SDK implements the Agent Communication Protocol in Python and allows you to easily wrap your agent in a webserver compatible with the protocol - you only need to define an agent task handler.
 
-
 ## Installation
+
 ```sh
 pip install agent-protocol
 ```
 
 Then add the following code to your agent:
+
 ```python
 from agent_protocol import (
     Agent,
     StepResult,
     StepHandler,
 )
 
 async def task_handler(task_input) -> StepHandler:
     # TODO: Initialize code for the agent task.
     async def step_handler(step_input) -> StepResult:
         # TODO: Execute code for the agent step.
         # The step could for example be a single iteration of a ReAct loop.
-        
+
         # TODO: Return the result of the step.
         return StepResult(
             output=...,
         )
 
     return step_handler
 
 if __name__ == "__main__":
     # Add the task handler and start the server
     Agent.handle_task(task_handler).start()
 ```
 
-
 ## Usage
+
 To start the server run the file where you added the code above:
+
 ```sh
 python file/where/you/added/code.py
 ```
 
 and then you can call the API using the following terminal commands:
 
 To **create a task** run:
+
 ```sh
 curl --request POST \
   --url http://localhost:8000/agent/tasks \
   --header 'Content-Type: application/json' \
   --data '{
 	"input": "task-input-to-your-agent"
 }'
 ```
 
 You will get a response like this:
+
 ```json
-{"input":"task-input-to-your-agent","task_id":"e6d768bb-4c50-4007-9853-aeffb46c77be","artifacts":[]}
+{
+  "input": "task-input-to-your-agent",
+  "task_id": "e6d768bb-4c50-4007-9853-aeffb46c77be",
+  "artifacts": []
+}
 ```
 
 Then to **execute one step of the task** copy the `task_id` you got from the previous request and run:
 
 ```sh
 curl --request POST \
   --url http://localhost:8000/agent/tasks/<task-id>/steps
 ```
 
 To get response like this:
+
 ```json
 {
-	"output":"output-from-the-agent",
-	"artifacts":[],"is_last":false,
-	"input":null,
-	"task_id":"e6d768bb-4c50-4007-9853-aeffb46c77be",
-	"step_id":"8ff8ba39-2c3e-4246-8086-fbd2a897240b"
+  "output": "output-from-the-agent",
+  "artifacts": [],
+  "is_last": false,
+  "input": null,
+  "task_id": "e6d768bb-4c50-4007-9853-aeffb46c77be",
+  "step_id": "8ff8ba39-2c3e-4246-8086-fbd2a897240b"
 }
 ```
 
+## Test compliance
+Part of the package is also a test suite that can be used to test compliance with the protocol. To run the tests, run the following command:
+
+```sh
+agent-protocol test --url <url>
+```
+
+In the background it uses pytest, you can pass any pytest arguments to the command above.
+
 ## Examples
+
 - [Smol Developer integration](./examples/smol_developer.py)
 - [Beebot integration](https://github.com/AutoPackAI/beebot/pull/3)
```

