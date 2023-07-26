# Comparing `tmp/bridgeapi-1.0.0b1.tar.gz` & `tmp/bridgeapi-1.0.0b2.tar.gz`

## Comparing `bridgeapi-1.0.0b1.tar` & `bridgeapi-1.0.0b2.tar`

### file list

```diff
@@ -1,13 +1,20 @@
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b1/src/bridgeapi/__about__.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b1/src/bridgeapi/__init__.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b1/src/bridgeapi/base_client.py
--rw-r--r--   0        0        0    16352 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b1/src/bridgeapi/client.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b1/src/bridgeapi/exceptions.py
--rw-r--r--   0        0        0     8186 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b1/src/bridgeapi/models.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b1/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b1/tests/test_base_client.py
--rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b1/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b1/LICENSE.txt
--rw-r--r--   0        0        0     4778 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b1/README.md
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/.envrc
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/.vscode/settings.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/src/bridgeapi/__about__.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/src/bridgeapi/__init__.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/src/bridgeapi/base_client.py
+-rw-r--r--   0        0        0    16307 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/src/bridgeapi/client.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/src/bridgeapi/exceptions.py
+-rw-r--r--   0        0        0     8305 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/src/bridgeapi/models.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/tests/__init__.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/tests/conftest.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/tests/test_base_client.py
+-rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/tests/test_client.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/tests/test_paginated_result.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/tests/test_user_client_auth.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/tests/cassettes/test_client/test_user_client[list_items].yaml
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/LICENSE.txt
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/README.md
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 bridgeapi-1.0.0b2/PKG-INFO
```

### Comparing `bridgeapi-1.0.0b1/src/bridgeapi/base_client.py` & `bridgeapi-1.0.0b2/src/bridgeapi/base_client.py`

 * *Files identical despite different names*

### Comparing `bridgeapi-1.0.0b1/src/bridgeapi/client.py` & `bridgeapi-1.0.0b2/src/bridgeapi/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,29 +166,28 @@
         auto_renew: bool = True,
     ):
         super().__init__(client_id, client_secret)
         self.user_email = user_email
         self.user_password = user_password
         self.auto_renew = auto_renew
 
-        n_auth_args = sum([user_uuid is None, access_token is None, expires_at is None])
-        if n_auth_args != 3:  # noqa: PLR2004
-            if n_auth_args != 0:
-                msg = (
-                    "all of [user_uuid, access_token, expires_at] must be passed when setting "
-                    "user auth"
-                )
-                raise ValueError(msg)
+        auth_args = [user_uuid, access_token, expires_at]
+        if all(arg is None for arg in auth_args):
+            self.user_uuid = None
+            self.access_token = None
+            self.expires_at = None
+        elif all(arg is not None for arg in auth_args):
             self.user_uuid = user_uuid
             self.access_token = access_token
             self.expires_at = expires_at
         else:
-            self.user_uuid = None
-            self.access_token = None
-            self.expires_at = None
+            msg = (
+                "all of (user_uuid, access_token, expires_at) must be passed if setting user auth"
+            )
+            raise ValueError(msg)
 
     def is_authenticated(self, delay: dt.timedelta = dt.timedelta(minutes=1)) -> bool:
         """Return whether the user authentication is valid (defined and not expired).
 
         Args:
             delay (dt.timedelta, default 1 minute): delay by which to anticipate
                 renewal before expiration, to avoid edge conditions at expiration time.
```

### Comparing `bridgeapi-1.0.0b1/src/bridgeapi/exceptions.py` & `bridgeapi-1.0.0b2/src/bridgeapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `bridgeapi-1.0.0b1/src/bridgeapi/models.py` & `bridgeapi-1.0.0b2/src/bridgeapi/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 import requests
 from pydantic import BaseModel, HttpUrl, PrivateAttr, constr
 from pydantic.generics import GenericModel
 
 from bridgeapi.base_client import BaseClient
 from bridgeapi.exceptions import PaginationError
 
-BaseModelT = TypeVar("BaseModelT", bound="BridgeBaseModel")
+ModelT = TypeVar("ModelT", bound="BaseResponseModel")
 
 
-class BridgeBaseModel(BaseModel):
+class BaseResponseModel(BaseModel):
     """Base model for all API resources. Allows storing the API response object along
     with the parsed data, accessible through the property `.response`.
 
     When there are nested models, the response will only be stored on the root
     container, and the property will be None in the children.
     """
 
     _response: requests.Response | None = PrivateAttr(None)
 
     @classmethod
-    def from_response(cls: type[BaseModelT], response: requests.Response) -> BaseModelT:
+    def from_response(cls: type[ModelT], response: requests.Response) -> ModelT:
         value = cls.parse_obj(response.json())
         value._response = response
         return value
 
     @property
     def response(self) -> requests.Response | None:
         return self._response
@@ -39,19 +39,20 @@
 _T = TypeVar("_T")
 
 
 class Pagination(BaseModel):
     next_uri: str | None = None
 
 
-class PaginatedResult(BridgeBaseModel, GenericModel, Generic[_T]):
+class PaginatedResult(BaseResponseModel, GenericModel, Generic[_T]):
     """Container storing results of a paginated API call."""
 
     resources: list[_T]
     pagination: Pagination
+    generated_at: dt.datetime | None  # Only exposed by list_categories
 
     _client: "BaseClient" = PrivateAttr()
     _page_number: int = PrivateAttr()
 
     @classmethod
     def from_response(
         cls, response: requests.Response, client: "BaseClient", page_number: int = 0
@@ -73,43 +74,43 @@
         return self.__class__.from_response(response, self._client, self._page_number + 1)
 
     def fetch_all(self) -> list[_T]:
         if self._page_number != 0:
             msg = "paginated result has already been partially consumed"
             raise PaginationError(msg)
         result = self
-        resources = result.resources
+        resources = result.resources.copy()
         while result.has_more():
             result = result.next_page()
             resources.extend(result.resources)
         return resources
 
 
 # Banks
 class BankFormFieldType(Enum):
     USER = "USER"
     PWD = "PWD"
     PWD2 = "PWD2"
 
 
-class BankFormField(BridgeBaseModel):
+class BankFormField(BaseResponseModel):
     label: str
     type: BankFormFieldType
     isNum: str  # '0' or '1'  # noqa: N815  # mixedCase
     maxLength: int | None = None  # noqa: N815
     minLength: int | None = None  # noqa: N815
 
 
-class BankTransferProperties(BridgeBaseModel):
+class BankTransferProperties(BaseResponseModel):
     nb_max_transactions: int
     max_size_label: int | None = None
     multiple_dates_transfers: bool
 
 
-class BankPaymentProperties(BridgeBaseModel):
+class BankPaymentProperties(BaseResponseModel):
     nb_max_transactions: int
     max_size_label: int
     multiple_dates_payments: bool
     sender_iban_available: bool
 
 
 class BankAuthenticationType(Enum):
@@ -131,15 +132,15 @@
 
 
 class BankChannelType(Enum):
     DSP2 = "dsp2"
     DIRECT_ACCESS = "direct_access"
 
 
-class Bank(BridgeBaseModel):
+class Bank(BaseResponseModel):
     id: int
     name: str
     # Known countries as of 2023-07: BE, DE, ES, FR, GB, IT, LU, NL, PT
     country_code: constr(min_length=2, max_length=2)
     logo_url: str  # Should be HttpUrl, but found ""
     authentication_type: BankAuthenticationType
     form: list[BankFormField]
@@ -153,75 +154,76 @@
     transfer: BankTransferProperties | None = None
     payment: BankPaymentProperties | None = None
     display_order: int | None = None
     authentication_page_url: str | None = None
 
 
 # Users
-class User(BridgeBaseModel):
+class User(BaseResponseModel):
     uuid: UUID
     email: str
 
 
-class UserAuthInfo(BridgeBaseModel):
+class UserAuthInfo(BaseResponseModel):
     access_token: str
     expires_at: dt.datetime
     user: User
 
 
-class UserEmailValidation(BridgeBaseModel):
+class UserEmailValidation(BaseResponseModel):
     name: Literal["email"]
     is_confirmed: bool
 
 
 # Bridge Connect
-class BridgeConnectUrl(BridgeBaseModel):
+class BridgeConnectUrl(BaseResponseModel):
     redirect_url: HttpUrl
 
 
 # Items
-class Item(BridgeBaseModel):
+class Item(BaseResponseModel):
     # Codes and documentation at https://docs.bridgeapi.io/reference/item-resource
     id: int
     status: int
     status_code_info: str
     status_code_description: str | None
     bank_id: int
 
 
-class ItemMfa(BridgeBaseModel):
+class ItemMfa(BaseResponseModel):
     type: str | None  # SMS or APP_TO_APP
     description: str | None
     label: str
     is_numeric: bool
 
 
-class ItemRefreshStatus(BridgeBaseModel):
+class ItemRefreshStatus(BaseResponseModel):
     # Codes and documentation at https://docs.bridgeapi.io/reference/get-a-refresh-status
+    id: str
     status: str
     refreshed_at: dt.datetime
     mfa: ItemMfa | None
     refreshed_accounts_count: int | None
     total_accounts_count: int | None
 
 
 # Accounts
-class LoanAccountDetails(BridgeBaseModel):
+class LoanAccountDetails(BaseResponseModel):
     next_payment_date: dt.date
     next_payment_amount: Decimal
     maturity_date: dt.date
     opening_date: dt.date
     interest_rate: float
     type: str
     borrowed_capital: Decimal
     repaid_capital: Decimal
     remaining_capital: Decimal
 
 
-class SavingsAccountDetails(BridgeBaseModel):
+class SavingsAccountDetails(BaseResponseModel):
     opening_date: dt.date
     interest_rate: float
     ceiling: Decimal
 
 
 class AccountType(Enum):
     CHECKING = "checking"
@@ -232,15 +234,15 @@
     SHARED_SAVING_PLAN = "shared_saving_plan"
     PENDING = "pending"
     LIFE_INSURANCE = "life_insurance"
     SPECIAL = "special"
     UNKNOWN = "unknown"
 
 
-class Account(BridgeBaseModel):
+class Account(BaseResponseModel):
     id: int
     name: str
     balance: Decimal
     status: int
     status_code_info: str
     status_code_description: str | None
     updated_at: dt.datetime
@@ -252,15 +254,15 @@
     loan_details: LoanAccountDetails | None
     savings_details: SavingsAccountDetails | None
     is_pro: bool
     iban: str | None
 
 
 # Transactions
-class Transaction(BridgeBaseModel):
+class Transaction(BaseResponseModel):
     id: int
     clean_description: str
     bank_description: str
     amount: Decimal
     date: dt.date
     updated_at: dt.datetime
     currency_code: constr(min_length=3, max_length=3)  # 3-letter ISO 4217 currency code
@@ -268,15 +270,15 @@
     category_id: int
     account_id: int
     is_future: bool
     show_client_side: bool
 
 
 # Stocks
-class Stock(BridgeBaseModel):
+class Stock(BaseResponseModel):
     id: int
     current_price: Decimal
     quantity: Decimal
     total_value: Decimal
     average_purchase_price: Decimal
     updated_at: dt.datetime
     ticker: str  # Stock 4-character identifier
@@ -288,22 +290,22 @@
     label: str
     value_date: dt.date
     is_deleted: bool
     account_id: int
 
 
 # Categories
-class Category(BridgeBaseModel):
+class Category(BaseResponseModel):
     id: int
     name: str
     parent_id: int | None
 
 
-class ChildCategory(BridgeBaseModel):
+class ChildCategory(BaseResponseModel):
     id: int
     name: str
 
 
-class ParentCategory(BridgeBaseModel):
+class ParentCategory(BaseResponseModel):
     id: int
     name: str
     categories: list[ChildCategory]
```

### Comparing `bridgeapi-1.0.0b1/.gitignore` & `bridgeapi-1.0.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `bridgeapi-1.0.0b1/LICENSE.txt` & `bridgeapi-1.0.0b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bridgeapi-1.0.0b1/README.md` & `bridgeapi-1.0.0b2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # bridgeapi
 
 [![PyPI - Version](https://img.shields.io/pypi/v/bridgeapi.svg)](https://pypi.org/project/bridgeapi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bridgeapi.svg)](https://pypi.org/project/bridgeapi)
 
 -----
 
-`bridgeapi` is a client for the [Bridge open banking API aggregator](https://bridgeapi.io).
+`bridgeapi` is a client for the [Bridge open banking API aggregator](https://bridgeapi.io) ([API documentation](https://docs.bridgeapi.io/docs)).
 
 ## Requirements
 
 Python 3.10+
 
 ## Installation
 
@@ -22,20 +22,22 @@
 ```python
 from bridgeapi import AppClient, UserClient
 
 app_client = AppClient("CLIENT_ID", "CLIENT_SECRET")
 app_client.list_banks()
 app_client.list_users()
 app_client.create_user("john@doe.com", "password")
+...
 
 user_client = UserClient("CLIENT_ID", "CLIENT_SECRET", "john@doe.com", "password")
 user_client.list_items()
 user_client.connect_item()
 user_client.list_accounts()
 user_client.list_transactions()
+...
 ```
 
 API endpoints are split between two clients:
 * `AppClient` handles all application-scoped endpoints, that don't depend on a user being
   authenticated. It only needs (client_id, client_secret) credentials to communicate with the API.
 * `UserClient` handles user-scoped endpoints, those that are specific to a user and require an
   access token and the `Authorization` header to communicate with the API. It needs (user_email,
@@ -128,15 +130,15 @@
 user_client = UserClient(
     "CLIENT_ID",
     "CLIENT_SECRET",
     "john@doe.com",
     "password",
     user_uuid="uuid",
     access_token="token",
-    expires_at="yyyy-mm-dd HH:MM:SS",
+    expires_at=datetime,  # "yyyy-mm-dd HH:MM:SS"
     auto_renew=False,
 )
 print(user_client.is_authenticated())  # True
 user_client.list_items()  # OK
 
 # Generate and store new authorization info
 auth_info = user_client.renew_auth()
```

### Comparing `bridgeapi-1.0.0b1/pyproject.toml` & `bridgeapi-1.0.0b2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -17,28 +17,31 @@
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = ["pydantic", "requests"]
+dependencies = ["pydantic == 1.*", "requests"]
 
 [project.urls]
 Documentation = "https://gitlab.com/alex-marty/bridgeapi"
 Issues = "https://gitlab.com/alex-marty/bridgeapi/-/issues"
 Source = "https://gitlab.com/alex-marty/bridgeapi"
 
 [tool.hatch.version]
 path = "src/bridgeapi/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
+  "pytest-mock",
+  "pytest-recording",
+  "vcrpy==4.*"
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
```

### Comparing `bridgeapi-1.0.0b1/PKG-INFO` & `bridgeapi-1.0.0b2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: bridgeapi
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Client for the Bridge open banking API aggregator
 Project-URL: Documentation, https://gitlab.com/alex-marty/bridgeapi
 Project-URL: Issues, https://gitlab.com/alex-marty/bridgeapi/-/issues
 Project-URL: Source, https://gitlab.com/alex-marty/bridgeapi
 Author-email: Alexandre Marty <contact@marty.in>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
-Requires-Dist: pydantic
+Requires-Dist: pydantic==1.*
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # bridgeapi
 
 [![PyPI - Version](https://img.shields.io/pypi/v/bridgeapi.svg)](https://pypi.org/project/bridgeapi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bridgeapi.svg)](https://pypi.org/project/bridgeapi)
 
 -----
 
-`bridgeapi` is a client for the [Bridge open banking API aggregator](https://bridgeapi.io).
+`bridgeapi` is a client for the [Bridge open banking API aggregator](https://bridgeapi.io) ([API documentation](https://docs.bridgeapi.io/docs)).
 
 ## Requirements
 
 Python 3.10+
 
 ## Installation
 
@@ -43,20 +43,22 @@
 ```python
 from bridgeapi import AppClient, UserClient
 
 app_client = AppClient("CLIENT_ID", "CLIENT_SECRET")
 app_client.list_banks()
 app_client.list_users()
 app_client.create_user("john@doe.com", "password")
+...
 
 user_client = UserClient("CLIENT_ID", "CLIENT_SECRET", "john@doe.com", "password")
 user_client.list_items()
 user_client.connect_item()
 user_client.list_accounts()
 user_client.list_transactions()
+...
 ```
 
 API endpoints are split between two clients:
 * `AppClient` handles all application-scoped endpoints, that don't depend on a user being
   authenticated. It only needs (client_id, client_secret) credentials to communicate with the API.
 * `UserClient` handles user-scoped endpoints, those that are specific to a user and require an
   access token and the `Authorization` header to communicate with the API. It needs (user_email,
@@ -149,15 +151,15 @@
 user_client = UserClient(
     "CLIENT_ID",
     "CLIENT_SECRET",
     "john@doe.com",
     "password",
     user_uuid="uuid",
     access_token="token",
-    expires_at="yyyy-mm-dd HH:MM:SS",
+    expires_at=datetime,  # "yyyy-mm-dd HH:MM:SS"
     auto_renew=False,
 )
 print(user_client.is_authenticated())  # True
 user_client.list_items()  # OK
 
 # Generate and store new authorization info
 auth_info = user_client.renew_auth()
```

