# Comparing `tmp/snitch-protos-0.0.47.tar.gz` & `tmp/snitch-protos-0.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snitch-protos-0.0.47.tar", last modified: Tue Jul 25 21:03:54 2023, max compression
+gzip compressed data, was "snitch-protos-0.0.48.tar", last modified: Wed Jul 26 20:59:58 2023, max compression
```

## Comparing `snitch-protos-0.0.47.tar` & `snitch-protos-0.0.48.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:03:54.743955 snitch-protos-0.0.47/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-25 21:03:54.743955 snitch-protos-0.0.47/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-25 21:03:00.000000 snitch-protos-0.0.47/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 21:03:54.743955 snitch-protos-0.0.47/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-25 21:03:52.000000 snitch-protos-0.0.47/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:03:54.743955 snitch-protos-0.0.47/snitch_protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:03:00.000000 snitch-protos-0.0.47/snitch_protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:03:54.743955 snitch-protos-0.0.47/snitch_protos/protos/
--rw-r--r--   0 runner    (1001) docker     (123)    30526 2023-07-25 21:03:00.000000 snitch-protos-0.0.47/snitch_protos/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:03:54.743955 snitch-protos-0.0.47/snitch_protos/protos/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-25 21:03:00.000000 snitch-protos-0.0.47/snitch_protos/protos/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:03:54.743955 snitch-protos-0.0.47/snitch_protos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-25 21:03:54.000000 snitch-protos-0.0.47/snitch_protos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-25 21:03:54.000000 snitch-protos-0.0.47/snitch_protos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 21:03:54.000000 snitch-protos-0.0.47/snitch_protos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 21:03:54.000000 snitch-protos-0.0.47/snitch_protos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:59:58.970237 snitch-protos-0.0.48/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-26 20:59:58.970237 snitch-protos-0.0.48/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-26 20:59:28.000000 snitch-protos-0.0.48/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 20:59:58.970237 snitch-protos-0.0.48/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-26 20:59:58.000000 snitch-protos-0.0.48/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:59:58.970237 snitch-protos-0.0.48/snitch_protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:59:28.000000 snitch-protos-0.0.48/snitch_protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:59:58.970237 snitch-protos-0.0.48/snitch_protos/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)    32411 2023-07-26 20:59:28.000000 snitch-protos-0.0.48/snitch_protos/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:59:58.970237 snitch-protos-0.0.48/snitch_protos/protos/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-26 20:59:28.000000 snitch-protos-0.0.48/snitch_protos/protos/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:59:58.970237 snitch-protos-0.0.48/snitch_protos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-26 20:59:58.000000 snitch-protos-0.0.48/snitch_protos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-26 20:59:58.000000 snitch-protos-0.0.48/snitch_protos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:59:58.000000 snitch-protos-0.0.48/snitch_protos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 20:59:58.000000 snitch-protos-0.0.48/snitch_protos.egg-info/top_level.txt
```

### Comparing `snitch-protos-0.0.47/PKG-INFO` & `snitch-protos-0.0.48/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snitch-protos
-Version: 0.0.47
+Version: 0.0.48
 Summary: Protobuf python package for Streamdal.com Snitch
 Home-page: https://github.com/streamdal/snitch-protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `snitch-protos-0.0.47/setup.py` & `snitch-protos-0.0.48/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='snitch-protos',
-    version='0.0.47',
+    version='0.0.48',
     description='Protobuf python package for Streamdal.com Snitch',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/streamdal/snitch-protos',
     author='Streamdal.com',
     author_email='engineering@streamdal.com',
     license='MIT',
```

### Comparing `snitch-protos-0.0.47/snitch_protos/protos/__init__.py` & `snitch-protos-0.0.48/snitch_protos/protos/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: common.proto, external_api.proto, internal_api.proto, pipeline.proto
+# sources: bus.proto, command.proto, common.proto, external.proto, info.proto, internal.proto, pipeline.proto, wasm.proto
 # plugin: python-betterproto
 # This file has been @generated
 
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
     AsyncIterator,
@@ -32,716 +32,804 @@
     RESPONSE_CODE_OK = 1
     RESPONSE_CODE_BAD_REQUEST = 2
     RESPONSE_CODE_NOT_FOUND = 3
     RESPONSE_CODE_INTERNAL_SERVER_ERROR = 4
     RESPONSE_CODE_GENERIC_ERROR = 5
 
 
-class WasmExitCode(betterproto.Enum):
-    """
-    Included in WASM response; SDK is responsible for interpreting the response
-    status and how it relates to the step condition. ie. WASM func returns
-    WASM_EXIT_CODE_INTERNAL_ERROR lookup ON_ERROR conditions to determine what
-    to do next. ie. WASM func returns WASM_EXIT_CODE_SUCCESS lookup ON_MATCH
-    conditions to determine what to do next;
-    """
+class OperationType(betterproto.Enum):
+    """Each SDK client is a $service + $component + $operation_type"""
 
-    WASM_EXIT_CODE_UNSET = 0
-    WASM_EXIT_CODE_SUCCESS = 1
-    WASM_EXIT_CODE_FAILURE = 2
-    WASM_EXIT_CODE_INTERNAL_ERROR = 3
+    OPERATION_TYPE_UNSET = 0
+    OPERATION_TYPE_CONSUMER = 1
+    OPERATION_TYPE_PRODUCER = 2
 
 
 class PipelineStepCondition(betterproto.Enum):
     """
     A condition defines how the SDK should handle a step response -- should it
     continue executing the pipeline, should it abort, should it notify the
     server? Each step can have multiple conditions.
     """
 
-    CONDITION_UNSET = 0
-    CONDITION_CONTINUE = 1
-    CONDITION_ABORT = 2
-    CONDITION_NOTIFY = 3
+    PIPELINE_STEP_CONDITION_UNSET = 0
+    PIPELINE_STEP_CONDITION_ABORT = 1
+    PIPELINE_STEP_CONDITION_NOTIFY = 2
 
 
-class CommandType(betterproto.Enum):
-    """Types of commands that can be sent to the SDK"""
-
-    SNITCH_COMMAND_TYPE_UNSET = 0
-    SNITCH_COMMAND_TYPE_KEEPALIVE = 1
-    SNITCH_COMMAND_TYPE_SET_PIPELINE = 2
-    SNITCH_COMMAND_TYPE_DELETE_PIPELINE = 3
-    SNITCH_COMMAND_TYPE_PAUSE_PIPELINE = 4
-    SNITCH_COMMAND_TYPE_UNPAUSE_PIPELINE = 5
+class ClientType(betterproto.Enum):
+    CLIENT_TYPE_UNSET = 0
+    CLIENT_TYPE_SDK = 1
+    CLIENT_TYPE_SHIM = 2
 
 
-class OperationType(betterproto.Enum):
-    OPERATION_TYPE_UNSET = 0
-    OPERATION_TYPE_CONSUMER = 1
-    OPERATION_TYPE_PRODUCER = 2
+class WasmExitCode(betterproto.Enum):
+    """
+    Included in WASM response; SDK is responsible for interpreting the response
+    status and how it relates to the step condition. ie. WASM func returns
+    WASM_EXIT_CODE_INTERNAL_ERROR lookup ON_ERROR conditions to determine what
+    to do next. ie. WASM func returns WASM_EXIT_CODE_SUCCESS lookup ON_MATCH
+    conditions to determine what to do next;
+    """
+
+    WASM_EXIT_CODE_UNSET = 0
+    WASM_EXIT_CODE_SUCCESS = 1
+    WASM_EXIT_CODE_FAILURE = 2
+    WASM_EXIT_CODE_INTERNAL_ERROR = 3
 
 
 @dataclass(eq=False, repr=False)
 class StandardResponse(betterproto.Message):
     """Common response message for many gRPC methods"""
 
     id: str = betterproto.string_field(1)
     """Co-relation ID for the request / response"""
 
     code: "ResponseCode" = betterproto.enum_field(2)
     message: str = betterproto.string_field(3)
-    metadata: Dict[str, str] = betterproto.map_field(
-        1000, betterproto.TYPE_STRING, betterproto.TYPE_STRING
-    )
-    """Debug info that server may populate with additional info."""
 
 
 @dataclass(eq=False, repr=False)
-class GetServicesRequest(betterproto.Message):
-    """protolint:disable INDENT"""
+class Audience(betterproto.Message):
+    """Used to indicate who a command is intended for"""
 
-    pass
+    service_name: str = betterproto.string_field(1)
+    """
+    Name of the service -- let's include the service name on all calls, we can
+    optimize later ~DS
+    """
 
+    component_name: str = betterproto.string_field(2)
+    """
+    Name of the component the SDK is interacting with (ie. kafka-$topic-name)
+    """
 
-@dataclass(eq=False, repr=False)
-class GetServicesResponse(betterproto.Message):
-    pass
+    operation_type: "OperationType" = betterproto.enum_field(3)
+    """Consumer or Producer"""
 
 
 @dataclass(eq=False, repr=False)
-class GetServiceRequest(betterproto.Message):
-    pass
-
+class Pipeline(betterproto.Message):
+    """
+    Pipeline is a structure that holds one or more pipeline steps. This
+    structure is intended to be immutable; clients are expected to generate
+    WASMRequest's that contain a pipeline step.
+    """
 
-@dataclass(eq=False, repr=False)
-class GetServiceResponse(betterproto.Message):
-    pass
+    id: str = betterproto.string_field(1)
+    """Set by snitch-server on Create; must be present on Update calls"""
 
+    name: str = betterproto.string_field(2)
+    """Friendly name for the pipeline"""
 
-@dataclass(eq=False, repr=False)
-class GetPipelinesRequest(betterproto.Message):
-    pass
+    steps: List["PipelineStep"] = betterproto.message_field(3)
+    """One or more steps to execute"""
 
 
 @dataclass(eq=False, repr=False)
-class GetPipelinesResponse(betterproto.Message):
-    pass
+class PipelineStep(betterproto.Message):
+    """A pipeline step is a single step in a pipeline."""
 
+    name: str = betterproto.string_field(1)
+    """Friendly name for the step"""
 
-@dataclass(eq=False, repr=False)
-class GetPipelineRequest(betterproto.Message):
-    pass
+    on_success: List["PipelineStepCondition"] = betterproto.enum_field(2)
+    """What should SDK do if step succeeds?"""
 
+    on_failure: List["PipelineStepCondition"] = betterproto.enum_field(3)
+    """What should SDK do if step fails?"""
 
-@dataclass(eq=False, repr=False)
-class GetPipelineResponse(betterproto.Message):
-    pass
+    detective: "steps.DetectiveStep" = betterproto.message_field(1000, group="step")
+    transform: "steps.TransformStep" = betterproto.message_field(1001, group="step")
+    encode: "steps.EncodeStep" = betterproto.message_field(1002, group="step")
+    decode: "steps.DecodeStep" = betterproto.message_field(1003, group="step")
+    custom: "steps.CustomStep" = betterproto.message_field(1004, group="step")
+    wasm_id: str = betterproto.string_field(10000)
+    """WASM module ID (set by snitch-server)"""
 
+    wasm_bytes: bytes = betterproto.bytes_field(10001)
+    """WASM module bytes (set by snitch-server)"""
 
-@dataclass(eq=False, repr=False)
-class SetPipelineRequest(betterproto.Message):
-    pass
+    wasm_function: str = betterproto.string_field(10002)
+    """WASM function name to execute (set by snitch-server)"""
 
 
 @dataclass(eq=False, repr=False)
-class SetPipelineResponse(betterproto.Message):
-    pass
+class Command(betterproto.Message):
+    """Command is used by snitch-server for sending commands to SDKs"""
 
+    audience: "Audience" = betterproto.message_field(1)
+    """Who is this command intended for?"""
 
-@dataclass(eq=False, repr=False)
-class DeletePipelineRequest(betterproto.Message):
-    pass
+    set_pipeline: "SetPipelineCommand" = betterproto.message_field(100, group="command")
+    delete_pipeline: "DeletePipelineCommand" = betterproto.message_field(
+        101, group="command"
+    )
+    pause_pipeline: "PausePipelineCommand" = betterproto.message_field(
+        102, group="command"
+    )
+    unpause_pipeline: "UnpausePipelineCommand" = betterproto.message_field(
+        103, group="command"
+    )
+    keep_alive: "KeepAliveCommand" = betterproto.message_field(104, group="command")
 
 
 @dataclass(eq=False, repr=False)
-class DeletePipelineResponse(betterproto.Message):
-    pass
-
+class SetPipelineCommand(betterproto.Message):
+    """Used for both Add and Update"""
 
-@dataclass(eq=False, repr=False)
-class GetStepsRequest(betterproto.Message):
-    pass
+    pipeline: "Pipeline" = betterproto.message_field(1)
 
 
 @dataclass(eq=False, repr=False)
-class GetStepsResponse(betterproto.Message):
-    pass
+class DeletePipelineCommand(betterproto.Message):
+    id: str = betterproto.string_field(1)
+    """Unique ID for the pipeline"""
 
 
 @dataclass(eq=False, repr=False)
-class CreateStepRequest(betterproto.Message):
-    pass
+class PausePipelineCommand(betterproto.Message):
+    id: str = betterproto.string_field(1)
+    """Unique ID for the pipeline"""
 
 
 @dataclass(eq=False, repr=False)
-class CreateStepResponse(betterproto.Message):
-    pass
+class UnpausePipelineCommand(betterproto.Message):
+    id: str = betterproto.string_field(1)
+    """Unique ID for the pipeline"""
 
 
 @dataclass(eq=False, repr=False)
-class UpdateStepRequest(betterproto.Message):
+class KeepAliveCommand(betterproto.Message):
     pass
 
 
 @dataclass(eq=False, repr=False)
-class UpdateStepResponse(betterproto.Message):
-    pass
+class ServiceInfo(betterproto.Message):
+    name: str = betterproto.string_field(1)
+    description: str = betterproto.string_field(2)
+    pipelines: List["PipelineInfo"] = betterproto.message_field(100)
+    consumers: List["ConsumerInfo"] = betterproto.message_field(101)
+    producers: List["ProducerInfo"] = betterproto.message_field(102)
+    clients: List["ClientInfo"] = betterproto.message_field(103)
 
 
 @dataclass(eq=False, repr=False)
-class DeleteStepRequest(betterproto.Message):
-    pass
+class PipelineInfo(betterproto.Message):
+    audience: "Audience" = betterproto.message_field(1)
+    pipeline: "Pipeline" = betterproto.message_field(2)
 
 
 @dataclass(eq=False, repr=False)
-class DeleteStepResponse(betterproto.Message):
+class ConsumerInfo(betterproto.Message):
     pass
 
 
 @dataclass(eq=False, repr=False)
-class TestRequest(betterproto.Message):
-    input: str = betterproto.string_field(1)
-
-
-@dataclass(eq=False, repr=False)
-class TestResponse(betterproto.Message):
-    output: str = betterproto.string_field(2)
-
-
-@dataclass(eq=False, repr=False)
-class WasmRequest(betterproto.Message):
-    """SDK generates a WASM request and passes this to the WASM func"""
-
-    step: "PipelineStep" = betterproto.message_field(1)
-    input: bytes = betterproto.bytes_field(2)
-
-
-@dataclass(eq=False, repr=False)
-class WasmResponse(betterproto.Message):
-    """Returned by all WASM functions"""
-
-    output: bytes = betterproto.bytes_field(1)
-    exit_code: "WasmExitCode" = betterproto.enum_field(2)
-    exit_msg: str = betterproto.string_field(3)
-
-
-@dataclass(eq=False, repr=False)
-class PipelineStep(betterproto.Message):
-    """
-    A PipelineCommand consists of one or more pipeline steps. A pipeline step
-    is an immutable set of instructions on how to execute a step. The SDK will
-    use the pipeline step to generate a WASM request.
-    """
-
-    id: str = betterproto.string_field(1)
-    """Unique ID for the step"""
-
-    name: str = betterproto.string_field(2)
-    """Friendly name for the step"""
-
-    conditions: List["PipelineStepCondition"] = betterproto.enum_field(3)
-    """Conditions that SDK should check before executing next step"""
-
-    detective: "steps.DetectiveStep" = betterproto.message_field(1000, group="step")
-    transform: "steps.TransformStep" = betterproto.message_field(1001, group="step")
-    encode: "steps.EncodeStep" = betterproto.message_field(1002, group="step")
-    decode: "steps.DecodeStep" = betterproto.message_field(1003, group="step")
-    custom: "steps.CustomStep" = betterproto.message_field(1004, group="step")
-    wasm_id: str = betterproto.string_field(10000)
-    """WASM module ID (set by backend)"""
-
-    wasm_bytes: bytes = betterproto.bytes_field(10001)
-    """WASM module bytes (set by backend)"""
-
-    wasm_function: str = betterproto.string_field(10002)
-    """WASM function name to execute (set by backend)"""
-
-
-@dataclass(eq=False, repr=False)
-class SetPipelineCommand(betterproto.Message):
-    """Used for both Add and Update"""
-
-    id: str = betterproto.string_field(1)
-    """Unique ID for the pipeline"""
-
-    name: str = betterproto.string_field(2)
-    """Friendly name for the pipeline"""
-
-    steps: List["PipelineStep"] = betterproto.message_field(3)
-    """One or more steps to execute"""
-
-
-@dataclass(eq=False, repr=False)
-class DeletePipelineCommand(betterproto.Message):
-    id: str = betterproto.string_field(1)
-    """Unique ID for the pipeline"""
+class ProducerInfo(betterproto.Message):
+    pass
 
 
 @dataclass(eq=False, repr=False)
-class PausePipelineCommand(betterproto.Message):
-    id: str = betterproto.string_field(1)
-    """Unique ID for the pipeline"""
+class ClientInfo(betterproto.Message):
+    """This should come from the register call"""
 
-
-@dataclass(eq=False, repr=False)
-class UnpausePipelineCommand(betterproto.Message):
-    id: str = betterproto.string_field(1)
-    """Unique ID for the pipeline"""
+    client_type: "ClientType" = betterproto.enum_field(1)
+    library_name: str = betterproto.string_field(2)
+    library_version: str = betterproto.string_field(3)
+    language: str = betterproto.string_field(4)
+    arch: str = betterproto.string_field(5)
+    os: str = betterproto.string_field(6)
 
 
 @dataclass(eq=False, repr=False)
 class HeartbeatRequest(betterproto.Message):
     """
     Each consumer and producer should send periodic heartbeats to the server to
     let the server know that they are still active.
     """
 
     audience: "Audience" = betterproto.message_field(1)
     last_activity_unix_timestamp_utc: int = betterproto.int64_field(2)
-    metadata: Dict[str, str] = betterproto.map_field(
-        1000, betterproto.TYPE_STRING, betterproto.TYPE_STRING
-    )
 
 
 @dataclass(eq=False, repr=False)
 class NotifyRequest(betterproto.Message):
-    rule_id: str = betterproto.string_field(1)
-    rule_name: str = betterproto.string_field(2)
+    pipeline_id: str = betterproto.string_field(1)
+    step_name: str = betterproto.string_field(2)
     audience: "Audience" = betterproto.message_field(3)
     occurred_at_unix_ts_utc: int = betterproto.int64_field(4)
-    metadata: Dict[str, str] = betterproto.map_field(
-        1000, betterproto.TYPE_STRING, betterproto.TYPE_STRING
+
+
+@dataclass(eq=False, repr=False)
+class Metrics(betterproto.Message):
+    name: str = betterproto.string_field(1)
+    labels: Dict[str, str] = betterproto.map_field(
+        2, betterproto.TYPE_STRING, betterproto.TYPE_STRING
     )
+    value: float = betterproto.double_field(3)
 
 
 @dataclass(eq=False, repr=False)
 class MetricsRequest(betterproto.Message):
-    rule_id: str = betterproto.string_field(1)
-    rule_name: str = betterproto.string_field(2)
-    audience: "Audience" = betterproto.message_field(3)
-    metadata: Dict[str, str] = betterproto.map_field(
-        1000, betterproto.TYPE_STRING, betterproto.TYPE_STRING
-    )
+    metrics: List["Metrics"] = betterproto.message_field(1)
 
 
 @dataclass(eq=False, repr=False)
 class RegisterRequest(betterproto.Message):
     service_name: str = betterproto.string_field(1)
     dry_run: bool = betterproto.bool_field(2)
     """
     If set, we know that any pipelines or steps executed in this SDK will NOT
     modify the input/output data. As in, the SDK will log what it _would_ do
     and always return the original data set.
     """
 
-    metadata: Dict[str, str] = betterproto.map_field(
-        1000, betterproto.TYPE_STRING, betterproto.TYPE_STRING
-    )
-    """snitch-server uses this under the hood for debug"""
+    client_info: "ClientInfo" = betterproto.message_field(3)
+    """Info about the client (lib name, lang, os, arch, etc.)"""
+
+    audiences: List["Audience"] = betterproto.message_field(4)
+    """
+    OPTIONAL -- if these are defined, these will show up in the UI even if
+    there is no active .Process() call from the SDK.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class DeregisterRequest(betterproto.Message):
     """
     Same as RegisterRequest - used for broadcasting a deregistration event
     """
 
     service_name: str = betterproto.string_field(1)
-    metadata: Dict[str, str] = betterproto.map_field(
-        1000, betterproto.TYPE_STRING, betterproto.TYPE_STRING
-    )
 
 
 @dataclass(eq=False, repr=False)
 class BusEvent(betterproto.Message):
     """Type used by `snitch-server` for sending messages on its local bus."""
 
-    request_id: str = betterproto.string_field(1)
-    source: str = betterproto.string_field(2)
-    command_response: "CommandResponse" = betterproto.message_field(100, group="event")
+    source: str = betterproto.string_field(1)
+    command_response: "Command" = betterproto.message_field(100, group="event")
     register_request: "RegisterRequest" = betterproto.message_field(101, group="event")
     deregister_request: "DeregisterRequest" = betterproto.message_field(
         102, group="event"
     )
     heartbeat_request: "HeartbeatRequest" = betterproto.message_field(
         103, group="event"
     )
     metadata: Dict[str, str] = betterproto.map_field(
         1000, betterproto.TYPE_STRING, betterproto.TYPE_STRING
     )
+    """
+    All gRPC metadata is stored in ctx; when request goes outside of gRPC
+    bounds, we will translate ctx metadata into this field. Example: 1. Request
+    comes into snitch-server via external gRPC to set new pipeline 2. snitch-
+    server has to send SetPipeline cmd to SDK via gRPC - it passes    on
+    original metadata in request. 3. snitch-server has to broadcast SetPipeline
+    cmd to other services via bus 4. Since this is not a gRPC call, snitch-
+    server translates ctx metadata to    this field and includes it in the bus
+    event.
+    """
 
 
 @dataclass(eq=False, repr=False)
-class CommandResponse(betterproto.Message):
-    """
-    The primary method to send commands to the SDK; server will send zero or
-    more RegisterResponse's with SetPipelineRequest on SDK instantiation.
-    """
+class GetServiceMapRequest(betterproto.Message):
+    pass
 
-    audience: "Audience" = betterproto.message_field(1)
-    """Who is this command intended for?"""
 
-    set_pipeline: "SetPipelineCommand" = betterproto.message_field(100, group="command")
-    delete_pipeline: "DeletePipelineCommand" = betterproto.message_field(
-        101, group="command"
-    )
-    pause_pipeline: "PausePipelineCommand" = betterproto.message_field(
-        102, group="command"
-    )
-    unpause_pipeline: "UnpausePipelineCommand" = betterproto.message_field(
-        103, group="command"
-    )
-    metadata: Dict[str, str] = betterproto.map_field(
-        1000, betterproto.TYPE_STRING, betterproto.TYPE_STRING
+@dataclass(eq=False, repr=False)
+class GetServiceMapResponse(betterproto.Message):
+    service_map: Dict[str, "ServiceInfo"] = betterproto.map_field(
+        1, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE
     )
+    """Key == service name"""
 
 
 @dataclass(eq=False, repr=False)
-class Audience(betterproto.Message):
-    """Used to indicate who a request/command is intended for"""
+class GetPipelinesRequest(betterproto.Message):
+    pass
 
-    service_name: str = betterproto.string_field(1)
-    """Name of the service"""
 
-    component_name: str = betterproto.string_field(2)
-    """
-    Name of the component the SDK is interacting with (ie. kafka-$topic-name)
-    """
+@dataclass(eq=False, repr=False)
+class GetPipelinesResponse(betterproto.Message):
+    pipelines: List["Pipeline"] = betterproto.message_field(1)
 
-    operation_type: "OperationType" = betterproto.enum_field(3)
-    """Consumer or Producer"""
+
+@dataclass(eq=False, repr=False)
+class GetPipelineRequest(betterproto.Message):
+    pipeline_id: str = betterproto.string_field(1)
 
 
-class ExternalStub(betterproto.ServiceStub):
-    async def get_services(
+@dataclass(eq=False, repr=False)
+class GetPipelineResponse(betterproto.Message):
+    pipeline: "Pipeline" = betterproto.message_field(1)
+
+
+@dataclass(eq=False, repr=False)
+class CreatePipelineRequest(betterproto.Message):
+    pipeline: "Pipeline" = betterproto.message_field(1)
+
+
+@dataclass(eq=False, repr=False)
+class UpdatePipelineRequest(betterproto.Message):
+    pipeline: "Pipeline" = betterproto.message_field(1)
+
+
+@dataclass(eq=False, repr=False)
+class DeletePipelineRequest(betterproto.Message):
+    pipeline_id: str = betterproto.string_field(1)
+
+
+@dataclass(eq=False, repr=False)
+class AttachPipelineRequest(betterproto.Message):
+    pipeline_id: str = betterproto.string_field(1)
+    audience: "Audience" = betterproto.message_field(2)
+
+
+@dataclass(eq=False, repr=False)
+class DetachPipelineRequest(betterproto.Message):
+    pipeline_id: str = betterproto.string_field(1)
+    audience: "Audience" = betterproto.message_field(2)
+
+
+@dataclass(eq=False, repr=False)
+class PausePipelineRequest(betterproto.Message):
+    pipeline_id: str = betterproto.string_field(1)
+
+
+@dataclass(eq=False, repr=False)
+class ResumePipelineRequest(betterproto.Message):
+    pipeline_id: str = betterproto.string_field(1)
+
+
+@dataclass(eq=False, repr=False)
+class TestRequest(betterproto.Message):
+    input: str = betterproto.string_field(1)
+
+
+@dataclass(eq=False, repr=False)
+class TestResponse(betterproto.Message):
+    output: str = betterproto.string_field(2)
+
+
+@dataclass(eq=False, repr=False)
+class WasmRequest(betterproto.Message):
+    """SDK generates a WASM request and passes this to the WASM func"""
+
+    step: "PipelineStep" = betterproto.message_field(1)
+    input: bytes = betterproto.bytes_field(2)
+
+
+@dataclass(eq=False, repr=False)
+class WasmResponse(betterproto.Message):
+    """Returned by all WASM functions"""
+
+    output: bytes = betterproto.bytes_field(1)
+    exit_code: "WasmExitCode" = betterproto.enum_field(2)
+    exit_msg: str = betterproto.string_field(3)
+
+
+class InternalStub(betterproto.ServiceStub):
+    async def register(
         self,
-        get_services_request: "GetServicesRequest",
+        register_request: "RegisterRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "GetServicesResponse":
-        return await self._unary_unary(
-            "/protos.External/GetServices",
-            get_services_request,
-            GetServicesResponse,
+    ) -> AsyncIterator["Command"]:
+        async for response in self._unary_stream(
+            "/protos.Internal/Register",
+            register_request,
+            Command,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
-        )
+        ):
+            yield response
 
-    async def get_service(
+    async def heartbeat(
         self,
-        get_service_request: "GetServiceRequest",
+        heartbeat_request: "HeartbeatRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "GetServiceResponse":
+    ) -> "StandardResponse":
         return await self._unary_unary(
-            "/protos.External/GetService",
-            get_service_request,
-            GetServiceResponse,
+            "/protos.Internal/Heartbeat",
+            heartbeat_request,
+            StandardResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    async def get_pipelines(
+    async def notify(
         self,
-        get_pipelines_request: "GetPipelinesRequest",
+        notify_request: "NotifyRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "GetPipelinesResponse":
+    ) -> "StandardResponse":
         return await self._unary_unary(
-            "/protos.External/GetPipelines",
-            get_pipelines_request,
-            GetPipelinesResponse,
+            "/protos.Internal/Notify",
+            notify_request,
+            StandardResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    async def get_pipeline(
+    async def metrics(
         self,
-        get_pipeline_request: "GetPipelineRequest",
+        metrics_request: "MetricsRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "GetPipelineResponse":
+    ) -> "StandardResponse":
         return await self._unary_unary(
-            "/protos.External/GetPipeline",
-            get_pipeline_request,
-            GetPipelineResponse,
+            "/protos.Internal/Metrics",
+            metrics_request,
+            StandardResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    async def set_pipeline(
+
+class ExternalStub(betterproto.ServiceStub):
+    async def get_service_map(
         self,
-        set_pipeline_request: "SetPipelineRequest",
+        get_service_map_request: "GetServiceMapRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "SetPipelineResponse":
+    ) -> "GetServiceMapResponse":
         return await self._unary_unary(
-            "/protos.External/SetPipeline",
-            set_pipeline_request,
-            SetPipelineResponse,
+            "/protos.External/GetServiceMap",
+            get_service_map_request,
+            GetServiceMapResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    async def delete_pipeline(
+    async def get_pipelines(
         self,
-        delete_pipeline_request: "DeletePipelineRequest",
+        get_pipelines_request: "GetPipelinesRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "DeletePipelineResponse":
+    ) -> "GetPipelinesResponse":
         return await self._unary_unary(
-            "/protos.External/DeletePipeline",
-            delete_pipeline_request,
-            DeletePipelineResponse,
+            "/protos.External/GetPipelines",
+            get_pipelines_request,
+            GetPipelinesResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    async def get_steps(
+    async def get_pipeline(
         self,
-        get_steps_request: "GetStepsRequest",
+        get_pipeline_request: "GetPipelineRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "GetStepsResponse":
+    ) -> "GetPipelineResponse":
         return await self._unary_unary(
-            "/protos.External/GetSteps",
-            get_steps_request,
-            GetStepsResponse,
+            "/protos.External/GetPipeline",
+            get_pipeline_request,
+            GetPipelineResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    async def create_step(
+    async def create_pipeline(
         self,
-        create_step_request: "CreateStepRequest",
+        create_pipeline_request: "CreatePipelineRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "CreateStepResponse":
+    ) -> "StandardResponse":
         return await self._unary_unary(
-            "/protos.External/CreateStep",
-            create_step_request,
-            CreateStepResponse,
+            "/protos.External/CreatePipeline",
+            create_pipeline_request,
+            StandardResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    async def update_step(
+    async def update_pipeline(
         self,
-        update_step_request: "UpdateStepRequest",
+        update_pipeline_request: "UpdatePipelineRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "UpdateStepResponse":
+    ) -> "StandardResponse":
         return await self._unary_unary(
-            "/protos.External/UpdateStep",
-            update_step_request,
-            UpdateStepResponse,
+            "/protos.External/UpdatePipeline",
+            update_pipeline_request,
+            StandardResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    async def delete_step(
+    async def delete_pipeline(
         self,
-        delete_step_request: "DeleteStepRequest",
+        delete_pipeline_request: "DeletePipelineRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "DeleteStepResponse":
+    ) -> "StandardResponse":
         return await self._unary_unary(
-            "/protos.External/DeleteStep",
-            delete_step_request,
-            DeleteStepResponse,
+            "/protos.External/DeletePipeline",
+            delete_pipeline_request,
+            StandardResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    async def test(
+    async def attach_pipeline(
         self,
-        test_request: "TestRequest",
+        attach_pipeline_request: "AttachPipelineRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "TestResponse":
+    ) -> "StandardResponse":
         return await self._unary_unary(
-            "/protos.External/Test",
-            test_request,
-            TestResponse,
+            "/protos.External/AttachPipeline",
+            attach_pipeline_request,
+            StandardResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-
-class InternalStub(betterproto.ServiceStub):
-    async def register(
+    async def detach_pipeline(
         self,
-        register_request: "RegisterRequest",
+        detach_pipeline_request: "DetachPipelineRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> AsyncIterator["CommandResponse"]:
-        async for response in self._unary_stream(
-            "/protos.Internal/Register",
-            register_request,
-            CommandResponse,
+    ) -> "StandardResponse":
+        return await self._unary_unary(
+            "/protos.External/DetachPipeline",
+            detach_pipeline_request,
+            StandardResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
-        ):
-            yield response
+        )
 
-    async def heartbeat(
+    async def pause_pipeline(
         self,
-        heartbeat_request: "HeartbeatRequest",
+        pause_pipeline_request: "PausePipelineRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
     ) -> "StandardResponse":
         return await self._unary_unary(
-            "/protos.Internal/Heartbeat",
-            heartbeat_request,
+            "/protos.External/PausePipeline",
+            pause_pipeline_request,
             StandardResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    async def notify(
+    async def resume_pipeline(
         self,
-        notify_request: "NotifyRequest",
+        resume_pipeline_request: "ResumePipelineRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
     ) -> "StandardResponse":
         return await self._unary_unary(
-            "/protos.Internal/Notify",
-            notify_request,
+            "/protos.External/ResumePipeline",
+            resume_pipeline_request,
             StandardResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    async def metrics(
+    async def test(
         self,
-        metrics_request: "MetricsRequest",
+        test_request: "TestRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "StandardResponse":
+    ) -> "TestResponse":
         return await self._unary_unary(
-            "/protos.Internal/Metrics",
-            metrics_request,
-            StandardResponse,
+            "/protos.External/Test",
+            test_request,
+            TestResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
 
-class ExternalBase(ServiceBase):
-    async def get_services(
-        self, get_services_request: "GetServicesRequest"
-    ) -> "GetServicesResponse":
+class InternalBase(ServiceBase):
+    async def register(
+        self, register_request: "RegisterRequest"
+    ) -> AsyncIterator["Command"]:
+        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
+        yield Command()
+
+    async def heartbeat(
+        self, heartbeat_request: "HeartbeatRequest"
+    ) -> "StandardResponse":
+        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
+
+    async def notify(self, notify_request: "NotifyRequest") -> "StandardResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
-    async def get_service(
-        self, get_service_request: "GetServiceRequest"
-    ) -> "GetServiceResponse":
+    async def metrics(self, metrics_request: "MetricsRequest") -> "StandardResponse":
+        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
+
+    async def __rpc_register(
+        self, stream: "grpclib.server.Stream[RegisterRequest, Command]"
+    ) -> None:
+        request = await stream.recv_message()
+        await self._call_rpc_handler_server_stream(
+            self.register,
+            stream,
+            request,
+        )
+
+    async def __rpc_heartbeat(
+        self, stream: "grpclib.server.Stream[HeartbeatRequest, StandardResponse]"
+    ) -> None:
+        request = await stream.recv_message()
+        response = await self.heartbeat(request)
+        await stream.send_message(response)
+
+    async def __rpc_notify(
+        self, stream: "grpclib.server.Stream[NotifyRequest, StandardResponse]"
+    ) -> None:
+        request = await stream.recv_message()
+        response = await self.notify(request)
+        await stream.send_message(response)
+
+    async def __rpc_metrics(
+        self, stream: "grpclib.server.Stream[MetricsRequest, StandardResponse]"
+    ) -> None:
+        request = await stream.recv_message()
+        response = await self.metrics(request)
+        await stream.send_message(response)
+
+    def __mapping__(self) -> Dict[str, grpclib.const.Handler]:
+        return {
+            "/protos.Internal/Register": grpclib.const.Handler(
+                self.__rpc_register,
+                grpclib.const.Cardinality.UNARY_STREAM,
+                RegisterRequest,
+                Command,
+            ),
+            "/protos.Internal/Heartbeat": grpclib.const.Handler(
+                self.__rpc_heartbeat,
+                grpclib.const.Cardinality.UNARY_UNARY,
+                HeartbeatRequest,
+                StandardResponse,
+            ),
+            "/protos.Internal/Notify": grpclib.const.Handler(
+                self.__rpc_notify,
+                grpclib.const.Cardinality.UNARY_UNARY,
+                NotifyRequest,
+                StandardResponse,
+            ),
+            "/protos.Internal/Metrics": grpclib.const.Handler(
+                self.__rpc_metrics,
+                grpclib.const.Cardinality.UNARY_UNARY,
+                MetricsRequest,
+                StandardResponse,
+            ),
+        }
+
+
+class ExternalBase(ServiceBase):
+    async def get_service_map(
+        self, get_service_map_request: "GetServiceMapRequest"
+    ) -> "GetServiceMapResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
     async def get_pipelines(
         self, get_pipelines_request: "GetPipelinesRequest"
     ) -> "GetPipelinesResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
     async def get_pipeline(
         self, get_pipeline_request: "GetPipelineRequest"
     ) -> "GetPipelineResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
-    async def set_pipeline(
-        self, set_pipeline_request: "SetPipelineRequest"
-    ) -> "SetPipelineResponse":
+    async def create_pipeline(
+        self, create_pipeline_request: "CreatePipelineRequest"
+    ) -> "StandardResponse":
+        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
+
+    async def update_pipeline(
+        self, update_pipeline_request: "UpdatePipelineRequest"
+    ) -> "StandardResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
     async def delete_pipeline(
         self, delete_pipeline_request: "DeletePipelineRequest"
-    ) -> "DeletePipelineResponse":
+    ) -> "StandardResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
-    async def get_steps(
-        self, get_steps_request: "GetStepsRequest"
-    ) -> "GetStepsResponse":
+    async def attach_pipeline(
+        self, attach_pipeline_request: "AttachPipelineRequest"
+    ) -> "StandardResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
-    async def create_step(
-        self, create_step_request: "CreateStepRequest"
-    ) -> "CreateStepResponse":
+    async def detach_pipeline(
+        self, detach_pipeline_request: "DetachPipelineRequest"
+    ) -> "StandardResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
-    async def update_step(
-        self, update_step_request: "UpdateStepRequest"
-    ) -> "UpdateStepResponse":
+    async def pause_pipeline(
+        self, pause_pipeline_request: "PausePipelineRequest"
+    ) -> "StandardResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
-    async def delete_step(
-        self, delete_step_request: "DeleteStepRequest"
-    ) -> "DeleteStepResponse":
+    async def resume_pipeline(
+        self, resume_pipeline_request: "ResumePipelineRequest"
+    ) -> "StandardResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
     async def test(self, test_request: "TestRequest") -> "TestResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
-    async def __rpc_get_services(
-        self, stream: "grpclib.server.Stream[GetServicesRequest, GetServicesResponse]"
-    ) -> None:
-        request = await stream.recv_message()
-        response = await self.get_services(request)
-        await stream.send_message(response)
-
-    async def __rpc_get_service(
-        self, stream: "grpclib.server.Stream[GetServiceRequest, GetServiceResponse]"
+    async def __rpc_get_service_map(
+        self,
+        stream: "grpclib.server.Stream[GetServiceMapRequest, GetServiceMapResponse]",
     ) -> None:
         request = await stream.recv_message()
-        response = await self.get_service(request)
+        response = await self.get_service_map(request)
         await stream.send_message(response)
 
     async def __rpc_get_pipelines(
         self, stream: "grpclib.server.Stream[GetPipelinesRequest, GetPipelinesResponse]"
     ) -> None:
         request = await stream.recv_message()
         response = await self.get_pipelines(request)
@@ -750,204 +838,132 @@
     async def __rpc_get_pipeline(
         self, stream: "grpclib.server.Stream[GetPipelineRequest, GetPipelineResponse]"
     ) -> None:
         request = await stream.recv_message()
         response = await self.get_pipeline(request)
         await stream.send_message(response)
 
-    async def __rpc_set_pipeline(
-        self, stream: "grpclib.server.Stream[SetPipelineRequest, SetPipelineResponse]"
+    async def __rpc_create_pipeline(
+        self, stream: "grpclib.server.Stream[CreatePipelineRequest, StandardResponse]"
     ) -> None:
         request = await stream.recv_message()
-        response = await self.set_pipeline(request)
+        response = await self.create_pipeline(request)
+        await stream.send_message(response)
+
+    async def __rpc_update_pipeline(
+        self, stream: "grpclib.server.Stream[UpdatePipelineRequest, StandardResponse]"
+    ) -> None:
+        request = await stream.recv_message()
+        response = await self.update_pipeline(request)
         await stream.send_message(response)
 
     async def __rpc_delete_pipeline(
-        self,
-        stream: "grpclib.server.Stream[DeletePipelineRequest, DeletePipelineResponse]",
+        self, stream: "grpclib.server.Stream[DeletePipelineRequest, StandardResponse]"
     ) -> None:
         request = await stream.recv_message()
         response = await self.delete_pipeline(request)
         await stream.send_message(response)
 
-    async def __rpc_get_steps(
-        self, stream: "grpclib.server.Stream[GetStepsRequest, GetStepsResponse]"
+    async def __rpc_attach_pipeline(
+        self, stream: "grpclib.server.Stream[AttachPipelineRequest, StandardResponse]"
     ) -> None:
         request = await stream.recv_message()
-        response = await self.get_steps(request)
+        response = await self.attach_pipeline(request)
         await stream.send_message(response)
 
-    async def __rpc_create_step(
-        self, stream: "grpclib.server.Stream[CreateStepRequest, CreateStepResponse]"
+    async def __rpc_detach_pipeline(
+        self, stream: "grpclib.server.Stream[DetachPipelineRequest, StandardResponse]"
     ) -> None:
         request = await stream.recv_message()
-        response = await self.create_step(request)
+        response = await self.detach_pipeline(request)
         await stream.send_message(response)
 
-    async def __rpc_update_step(
-        self, stream: "grpclib.server.Stream[UpdateStepRequest, UpdateStepResponse]"
+    async def __rpc_pause_pipeline(
+        self, stream: "grpclib.server.Stream[PausePipelineRequest, StandardResponse]"
     ) -> None:
         request = await stream.recv_message()
-        response = await self.update_step(request)
+        response = await self.pause_pipeline(request)
         await stream.send_message(response)
 
-    async def __rpc_delete_step(
-        self, stream: "grpclib.server.Stream[DeleteStepRequest, DeleteStepResponse]"
+    async def __rpc_resume_pipeline(
+        self, stream: "grpclib.server.Stream[ResumePipelineRequest, StandardResponse]"
     ) -> None:
         request = await stream.recv_message()
-        response = await self.delete_step(request)
+        response = await self.resume_pipeline(request)
         await stream.send_message(response)
 
     async def __rpc_test(
         self, stream: "grpclib.server.Stream[TestRequest, TestResponse]"
     ) -> None:
         request = await stream.recv_message()
         response = await self.test(request)
         await stream.send_message(response)
 
     def __mapping__(self) -> Dict[str, grpclib.const.Handler]:
         return {
-            "/protos.External/GetServices": grpclib.const.Handler(
-                self.__rpc_get_services,
-                grpclib.const.Cardinality.UNARY_UNARY,
-                GetServicesRequest,
-                GetServicesResponse,
-            ),
-            "/protos.External/GetService": grpclib.const.Handler(
-                self.__rpc_get_service,
+            "/protos.External/GetServiceMap": grpclib.const.Handler(
+                self.__rpc_get_service_map,
                 grpclib.const.Cardinality.UNARY_UNARY,
-                GetServiceRequest,
-                GetServiceResponse,
+                GetServiceMapRequest,
+                GetServiceMapResponse,
             ),
             "/protos.External/GetPipelines": grpclib.const.Handler(
                 self.__rpc_get_pipelines,
                 grpclib.const.Cardinality.UNARY_UNARY,
                 GetPipelinesRequest,
                 GetPipelinesResponse,
             ),
             "/protos.External/GetPipeline": grpclib.const.Handler(
                 self.__rpc_get_pipeline,
                 grpclib.const.Cardinality.UNARY_UNARY,
                 GetPipelineRequest,
                 GetPipelineResponse,
             ),
-            "/protos.External/SetPipeline": grpclib.const.Handler(
-                self.__rpc_set_pipeline,
+            "/protos.External/CreatePipeline": grpclib.const.Handler(
+                self.__rpc_create_pipeline,
                 grpclib.const.Cardinality.UNARY_UNARY,
-                SetPipelineRequest,
-                SetPipelineResponse,
+                CreatePipelineRequest,
+                StandardResponse,
+            ),
+            "/protos.External/UpdatePipeline": grpclib.const.Handler(
+                self.__rpc_update_pipeline,
+                grpclib.const.Cardinality.UNARY_UNARY,
+                UpdatePipelineRequest,
+                StandardResponse,
             ),
             "/protos.External/DeletePipeline": grpclib.const.Handler(
                 self.__rpc_delete_pipeline,
                 grpclib.const.Cardinality.UNARY_UNARY,
                 DeletePipelineRequest,
-                DeletePipelineResponse,
+                StandardResponse,
             ),
-            "/protos.External/GetSteps": grpclib.const.Handler(
-                self.__rpc_get_steps,
+            "/protos.External/AttachPipeline": grpclib.const.Handler(
+                self.__rpc_attach_pipeline,
                 grpclib.const.Cardinality.UNARY_UNARY,
-                GetStepsRequest,
-                GetStepsResponse,
+                AttachPipelineRequest,
+                StandardResponse,
             ),
-            "/protos.External/CreateStep": grpclib.const.Handler(
-                self.__rpc_create_step,
+            "/protos.External/DetachPipeline": grpclib.const.Handler(
+                self.__rpc_detach_pipeline,
                 grpclib.const.Cardinality.UNARY_UNARY,
-                CreateStepRequest,
-                CreateStepResponse,
+                DetachPipelineRequest,
+                StandardResponse,
             ),
-            "/protos.External/UpdateStep": grpclib.const.Handler(
-                self.__rpc_update_step,
+            "/protos.External/PausePipeline": grpclib.const.Handler(
+                self.__rpc_pause_pipeline,
                 grpclib.const.Cardinality.UNARY_UNARY,
-                UpdateStepRequest,
-                UpdateStepResponse,
+                PausePipelineRequest,
+                StandardResponse,
             ),
-            "/protos.External/DeleteStep": grpclib.const.Handler(
-                self.__rpc_delete_step,
+            "/protos.External/ResumePipeline": grpclib.const.Handler(
+                self.__rpc_resume_pipeline,
                 grpclib.const.Cardinality.UNARY_UNARY,
-                DeleteStepRequest,
-                DeleteStepResponse,
+                ResumePipelineRequest,
+                StandardResponse,
             ),
             "/protos.External/Test": grpclib.const.Handler(
                 self.__rpc_test,
                 grpclib.const.Cardinality.UNARY_UNARY,
                 TestRequest,
                 TestResponse,
             ),
         }
-
-
-class InternalBase(ServiceBase):
-    async def register(
-        self, register_request: "RegisterRequest"
-    ) -> AsyncIterator["CommandResponse"]:
-        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
-        yield CommandResponse()
-
-    async def heartbeat(
-        self, heartbeat_request: "HeartbeatRequest"
-    ) -> "StandardResponse":
-        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
-
-    async def notify(self, notify_request: "NotifyRequest") -> "StandardResponse":
-        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
-
-    async def metrics(self, metrics_request: "MetricsRequest") -> "StandardResponse":
-        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
-
-    async def __rpc_register(
-        self, stream: "grpclib.server.Stream[RegisterRequest, CommandResponse]"
-    ) -> None:
-        request = await stream.recv_message()
-        await self._call_rpc_handler_server_stream(
-            self.register,
-            stream,
-            request,
-        )
-
-    async def __rpc_heartbeat(
-        self, stream: "grpclib.server.Stream[HeartbeatRequest, StandardResponse]"
-    ) -> None:
-        request = await stream.recv_message()
-        response = await self.heartbeat(request)
-        await stream.send_message(response)
-
-    async def __rpc_notify(
-        self, stream: "grpclib.server.Stream[NotifyRequest, StandardResponse]"
-    ) -> None:
-        request = await stream.recv_message()
-        response = await self.notify(request)
-        await stream.send_message(response)
-
-    async def __rpc_metrics(
-        self, stream: "grpclib.server.Stream[MetricsRequest, StandardResponse]"
-    ) -> None:
-        request = await stream.recv_message()
-        response = await self.metrics(request)
-        await stream.send_message(response)
-
-    def __mapping__(self) -> Dict[str, grpclib.const.Handler]:
-        return {
-            "/protos.Internal/Register": grpclib.const.Handler(
-                self.__rpc_register,
-                grpclib.const.Cardinality.UNARY_STREAM,
-                RegisterRequest,
-                CommandResponse,
-            ),
-            "/protos.Internal/Heartbeat": grpclib.const.Handler(
-                self.__rpc_heartbeat,
-                grpclib.const.Cardinality.UNARY_UNARY,
-                HeartbeatRequest,
-                StandardResponse,
-            ),
-            "/protos.Internal/Notify": grpclib.const.Handler(
-                self.__rpc_notify,
-                grpclib.const.Cardinality.UNARY_UNARY,
-                NotifyRequest,
-                StandardResponse,
-            ),
-            "/protos.Internal/Metrics": grpclib.const.Handler(
-                self.__rpc_metrics,
-                grpclib.const.Cardinality.UNARY_UNARY,
-                MetricsRequest,
-                StandardResponse,
-            ),
-        }
```

### Comparing `snitch-protos-0.0.47/snitch_protos/protos/steps/__init__.py` & `snitch-protos-0.0.48/snitch_protos/protos/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `snitch-protos-0.0.47/snitch_protos.egg-info/PKG-INFO` & `snitch-protos-0.0.48/snitch_protos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snitch-protos
-Version: 0.0.47
+Version: 0.0.48
 Summary: Protobuf python package for Streamdal.com Snitch
 Home-page: https://github.com/streamdal/snitch-protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

