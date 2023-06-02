# Comparing `tmp/langchainplus_sdk-0.0.2.tar.gz` & `tmp/langchainplus_sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchainplus_sdk-0.0.2.tar", max compression
+gzip compressed data, was "langchainplus_sdk-0.0.3.tar", max compression
```

## Comparing `langchainplus_sdk-0.0.2.tar` & `langchainplus_sdk-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0     6974 2023-06-02 03:35:04.040844 langchainplus_sdk-0.0.2/README.md
--rw-r--r--   0        0        0      119 2023-06-02 03:35:04.040844 langchainplus_sdk-0.0.2/langchainplus_sdk/__init__.py
--rw-r--r--   0        0        0    17480 2023-06-02 03:35:04.040844 langchainplus_sdk-0.0.2/langchainplus_sdk/client.py
--rw-r--r--   0        0        0     6994 2023-06-02 03:35:04.040844 langchainplus_sdk-0.0.2/langchainplus_sdk/run_trees.py
--rw-r--r--   0        0        0     6893 2023-06-02 03:35:04.040844 langchainplus_sdk-0.0.2/langchainplus_sdk/schemas.py
--rw-r--r--   0        0        0     2801 2023-06-02 03:35:04.040844 langchainplus_sdk-0.0.2/langchainplus_sdk/utils.py
--rw-r--r--   0        0        0      792 2023-06-02 03:35:04.040844 langchainplus_sdk-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     7607 1970-01-01 00:00:00.000000 langchainplus_sdk-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     8124 2023-06-02 21:13:33.795742 langchainplus_sdk-0.0.3/README.md
+-rw-r--r--   0        0        0      529 2023-06-02 21:13:33.795742 langchainplus_sdk-0.0.3/langchainplus_sdk/__init__.py
+-rw-r--r--   0        0        0    18507 2023-06-02 21:13:33.799742 langchainplus_sdk-0.0.3/langchainplus_sdk/client.py
+-rw-r--r--   0        0        0      250 2023-06-02 21:13:33.799742 langchainplus_sdk-0.0.3/langchainplus_sdk/evaluation/__init__.py
+-rw-r--r--   0        0        0      738 2023-06-02 21:13:33.799742 langchainplus_sdk-0.0.3/langchainplus_sdk/evaluation/evaluator.py
+-rw-r--r--   0        0        0     1545 2023-06-02 21:13:33.799742 langchainplus_sdk-0.0.3/langchainplus_sdk/evaluation/string_evaluator.py
+-rw-r--r--   0        0        0     7178 2023-06-02 21:13:33.799742 langchainplus_sdk-0.0.3/langchainplus_sdk/run_trees.py
+-rw-r--r--   0        0        0     7001 2023-06-02 21:13:33.799742 langchainplus_sdk-0.0.3/langchainplus_sdk/schemas.py
+-rw-r--r--   0        0        0     3235 2023-06-02 21:13:33.799742 langchainplus_sdk-0.0.3/langchainplus_sdk/utils.py
+-rw-r--r--   0        0        0      782 2023-06-02 21:13:33.799742 langchainplus_sdk-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8739 1970-01-01 00:00:00.000000 langchainplus_sdk-0.0.3/PKG-INFO
```

### Comparing `langchainplus_sdk-0.0.2/README.md` & `langchainplus_sdk-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 Note: Save the API Key in a secure location. It will not be shown again.
 
 ## 2. Log Traces
 
 You can log traces natively in your LangChain application or using a LangChainPlus RunTree.
 
-#### Logging Traces with LangChain
+### Logging Traces with LangChain
 
 LangChainPlus seamlessly integrates with the Python LangChain library to record traces from your LLM applications.
 
 1. **Copy the environment variables from the Settings Page and add them to your application.**
 
 Tracing can be activated by setting the following environment variables or by manually specifying the LangChainTracer.
 
@@ -60,15 +60,15 @@
 chat = ChatOpenAI()
 response = chat.predict(
     "Translate this sentence from English to French. I love programming."
 )
 print(response)
 ```
 
-## Logging Traces Outside LangChain
+### Logging Traces Outside LangChain
 
 _Note: this API is experimental and may change in the future_
 
 You can still use the LangChainPlus development platform without depending on any
 LangChain code. You can connect either by setting the appropriate environment variables,
 or by directly specifying the connection information in the RunTree.
 
@@ -155,19 +155,14 @@
 
 ## Create a Dataset from Existing Runs
 
 Once your runs are stored in LangChainPlus, you can convert them into a dataset.
 For this example, we will do so using the Client, but you can also do this using
 the web interface, as explained in the [LangChainPlus docs](https://docs.langchain.plus/docs/).
 
-
-## Additional Documentation
-
-To learn more about the LangChainPlus platform, check out the [docs](https://docs.langchain.plus/docs/).
-
 ```python
 from langchainplus_sdk import LangChainPlusClient
 
 client = LangChainPlusClient()
 dataset_name = "Example Dataset"
 # We will only use examples from the top level AgentExecutor run here,
 # and exclude runs that errored.
@@ -180,9 +175,51 @@
 dataset = client.create_dataset(dataset_name, description="An example dataset")
 for run in runs:
     client.create_example(
         inputs=run.inputs,
         outputs=run.outputs,
         dataset_id=dataset.id,
     )
+```
+
+## Evaluating Runs
+
+You can run evaluations directly using the LangChainPlus client.
+
+```python
+from typing import Optional
+from langchainplus_sdk.evaluation import StringEvaluator
+
+
+def jaccard_chars(output: str, answer: str) -> float:
+    """Naive Jaccard similarity between two strings."""
+    prediction_chars = set(output.strip().lower())
+    answer_chars = set(answer.strip().lower())
+    intersection = prediction_chars.intersection(answer_chars)
+    union = prediction_chars.union(answer_chars)
+    return len(intersection) / len(union)
+
+
+def grader(run_input: str, run_output: str, answer: Optional[str]) -> dict:
+    """Compute the score and/or label for this run."""
+    if answer is None:
+        value = "AMBIGUOUS"
+        score = 0.5
+    else:
+        score = jaccard_chars(run_output, answer)
+        value = "CORRECT" if score > 0.9 else "INCORRECT"
+    return dict(score=score, value=value)
 
-```
+evaluator = StringEvaluator(evaluation_name="Jaccard", grading_function=grader)
+
+runs = client.list_runs(
+    session_name="my_session",
+    execution_order=1,
+    error=False,
+)
+for run in runs:
+    client.evaluate_run(run, evaluator)
+```
+
+## Additional Documentation
+
+To learn more about the LangChainPlus platform, check out the [docs](https://docs.langchain.plus/docs/).
```

### Comparing `langchainplus_sdk-0.0.2/langchainplus_sdk/client.py` & `langchainplus_sdk-0.0.3/langchainplus_sdk/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from tenacity import (
     before_sleep_log,
     retry_if_exception_type,
     stop_after_attempt,
     wait_exponential,
 )
 
+from langchainplus_sdk.evaluation.evaluator import RunEvaluator
 from langchainplus_sdk.schemas import (
     APIFeedbackSource,
     Dataset,
     DatasetCreate,
     Example,
     ExampleCreate,
     ExampleUpdate,
@@ -43,14 +44,16 @@
     ListRunsQueryParams,
     ModelFeedbackSource,
     Run,
     TracerSession,
 )
 from langchainplus_sdk.utils import (
     LangChainPlusAPIError,
+    LangChainPlusError,
+    LangChainPlusUserError,
     raise_for_status_with_text,
     request_with_retries,
     xor_args,
 )
 
 if TYPE_CHECKING:
     import pandas as pd
@@ -92,24 +95,24 @@
     @root_validator(pre=True)
     def validate_api_key_if_hosted(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Verify API key is provided if url not localhost."""
         api_url: str = values.get("api_url", "http://localhost:1984")
         api_key: Optional[str] = values.get("api_key")
         if not _is_localhost(api_url):
             if not api_key:
-                raise ValueError(
+                raise LangChainPlusUserError(
                     "API key must be provided when using hosted LangChain+ API"
                 )
         return values
 
     def _repr_html_(self) -> str:
         """Return an HTML representation of the instance with a link to the URL."""
         if _is_localhost(self.api_url):
             link = "http://localhost"
-        elif "dev" in self.api_url.split("."):
+        elif "dev" in self.api_url.split(".", maxsplit=1)[0]:
             link = "https://dev.langchain.plus"
         else:
             link = "https://www.langchain.plus"
         return f'<a href="{link}", target="_blank" rel="noopener">LangChain+ Client</a>'
 
     def __repr__(self) -> str:
         """Return a string representation of the instance with a link to the URL."""
@@ -239,26 +242,19 @@
         params: Dict[str, Any] = {"limit": 1}
         if session_id is not None:
             path += f"/{session_id}"
         elif session_name is not None:
             params["name"] = session_name
         else:
             raise ValueError("Must provide session_name or session_id")
-        response = self._get_with_retries(
-            path,
-            params=params,
-        )
-        response = self._get_with_retries(
-            path,
-            params=params,
-        )
+        response = self._get_with_retries(path, params=params)
         result = response.json()
         if isinstance(result, list):
             if len(result) == 0:
-                raise ValueError(f"Session {session_name} not found")
+                raise LangChainPlusError(f"Session {session_name} not found")
             return TracerSession(**result[0])
         return TracerSession(**response.json())
 
     def list_sessions(self) -> Iterator[TracerSession]:
         """List sessions from the LangChain+ API."""
         response = self._get_with_retries("/sessions")
         yield from [TracerSession(**session) for session in response.json()]
@@ -313,15 +309,15 @@
         response = self._get_with_retries(
             path,
             params=params,
         )
         result = response.json()
         if isinstance(result, list):
             if len(result) == 0:
-                raise ValueError(f"Dataset {dataset_name} not found")
+                raise LangChainPlusError(f"Dataset {dataset_name} not found")
             return Dataset(**result[0])
         return Dataset(**result)
 
     def list_datasets(self, limit: int = 100) -> Iterator[Dataset]:
         """List the datasets on the LangChain+ API."""
         response = self._get_with_retries("/datasets", params={"limit": limit})
         yield from [Dataset(**dataset) for dataset in response.json()]
@@ -420,14 +416,44 @@
         response = requests.delete(
             f"{self.api_url}/examples/{example_id}",
             headers=self._headers,
         )
         raise_for_status_with_text(response)
         return Example(**response.json())
 
+    def evaluate_run(
+        self,
+        run: Union[Run, str, UUID],
+        evaluator: RunEvaluator,
+    ) -> Feedback:
+        """Evaluate a run."""
+        if isinstance(run, (str, UUID)):
+            run_ = self.read_run(run)
+        elif isinstance(run, Run):
+            run_ = run
+        else:
+            raise TypeError(f"Invalid run type: {type(run)}")
+        if run_.reference_example_id is not None:
+            reference_example = self.read_example(run_.reference_example_id)
+        else:
+            reference_example = None
+        feedback_result = evaluator.evaluate_run(
+            run_,
+            example=reference_example,
+        )
+        return self.create_feedback(
+            run_.id,
+            feedback_result.key,
+            score=feedback_result.score,
+            value=feedback_result.value,
+            comment=feedback_result.comment,
+            correction=feedback_result.correction,
+            feedback_source_type=FeedbackSourceType.MODEL,
+        )
+
     def create_feedback(
         self,
         run_id: ID_TYPE,
         key: str,
         *,
         score: Union[float, int, bool, None] = None,
         value: Union[float, int, bool, str, dict, None] = None,
```

### Comparing `langchainplus_sdk-0.0.2/langchainplus_sdk/run_trees.py` & `langchainplus_sdk-0.0.3/langchainplus_sdk/run_trees.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,29 +13,33 @@
     before_sleep_log,
     retry_if_exception_type,
     stop_after_attempt,
     wait_exponential_jitter,
 )
 
 from langchainplus_sdk.schemas import RunBase, RunTypeEnum, RunUpdate
-from langchainplus_sdk.utils import LangChainPlusAPIError, request_with_retries
+from langchainplus_sdk.utils import (
+    LangChainPlusAPIError,
+    get_runtime_environment,
+    request_with_retries,
+)
 
 logger = logging.getLogger(__name__)
 _THREAD_POOL_EXECUTOR: Optional[ThreadPoolExecutor] = None
 
 
 def _ensure_thread_pool() -> ThreadPoolExecutor:
     """Ensure a thread pool exists in the current context."""
     global _THREAD_POOL_EXECUTOR
     if _THREAD_POOL_EXECUTOR is None:
         _THREAD_POOL_EXECUTOR = ThreadPoolExecutor(max_workers=1)
     return _THREAD_POOL_EXECUTOR
 
 
-def flush_all_runs() -> None:
+def await_all_runs() -> None:
     """Flush the thread pool."""
     global _THREAD_POOL_EXECUTOR
     if _THREAD_POOL_EXECUTOR is not None:
         _THREAD_POOL_EXECUTOR.shutdown(wait=True)
         _THREAD_POOL_EXECUTOR = None
 
 
@@ -89,14 +93,17 @@
             values["execution_order"] = 1
         if "child_execution_order" not in values:
             values["child_execution_order"] = values["execution_order"]
         if values.get("session_name") is None:
             values["session_name"] = os.environ.get("LANGCHAIN_SESSION", "default")
         if values.get("parent_run") is not None:
             values["parent_run_id"] = values["parent_run"].id
+        extra = values.get("extra", {})
+        extra["runtime"] = get_runtime_environment()
+        values["extra"] = extra
         return values
 
     @property
     def _headers(self) -> Dict[str, str]:
         headers = {"Content-Type": "application/json"}
         if self.api_key:
             headers["x-api-key"] = self.api_key
@@ -191,10 +198,10 @@
             },
             retry_config=self.retry_config,
         )
 
     def patch(self) -> Future:
         """Patch the run tree to the API in a background thread."""
         executor = _ensure_thread_pool()
-        run_update = RunUpdate(**self.dict())
+        run_update = RunUpdate(**self.dict(exclude_none=True))
         data = run_update.json(exclude_none=True)
         return executor.submit(self._patch, data=data)
```

### Comparing `langchainplus_sdk-0.0.2/langchainplus_sdk/schemas.py` & `langchainplus_sdk-0.0.3/langchainplus_sdk/schemas.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 """Schemas for the langchainplus API."""
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
-from typing import Any, Dict, List, Mapping, Optional, Sequence, Union
+from typing import Any, Dict, List, Optional, Sequence, Union
 from uuid import UUID, uuid4
 
-from pydantic import BaseModel, Field, root_validator
+from pydantic import (
+    BaseModel,
+    Field,
+    StrictBool,
+    StrictFloat,
+    StrictInt,
+    root_validator,
+)
 from typing_extensions import Literal
 
+SCORE_TYPE = Union[StrictBool, StrictInt, StrictFloat, None]
+VALUE_TYPE = Union[Dict, StrictBool, StrictInt, StrictFloat, str, None]
+
 
 class ExampleBase(BaseModel):
     """Example base model."""
 
     dataset_id: UUID
     inputs: Dict[str, Any]
     outputs: Optional[Dict[str, Any]] = Field(default=None)
@@ -98,14 +108,15 @@
     run_type: RunTypeEnum
     parent_run_id: Optional[UUID]
 
 
 class Run(RunBase):
     """Run schema when loading from the DB."""
 
+    id: UUID
     name: str
     child_runs: List[Run] = Field(default_factory=list)
 
     @root_validator(pre=True)
     def assign_name(cls, values: dict) -> dict:
         """Assign name to the run."""
         if "name" not in values:
@@ -203,45 +214,43 @@
     """The time the feedback was created."""
     modified_at: datetime = Field(default_factory=datetime.utcnow)
     """The time the feedback was last modified."""
     run_id: UUID
     """The associated run ID this feedback is logged for."""
     key: str
     """The metric name, tag, or aspect to provide feedback on."""
-    score: Union[float, int, bool, None] = None
+    score: SCORE_TYPE = None
     """Value or score to assign the run."""
-    value: Union[float, int, bool, str, dict, None] = None
+    value: VALUE_TYPE = None
     """The display value, tag or other value for the feedback if not a metric."""
     comment: Optional[str] = None
     """Comment or explanation for the feedback."""
     correction: Union[str, dict, None] = None
     """Correction for the run."""
-    feedback_source: Optional[
-        Union[APIFeedbackSource, ModelFeedbackSource, Mapping[str, Any]]
-    ] = None
+    feedback_source: Optional[FeedbackSourceBase] = None
     """The source of the feedback."""
 
     class Config:
         frozen = True
 
 
 class FeedbackCreate(FeedbackBase):
     """Schema used for creating feedback."""
 
     id: UUID = Field(default_factory=uuid4)
 
-    feedback_source: APIFeedbackSource
+    feedback_source: FeedbackSourceBase
     """The source of the feedback."""
 
 
 class Feedback(FeedbackBase):
     """Schema for getting feedback."""
 
     id: UUID
-    feedback_source: Optional[Dict] = None
+    feedback_source: Optional[FeedbackSourceBase] = None
     """The source of the feedback. In this case"""
 
 
 class ListFeedbackQueryParams(BaseModel):
     """Query Params for listing feedbacks."""
 
     run: Optional[Sequence[UUID]] = None
@@ -255,12 +264,11 @@
         frozen = True
 
 
 class TracerSession(BaseModel):
     """TracerSession schema for the V2 API."""
 
     id: UUID
-
     start_time: datetime = Field(default_factory=datetime.utcnow)
     name: Optional[str] = None
     extra: Optional[Dict[str, Any]] = None
     tenant_id: UUID
```

### Comparing `langchainplus_sdk-0.0.2/langchainplus_sdk/utils.py` & `langchainplus_sdk-0.0.3/langchainplus_sdk/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Generic utility functions."""
+import platform
+from functools import lru_cache
 from typing import Any, Callable, Mapping, Tuple
 
 import requests
 from requests import HTTPError, Response
 from tenacity import Retrying
 
 
@@ -70,7 +72,21 @@
 
 def raise_for_status_with_text(response: Response) -> None:
     """Raise an error with the response text."""
     try:
         response.raise_for_status()
     except HTTPError as e:
         raise ValueError(response.text) from e
+
+
+@lru_cache(maxsize=1)
+def get_runtime_environment() -> dict:
+    """Get information about the environment."""
+    # Lazy import to avoid circular imports
+    from langchainplus_sdk import __version__
+
+    return {
+        "library_version": __version__,
+        "platform": platform.platform(),
+        "runtime": "python",
+        "runtime_version": platform.python_version(),
+    }
```

### Comparing `langchainplus_sdk-0.0.2/pyproject.toml` & `langchainplus_sdk-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "langchainplus-sdk"
-version = "0.0.2"
+version = "0.0.3"
 description = "Client library to connect to the LangChainPlus LLM Tracing and Evaluation Platform."
 authors = ["LangChain"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "langchainplus_sdk"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-pydantic = "^1.10.8"
-requests = "^2.31.0"
-tenacity = "^8.2.2"
+pydantic = "^1"
+requests = "^2"
+tenacity = "^8.1.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 black = "^23.3.0"
 mypy = "^1.3.0"
 ruff = "^0.0.270"
```

### Comparing `langchainplus_sdk-0.0.2/PKG-INFO` & `langchainplus_sdk-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: langchainplus-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Client library to connect to the LangChainPlus LLM Tracing and Evaluation Platform.
 License: MIT
 Author: LangChain
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=1.10.8,<2.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: tenacity (>=8.2.2,<9.0.0)
+Requires-Dist: pydantic (>=1,<2)
+Requires-Dist: requests (>=2,<3)
+Requires-Dist: tenacity (>=8.1.0,<9.0.0)
 Description-Content-Type: text/markdown
 
 # LangChainPlus Client SDK
 
 This package contains the Python client for interacting with the [LangChainPlus platform](https://www.langchain.plus/).
 
 To install:
@@ -45,15 +45,15 @@
 
 Note: Save the API Key in a secure location. It will not be shown again.
 
 ## 2. Log Traces
 
 You can log traces natively in your LangChain application or using a LangChainPlus RunTree.
 
-#### Logging Traces with LangChain
+### Logging Traces with LangChain
 
 LangChainPlus seamlessly integrates with the Python LangChain library to record traces from your LLM applications.
 
 1. **Copy the environment variables from the Settings Page and add them to your application.**
 
 Tracing can be activated by setting the following environment variables or by manually specifying the LangChainTracer.
 
@@ -77,15 +77,15 @@
 chat = ChatOpenAI()
 response = chat.predict(
     "Translate this sentence from English to French. I love programming."
 )
 print(response)
 ```
 
-## Logging Traces Outside LangChain
+### Logging Traces Outside LangChain
 
 _Note: this API is experimental and may change in the future_
 
 You can still use the LangChainPlus development platform without depending on any
 LangChain code. You can connect either by setting the appropriate environment variables,
 or by directly specifying the connection information in the RunTree.
 
@@ -172,19 +172,14 @@
 
 ## Create a Dataset from Existing Runs
 
 Once your runs are stored in LangChainPlus, you can convert them into a dataset.
 For this example, we will do so using the Client, but you can also do this using
 the web interface, as explained in the [LangChainPlus docs](https://docs.langchain.plus/docs/).
 
-
-## Additional Documentation
-
-To learn more about the LangChainPlus platform, check out the [docs](https://docs.langchain.plus/docs/).
-
 ```python
 from langchainplus_sdk import LangChainPlusClient
 
 client = LangChainPlusClient()
 dataset_name = "Example Dataset"
 # We will only use examples from the top level AgentExecutor run here,
 # and exclude runs that errored.
@@ -197,9 +192,52 @@
 dataset = client.create_dataset(dataset_name, description="An example dataset")
 for run in runs:
     client.create_example(
         inputs=run.inputs,
         outputs=run.outputs,
         dataset_id=dataset.id,
     )
+```
+
+## Evaluating Runs
+
+You can run evaluations directly using the LangChainPlus client.
+
+```python
+from typing import Optional
+from langchainplus_sdk.evaluation import StringEvaluator
+
+
+def jaccard_chars(output: str, answer: str) -> float:
+    """Naive Jaccard similarity between two strings."""
+    prediction_chars = set(output.strip().lower())
+    answer_chars = set(answer.strip().lower())
+    intersection = prediction_chars.intersection(answer_chars)
+    union = prediction_chars.union(answer_chars)
+    return len(intersection) / len(union)
+
+
+def grader(run_input: str, run_output: str, answer: Optional[str]) -> dict:
+    """Compute the score and/or label for this run."""
+    if answer is None:
+        value = "AMBIGUOUS"
+        score = 0.5
+    else:
+        score = jaccard_chars(run_output, answer)
+        value = "CORRECT" if score > 0.9 else "INCORRECT"
+    return dict(score=score, value=value)
 
+evaluator = StringEvaluator(evaluation_name="Jaccard", grading_function=grader)
+
+runs = client.list_runs(
+    session_name="my_session",
+    execution_order=1,
+    error=False,
+)
+for run in runs:
+    client.evaluate_run(run, evaluator)
 ```
+
+## Additional Documentation
+
+To learn more about the LangChainPlus platform, check out the [docs](https://docs.langchain.plus/docs/).
+
```

