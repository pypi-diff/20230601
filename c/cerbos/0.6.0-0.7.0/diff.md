# Comparing `tmp/cerbos-0.6.0.tar.gz` & `tmp/cerbos-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbos-0.6.0.tar", last modified: Tue May  2 07:52:54 2023, max compression
+gzip compressed data, was "cerbos-0.7.0.tar", last modified: Thu Jun  1 11:14:16 2023, max compression
```

## Comparing `cerbos-0.6.0.tar` & `cerbos-0.7.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11357 2023-05-02 07:52:27.167645 cerbos-0.6.0/LICENSE
--rw-r--r--   0        0        0     2999 2023-05-02 07:52:27.167645 cerbos-0.6.0/README.md
--rw-r--r--   0        0        0      167 2023-05-02 07:52:27.167645 cerbos-0.6.0/cerbos/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 07:52:27.167645 cerbos-0.6.0/cerbos/sdk/__init__.py
--rw-r--r--   0        0        0    12680 2023-05-02 07:52:27.167645 cerbos-0.6.0/cerbos/sdk/_async/client.py
--rw-r--r--   0        0        0    12492 2023-05-02 07:52:53.752997 cerbos-0.6.0/cerbos/sdk/_sync/client.py
--rw-r--r--   0        0        0      485 2023-05-02 07:52:27.167645 cerbos-0.6.0/cerbos/sdk/client.py
--rw-r--r--   0        0        0      759 2023-05-02 07:52:27.167645 cerbos-0.6.0/cerbos/sdk/container.py
--rw-r--r--   0        0        0     6262 2023-05-02 07:52:27.167645 cerbos-0.6.0/cerbos/sdk/model.py
--rw-r--r--   0        0        0     1800 2023-05-02 07:52:27.167645 cerbos-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0     1303 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/check.py
--rw-r--r--   0        0        0     2017 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0      578 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/_schemas/leave_request.json
--rw-r--r--   0        0        0     1030 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/_schemas/principal.json
--rw-r--r--   0        0        0      402 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/_schemas/purchase_order.json
--rw-r--r--   0        0        0      387 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/_schemas/salary_record.json
--rw-r--r--   0        0        0      451 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/derived_roles/common_roles.yaml
--rw-r--r--   0        0        0      323 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/derived_roles/derived_roles_01.yaml
--rw-r--r--   0        0        0      492 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/derived_roles/derived_roles_02.yaml
--rw-r--r--   0        0        0      599 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/derived_roles/derived_roles_03.yaml
--rw-r--r--   0        0        0      484 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/principal_policies/policy_01.yaml
--rw-r--r--   0        0        0      300 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/principal_policies/policy_02.yaml
--rw-r--r--   0        0        0      226 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/principal_policies/policy_02_acme.hr.yaml
--rw-r--r--   0        0        0      499 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/principal_policies/policy_02_acme.yaml
--rw-r--r--   0        0        0     1587 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/resource_policies/policy_01.yaml
--rw-r--r--   0        0        0      624 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/resource_policies/policy_02.yaml
--rw-r--r--   0        0        0      526 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/resource_policies/policy_03.yaml
--rw-r--r--   0        0        0      689 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/resource_policies/policy_04.yaml
--rw-r--r--   0        0        0      377 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/resource_policies/policy_05.yaml
--rw-r--r--   0        0        0      704 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/resource_policies/policy_05_acme.hr.uk.yaml
--rw-r--r--   0        0        0     1138 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/resource_policies/policy_05_acme.hr.yaml
--rw-r--r--   0        0        0      535 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/resource_policies/policy_05_acme.yaml
--rw-r--r--   0        0        0      450 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/tests/policy_04_test.yaml
--rw-r--r--   0        0        0    16690 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/test_client.py
--rw-r--r--   0        0        0     2061 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/test_plan_response.py
--rw-r--r--   0        0        0     3538 1970-01-01 00:00:00.000000 cerbos-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-31 13:15:16.875866 cerbos-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2999 2023-05-31 13:15:16.875961 cerbos-0.7.0/README.md
+-rw-r--r--   0        0        0      167 2023-05-31 13:15:16.876102 cerbos-0.7.0/cerbos/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 13:15:16.876205 cerbos-0.7.0/cerbos/sdk/__init__.py
+-rw-r--r--   0        0        0    12680 2023-05-31 13:15:16.876440 cerbos-0.7.0/cerbos/sdk/_async/client.py
+-rw-r--r--   0        0        0    12492 2023-06-01 11:14:15.625639 cerbos-0.7.0/cerbos/sdk/_sync/client.py
+-rw-r--r--   0        0        0      485 2023-05-31 13:15:16.876736 cerbos-0.7.0/cerbos/sdk/client.py
+-rw-r--r--   0        0        0      759 2023-05-31 13:15:16.876850 cerbos-0.7.0/cerbos/sdk/container.py
+-rw-r--r--   0        0        0     6414 2023-06-01 11:00:22.813867 cerbos-0.7.0/cerbos/sdk/model.py
+-rw-r--r--   0        0        0     1800 2023-05-31 13:15:16.877903 cerbos-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-31 13:15:16.878037 cerbos-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0     1303 2023-05-31 13:15:16.878187 cerbos-0.7.0/tests/check.py
+-rw-r--r--   0        0        0     2017 2023-06-01 10:46:38.636813 cerbos-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0      578 2023-05-31 13:15:16.878589 cerbos-0.7.0/tests/store/_schemas/leave_request.json
+-rw-r--r--   0        0        0     1030 2023-05-31 13:15:16.878712 cerbos-0.7.0/tests/store/_schemas/principal.json
+-rw-r--r--   0        0        0      402 2023-05-31 13:15:16.878820 cerbos-0.7.0/tests/store/_schemas/purchase_order.json
+-rw-r--r--   0        0        0      387 2023-05-31 13:15:16.878921 cerbos-0.7.0/tests/store/_schemas/salary_record.json
+-rw-r--r--   0        0        0      451 2023-05-31 13:15:16.879097 cerbos-0.7.0/tests/store/derived_roles/common_roles.yaml
+-rw-r--r--   0        0        0      323 2023-05-31 13:15:16.879216 cerbos-0.7.0/tests/store/derived_roles/derived_roles_01.yaml
+-rw-r--r--   0        0        0      492 2023-05-31 13:15:16.879320 cerbos-0.7.0/tests/store/derived_roles/derived_roles_02.yaml
+-rw-r--r--   0        0        0      599 2023-05-31 13:15:16.879415 cerbos-0.7.0/tests/store/derived_roles/derived_roles_03.yaml
+-rw-r--r--   0        0        0      577 2023-06-01 11:00:22.814362 cerbos-0.7.0/tests/store/principal_policies/policy_01.yaml
+-rw-r--r--   0        0        0      300 2023-05-31 13:15:16.879688 cerbos-0.7.0/tests/store/principal_policies/policy_02.yaml
+-rw-r--r--   0        0        0      226 2023-05-31 13:15:16.879796 cerbos-0.7.0/tests/store/principal_policies/policy_02_acme.hr.yaml
+-rw-r--r--   0        0        0      499 2023-05-31 13:15:16.879901 cerbos-0.7.0/tests/store/principal_policies/policy_02_acme.yaml
+-rw-r--r--   0        0        0     2090 2023-06-01 11:00:22.814718 cerbos-0.7.0/tests/store/resource_policies/policy_01.yaml
+-rw-r--r--   0        0        0      624 2023-05-31 13:15:16.880129 cerbos-0.7.0/tests/store/resource_policies/policy_02.yaml
+-rw-r--r--   0        0        0      526 2023-05-31 13:15:16.880219 cerbos-0.7.0/tests/store/resource_policies/policy_03.yaml
+-rw-r--r--   0        0        0      689 2023-05-31 13:15:16.880312 cerbos-0.7.0/tests/store/resource_policies/policy_04.yaml
+-rw-r--r--   0        0        0      377 2023-05-31 13:15:16.880396 cerbos-0.7.0/tests/store/resource_policies/policy_05.yaml
+-rw-r--r--   0        0        0      704 2023-05-31 13:15:16.880469 cerbos-0.7.0/tests/store/resource_policies/policy_05_acme.hr.uk.yaml
+-rw-r--r--   0        0        0     1138 2023-05-31 13:15:16.880539 cerbos-0.7.0/tests/store/resource_policies/policy_05_acme.hr.yaml
+-rw-r--r--   0        0        0      535 2023-05-31 13:15:16.880609 cerbos-0.7.0/tests/store/resource_policies/policy_05_acme.yaml
+-rw-r--r--   0        0        0      450 2023-05-31 13:15:16.880742 cerbos-0.7.0/tests/store/tests/policy_04_test.yaml
+-rw-r--r--   0        0        0    20323 2023-06-01 11:00:22.814961 cerbos-0.7.0/tests/test_client.py
+-rw-r--r--   0        0        0     2061 2023-05-31 13:15:16.880988 cerbos-0.7.0/tests/test_plan_response.py
+-rw-r--r--   0        0        0     3538 1970-01-01 00:00:00.000000 cerbos-0.7.0/PKG-INFO
```

### Comparing `cerbos-0.6.0/LICENSE` & `cerbos-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cerbos-0.6.0/README.md` & `cerbos-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `cerbos-0.6.0/cerbos/sdk/_async/client.py` & `cerbos-0.7.0/cerbos/sdk/_async/client.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.6.0/cerbos/sdk/_sync/client.py` & `cerbos-0.7.0/cerbos/sdk/_sync/client.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.6.0/cerbos/sdk/container.py` & `cerbos-0.7.0/cerbos/sdk/container.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.6.0/cerbos/sdk/model.py` & `cerbos-0.7.0/cerbos/sdk/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,25 +92,33 @@
     path: str
     message: str
     source: Source
 
 
 @dataclass_json(letter_case=LetterCase.CAMEL)
 @dataclass
+class OutputEntry:
+    src: str
+    val: Any
+
+
+@dataclass_json(letter_case=LetterCase.CAMEL)
+@dataclass
 class APIError:
     code: int
     message: str
 
 
 @dataclass_json(letter_case=LetterCase.CAMEL)
 @dataclass
 class CheckResourcesResult:
     resource: Resource
     actions: Dict[str, Effect]
     validation_errors: Optional[List[ValidationError]] = None
+    outputs: Optional[List[OutputEntry]] = None
 
     def is_allowed(self, action: str) -> bool:
         if action in self.actions:
             return self.actions[action] == Effect.ALLOW
 
         return False
```

### Comparing `cerbos-0.6.0/pyproject.toml` & `cerbos-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "requests-toolbelt>=0.9.1",
     "httpx[http2]>=0.22.0",
     "anyio>=3.6.1",
     "tenacity>=8.1.0",
 ]
 requires-python = ">=3.8"
 dynamic = []
-version = "0.6.0"
+version = "0.7.0"
 
 [project.urls]
 Homepage = "https://cerbos.dev"
 
 [project.optional-dependencies]
 testcontainers = [
     "testcontainers>=3.5.3",
```

### Comparing `cerbos-0.6.0/tests/check.py` & `cerbos-0.7.0/tests/check.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.6.0/tests/conftest.py` & `cerbos-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.6.0/tests/store/_schemas/leave_request.json` & `cerbos-0.7.0/tests/store/_schemas/leave_request.json`

 * *Files identical despite different names*

### Comparing `cerbos-0.6.0/tests/store/_schemas/principal.json` & `cerbos-0.7.0/tests/store/_schemas/principal.json`

 * *Files identical despite different names*

### Comparing `cerbos-0.6.0/tests/store/derived_roles/derived_roles_03.yaml` & `cerbos-0.7.0/tests/store/derived_roles/derived_roles_03.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.6.0/tests/store/resource_policies/policy_01.yaml` & `cerbos-0.7.0/tests/store/resource_policies/policy_01.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -34,14 +34,29 @@
       effect: EFFECT_ALLOW
 
     - actions: ["view:public"]
       derivedRoles:
         - any_employee
       effect: EFFECT_ALLOW
       name: public-view
+      output:
+        expr: |-
+          {
+            "pID": P.id,
+            "keys": R.attr.id,
+            "formatted_%s".format(["string"]): "id:%s".format([P.id]),
+            "some_bool": true,
+            "some_list": ["foo", "bar"],
+            "something_nested": {
+              "nested_str": "foo",
+              "nested_bool": false,
+              "nested_list": ["nest_foo", 1.01],
+              "nested_formatted_%s".format(["string"]): "id:%s".format([P.id]),
+            },
+          }
 
     - actions: ["approve"]
       condition:
         match:
           expr: request.resource.attr.status == V.pending_approval
       derivedRoles:
         - direct_manager
```

### Comparing `cerbos-0.6.0/tests/store/resource_policies/policy_02.yaml` & `cerbos-0.7.0/tests/store/resource_policies/policy_02.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.6.0/tests/store/resource_policies/policy_03.yaml` & `cerbos-0.7.0/tests/store/resource_policies/policy_03.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.6.0/tests/store/resource_policies/policy_04.yaml` & `cerbos-0.7.0/tests/store/resource_policies/policy_04.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.6.0/tests/store/resource_policies/policy_05_acme.hr.uk.yaml` & `cerbos-0.7.0/tests/store/resource_policies/policy_05_acme.hr.uk.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.6.0/tests/store/resource_policies/policy_05_acme.hr.yaml` & `cerbos-0.7.0/tests/store/resource_policies/policy_05_acme.hr.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.6.0/tests/store/resource_policies/policy_05_acme.yaml` & `cerbos-0.7.0/tests/store/resource_policies/policy_05_acme.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.6.0/tests/test_client.py` & `cerbos-0.7.0/tests/test_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -69,14 +69,23 @@
         resourcedesc_leave_req_invalid: ResourceDesc,
     ):
         have = cerbos_client.plan_resources(
             "approve", principal_maggie_invalid, resourcedesc_leave_req_invalid
         )
         _assert_plan_resources_validation(have)
 
+    def test_check_resources_with_output(
+        self,
+        cerbos_client: CerbosClient,
+        principal_john: Principal,
+        resource_list: ResourceList,
+    ):
+        have = cerbos_client.check_resources(principal_john, resource_list)
+        _assert_check_resources_with_output(have)
+
     @patch("httpx.Client.post")
     def test_request_retries_on_failure(
         self,
         post_mock,
         principal_john: Principal,
         resource_list: ResourceList,
     ):
@@ -193,14 +202,24 @@
 
     def test_check_resources(
         self, principal_ctx: PrincipalContext, resource_list: ResourceList
     ):
         have = principal_ctx.check_resources(resource_list)
         _assert_check_resources(have)
 
+    def test_check_resources_with_output(
+        self,
+        cerbos_client: CerbosClient,
+        principal_donald: Principal,
+        resource_list: ResourceList,
+    ):
+        principal_ctx_override = cerbos_client.with_principal(principal_donald)
+        have = principal_ctx_override.check_resources(resource_list)
+        _assert_check_resources_principal_override_with_output(have)
+
     def test_plan_resources(
         self, principal_ctx: PrincipalContext, resourcedesc_leave_req: ResourceDesc
     ):
         have = principal_ctx.plan_resources("view:*", resourcedesc_leave_req)
         _assert_plan_resources(have)
 
 
@@ -263,14 +282,23 @@
         resourcedesc_leave_req_invalid: ResourceDesc,
     ):
         have = await cerbos_async_client.plan_resources(
             "approve", principal_maggie_invalid, resourcedesc_leave_req_invalid
         )
         _assert_plan_resources_validation(have)
 
+    async def test_check_resources_with_output(
+        self,
+        cerbos_async_client: AsyncCerbosClient,
+        principal_john: Principal,
+        resource_list: ResourceList,
+    ):
+        have = await cerbos_async_client.check_resources(principal_john, resource_list)
+        _assert_check_resources_with_output(have)
+
     @patch("httpx.AsyncClient.post")
     async def test_request_retries_on_failure(
         self,
         post_mock,
         principal_john: Principal,
         resource_list: ResourceList,
     ):
@@ -398,14 +426,26 @@
 
     async def test_check_resources(
         self, async_principal_ctx: AsyncPrincipalContext, resource_list: ResourceList
     ):
         have = await async_principal_ctx.check_resources(resource_list)
         _assert_check_resources(have)
 
+    async def test_check_resources_with_output(
+        self,
+        cerbos_async_client: AsyncCerbosClient,
+        principal_donald: Principal,
+        resource_list: ResourceList,
+    ):
+        async_principal_ctx_override = cerbos_async_client.with_principal(
+            principal_donald
+        )
+        have = await async_principal_ctx_override.check_resources(resource_list)
+        _assert_check_resources_principal_override_with_output(have)
+
     async def test_plan_resources(
         self,
         async_principal_ctx: AsyncPrincipalContext,
         resourcedesc_leave_req: ResourceDesc,
     ):
         have = await async_principal_ctx.plan_resources(
             "view:*", resourcedesc_leave_req
@@ -454,14 +494,71 @@
     assert have.resource_kind == "leave_request"
     assert have.policy_version == "20210210"
     assert have.filter.kind == PlanResourcesFilterKind.ALWAYS_DENIED
     assert have.filter.condition is None
     assert len(have.validation_errors) == 2
 
 
+def _assert_check_resources_with_output(have: CheckResourcesResponse):
+    xx125 = have.get_resource(
+        "XX125", predicate=lambda r: r.policy_version == "20210210"
+    )
+    assert xx125 is not None
+    assert len(xx125.outputs) == 1
+    outputs = xx125.outputs[0].to_dict()
+    assert outputs == {
+        "src": "cerbos.resource.leave_request.v20210210#public-view",
+        "val": {
+            "formatted_string": "id:john",
+            "keys": "XX125",
+            "pID": "john",
+            "some_bool": True,
+            "some_list": ["foo", "bar"],
+            "something_nested": {
+                "nested_bool": False,
+                "nested_formatted_string": "id:john",
+                "nested_list": ["nest_foo", 1.01],
+                "nested_str": "foo",
+            },
+        },
+    }
+
+
+def _assert_check_resources_principal_override_with_output(
+    have: CheckResourcesResponse,
+):
+    xx125 = have.get_resource(
+        "XX125", predicate=lambda r: r.policy_version == "20210210"
+    )
+    assert xx125 is not None
+    assert len(xx125.outputs) == 2
+    s = next(filter(lambda x: isinstance(x.val, str), xx125.outputs))
+    d = next(filter(lambda x: isinstance(x.val, dict), xx125.outputs))
+    assert s.to_dict() == {
+        "src": "cerbos.principal.donald_duck.v20210210#dev_admin",
+        "val": "dev_record_override:donald_duck",
+    }
+    assert d.to_dict() == {
+        "src": "cerbos.resource.leave_request.v20210210#public-view",
+        "val": {
+            "formatted_string": "id:donald_duck",
+            "keys": "XX125",
+            "pID": "donald_duck",
+            "some_bool": True,
+            "some_list": ["foo", "bar"],
+            "something_nested": {
+                "nested_bool": False,
+                "nested_formatted_string": "id:donald_duck",
+                "nested_list": ["nest_foo", 1.01],
+                "nested_str": "foo",
+            },
+        },
+    }
+
+
 @pytest.fixture
 def principal_ctx(cerbos_client, principal_john):
     return cerbos_client.with_principal(principal_john)
 
 
 @pytest.fixture
 def async_principal_ctx(cerbos_async_client, principal_john):
@@ -553,14 +650,24 @@
             "managed_geographies": "GB",
             "team": "design",
         },
     )
 
 
 @pytest.fixture
+def principal_donald():
+    return Principal(
+        "donald_duck",
+        roles={"employee"},
+        policy_version="20210210",
+        attr={"department": "engineering", "geography": "GB", "team": "QA"},
+    )
+
+
+@pytest.fixture
 def principal_maggie_invalid():
     return Principal(
         "maggie",
         roles={"manager"},
         policy_version="20210210",
         attr={
             "reader": False,
```

### Comparing `cerbos-0.6.0/tests/test_plan_response.py` & `cerbos-0.7.0/tests/test_plan_response.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.6.0/PKG-INFO` & `cerbos-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbos
-Version: 0.6.0
+Version: 0.7.0
 Summary: SDK for working with Cerbos: an open core, language-agnostic, scalable authorization solution
 License: Apache-2.0
 Author-email: Cerbos Developers <sdk+python@cerbos.dev>
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
```

