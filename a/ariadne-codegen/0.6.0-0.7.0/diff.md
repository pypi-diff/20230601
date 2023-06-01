# Comparing `tmp/ariadne_codegen-0.6.0.tar.gz` & `tmp/ariadne_codegen-0.7.0.tar.gz`

## Comparing `ariadne_codegen-0.6.0.tar` & `ariadne_codegen-0.7.0.tar`

### file list

```diff
@@ -1,45 +1,48 @@
--rw-r--r--   0        0        0    10651 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/EXAMPLE.md
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/__init__.py
--rw-r--r--   0        0        0     8798 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/codegen.py
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/config.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/exceptions.py
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/py.typed
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/schema.py
--rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/settings.py
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/__init__.py
--rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/arguments.py
--rw-r--r--   0        0        0     9557 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/client.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/constants.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/enums.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/init_file.py
--rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/input_fields.py
--rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/input_types.py
--rw-r--r--   0        0        0    14095 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/package.py
--rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/result_fields.py
--rw-r--r--   0        0        0    13819 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/result_types.py
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/scalars.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/dependencies/__init__.py
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/dependencies/async_base_client.py
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/dependencies/base_client.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/dependencies/base_model.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/dependencies/exceptions.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/dependencies/scalars.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/__init__.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/constants.py
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/directives.py
--rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/fields.py
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/named_types.py
--rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/schema.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/plugins/__init__.py
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/plugins/base.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/plugins/explorer.py
--rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/plugins/manager.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/.gitignore
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/LICENSE
--rw-r--r--   0        0        0     9322 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/README.md
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    12143 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/EXAMPLE.md
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/__init__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/__main__.py
+-rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/codegen.py
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/config.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/exceptions.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/py.typed
+-rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/schema.py
+-rw-r--r--   0        0        0     7958 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/settings.py
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/__init__.py
+-rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/arguments.py
+-rw-r--r--   0        0        0    12293 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/client.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/constants.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/enums.py
+-rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/fragments.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/init_file.py
+-rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/input_fields.py
+-rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/input_types.py
+-rw-r--r--   0        0        0    15638 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/package.py
+-rw-r--r--   0        0        0     8810 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/result_fields.py
+-rw-r--r--   0        0        0    20819 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/result_types.py
+-rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/scalars.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/dependencies/__init__.py
+-rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/dependencies/async_base_client.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/dependencies/base_client.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/dependencies/base_model.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/dependencies/exceptions.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/dependencies/scalars.py
+-rw-r--r--   0        0        0    14332 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/contrib/shorter_results.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/__init__.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/constants.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/directives.py
+-rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/fields.py
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/named_types.py
+-rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/schema.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/plugins/__init__.py
+-rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/plugins/base.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/plugins/explorer.py
+-rw-r--r--   0        0        0     7821 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/plugins/manager.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/LICENSE
+-rw-r--r--   0        0        0    11177 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/README.md
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    12859 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/PKG-INFO
```

### Comparing `ariadne_codegen-0.6.0/EXAMPLE.md` & `ariadne_codegen-0.7.0/EXAMPLE.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,18 @@
   mutation: Mutation
 }
 
 type Query {
   users(country: String): [User!]!
 }
 
+type Subscription {
+  usersCounter: Int!
+}
+
 type Mutation {
   userCreate(userData: UserCreateInput!): User
   userPreferences(data: UserPreferencesInput): Boolean!
 }
 
 input UserCreateInput {
   firstName: String
@@ -66,15 +70,15 @@
   receivePushNotifications: Boolean!
   receiveSms: Boolean!
   title: String!
 }
 ```
 
 
-## Queries/mutations file
+## Queries/mutations/subscriptions file
 
 ```gql
 mutation CreateUser($userData: UserCreateInput!) {
     userCreate(userData: $userData) {
         id
     }
 }
@@ -104,14 +108,18 @@
     email
 }
 
 fragment UserPersonalData on User {
     firstName
     lastName
 }
+
+subscription GetUsersCounter {
+    usersCounter
+}
 ```
 
 
 ## Running
 
 Add `[tool.ariadne-codegen]` section to `pyproject.toml` with paths to files with [schema](#schema-file) and [queries/mutations](#queriesmutations-file).
 
@@ -139,32 +147,35 @@
     __init__.py
     async_base_client.py
     base_model.py
     client.py
     create_user.py
     enums.py
     exceptions.py
+    fragments.py
+    get_users_counter.py
     input_types.py
     list_all_users.py
     list_users_by_country.py
     scalars.py
 ```
 
 ### Client class
 
 Generated client class inherits from `AsyncBaseClient` and has async method for every provided query/mutation.
 
 ```py
 # graphql_client/client.py
 
-from typing import Optional, Union
+from typing import AsyncIterator, Optional, Union
 
 from .async_base_client import AsyncBaseClient
 from .base_model import UNSET, UnsetType
 from .create_user import CreateUser
+from .get_users_counter import GetUsersCounter
 from .input_types import UserCreateInput
 from .list_all_users import ListAllUsers
 from .list_users_by_country import ListUsersByCountry
 
 
 def gql(q: str) -> str:
     return q
@@ -231,14 +242,26 @@
             }
             """
         )
         variables: dict[str, object] = {"country": country}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return ListUsersByCountry.parse_obj(data)
+
+    async def get_users_counter(self) -> AsyncIterator[GetUsersCounter]:
+        query = gql(
+            """
+            subscription GetUsersCounter {
+              usersCounter
+            }
+            """
+        )
+        variables: dict[str, object] = {}
+        async for data in self.execute_ws(query=query, variables=variables):
+            yield GetUsersCounter.parse_obj(data)
 ```
 
 ### Base client
 
 Base client is copied from path provided in `base_client_file_path` and has to contain definition of class with name provided in `base_client_name`.
 
 ### Base model
@@ -321,17 +344,17 @@
     WHITE = "WHITE"
     RED = "RED"
     GREEN = "GREEN"
     BLUE = "BLUE"
     YELLOW = "YELLOW"
 ```
 
-### Query/mutation types
+### Query/mutation/subscription types
 
-For every provided query/mutation there is generated file, that contains models which correspond to return type of operation. File name is generated by converting query/mutation name to snake case. Root models has the same name as query/mutation, and depend classes use it as prefix in their names.
+For every provided query/mutation/subscription there is a generated file that contains models which correspond to return type of operation. File name is generated by converting operation name to snake case. Root models has the same name as query/mutation/subscription, and depend classes use it as prefix in their names.
 
 ```py
 # graphql_client/create_user.py
 
 from typing import Optional
 
 from pydantic import Field
@@ -387,30 +410,70 @@
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import Color
+from .fragments import BasicUser, UserPersonalData
 
 
 class ListUsersByCountry(BaseModel):
     users: List["ListUsersByCountryUsers"]
 
 
-class ListUsersByCountryUsers(BaseModel):
+class ListUsersByCountryUsers(BasicUser, UserPersonalData):
+    favourite_color: Optional[Color] = Field(alias="favouriteColor")
+
+
+ListUsersByCountry.update_forward_refs()
+ListUsersByCountryUsers.update_forward_refs()
+```
+
+```py
+# graphql_client/get_users_counter.py
+
+from pydantic import Field
+
+from .base_model import BaseModel
+
+
+class GetUsersCounter(BaseModel):
+    users_counter: int = Field(alias="usersCounter")
+
+
+GetUsersCounter.update_forward_refs()
+```
+
+### Fragments file
+
+This file contains classes generated from all fragments used in any provided operation.
+
+```py
+# graphql_client/fragments.py
+
+from typing import Optional
+
+from pydantic import Field
+
+from .base_model import BaseModel
+
+
+class BasicUser(BaseModel):
     id: str
     email: str
+
+
+class UserPersonalData(BaseModel):
     first_name: Optional[str] = Field(alias="firstName")
     last_name: Optional[str] = Field(alias="lastName")
-    favourite_color: Optional[Color] = Field(alias="favouriteColor")
 
 
-ListUsersByCountry.update_forward_refs()
-ListUsersByCountryUsers.update_forward_refs()
+BasicUser.update_forward_refs()
+UserPersonalData.update_forward_refs()
 ```
 
 ### Init file
 
 Generated init file contains reimports and list of all generated classes.
 
 ```py
@@ -424,39 +487,44 @@
 from .exceptions import (
     GraphQLClientError,
     GraphQLClientGraphQLError,
     GraphQLClientGraphQLMultiError,
     GraphQLClientHttpError,
     GraphQlClientInvalidResponseError,
 )
+from .fragments import BasicUser, UserPersonalData
+from .get_users_counter import GetUsersCounter
 from .input_types import (
     LocationInput,
     NotificationsPreferencesInput,
     UserCreateInput,
     UserPreferencesInput,
 )
 from .list_all_users import ListAllUsers, ListAllUsersUsers, ListAllUsersUsersLocation
 from .list_users_by_country import ListUsersByCountry, ListUsersByCountryUsers
 
 __all__ = [
     "AsyncBaseClient",
     "BaseModel",
+    "BasicUser",
     "Client",
     "Color",
     "CreateUser",
     "CreateUserUserCreate",
+    "GetUsersCounter",
     "GraphQLClientError",
     "GraphQLClientGraphQLError",
     "GraphQLClientGraphQLMultiError",
     "GraphQLClientHttpError",
     "GraphQlClientInvalidResponseError",
     "ListAllUsers",
     "ListAllUsersUsers",
     "ListAllUsersUsersLocation",
     "ListUsersByCountry",
     "ListUsersByCountryUsers",
     "LocationInput",
     "NotificationsPreferencesInput",
     "UserCreateInput",
+    "UserPersonalData",
     "UserPreferencesInput",
 ]
 ```
```

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/codegen.py` & `ariadne_codegen-0.7.0/ariadne_codegen/codegen.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import ast
-from typing import Any, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from graphql import (
     GraphQLEnumType,
     GraphQLInputObjectType,
     GraphQLInterfaceType,
     GraphQLList,
     GraphQLNonNull,
@@ -265,34 +265,23 @@
 
 
 def generate_lambda(body: ast.expr, args: Optional[ast.arguments] = None) -> ast.Lambda:
     """Generate lambda definition."""
     return ast.Lambda(args=args or generate_arguments(), body=body)
 
 
-def generate_field_with_alias(name):
+def generate_pydantic_field(keywords: Dict[str, ast.expr]) -> ast.Call:
     return generate_call(
         func=generate_name(FIELD_CLASS),
         keywords=[
-            generate_keyword(
-                arg="alias",
-                value=generate_constant(name),
-            )
+            generate_keyword(arg=arg, value=value) for arg, value in keywords.items()
         ],
     )
 
 
-def generate_typename_field_definition():
-    return generate_ann_assign(
-        target="__typename__",
-        annotation=generate_name("str"),
-        value=generate_field_with_alias("__typename"),
-    )
-
-
 def generate_module(body: List[ast.stmt]) -> ast.Module:
     return ast.Module(body=body, type_ignores=[])
 
 
 def generate_subscript(value: ast.expr, slice_: ast.expr) -> ast.Subscript:
     return ast.Subscript(value=value, slice=slice_)
 
@@ -312,7 +301,31 @@
         name=name,
         args=arguments,
         body=body if body else [ast.Pass()],
         decorator_list=[],
         returns=return_type,
         lineno=lineno,
     )
+
+
+def generate_async_for(
+    target: ast.expr,
+    iter_: ast.expr,
+    body: Optional[List[ast.stmt]] = None,
+    orelse: Optional[List[ast.stmt]] = None,
+    lineno: int = 1,
+) -> ast.AsyncFor:
+    return ast.AsyncFor(
+        target=target,
+        iter=iter_,
+        body=body or [ast.Pass()],
+        orelse=orelse or [],
+        lineno=lineno,
+    )
+
+
+def generate_yield(value: Optional[ast.expr] = None) -> ast.Yield:
+    return ast.Yield(value=value)
+
+
+def generate_pass() -> ast.Pass:
+    return ast.Pass()
```

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/config.py` & `ariadne_codegen-0.7.0/ariadne_codegen/config.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/exceptions.py` & `ariadne_codegen-0.7.0/ariadne_codegen/exceptions.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/main.py` & `ariadne_codegen-0.7.0/ariadne_codegen/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sys
 
 import click
+from graphql import assert_valid_schema
 
 from .client_generators.package import PackageGenerator
 from .config import get_client_settings, get_config_dict, get_graphql_schema_settings
 from .graphql_schema_generators.schema import generate_graphql_schema_file
 from .plugins.explorer import get_plugins_types
 from .plugins.manager import PluginManager
 from .schema import (
@@ -33,25 +34,34 @@
 
     if strategy == Strategy.GRAPHQL_SCHEMA:
         graphql_schema(config_dict)
 
 
 def client(config_dict):
     settings = get_client_settings(config_dict)
+
     if settings.schema_path:
         schema = get_graphql_schema_from_path(settings.schema_path)
         schema_source = settings.schema_path
     else:
         schema = get_graphql_schema_from_url(
             url=settings.remote_schema_url,
             headers=settings.remote_schema_headers,
             verify_ssl=settings.remote_schema_verify_ssl,
         )
         schema_source = settings.remote_schema_url
 
+    plugin_manager = PluginManager(
+        schema=schema,
+        config_dict=config_dict,
+        plugins_types=get_plugins_types(settings.plugins),
+    )
+    schema = plugin_manager.process_schema(schema)
+    assert_valid_schema(schema)
+
     definitions = get_graphql_queries(settings.queries_path)
     queries = filter_operations_definitions(definitions)
     fragments = filter_fragments_definitions(definitions)
 
     sys.stdout.write(settings.used_settings_message)
 
     package_generator = PackageGenerator(
@@ -59,52 +69,53 @@
         target_path=settings.target_package_path,
         schema=schema,
         client_name=settings.client_name,
         client_file_name=settings.client_file_name,
         base_client_name=settings.base_client_name,
         base_client_file_path=settings.base_client_file_path,
         input_types_module_name=settings.input_types_module_name,
+        fragments_module_name=settings.fragments_module_name,
         queries_source=settings.queries_path,
         schema_source=schema_source,
         include_comments=settings.include_comments,
         fragments=fragments,
         convert_to_snake_case=settings.convert_to_snake_case,
         async_client=settings.async_client,
         files_to_include=settings.files_to_include,
         custom_scalars=settings.scalars,
-        plugin_manager=PluginManager(
-            schema=schema,
-            config_dict=config_dict,
-            plugins_types=get_plugins_types(settings.plugins),
-        ),
+        plugin_manager=plugin_manager,
     )
     for query in queries:
         package_generator.add_operation(query)
     generated_files = package_generator.generate()
 
     sys.stdout.write("\nGenerated files:\n  " + "\n  ".join(generated_files) + "\n")
 
 
 def graphql_schema(config_dict):
     settings = get_graphql_schema_settings(config_dict)
-    sys.stdout.write(settings.used_settings_message)
 
     schema = (
         get_graphql_schema_from_path(settings.schema_path)
         if settings.schema_path
         else get_graphql_schema_from_url(
             url=settings.remote_schema_url,
             headers=settings.remote_schema_headers,
             verify_ssl=settings.remote_schema_verify_ssl,
         )
     )
+    plugin_manager = PluginManager(
+        schema=schema,
+        config_dict=config_dict,
+        plugins_types=get_plugins_types(settings.plugins),
+    )
+    schema = plugin_manager.process_schema(schema)
+    assert_valid_schema(schema)
+
+    sys.stdout.write(settings.used_settings_message)
 
     generate_graphql_schema_file(
         schema=schema,
         target_file_path=settings.target_file_path,
         type_map_name=settings.type_map_variable_name,
         schema_variable_name=settings.schema_variable_name,
     )
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/schema.py` & `ariadne_codegen-0.7.0/ariadne_codegen/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from graphql import (
     DefinitionNode,
     FragmentDefinitionNode,
     GraphQLSchema,
     GraphQLSyntaxError,
     IntrospectionQuery,
     OperationDefinitionNode,
-    assert_valid_schema,
     build_ast_schema,
     build_client_schema,
     get_introspection_query,
     parse,
 )
 
 from .exceptions import IntrospectionError, InvalidGraphqlSyntax
@@ -40,15 +39,16 @@
     return queries_ast.definitions
 
 
 def get_graphql_schema_from_url(
     url: str, headers: Optional[Dict[str, str]] = None, verify_ssl: bool = True
 ) -> GraphQLSchema:
     return build_client_schema(
-        introspect_remote_schema(url=url, headers=headers, verify_ssl=verify_ssl)
+        introspect_remote_schema(url=url, headers=headers, verify_ssl=verify_ssl),
+        assume_valid=True,
     )
 
 
 def introspect_remote_schema(
     url: str, headers: Optional[Dict[str, str]] = None, verify_ssl: bool = True
 ) -> IntrospectionQuery:
     try:
@@ -86,16 +86,15 @@
     return cast(IntrospectionQuery, data)
 
 
 def get_graphql_schema_from_path(schema_path: str) -> GraphQLSchema:
     """Get graphql schema build from provided path."""
     schema_str = load_graphql_files_from_path(Path(schema_path))
     graphql_ast = parse(schema_str)
-    schema: GraphQLSchema = build_ast_schema(graphql_ast)
-    assert_valid_schema(schema)
+    schema: GraphQLSchema = build_ast_schema(graphql_ast, assume_valid=True)
     return schema
 
 
 def load_graphql_files_from_path(path: Path) -> str:
     """
     Get schema from given path.
     If path is a directory, collect schemas from multiple files.
```

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/settings.py` & `ariadne_codegen-0.7.0/ariadne_codegen/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 @dataclass
 class BaseSettings:
     schema_path: Optional[str] = None
     remote_schema_url: Optional[str] = None
     remote_schema_headers: dict = field(default_factory=dict)
     remote_schema_verify_ssl: bool = True
+    plugins: List[str] = field(default_factory=list)
 
     def __post_init__(self):
         if not self.schema_path and not self.remote_schema_url:
             raise InvalidConfiguration(
                 "Schema source not provided. Use schema_path or remote_schema_url"
             )
 
@@ -45,19 +46,19 @@
     target_package_path: str = field(default_factory=lambda: Path.cwd().as_posix())
     client_name: str = "Client"
     client_file_name: str = "client"
     base_client_name: Optional[str] = None
     base_client_file_path: Optional[str] = None
     enums_module_name: str = "enums"
     input_types_module_name: str = "input_types"
+    fragments_module_name: str = "fragments"
     include_comments: bool = True
     convert_to_snake_case: bool = True
     async_client: bool = True
     files_to_include: List[str] = field(default_factory=list)
-    plugins: List[str] = field(default_factory=list)
     scalars: Dict[str, ScalarData] = field(default_factory=dict)
 
     def __post_init__(self):
         if not self.queries_path:
             raise TypeError("__init__ missing 1 required argument: 'queries_path'")
         super().__post_init__()
 
@@ -128,14 +129,15 @@
             Using '{self.target_package_name}' as package name.
             Generating package into '{self.target_package_path}'.
             Using '{self.client_name}' as client name.
             Using '{self.base_client_name}' as base client class.
             Coping base client class from '{self.base_client_file_path}'.
             Generating enums into '{self.enums_module_name}.py'.
             Generating inputs into '{self.input_types_module_name}.py'.
+            Generating fragments into '{self.fragments_module_name}.py'.
             {comments_msg}
             {snake_case_msg}
             {async_client_msg}
             {files_to_include_msg}
             {plugins_msg}
             """
         )
@@ -150,21 +152,28 @@
     def __post_init__(self):
         super().__post_init__()
         assert_string_is_valid_python_identifier(self.schema_variable_name)
         assert_string_is_valid_python_identifier(self.type_map_variable_name)
 
     @property
     def used_settings_message(self):
+        plugins_list = ",".join(self.plugins)
+        plugins_msg = (
+            f"Plugins to use: {plugins_list}"
+            if self.plugins
+            else "No plugin is being used."
+        )
         return dedent(
             f"""\
             Selected strategy: {Strategy.GRAPHQL_SCHEMA}
             Using schema from '{self.schema_path or self.remote_schema_url}'.
             Saving graphql schema to: {self.target_file_path}.
             Using {self.schema_variable_name} as variable name for schema.
             Using {self.type_map_variable_name} as variable name for type map.
+            {plugins_msg}
             """
         )
 
 
 def assert_path_exists(path: str):
     if not Path(path).exists():
         raise InvalidConfiguration(f"Provided path {path} doesn't exist.")
```

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/utils.py` & `ariadne_codegen-0.7.0/ariadne_codegen/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -78,18 +78,21 @@
 
 
 def process_name(
     name: str,
     convert_to_snake_case: bool,
     plugin_manager: Optional[PluginManager] = None,
     node: Optional[Node] = None,
+    trim_leading_underscore: bool = False,
 ) -> str:
     """Processes the GraphQL name to remove keywords
     and optionally convert to snake_case."""
     processed_name = name
     if convert_to_snake_case:
         processed_name = str_to_snake_case(processed_name)
     if iskeyword(processed_name):
         processed_name += "_"
+    if trim_leading_underscore:
+        processed_name = processed_name.lstrip("_")
     if plugin_manager:
         processed_name = plugin_manager.process_name(processed_name, node=node)
     return processed_name
```

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/arguments.py` & `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/arguments.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/client.py` & `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,47 @@
 import ast
-from typing import Dict, List, Optional, Union, cast
+from typing import Dict, List, Optional, Union
 
-from graphql import OperationDefinitionNode
+from graphql import OperationDefinitionNode, OperationType
 
 from ..codegen import (
     generate_ann_assign,
     generate_arg,
     generate_arguments,
     generate_assign,
+    generate_async_for,
     generate_async_method_definition,
     generate_attribute,
     generate_await,
     generate_call,
     generate_class_def,
     generate_constant,
+    generate_expr,
     generate_import_from,
     generate_keyword,
     generate_method_definition,
     generate_module,
     generate_name,
     generate_return,
     generate_subscript,
     generate_tuple,
+    generate_yield,
 )
+from ..exceptions import NotSupported
 from ..plugins.manager import PluginManager
 from .arguments import ArgumentsGenerator
-from .constants import ANY, LIST, OPTIONAL, TYPING_MODULE, UNION
+from .constants import (
+    ANY,
+    ASYNC_ITERATOR,
+    LIST,
+    OPTIONAL,
+    PARSE_OBJ_METHOD,
+    TYPING_MODULE,
+    UNION,
+)
 from .scalars import ScalarData, generate_scalar_imports
 
 
 class ClientGenerator:
     def __init__(
         self,
         name: str,
@@ -47,15 +59,17 @@
         self.input_types_module_name = input_types_module_name
         self.plugin_manager = plugin_manager
         self.custom_scalars = custom_scalars if custom_scalars else {}
         self.arguments_generator = arguments_generator
 
         self._imports: List[ast.ImportFrom] = []
         self._add_import(
-            generate_import_from([OPTIONAL, LIST, ANY, UNION], TYPING_MODULE)
+            generate_import_from(
+                [OPTIONAL, LIST, ANY, UNION, ASYNC_ITERATOR], TYPING_MODULE
+            )
         )
         self._add_import(base_client_import)
         self._add_import(unset_import)
 
         self._class_def = generate_class_def(name=name, base_names=[base_client])
         self._gql_func_name = "gql"
         self._operation_str_variable = "query"
@@ -111,49 +125,83 @@
         operation_str: str,
         async_: bool = True,
     ):
         """Add method to client."""
         arguments, arguments_dict = self.arguments_generator.generate(
             definition.variable_definitions
         )
-        method_def = (
-            self._generate_async_method(
+        if definition.operation == OperationType.SUBSCRIPTION:
+            if not async_:
+                raise NotSupported(
+                    "Subscriptions are only available when using async client."
+                )
+            method_def: Union[
+                ast.FunctionDef, ast.AsyncFunctionDef
+            ] = self._generate_subscription_method_def(
                 name=name,
                 return_type=return_type,
                 arguments=arguments,
                 arguments_dict=arguments_dict,
                 operation_str=operation_str,
             )
-            if async_
-            else self._generate_method(
+        elif async_:
+            method_def = self._generate_async_method(
                 name=name,
                 return_type=return_type,
                 arguments=arguments,
                 arguments_dict=arguments_dict,
                 operation_str=operation_str,
             )
-        )
+        else:
+            method_def = self._generate_method(
+                name=name,
+                return_type=return_type,
+                arguments=arguments,
+                arguments_dict=arguments_dict,
+                operation_str=operation_str,
+            )
+
         method_def.lineno = len(self._class_def.body) + 1
         if self.plugin_manager:
-            method_def = self.plugin_manager.generate_client_method(
-                cast(Union[ast.FunctionDef, ast.AsyncFunctionDef], method_def)
-            )
+            method_def = self.plugin_manager.generate_client_method(method_def)
+
         self._class_def.body.append(method_def)
         self._add_import(
             generate_import_from(names=[return_type], from_=return_type_module, level=1)
         )
 
     def _add_import(self, import_: Optional[ast.ImportFrom] = None):
         if not import_:
             return
         if self.plugin_manager:
             import_ = self.plugin_manager.generate_client_import(import_)
         if import_.names and import_.module:
             self._imports.append(import_)
 
+    def _generate_subscription_method_def(
+        self,
+        name: str,
+        return_type: str,
+        arguments: ast.arguments,
+        arguments_dict: ast.Dict,
+        operation_str: str,
+    ) -> ast.AsyncFunctionDef:
+        return generate_async_method_definition(
+            name=name,
+            arguments=arguments,
+            return_type=generate_subscript(
+                value=generate_name(ASYNC_ITERATOR), slice_=generate_name(return_type)
+            ),
+            body=[
+                self._generate_operation_str_assign(operation_str, 1),
+                self._generate_variables_assign(arguments_dict, 2),
+                self._generate_async_generator_loop(return_type, 3),
+            ],
+        )
+
     def _generate_async_method(
         self,
         name: str,
         return_type: str,
         arguments: ast.arguments,
         arguments_dict: ast.Dict,
         operation_str: str,
@@ -252,19 +300,54 @@
                 args=[generate_name(self._response_variable)],
             ),
         )
 
     def _generate_return_parsed_obj(self, return_type: str) -> ast.Return:
         return generate_return(
             generate_call(
-                func=generate_attribute(generate_name(return_type), "parse_obj"),
+                func=generate_attribute(generate_name(return_type), PARSE_OBJ_METHOD),
                 args=[generate_name(self._data_variable)],
             )
         )
 
+    def _generate_async_generator_loop(
+        self, return_type: str, lineno: int = 1
+    ) -> ast.AsyncFor:
+        return generate_async_for(
+            target=generate_name(self._data_variable),
+            iter_=generate_call(
+                func=generate_attribute(value=generate_name("self"), attr="execute_ws"),
+                keywords=[
+                    generate_keyword(
+                        arg="query",
+                        value=generate_name(self._operation_str_variable),
+                    ),
+                    generate_keyword(
+                        arg="variables",
+                        value=generate_name(self._variables_dict_variable),
+                    ),
+                ],
+            ),
+            body=[self._generate_yield_parsed_obj(return_type)],
+            lineno=lineno,
+        )
+
+    def _generate_yield_parsed_obj(self, return_type: str) -> ast.Expr:
+        return generate_expr(
+            generate_yield(
+                generate_call(
+                    func=generate_attribute(
+                        value=generate_name(return_type),
+                        attr=PARSE_OBJ_METHOD,
+                    ),
+                    args=[generate_name(self._data_variable)],
+                )
+            )
+        )
+
     def _generate_gql_func(self) -> ast.FunctionDef:
         str_name = generate_name("str")
         arg = "q"
         return generate_method_definition(
             name=self._gql_func_name,
             arguments=generate_arguments([generate_arg(arg, str_name)]),
             return_type=str_name,
```

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/constants.py` & `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,27 +10,34 @@
 }
 OPTIONAL: str = "Optional"
 LIST: str = "List"
 UNION: str = "Union"
 ANY: str = "Any"
 DICT = "Dict"
 CALLABLE = "Callable"
+ANNOTATED = "Annotated"
+LITERAL = "Literal"
+ASYNC_ITERATOR = "AsyncIterator"
 
 TIMESTAMP_COMMENT = "# Generated by ariadne-codegen on {}\n"
 SOURCE_COMMENT = "# Source: {}\n"
 COMMENT_DATETIME_FORMAT = "%Y-%m-%d %H:%M"
 
 BASE_MODEL_CLASS_NAME = "BaseModel"
 
 TYPENAME_FIELD_NAME = "__typename"
+TYPENAME_ALIAS = "typename__"
 
 TYPING_MODULE = "typing"
 PYDANTIC_MODULE = "pydantic"
 FIELD_CLASS = "Field"
+ALIAS_KEYWORD = "alias"
+DISCRIMINATOR_KEYWORD = "discriminator"
 UPDATE_FORWARD_REFS_METHOD = "update_forward_refs"
+PARSE_OBJ_METHOD = "parse_obj"
 ENUM_MODULE = "enum"
 ENUM_CLASS = "Enum"
 
 MIXIN_NAME = "mixin"
 MIXIN_FROM_NAME = "from"
 MIXIN_IMPORT_NAME = "import"
```

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/enums.py` & `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/enums.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/init_file.py` & `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/init_file.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/input_fields.py` & `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/input_fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     generate_lambda,
     generate_list,
     generate_list_annotation,
     generate_name,
     generate_subscript,
 )
 from ..exceptions import ParsingError
-from .constants import ANY, FIELD_CLASS, SIMPLE_TYPE_MAP
+from .constants import ANY, FIELD_CLASS, PARSE_OBJ_METHOD, SIMPLE_TYPE_MAP
 from .scalars import ScalarData
 from .types import Annotation, CodegenInputFieldType
 
 
 # pylint: disable=too-many-return-statements
 def parse_input_field_type(
     type_: CodegenInputFieldType,
@@ -172,15 +172,15 @@
                                 func=generate_attribute(
                                     value=generate_subscript(
                                         value=generate_call(
                                             func=generate_name("globals")
                                         ),
                                         slice_=generate_constant(field_type),
                                     ),
-                                    attr="parse_obj",
+                                    attr=PARSE_OBJ_METHOD,
                                 ),
                                 args=[dict_],
                             )
                         ),
                     )
                 ],
             )
```

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/input_types.py` & `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/input_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,26 @@
     GraphQLScalarType,
     GraphQLSchema,
 )
 
 from ..codegen import (
     generate_ann_assign,
     generate_class_def,
+    generate_constant,
     generate_expr,
-    generate_field_with_alias,
     generate_import_from,
     generate_keyword,
     generate_method_call,
     generate_module,
+    generate_pydantic_field,
 )
 from ..plugins.manager import PluginManager
 from ..utils import process_name
 from .constants import (
+    ALIAS_KEYWORD,
     ANY,
     BASE_MODEL_CLASS_NAME,
     FIELD_CLASS,
     LIST,
     OPTIONAL,
     PYDANTIC_MODULE,
     TYPING_MODULE,
@@ -110,14 +112,15 @@
 
         for lineno, (org_name, field) in enumerate(definition.fields.items(), start=1):
             name = process_name(
                 org_name,
                 convert_to_snake_case=self.convert_to_snake_case,
                 plugin_manager=self.plugin_manager,
                 node=field,
+                trim_leading_underscore=True,
             )
             annotation, field_type = parse_input_field_type(
                 field.type, custom_scalars=self.custom_scalars
             )
             field_implementation = generate_ann_assign(
                 target=name,
                 annotation=annotation,
@@ -146,15 +149,17 @@
         return class_def
 
     def _process_field_value(
         self,
         field_implementation: ast.AnnAssign,
         alias: str,
     ) -> ast.Call:
-        field_with_alias = generate_field_with_alias(alias)
+        field_with_alias = generate_pydantic_field(
+            {ALIAS_KEYWORD: generate_constant(alias)}
+        )
         if field_implementation.value:
             if (
                 isinstance(field_implementation.value, ast.Call)
                 and isinstance(field_implementation.value.func, ast.Name)
                 and field_implementation.value.func.id == FIELD_CLASS
             ):
                 field_with_alias.keywords.extend(field_implementation.value.keywords)
```

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/package.py` & `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/package.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import ast
 from datetime import datetime
 from pathlib import Path
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Set
 
 from graphql import FragmentDefinitionNode, GraphQLSchema, OperationDefinitionNode
 
 from ..codegen import generate_import_from
 from ..exceptions import ParsingError
 from ..plugins.manager import PluginManager
 from ..utils import ast_to_str, process_name, str_to_pascal_case
@@ -19,14 +19,15 @@
     GRAPHQL_CLIENT_EXCEPTIONS_NAMES,
     SOURCE_COMMENT,
     TIMESTAMP_COMMENT,
     UNSET_NAME,
     UNSET_TYPE_NAME,
 )
 from .enums import EnumsGenerator
+from .fragments import FragmentsGenerator
 from .init_file import InitFileGenerator
 from .input_types import InputTypesGenerator
 from .result_types import ResultTypesGenerator
 from .scalars import ScalarData, ScalarsDefinitionsGenerator
 
 
 class PackageGenerator:
@@ -37,14 +38,15 @@
         schema: GraphQLSchema,
         client_name: str = "Client",
         client_file_name: str = "client",
         base_client_name: str = "AsyncBaseClient",
         base_client_file_path: Optional[str] = None,
         enums_module_name: str = "enums",
         input_types_module_name: str = "input_types",
+        fragments_module_name: str = "fragments",
         include_comments: bool = True,
         queries_source: str = "",
         schema_source: str = "",
         convert_to_snake_case: bool = True,
         async_client: bool = True,
         fragments: Optional[List[FragmentDefinitionNode]] = None,
         init_generator: Optional[InitFileGenerator] = None,
@@ -80,14 +82,15 @@
 
         self.files_to_include = (
             [Path(f) for f in files_to_include] if files_to_include else []
         )
 
         self.enums_module_name = enums_module_name
         self.input_types_module_name = input_types_module_name
+        self.fragments_module_name = fragments_module_name
         self.client_file_name = client_file_name
 
         self.include_comments = include_comments
         self.queries_source = queries_source
         self.schema_source = schema_source
         self.convert_to_snake_case = convert_to_snake_case
         self.async_client = async_client
@@ -155,25 +158,28 @@
 
         self.scalars_definitions_generator = ScalarsDefinitionsGenerator(
             scalars_data=list(self.custom_scalars.values()),
             plugin_manager=self.plugin_manager,
         )
         self.scalars_definitions_file_name = "scalars"
 
+        self._unpacked_fragments: Set[str] = set()
+
     def generate(self) -> List[str]:
         """Generate package with graphql client."""
         self._validate_unique_file_names()
         if not self.package_path.exists():
             self.package_path.mkdir()
-        self._generate_client()
         self._generate_enums()
         self._generate_input_types()
         self._generate_result_types()
+        self._generate_fragments()
         self._copy_files()
         self._generate_scalars_definitions()
+        self._generate_client()
         self._generate_init()
 
         return sorted(self.generated_files)
 
     def add_operation(self, definition: OperationDefinitionNode):
         name = definition.name
         if not name:
@@ -189,20 +195,24 @@
         module_name = method_name
         file_name = f"{module_name}.py"
 
         query_types_generator = ResultTypesGenerator(
             schema=self.schema,
             operation_definition=definition,
             enums_module_name=self.enums_module_name,
+            fragments_module_name=self.fragments_module_name,
             fragments_definitions=self.fragments_definitions,
             base_model_import=self.base_model_import,
             convert_to_snake_case=self.convert_to_snake_case,
             custom_scalars=self.custom_scalars,
             plugin_manager=self.plugin_manager,
         )
+        self._unpacked_fragments = self._unpacked_fragments.union(
+            query_types_generator.get_unpacked_fragments()
+        )
         self.result_types_files[file_name] = query_types_generator.generate()
         operation_str = query_types_generator.get_operation_as_str()
         self.init_generator.add_import(
             query_types_generator.get_generated_public_names(), module_name, 1
         )
 
         self.client_generator.add_method(
@@ -225,14 +235,15 @@
             [
                 f"{self.client_file_name}.py",
                 self.base_client_file_path.name,
                 self.base_model_file_path.name,
                 f"{self.enums_module_name}.py",
                 f"{self.input_types_module_name}.py",
                 f"{self.scalars_definitions_file_name}.py",
+                f"{self.fragments_module_name}.py",
             ]
             + list(self.result_types_files.keys())
             + [f.name for f in self.files_to_include]
         )
         if self.include_exceptions_file:
             file_names.append(self.exceptions_file_path.name)
 
@@ -302,14 +313,39 @@
                 ast_to_str(module), self.queries_source
             )
             if self.plugin_manager:
                 code = self.plugin_manager.generate_result_types_code(code)
             file_path.write_text(code)
             self.generated_files.append(file_path.name)
 
+    def _generate_fragments(self):
+        if not set(self.fragments_definitions.keys()).difference(
+            self._unpacked_fragments
+        ):
+            return
+
+        generator = FragmentsGenerator(
+            schema=self.schema,
+            enums_module_name=self.enums_module_name,
+            fragments_definitions=self.fragments_definitions,
+            exclude_names=self._unpacked_fragments,
+            base_model_import=self.base_model_import,
+            convert_to_snake_case=self.convert_to_snake_case,
+            custom_scalars=self.custom_scalars,
+            plugin_manager=self.plugin_manager,
+        )
+        module = generator.generate()
+        file_path = self.package_path / f"{self.fragments_module_name}.py"
+        code = self._proccess_generated_code(ast_to_str(module), self.queries_source)
+        file_path.write_text(code)
+        self.generated_files.append(file_path.name)
+        self.init_generator.add_import(
+            generator.get_generated_public_names(), self.fragments_module_name, 1
+        )
+
     def _copy_files(self):
         files_to_copy = self.files_to_include + [
             self.base_client_file_path,
             self.base_model_file_path,
         ]
         if self.include_exceptions_file:
             files_to_copy.append(self.exceptions_file_path)
```

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/result_types.py` & `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/result_types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,127 +1,160 @@
 import ast
-from typing import Dict, List, Optional, Tuple, cast
+from copy import deepcopy
+from typing import Any, Dict, List, Optional, Set, Tuple, cast
 
 from graphql import (
     DirectiveNode,
+    ExecutableDefinitionNode,
     FieldNode,
     FragmentDefinitionNode,
     FragmentSpreadNode,
+    GraphQLAbstractType,
     GraphQLEnumType,
     GraphQLField,
     GraphQLNonNull,
     GraphQLObjectType,
     GraphQLScalarType,
     GraphQLSchema,
+    GraphQLUnionType,
     InlineFragmentNode,
     NameNode,
     OperationDefinitionNode,
     OperationType,
     SelectionNode,
     SelectionSetNode,
     StringValueNode,
+    Visitor,
+    is_abstract_type,
     print_ast,
+    visit,
 )
 
 from ..codegen import (
     generate_ann_assign,
     generate_class_def,
+    generate_constant,
     generate_expr,
-    generate_field_with_alias,
     generate_import_from,
     generate_method_call,
     generate_module,
+    generate_pass,
+    generate_pydantic_field,
 )
 from ..exceptions import NotSupported, ParsingError
 from ..plugins.manager import PluginManager
 from ..utils import process_name, str_to_pascal_case
 from .constants import (
+    ALIAS_KEYWORD,
+    ANNOTATED,
     ANY,
     BASE_MODEL_CLASS_NAME,
+    DISCRIMINATOR_KEYWORD,
     FIELD_CLASS,
     LIST,
+    LITERAL,
     MIXIN_FROM_NAME,
     MIXIN_IMPORT_NAME,
     MIXIN_NAME,
     OPTIONAL,
     PYDANTIC_MODULE,
+    TYPENAME_ALIAS,
     TYPENAME_FIELD_NAME,
     TYPING_MODULE,
     UNION,
     UPDATE_FORWARD_REFS_METHOD,
 )
-from .result_fields import FieldNames, parse_operation_field
+from .result_fields import FieldNames, is_union, parse_operation_field
 from .scalars import ScalarData, generate_scalar_imports
 from .types import CodegenResultFieldType
 
 
 class ResultTypesGenerator:
     def __init__(
         self,
         schema: GraphQLSchema,
-        operation_definition: OperationDefinitionNode,
+        operation_definition: ExecutableDefinitionNode,
         enums_module_name: str,
+        fragments_module_name: Optional[str] = None,
         fragments_definitions: Optional[Dict[str, FragmentDefinitionNode]] = None,
         base_model_import: Optional[ast.ImportFrom] = None,
         convert_to_snake_case: bool = True,
         custom_scalars: Optional[Dict[str, ScalarData]] = None,
         plugin_manager: Optional[PluginManager] = None,
     ) -> None:
         self.schema = schema
         self.operation_definition = operation_definition
         if not self.operation_definition.name:
             raise NotSupported("Operations without name are not supported.")
+        self._operation_name = self.operation_definition.name.value
 
         self.enums_module_name = enums_module_name
+        self.fragments_module_name = fragments_module_name
         self.fragments_definitions = (
             fragments_definitions if fragments_definitions else {}
         )
         self.custom_scalars = custom_scalars if custom_scalars else {}
         self.convert_to_snake_case = convert_to_snake_case
         self.plugin_manager = plugin_manager
 
         self._imports: List[ast.ImportFrom] = [
-            generate_import_from([OPTIONAL, UNION, ANY, LIST], TYPING_MODULE),
+            generate_import_from(
+                [OPTIONAL, UNION, ANY, LIST, LITERAL, ANNOTATED], TYPING_MODULE
+            ),
             generate_import_from([FIELD_CLASS], PYDANTIC_MODULE),
             base_model_import
             or generate_import_from([BASE_MODEL_CLASS_NAME], PYDANTIC_MODULE),
         ]
         self._public_names: List[str] = []
-        self._class_defs: List[ast.ClassDef] = []
         self._used_enums: List[str] = []
         self._used_scalars: List[str] = []
-        self._used_fragments_names: set[str] = set()
+        self._fragments_used_as_mixins: Set[str] = set()
+        self._unpacked_fragments: Set[str] = set()
 
-        self._class_defs = self._parse_type_definition(
-            class_name=str_to_pascal_case(self.operation_definition.name.value),
-            type_name=self._get_operation_type_name(
-                self.operation_definition.operation
-            ),
-            selection_set=self.operation_definition.selection_set,
-        )
+        if isinstance(
+            self.operation_definition, FragmentDefinitionNode
+        ) and self._unpack_fragment(self.operation_definition):
+            self._class_defs = []
+        else:
+            self._class_defs = self._parse_type_definition(
+                class_name=str_to_pascal_case(self._operation_name),
+                type_name=self._get_operation_type_name(self.operation_definition),
+                selection_set=self.operation_definition.selection_set,
+            )
+
+        self._add_enums_scalars_fragments_imports()
 
-    def _get_operation_type_name(self, operation_type: OperationType) -> str:
-        if operation_type == OperationType.QUERY and self.schema.query_type:
+    def _get_operation_type_name(self, definition: ExecutableDefinitionNode) -> str:
+        if isinstance(definition, FragmentDefinitionNode):
+            return definition.type_condition.name.value
+
+        if (
+            isinstance(definition, OperationDefinitionNode)
+            and definition.operation == OperationType.QUERY
+            and self.schema.query_type
+        ):
             return self.schema.query_type.name
 
-        if operation_type == OperationType.MUTATION and self.schema.mutation_type:
+        if (
+            isinstance(definition, OperationDefinitionNode)
+            and definition.operation == OperationType.MUTATION
+            and self.schema.mutation_type
+        ):
             return self.schema.mutation_type.name
 
-        raise NotSupported(f"Not supported operation type: {operation_type}")
+        if (
+            isinstance(definition, OperationDefinitionNode)
+            and definition.operation == OperationType.SUBSCRIPTION
+            and self.schema.subscription_type
+        ):
+            return self.schema.subscription_type.name
 
-    def generate(self) -> ast.Module:
-        if self._used_enums:
-            self._imports.append(
-                generate_import_from(self._used_enums, self.enums_module_name, 1)
-            )
-        if self._used_scalars:
-            for scalar_name in self._used_scalars:
-                scalar_data = self.custom_scalars[scalar_name]
-                self._imports.extend(generate_scalar_imports(scalar_data))
+        raise NotSupported(f"Not supported operation type: {definition}")
 
+    def generate(self) -> ast.Module:
         update_forward_refs_calls = [
             generate_expr(
                 generate_method_call(class_def.name, UPDATE_FORWARD_REFS_METHOD)
             )
             for class_def in self._class_defs
         ]
         module_body = (
@@ -133,128 +166,169 @@
         module = generate_module(module_body)
         if self.plugin_manager:
             module = self.plugin_manager.generate_result_types_module(
                 module, operation_definition=self.operation_definition
             )
         return module
 
+    def get_imports(self) -> List[ast.ImportFrom]:
+        return self._imports
+
+    def get_classes(self) -> List[ast.ClassDef]:
+        return self._class_defs
+
     def get_operation_as_str(self) -> str:
-        operation_str = print_ast(self.operation_definition)
-        if self._used_fragments_names:
-            for used_fragment in sorted(self._used_fragments_names):
+        operation_str = print_ast(
+            self._get_operation_definition_without_mixin_directive()
+        )
+        if self._fragments_used_as_mixins or self._unpacked_fragments:
+            for used_fragment in sorted(self._get_all_related_fragments()):
                 operation_str += "\n\n" + print_ast(
                     self.fragments_definitions[used_fragment]
                 )
 
         if self.plugin_manager:
             operation_str = self.plugin_manager.generate_operation_str(
                 operation_str, operation_definition=self.operation_definition
             )
         return operation_str
 
     def get_generated_public_names(self) -> List[str]:
         return self._public_names
 
+    def get_unpacked_fragments(self) -> Set[str]:
+        return self._unpacked_fragments
+
+    def get_fragments_used_as_mixins(self) -> Set[str]:
+        return self._fragments_used_as_mixins
+
     def _parse_type_definition(
         self,
         class_name: str,
         type_name: str,
         selection_set: SelectionSetNode,
         add_typename: bool = False,
         extra_bases: Optional[List[str]] = None,
+        typename_values: Optional[List[str]] = None,
     ) -> List[ast.ClassDef]:
-        class_bases = [BASE_MODEL_CLASS_NAME]
-        if extra_bases:
-            class_bases.extend(extra_bases)
-        class_def = generate_class_def(class_name, class_bases)
-
-        if class_def.name in self._public_names:
+        if class_name in self._public_names:
             return []
-        self._public_names.append(class_def.name)
+        self._public_names.append(class_name)
 
-        extra_classes = []
-        resolved_selection_set = self._resolve_selection_set(selection_set, type_name)
+        resolved_selection_set, fragments = self._resolve_selection_set(
+            selection_set, type_name
+        )
         if add_typename:
             (
                 resolved_selection_set,
                 selection_set.selections,
             ) = self._add_typename_field_to_selections(
                 resolved_selection_set, selection_set
             )
+
+        if fragments:
+            class_bases = [str_to_pascal_case(f) for f in sorted(fragments)]
+        else:
+            class_bases = [BASE_MODEL_CLASS_NAME]
+        if extra_bases:
+            class_bases.extend(extra_bases)
+        class_def = generate_class_def(class_name, class_bases)
+
+        extra_classes = []
         for lineno, field in enumerate(
             resolved_selection_set,
             start=1,
         ):
             field_name = self._get_field_name(field)
             name = self._process_field_name(field_name, field=field)
             field_definition = self._get_field_from_schema(type_name, field.name.value)
             annotation, field_types_names = parse_operation_field(
                 field=field,
                 type_=cast(CodegenResultFieldType, field_definition.type),
                 directives=field.directives,
                 class_name=class_name + str_to_pascal_case(name),
+                typename_values=typename_values,
                 custom_scalars=self.custom_scalars,
+                fragments_definitions=self.fragments_definitions,
             )
 
             field_implementation = generate_ann_assign(
                 target=name,
                 annotation=annotation,
                 lineno=lineno,
             )
-            if name != field_name:
-                field_implementation.value = generate_field_with_alias(field_name)
-
-            if self.plugin_manager:
-                field_implementation = self.plugin_manager.generate_result_field(
-                    field_implementation,
-                    operation_definition=self.operation_definition,
-                    field=field,
-                )
+            field_implementation = self._process_field_implementation(
+                field_implementation, field_schema_name=field_name, field=field
+            )
 
             class_def.body.append(field_implementation)
 
             extra_classes.extend(
                 self._parse_field_selection_set_types(
                     selection_set=field.selection_set,
                     field_types_names=field_types_names,
                     extra_bases=self._parse_mixin_directives(field),
                 )
             )
             self._save_used_enums(field_types_names)
             self._save_used_scalars(field_types_names)
 
-            if self.plugin_manager:
-                class_def = self.plugin_manager.generate_result_class(
-                    class_def,
-                    operation_definition=self.operation_definition,
-                    selection_set=selection_set,
-                )
+        if not class_def.body:
+            class_def.body.append(generate_pass())
+
+        if self.plugin_manager:
+            class_def = self.plugin_manager.generate_result_class(
+                class_def,
+                operation_definition=self.operation_definition,
+                selection_set=selection_set,
+            )
+
         return [class_def] + extra_classes
 
     def _resolve_selection_set(
         self, selection_set: SelectionSetNode, root_type: str = ""
-    ) -> List[FieldNode]:
+    ) -> Tuple[List[FieldNode], Set[str]]:
         fields = []
+        fragments = set()
         for selection in selection_set.selections:
             if isinstance(selection, FieldNode):
                 fields.append(selection)
             elif isinstance(selection, FragmentSpreadNode):
-                self._used_fragments_names.add(selection.name.value)
-                fields.extend(
-                    self._resolve_selection_set(
-                        self.fragments_definitions[selection.name.value].selection_set,
-                        root_type,
+                fragment_def = self.fragments_definitions[selection.name.value]
+                if not self._unpack_fragment(fragment_def):
+                    fragments.add(selection.name.value)
+                else:
+                    self._unpacked_fragments.add(selection.name.value)
+                    sub_fields, sub_fragments = self._resolve_selection_set(
+                        fragment_def.selection_set, root_type
                     )
-                )
+                    fields.extend(sub_fields)
+                    fragments = fragments.union(sub_fragments)
             elif isinstance(selection, InlineFragmentNode):
                 if selection.type_condition.name.value == root_type:
-                    fields.extend(
-                        self._resolve_selection_set(selection.selection_set, root_type)
+                    sub_fields, sub_fragments = self._resolve_selection_set(
+                        selection.selection_set, root_type
                     )
-        return fields
+                    fields.extend(sub_fields)
+                    fragments = fragments.union(sub_fragments)
+        self._fragments_used_as_mixins = self._fragments_used_as_mixins.union(
+            set(fragments)
+        )
+        return fields, fragments
+
+    def _unpack_fragment(self, fragment_def: FragmentDefinitionNode) -> bool:
+        if fragment_def.name and isinstance(
+            self.schema.type_map.get(fragment_def.type_condition.name.value),
+            GraphQLUnionType,
+        ):
+            return True
+        for fragment_selection in fragment_def.selection_set.selections:
+            if isinstance(fragment_selection, InlineFragmentNode):
+                return True
+        return False
 
     def _add_typename_field_to_selections(
         self, resolved_fields: List[FieldNode], selection_set: SelectionSetNode
     ) -> Tuple[List[FieldNode], Tuple[SelectionNode, ...]]:
         field_names = {f.name.value for f in resolved_fields}
         if TYPENAME_FIELD_NAME not in field_names:
             typename_field = FieldNode(name=NameNode(value=TYPENAME_FIELD_NAME))
@@ -266,21 +340,22 @@
 
     def _get_field_name(self, field: FieldNode) -> str:
         if field.alias:
             return field.alias.value
         return field.name.value
 
     def _process_field_name(self, name: str, field: FieldNode) -> str:
-        if self.convert_to_snake_case and name == TYPENAME_FIELD_NAME:
-            return "__typename__"
+        if name == TYPENAME_FIELD_NAME:
+            return TYPENAME_ALIAS
         return process_name(
             name,
             convert_to_snake_case=self.convert_to_snake_case,
             plugin_manager=self.plugin_manager,
             node=field,
+            trim_leading_underscore=True,
         )
 
     def _get_field_from_schema(self, type_name: str, field_name: str) -> GraphQLField:
         try:
             return cast(GraphQLObjectType, self.schema.type_map[type_name]).fields[
                 field_name
             ]
@@ -289,14 +364,43 @@
                 return GraphQLField(
                     type_=GraphQLNonNull(type_=GraphQLScalarType(name="String"))
                 )
             raise ParsingError(
                 f"Field {field_name} not found in type {type_name}."
             ) from exc
 
+    def _process_field_implementation(
+        self,
+        field_implementation: ast.AnnAssign,
+        field_schema_name: str,
+        field: FieldNode,
+    ) -> ast.AnnAssign:
+        keywords: Dict[str, ast.expr] = {}
+
+        if (
+            isinstance(field_implementation.target, ast.Name)
+            and field_implementation.target.id != field_schema_name
+        ):
+            keywords[ALIAS_KEYWORD] = generate_constant(field_schema_name)
+
+        if is_union(field_implementation.annotation):
+            keywords[DISCRIMINATOR_KEYWORD] = generate_constant(TYPENAME_ALIAS)
+
+        if keywords:
+            field_implementation.value = generate_pydantic_field(keywords)
+
+        if self.plugin_manager:
+            field_implementation = self.plugin_manager.generate_result_field(
+                field_implementation,
+                operation_definition=self.operation_definition,
+                field=field,
+            )
+
+        return field_implementation
+
     def _parse_mixin_directives(self, field: FieldNode) -> List[str]:
         if not field.directives:
             return []
         directives = [
             d for d in field.directives if d.name and d.name.value == MIXIN_NAME
         ]
         extra_base_classes: List[str] = []
@@ -335,31 +439,112 @@
         selection_set: Optional[SelectionSetNode],
         field_types_names: List[FieldNames],
         extra_bases: Optional[List[str]] = None,
     ) -> List[ast.ClassDef]:
         if selection_set:
             generated_classes = []
             add_typename = len(field_types_names) > 1
+            typename_values = self._get_typename_values(field_types_names)
             for field_type_names in field_types_names:
                 generated_classes.extend(
                     self._parse_type_definition(
                         class_name=field_type_names.class_name,
                         type_name=field_type_names.type_name,
                         selection_set=selection_set,
                         add_typename=add_typename,
                         extra_bases=extra_bases,
+                        typename_values=typename_values[field_type_names.type_name],
                     )
                 )
             return generated_classes
         return []
 
+    def _get_typename_values(
+        self, field_types_names: List[FieldNames]
+    ) -> Dict[str, List[str]]:
+        types_names = [n.type_name for n in field_types_names]
+        result = {name: [name] for name in types_names}
+
+        schema_types = [self.schema.type_map[n] for n in types_names]
+        abstract_type = next(filter(is_abstract_type, schema_types), None)
+        abstract_type = cast(GraphQLAbstractType, abstract_type)
+        if not abstract_type:
+            return result
+
+        possible_types = self.schema.get_possible_types(abstract_type)
+        possible_types_names = [t.name for t in possible_types]
+        types_without_class = list(set(possible_types_names) - set(types_names))
+
+        result[abstract_type.name].extend(types_without_class)
+        return result
+
     def _save_used_enums(self, field_types_names: List[FieldNames]):
         for field_type_name in field_types_names:
             if isinstance(
                 self.schema.type_map.get(field_type_name.type_name), GraphQLEnumType
             ):
                 self._used_enums.append(field_type_name.type_name)
 
     def _save_used_scalars(self, field_types_names: List[FieldNames]):
         for field_type_name in field_types_names:
             if field_type_name.type_name in self.custom_scalars:
                 self._used_scalars.append(field_type_name.type_name)
+
+    def _add_enums_scalars_fragments_imports(self):
+        if self._used_enums:
+            self._imports.append(
+                generate_import_from(self._used_enums, self.enums_module_name, 1)
+            )
+        if self._used_scalars:
+            for scalar_name in self._used_scalars:
+                scalar_data = self.custom_scalars[scalar_name]
+                self._imports.extend(generate_scalar_imports(scalar_data))
+
+        if (
+            isinstance(self.operation_definition, OperationDefinitionNode)
+            and self._fragments_used_as_mixins
+            and self.fragments_module_name
+        ):
+            self._imports.append(
+                generate_import_from(
+                    [str_to_pascal_case(f) for f in self._fragments_used_as_mixins],
+                    self.fragments_module_name,
+                    1,
+                )
+            )
+
+    def _get_all_related_fragments(self) -> Set[str]:
+        fragments_names: Set[str] = self._fragments_used_as_mixins.copy()
+        for fragment_name in self._fragments_used_as_mixins:
+            fragment_def = self.fragments_definitions[fragment_name]
+            fragments_names = fragments_names.union(
+                self._get_fragments_names(fragment_def.selection_set)
+            )
+        return fragments_names.union(self._unpacked_fragments)
+
+    def _get_fragments_names(self, selection_set: SelectionSetNode) -> Set[str]:
+        names: Set[str] = set()
+        for node in selection_set.selections:
+            if isinstance(node, FragmentSpreadNode):
+                name = node.name.value
+                names.add(name)
+                names = names.union(
+                    self._get_fragments_names(
+                        self.fragments_definitions[name].selection_set
+                    )
+                )
+            elif isinstance(node, FieldNode) and node.selection_set:
+                names = names.union(self._get_fragments_names(node.selection_set))
+        return names
+
+    def _get_operation_definition_without_mixin_directive(self):
+        class RemoveMixinVisitor(Visitor):
+            @staticmethod
+            def enter_field(node: FieldNode, *_args: Any) -> FieldNode:
+                node.directives = tuple(
+                    d for d in node.directives or [] if d.name.value != MIXIN_NAME
+                )
+                return node
+
+        operation_def = deepcopy(self.operation_definition)
+        visit(operation_def, RemoveMixinVisitor())
+        return operation_def
```

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/scalars.py` & `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/scalars.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 @dataclass
 class ScalarData:
     type_: str
     serialize: Optional[str] = None
     parse: Optional[str] = None
     import_: Optional[str] = None
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         self.type_name: str = self._get_object_name(self.type_)
         self.parse_name: Optional[str] = (
             self._get_object_name(self.parse) if self.parse else None
         )
         self.serialize_name: Optional[str] = (
             self._get_object_name(self.serialize) if self.serialize else None
         )
@@ -116,22 +116,22 @@
                 List[ast.stmt],
                 self._imports
                 + [
                     self._generate_dict_assignment(
                         name=SCALARS_PARSE_DICT_NAME,
                         dict_=self._parse_dict,
                         callable_annotation=generate_tuple(
-                            [generate_list([generate_name("str")]), generate_name(ANY)]
+                            [generate_list([generate_name(ANY)]), generate_name(ANY)]
                         ),
                     ),
                     self._generate_dict_assignment(
                         name=SCALARS_SERIALIZE_DICT_NAME,
                         dict_=self._serialize_dict,
                         callable_annotation=generate_tuple(
-                            [generate_list([generate_name(ANY)]), generate_name("str")]
+                            [generate_list([generate_name(ANY)]), generate_name(ANY)]
                         ),
                     ),
                 ],
             )
         )
         if self.plugin_manager:
             module = self.plugin_manager.generate_scalars_module(module)
```

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/types.py` & `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/types.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/dependencies/async_base_client.py` & `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/dependencies/base_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,55 @@
+import json
 from typing import Any, Dict, Optional, TypeVar, cast
 
 import httpx
 from pydantic import BaseModel
+from pydantic.json import pydantic_encoder
 
 from .base_model import UNSET
 from .exceptions import (
     GraphQLClientGraphQLMultiError,
     GraphQLClientHttpError,
     GraphQlClientInvalidResponseError,
 )
 
-Self = TypeVar("Self", bound="AsyncBaseClient")
+Self = TypeVar("Self", bound="BaseClient")
 
 
-class AsyncBaseClient:
+class BaseClient:
     def __init__(
         self,
         url: str = "",
         headers: Optional[Dict[str, str]] = None,
-        http_client: Optional[httpx.AsyncClient] = None,
+        http_client: Optional[httpx.Client] = None,
     ) -> None:
         self.url = url
         self.headers = headers
 
-        self.http_client = (
-            http_client if http_client else httpx.AsyncClient(headers=headers)
-        )
+        self.http_client = http_client if http_client else httpx.Client(headers=headers)
 
-    async def __aenter__(self: Self) -> Self:
+    def __enter__(self: Self) -> Self:
         return self
 
-    async def __aexit__(
+    def __exit__(
         self,
         exc_type: object,
         exc_val: object,
         exc_tb: object,
     ) -> None:
-        await self.http_client.aclose()
+        self.http_client.close()
 
-    async def execute(
+    def execute(
         self, query: str, variables: Optional[Dict[str, Any]] = None
     ) -> httpx.Response:
         payload: Dict[str, Any] = {"query": query}
         if variables:
             payload["variables"] = self._convert_dict_to_json_serializable(variables)
-        return await self.http_client.post(url=self.url, json=payload)
+        content = json.dumps(payload, default=pydantic_encoder)
+        return self.http_client.post(url=self.url, content=content)
 
     def get_data(self, response: httpx.Response) -> dict[str, Any]:
         if not response.is_success:
             raise GraphQLClientHttpError(
                 status_code=response.status_code, response=response
             )
```

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/dependencies/base_model.py` & `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/dependencies/base_model.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/dependencies/exceptions.py` & `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/dependencies/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
     """Base exception."""
 
@@ -65,7 +65,15 @@
     def from_errors_dicts(
         cls, errors_dicts: List[dict[str, Any]], data: dict[str, Any]
     ) -> "GraphQLClientGraphQLMultiError":
         return cls(
             errors=[GraphQLClientGraphQLError.from_dict(e) for e in errors_dicts],
             data=data,
         )
+
+
+class GraphQLClientInvalidMessageFormat(GraphQLClientError):
+    def __init__(self, message: Union[str, bytes]) -> None:
+        self.message = message
+
+    def __str__(self) -> str:
+        return "Invalid message format."
```

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/directives.py` & `ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/directives.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/fields.py` & `ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/fields.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/named_types.py` & `ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/named_types.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/schema.py` & `ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/schema.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/utils.py` & `ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/utils.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/plugins/base.py` & `ariadne_codegen-0.7.0/ariadne_codegen/plugins/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import ast
 from typing import Dict, Optional, Tuple, Union
 
 from graphql import (
+    ExecutableDefinitionNode,
     FieldNode,
+    FragmentDefinitionNode,
     GraphQLEnumType,
     GraphQLInputField,
     GraphQLInputObjectType,
     GraphQLSchema,
     Node,
-    OperationDefinitionNode,
     SelectionSetNode,
     VariableDefinitionNode,
 )
 
 
 # pylint: disable=too-many-public-methods
 class Plugin:
@@ -84,38 +85,38 @@
         input_field: GraphQLInputField,
         field_name: str,
     ) -> ast.AnnAssign:
         return field_implementation
 
     # pylint: disable=unused-argument
     def generate_result_types_module(
-        self, module: ast.Module, operation_definition: OperationDefinitionNode
+        self, module: ast.Module, operation_definition: ExecutableDefinitionNode
     ) -> ast.Module:
         return module
 
     # pylint: disable=unused-argument
     def generate_operation_str(
-        self, operation_str: str, operation_definition: OperationDefinitionNode
+        self, operation_str: str, operation_definition: ExecutableDefinitionNode
     ) -> str:
         return operation_str
 
     # pylint: disable=unused-argument
     def generate_result_class(
         self,
         class_def: ast.ClassDef,
-        operation_definition: OperationDefinitionNode,
+        operation_definition: ExecutableDefinitionNode,
         selection_set: SelectionSetNode,
     ) -> ast.ClassDef:
         return class_def
 
     # pylint: disable=unused-argument
     def generate_result_field(
         self,
         field_implementation: ast.AnnAssign,
-        operation_definition: OperationDefinitionNode,
+        operation_definition: ExecutableDefinitionNode,
         field: FieldNode,
     ) -> ast.AnnAssign:
         return field_implementation
 
     def generate_scalars_module(self, module: ast.Module) -> ast.Module:
         return module
 
@@ -145,7 +146,18 @@
 
     def generate_init_code(self, generated_code: str) -> str:
         return generated_code
 
     # pylint: disable=unused-argument
     def process_name(self, name: str, node: Optional[Node] = None) -> str:
         return name
+
+    # pylint: disable=unused-argument
+    def generate_fragments_module(
+        self,
+        module: ast.Module,
+        fragments_definitions: Dict[str, FragmentDefinitionNode],
+    ) -> ast.Module:
+        return module
+
+    def process_schema(self, schema: GraphQLSchema) -> GraphQLSchema:
+        return schema
```

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/plugins/explorer.py` & `ariadne_codegen-0.7.0/ariadne_codegen/plugins/explorer.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.6.0/ariadne_codegen/plugins/manager.py` & `ariadne_codegen-0.7.0/ariadne_codegen/plugins/manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import ast
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 from graphql import (
+    ExecutableDefinitionNode,
     FieldNode,
+    FragmentDefinitionNode,
     GraphQLEnumType,
     GraphQLInputField,
     GraphQLInputObjectType,
     GraphQLSchema,
     Node,
-    OperationDefinitionNode,
     SelectionSetNode,
     VariableDefinitionNode,
 )
 
 from .base import Plugin
 
 
@@ -109,48 +110,48 @@
             "generate_input_field",
             field_implementation,
             input_field=input_field,
             field_name=field_name,
         )
 
     def generate_result_types_module(
-        self, module: ast.Module, operation_definition: OperationDefinitionNode
+        self, module: ast.Module, operation_definition: ExecutableDefinitionNode
     ) -> ast.Module:
         return self._apply_plugins_on_object(
             "generate_result_types_module",
             module,
             operation_definition=operation_definition,
         )
 
     def generate_operation_str(
-        self, operation_str: str, operation_definition: OperationDefinitionNode
+        self, operation_str: str, operation_definition: ExecutableDefinitionNode
     ) -> str:
         return self._apply_plugins_on_object(
             "generate_operation_str",
             operation_str,
             operation_definition=operation_definition,
         )
 
     def generate_result_class(
         self,
         class_def: ast.ClassDef,
-        operation_definition: OperationDefinitionNode,
+        operation_definition: ExecutableDefinitionNode,
         selection_set: SelectionSetNode,
     ) -> ast.ClassDef:
         return self._apply_plugins_on_object(
             "generate_result_class",
             class_def,
             operation_definition=operation_definition,
             selection_set=selection_set,
         )
 
     def generate_result_field(
         self,
         field_implementation: ast.AnnAssign,
-        operation_definition: OperationDefinitionNode,
+        operation_definition: ExecutableDefinitionNode,
         field: FieldNode,
     ) -> ast.AnnAssign:
         return self._apply_plugins_on_object(
             "generate_result_field",
             field_implementation,
             operation_definition=operation_definition,
             field=field,
@@ -186,7 +187,28 @@
         return self._apply_plugins_on_object("generate_scalars_code", generated_code)
 
     def generate_init_code(self, generated_code: str) -> str:
         return self._apply_plugins_on_object("generate_init_code", generated_code)
 
     def process_name(self, name: str, node: Optional[Node] = None) -> str:
         return self._apply_plugins_on_object("process_name", name, node=node)
+
+    def generate_fragments_module(
+        self,
+        module: ast.Module,
+        fragments_definitions: Dict[str, FragmentDefinitionNode],
+    ) -> ast.Module:
+        return self._apply_plugins_on_object(
+            "generate_fragments_module",
+            module,
+            fragments_definitions=fragments_definitions,
+        )
+
+    def process_schema(self, schema: GraphQLSchema) -> GraphQLSchema:
+        processed_schema = schema
+        for plugin in self.plugins:
+            processed_schema = plugin.process_schema(processed_schema)
+
+            for plugin in self.plugins:
+                plugin.schema = processed_schema
+
+        return processed_schema
```

### Comparing `ariadne_codegen-0.6.0/.gitignore` & `ariadne_codegen-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.6.0/LICENSE` & `ariadne_codegen-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.6.0/README.md` & `ariadne_codegen-0.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 
 [![Build Status](https://github.com/mirumee/ariadne-codegen/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/mirumee/ariadne-codegen/actions)
 
 - - - - -
 
 # Ariadne Code Generator
 
-Python code generator that takes graphql schema, queries and mutations and generates Python package with fully typed and asynchronous GraphQL client.
+Python code generator that takes graphql schema, queries, mutations and subscriptions and generates Python package with fully typed and asynchronous GraphQL client.
 
 It's available as `ariadne-codegen` command and reads configuration from the `pyproject.toml` file:
 
 ```
 $ ariadne-codegen
 ```
 
+It can also be run as `python -m ariadne_codegen`.
+
 
 ## Features
 
 - Generate pydantic models from schema types, inputs and enums.
 - Generate pydantic models for GraphQL results.
 - Generate client package with each GraphQL operation available as async method.
 
@@ -26,19 +28,33 @@
 
 Ariadne Code Generator can be installed with pip:
 
 ```
 $ pip install ariadne-codegen
 ```
 
+To support subscriptions, default base client requires `websockets` package:
+
+```
+$ pip install ariadne-codegen[subscriptions]
+```
+
 
 ## Configuration
 
 `ariadne-codegen` reads configuration from `[tool.ariadne-codegen]` section in your `pyproject.toml`. You can use other configuration file with `--config` option, eg. `ariadne-codegen --config custom_file.toml`
 
+Minimal configuration for client generation:
+
+```toml
+[tool.ariadne-codegen]
+schema_path = "schema.graphql"
+queries_path = "queries.graphql"
+```
+
 Required settings:
 
 - `queries_path` - path to file/directory with queries
 
 One of the following 2 parameters is required, in case of providing both of them `schema_path` is prioritized:
 
 - `schema_path` - path to file/directory with graphql schema
@@ -52,26 +68,34 @@
 - `target_package_path` (defaults to cwd) - path where to generate package
 - `client_name` (defaults to `"Client"`) - name of generated client class
 - `client_file_name` (defaults to `"client"`) - name of file with generated client class
 - `base_client_name` (defaults to `"AsyncBaseClient"`) - name of base client class
 - `base_client_file_path` (defaults to `.../graphql_sdk_gen/generators/async_base_client.py`) - path to file where `base_client_name` is defined
 - `enums_module_name` (defaults to `"enums"`) - name of file with generated enums models
 - `input_types_module_name` (defaults to `"input_types"`) - name of file with generated input types models
+- `fragments_module_name` (defaults to `"fragments"`) - name of file with generated fragments models
 - `include_comments` (defaults to `true`) - a flag that specifies whether to include comments in generated files
 - `convert_to_snake_case` (defaults to `true`) - a flag that specifies whether to convert fields and arguments names to snake case
 - `async_client` (defaults to `true`) - default generated client is `async`, change this to option `false` to generate synchronous client instead
 - `files_to_include` (defaults to `[]`) - list of files which will be copied into generated package
 - `plugins` (defaults to `[]`) - list of plugins to use during generation
 
 
 ## Plugins
 
 Ariadne Codegen implements a plugin system that enables further customization and fine-tuning of generated Python code. It’s documentation is available separately in the [PLUGINS.md](https://github.com/mirumee/ariadne-codegen/blob/main/PLUGINS.md) file.
 
 
+### Standard plugins
+
+Ariadne Codegen ships with optional plugins importable from the `ariadne_codegen.contrib` package:
+
+- [`ariadne_codegen.contrib.shorter_results.ShorterResultsPlugin`](ariadne_codegen/contrib/shorter_results.py) - This plugin processes generated client methods for operations where only single top field is requested, so they return this field's value directly instead of operation's result type. For example get_user method generated for query `GetUser() { user(...) { ... }}` will return value of user field directly instead of `GetUserResult`.
+
+
 ## Using generated client
 
 Generated client can be imported from package:
 ```py
 from {target_package_name}.{client_file_name} import {client_name}
 ```
 
@@ -88,14 +112,22 @@
 ```
 
 For more complex scenarios, you can pass your own http client:
 ```py
 client = Client(http_client=CustomComplexHttpClient())
 ```
 
+`CustomComplexHttpClient` needs to be an instance of `httpx.AsyncClient` for async client, or `httpx.Client` for sync.
+
+
+### Websockets
+
+To handle subscriptions, default `AsyncBaseClient` uses [websockets](https://github.com/python-websockets/websockets) and implements [graphql-transport-ws](https://github.com/enisdenjo/graphql-ws/blob/master/PROTOCOL.md) subprotocol. Arguments `ws_origin` and `ws_headers` are added as headers to the handshake request and `ws_connection_init_payload` is used as payload of [ConnectionInit](https://github.com/enisdenjo/graphql-ws/blob/master/PROTOCOL.md#connectioninit) message.
+
+
 ## Custom scalars
 
 By default, not built-in scalars are represented as `typing.Any` in generated client.
 You can provide information about specific scalar by adding section to `pyproject.toml`:
 
 ```toml
 [tool.ariadne-codegen.scalars.{graphql scalar name}]
@@ -106,15 +138,15 @@
 
 All occurrences of `{graphql scalar name}` will be represented as `type`. If provided, `serialize` and `parse` will be used for serialization and deserialization.
 If `type`/`serialize`/`parse` contains at least one `.` then string will be split by it's last occurrence. First part will be used as module to import from, and second part as type/method name. For example, `type = "custom_scalars.a.ScalarA"` will produce `from custom_scalars.a import ScalarA`.
 
 
 ### Example with scalar mapped to built-in type
 
-In this case scalar is mapped to built-in `str` which doesn\`t require custom `serialize ` and `parse` methods. 
+In this case scalar is mapped to built-in `str` which doesn't require custom `serialize ` and `parse` methods.
 
 ```toml
 [tool.ariadne-codegen.scalars.SCALARA]
 type = "str"
 ```
 
 
@@ -162,15 +194,16 @@
 ```
 
 This directive can be used along with `files_to_include` option to extend functionality of generated classes.
 
 
 #### Example of usage of `mixin` and `files_to_include`:
 
-Query with `mixin` directive: 
+Query with `mixin` directive:
+
 ```gql
 query listUsers {
     users @mixin(from: ".mixins", import: "UsersMixin") {
         id
     }
 }
 ```
@@ -199,41 +232,44 @@
 ```
 
 
 ## Generated code dependencies
 
 Generated code requires:
 
-- pydantic
-- httpx (can be avoided by providing another base client class with `base_client_file_path` and `base_client_name` parameters)
+- [pydantic](https://github.com/pydantic/pydantic)
+- [httpx](https://github.com/encode/httpx)
+- [websockets](https://github.com/python-websockets/websockets) (only for default async base client)
+
+Both `httpx` and `websockets` dependencies can be avoided by providing another base client class with `base_client_file_path` and `base_client_name` options.
 
 
 ## Example
 
 Example with simple schema and few queries and mutations is available [here](https://github.com/mirumee/ariadne-codegen/blob/main/EXAMPLE.md).
 
 
 ## Generating graphql schema's python representation
 
 Instead of generating client, you can generate file with a copy of GraphQL schema as `GraphQLSchema` declaration. To do this call `ariadne-codegen` with `graphqlschema` argument:
 ```
 ariadne-codegen graphqlschema
 ```
 
-`graphqlschema` mode reads configuration from the same place as [`client`](#configuration) but uses only `schema_path`, `remote_schema_url`, `remote_schema_headers` and `remote_schema_verify_ssl` options with addition to some extra options specific to it:    
+`graphqlschema` mode reads configuration from the same place as [`client`](#configuration) but uses only `schema_path`, `remote_schema_url`, `remote_schema_headers`, `remote_schema_verify_ssl` and `plugins` options with addition to some extra options specific to it:
 
 - `target_file_path` (defaults to `"schema.py"`) - destination path for generated file
 - `schema_variable_name` (defaults to `"schema"`) - name for schema variable, must be valid python identifier
 - `type_map_variable_name` (defaults to `"type_map"`) - name for type map variable, must be valid python identifier
 
 Generated file contains:
 
 - Necessary imports
 - Type map declaration `{type_map_variable_name}: TypeMap = {...}`
-- Schema declaration `{schema_variable_name}: GraphQLSchema = GraphQLSchema(...)` 
+- Schema declaration `{schema_variable_name}: GraphQLSchema = GraphQLSchema(...)`
 
 
 ## Contributing
 
 We welcome all contributions to Ariadne! If you've found a bug or issue, feel free to use [GitHub issues](https://github.com/mirumee/ariadne-codegen/issues). If you have any questions or feedback, don't hesitate to catch us on [GitHub discussions](https://github.com/mirumee/ariadne/discussions/).
 
 For guidance and instructions, please see [CONTRIBUTING.md](CONTRIBUTING.md).
```

### Comparing `ariadne_codegen-0.6.0/pyproject.toml` & `ariadne_codegen-0.7.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ariadne-codegen"
 description = "Generate fully typed GraphQL client from schema, queries and mutations!"
 authors = [{ name = "Mirumee Software", email = "hello@mirumee.com" }]
-version = "0.6.0"
+version = "0.7.0"
 readme = "README.md"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
@@ -34,38 +34,40 @@
 dev = [
   "pytest",
   "pylint",
   "mypy",
   "types-toml",
   "pytest-mock",
   "pytest-asyncio",
+  "pytest-httpx",
   "freezegun",
 ]
+subscriptions = ["websockets~=11.0"]
 
 [project.scripts]
 ariadne-codegen = "ariadne_codegen.main:main"
 
 [project.urls]
 "Homepage" = "https://ariadnegraphql.org/"
 "Repository" = "https://github.com/mirumee/ariadne-codegen"
 "Bug Tracker" = "https://github.com/mirumee/ariadne-codegen/issues"
 "Community" = "https://github.com/mirumee/ariadne/discussions"
 "Twitter" = "https://twitter.com/AriadneGraphQL"
 
 [tool.pylint.messages_control]
 max-line-length = 88
 disable = [
-    "missing-docstring",
-    "redefined-outer-name",
-    "too-few-public-methods",
-    "too-many-instance-attributes",
-    "too-many-arguments",
-    "duplicate-code",
-    "no-name-in-module",
-    "too-many-locals",
+  "missing-docstring",
+  "redefined-outer-name",
+  "too-few-public-methods",
+  "too-many-instance-attributes",
+  "too-many-arguments",
+  "duplicate-code",
+  "no-name-in-module",
+  "too-many-locals",
 ]
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 [tool.isort]
 profile = "black"
@@ -75,10 +77,8 @@
   "ariadne_codegen/**/*.py",
   "ariadne_codegen/py.typed",
   "LICENSE",
   "README.md",
   "EXAMPLE.md",
   "pyproject.toml",
 ]
-exclude = [
-  "tests",
-]
+exclude = ["tests"]
```

### Comparing `ariadne_codegen-0.6.0/PKG-INFO` & `ariadne_codegen-0.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ariadne-codegen
-Version: 0.6.0
+Version: 0.7.0
 Summary: Generate fully typed GraphQL client from schema, queries and mutations!
 Project-URL: Homepage, https://ariadnegraphql.org/
 Project-URL: Repository, https://github.com/mirumee/ariadne-codegen
 Project-URL: Bug Tracker, https://github.com/mirumee/ariadne-codegen/issues
 Project-URL: Community, https://github.com/mirumee/ariadne/discussions
 Project-URL: Twitter, https://twitter.com/AriadneGraphQL
 Author-email: Mirumee Software <hello@mirumee.com>
@@ -28,34 +28,39 @@
 Requires-Dist: toml~=0.10
 Provides-Extra: dev
 Requires-Dist: freezegun; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pylint; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-asyncio; extra == 'dev'
+Requires-Dist: pytest-httpx; extra == 'dev'
 Requires-Dist: pytest-mock; extra == 'dev'
 Requires-Dist: types-toml; extra == 'dev'
+Provides-Extra: subscriptions
+Requires-Dist: websockets~=11.0; extra == 'subscriptions'
 Description-Content-Type: text/markdown
 
 [![Ariadne](https://ariadnegraphql.org/img/logo-horizontal-sm.png)](https://ariadnegraphql.org)
 
 [![Build Status](https://github.com/mirumee/ariadne-codegen/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/mirumee/ariadne-codegen/actions)
 
 - - - - -
 
 # Ariadne Code Generator
 
-Python code generator that takes graphql schema, queries and mutations and generates Python package with fully typed and asynchronous GraphQL client.
+Python code generator that takes graphql schema, queries, mutations and subscriptions and generates Python package with fully typed and asynchronous GraphQL client.
 
 It's available as `ariadne-codegen` command and reads configuration from the `pyproject.toml` file:
 
 ```
 $ ariadne-codegen
 ```
 
+It can also be run as `python -m ariadne_codegen`.
+
 
 ## Features
 
 - Generate pydantic models from schema types, inputs and enums.
 - Generate pydantic models for GraphQL results.
 - Generate client package with each GraphQL operation available as async method.
 
@@ -64,19 +69,33 @@
 
 Ariadne Code Generator can be installed with pip:
 
 ```
 $ pip install ariadne-codegen
 ```
 
+To support subscriptions, default base client requires `websockets` package:
+
+```
+$ pip install ariadne-codegen[subscriptions]
+```
+
 
 ## Configuration
 
 `ariadne-codegen` reads configuration from `[tool.ariadne-codegen]` section in your `pyproject.toml`. You can use other configuration file with `--config` option, eg. `ariadne-codegen --config custom_file.toml`
 
+Minimal configuration for client generation:
+
+```toml
+[tool.ariadne-codegen]
+schema_path = "schema.graphql"
+queries_path = "queries.graphql"
+```
+
 Required settings:
 
 - `queries_path` - path to file/directory with queries
 
 One of the following 2 parameters is required, in case of providing both of them `schema_path` is prioritized:
 
 - `schema_path` - path to file/directory with graphql schema
@@ -90,26 +109,34 @@
 - `target_package_path` (defaults to cwd) - path where to generate package
 - `client_name` (defaults to `"Client"`) - name of generated client class
 - `client_file_name` (defaults to `"client"`) - name of file with generated client class
 - `base_client_name` (defaults to `"AsyncBaseClient"`) - name of base client class
 - `base_client_file_path` (defaults to `.../graphql_sdk_gen/generators/async_base_client.py`) - path to file where `base_client_name` is defined
 - `enums_module_name` (defaults to `"enums"`) - name of file with generated enums models
 - `input_types_module_name` (defaults to `"input_types"`) - name of file with generated input types models
+- `fragments_module_name` (defaults to `"fragments"`) - name of file with generated fragments models
 - `include_comments` (defaults to `true`) - a flag that specifies whether to include comments in generated files
 - `convert_to_snake_case` (defaults to `true`) - a flag that specifies whether to convert fields and arguments names to snake case
 - `async_client` (defaults to `true`) - default generated client is `async`, change this to option `false` to generate synchronous client instead
 - `files_to_include` (defaults to `[]`) - list of files which will be copied into generated package
 - `plugins` (defaults to `[]`) - list of plugins to use during generation
 
 
 ## Plugins
 
 Ariadne Codegen implements a plugin system that enables further customization and fine-tuning of generated Python code. It’s documentation is available separately in the [PLUGINS.md](https://github.com/mirumee/ariadne-codegen/blob/main/PLUGINS.md) file.
 
 
+### Standard plugins
+
+Ariadne Codegen ships with optional plugins importable from the `ariadne_codegen.contrib` package:
+
+- [`ariadne_codegen.contrib.shorter_results.ShorterResultsPlugin`](ariadne_codegen/contrib/shorter_results.py) - This plugin processes generated client methods for operations where only single top field is requested, so they return this field's value directly instead of operation's result type. For example get_user method generated for query `GetUser() { user(...) { ... }}` will return value of user field directly instead of `GetUserResult`.
+
+
 ## Using generated client
 
 Generated client can be imported from package:
 ```py
 from {target_package_name}.{client_file_name} import {client_name}
 ```
 
@@ -126,14 +153,22 @@
 ```
 
 For more complex scenarios, you can pass your own http client:
 ```py
 client = Client(http_client=CustomComplexHttpClient())
 ```
 
+`CustomComplexHttpClient` needs to be an instance of `httpx.AsyncClient` for async client, or `httpx.Client` for sync.
+
+
+### Websockets
+
+To handle subscriptions, default `AsyncBaseClient` uses [websockets](https://github.com/python-websockets/websockets) and implements [graphql-transport-ws](https://github.com/enisdenjo/graphql-ws/blob/master/PROTOCOL.md) subprotocol. Arguments `ws_origin` and `ws_headers` are added as headers to the handshake request and `ws_connection_init_payload` is used as payload of [ConnectionInit](https://github.com/enisdenjo/graphql-ws/blob/master/PROTOCOL.md#connectioninit) message.
+
+
 ## Custom scalars
 
 By default, not built-in scalars are represented as `typing.Any` in generated client.
 You can provide information about specific scalar by adding section to `pyproject.toml`:
 
 ```toml
 [tool.ariadne-codegen.scalars.{graphql scalar name}]
@@ -144,15 +179,15 @@
 
 All occurrences of `{graphql scalar name}` will be represented as `type`. If provided, `serialize` and `parse` will be used for serialization and deserialization.
 If `type`/`serialize`/`parse` contains at least one `.` then string will be split by it's last occurrence. First part will be used as module to import from, and second part as type/method name. For example, `type = "custom_scalars.a.ScalarA"` will produce `from custom_scalars.a import ScalarA`.
 
 
 ### Example with scalar mapped to built-in type
 
-In this case scalar is mapped to built-in `str` which doesn\`t require custom `serialize ` and `parse` methods. 
+In this case scalar is mapped to built-in `str` which doesn't require custom `serialize ` and `parse` methods.
 
 ```toml
 [tool.ariadne-codegen.scalars.SCALARA]
 type = "str"
 ```
 
 
@@ -200,15 +235,16 @@
 ```
 
 This directive can be used along with `files_to_include` option to extend functionality of generated classes.
 
 
 #### Example of usage of `mixin` and `files_to_include`:
 
-Query with `mixin` directive: 
+Query with `mixin` directive:
+
 ```gql
 query listUsers {
     users @mixin(from: ".mixins", import: "UsersMixin") {
         id
     }
 }
 ```
@@ -237,41 +273,44 @@
 ```
 
 
 ## Generated code dependencies
 
 Generated code requires:
 
-- pydantic
-- httpx (can be avoided by providing another base client class with `base_client_file_path` and `base_client_name` parameters)
+- [pydantic](https://github.com/pydantic/pydantic)
+- [httpx](https://github.com/encode/httpx)
+- [websockets](https://github.com/python-websockets/websockets) (only for default async base client)
+
+Both `httpx` and `websockets` dependencies can be avoided by providing another base client class with `base_client_file_path` and `base_client_name` options.
 
 
 ## Example
 
 Example with simple schema and few queries and mutations is available [here](https://github.com/mirumee/ariadne-codegen/blob/main/EXAMPLE.md).
 
 
 ## Generating graphql schema's python representation
 
 Instead of generating client, you can generate file with a copy of GraphQL schema as `GraphQLSchema` declaration. To do this call `ariadne-codegen` with `graphqlschema` argument:
 ```
 ariadne-codegen graphqlschema
 ```
 
-`graphqlschema` mode reads configuration from the same place as [`client`](#configuration) but uses only `schema_path`, `remote_schema_url`, `remote_schema_headers` and `remote_schema_verify_ssl` options with addition to some extra options specific to it:    
+`graphqlschema` mode reads configuration from the same place as [`client`](#configuration) but uses only `schema_path`, `remote_schema_url`, `remote_schema_headers`, `remote_schema_verify_ssl` and `plugins` options with addition to some extra options specific to it:
 
 - `target_file_path` (defaults to `"schema.py"`) - destination path for generated file
 - `schema_variable_name` (defaults to `"schema"`) - name for schema variable, must be valid python identifier
 - `type_map_variable_name` (defaults to `"type_map"`) - name for type map variable, must be valid python identifier
 
 Generated file contains:
 
 - Necessary imports
 - Type map declaration `{type_map_variable_name}: TypeMap = {...}`
-- Schema declaration `{schema_variable_name}: GraphQLSchema = GraphQLSchema(...)` 
+- Schema declaration `{schema_variable_name}: GraphQLSchema = GraphQLSchema(...)`
 
 
 ## Contributing
 
 We welcome all contributions to Ariadne! If you've found a bug or issue, feel free to use [GitHub issues](https://github.com/mirumee/ariadne-codegen/issues). If you have any questions or feedback, don't hesitate to catch us on [GitHub discussions](https://github.com/mirumee/ariadne/discussions/).
 
 For guidance and instructions, please see [CONTRIBUTING.md](CONTRIBUTING.md).
```

