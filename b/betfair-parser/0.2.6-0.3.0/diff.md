# Comparing `tmp/betfair_parser-0.2.6.tar.gz` & `tmp/betfair_parser-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betfair_parser-0.2.6.tar", max compression
+gzip compressed data, was "betfair_parser-0.3.0.tar", max compression
```

## Comparing `betfair_parser-0.2.6.tar` & `betfair_parser-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,34 @@
--rw-r--r--   0        0        0      386 2023-05-28 02:35:07.711966 betfair_parser-0.2.6/README.md
--rw-r--r--   0        0        0        0 2023-05-28 02:35:07.711966 betfair_parser-0.2.6/betfair_parser/__init__.py
--rw-r--r--   0        0        0      919 2023-05-28 02:35:07.711966 betfair_parser-0.2.6/betfair_parser/core.py
--rw-r--r--   0        0        0        0 2023-05-28 02:35:07.711966 betfair_parser-0.2.6/betfair_parser/spec/__init__.py
--rw-r--r--   0        0        0       85 2023-05-28 02:35:07.711966 betfair_parser-0.2.6/betfair_parser/spec/accounts/__init__.py
--rw-r--r--   0        0        0     2929 2023-05-28 02:35:07.711966 betfair_parser-0.2.6/betfair_parser/spec/accounts/enums.py
--rw-r--r--   0        0        0     3127 2023-05-28 02:35:07.711966 betfair_parser-0.2.6/betfair_parser/spec/accounts/operations.py
--rw-r--r--   0        0        0    11161 2023-05-28 02:35:07.711966 betfair_parser-0.2.6/betfair_parser/spec/accounts/type_definitions.py
--rw-r--r--   0        0        0       84 2023-05-28 02:35:07.711966 betfair_parser-0.2.6/betfair_parser/spec/betting/__init__.py
--rw-r--r--   0        0        0    20833 2023-05-28 02:35:07.711966 betfair_parser-0.2.6/betfair_parser/spec/betting/enums.py
--rw-r--r--   0        0        0     9556 2023-05-28 02:35:07.711966 betfair_parser-0.2.6/betfair_parser/spec/betting/listings.py
--rw-r--r--   0        0        0      134 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/betting/operations.py
--rw-r--r--   0        0        0     8762 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/betting/orders.py
--rw-r--r--   0        0        0    29242 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/betting/type_definitions.py
--rw-r--r--   0        0        0     5811 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/common.py
--rw-r--r--   0        0        0      923 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/constants.py
--rw-r--r--   0        0        0     7970 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/error.py
--rw-r--r--   0        0        0     1775 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/heartbeat.py
--rw-r--r--   0        0        0     4181 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/navigation.py
--rw-r--r--   0        0        0     2975 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/race_status.py
--rw-r--r--   0        0        0      324 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/streaming/__init__.py
--rw-r--r--   0        0        0     6233 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/streaming/mcm.py
--rw-r--r--   0        0        0     2247 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/streaming/ocm.py
--rw-r--r--   0        0        0     2422 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/spec/streaming/status.py
--rw-r--r--   0        0        0     2148 2023-05-28 02:35:07.715966 betfair_parser-0.2.6/betfair_parser/strenums.py
--rw-r--r--   0        0        0      737 2023-05-28 02:35:37.971668 betfair_parser-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 betfair_parser-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1286 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0      614 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/betfair_parser/__init__.py
+-rw-r--r--   0        0        0     2038 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/betfair_parser/client.py
+-rw-r--r--   0        0        0     2417 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/betfair_parser/endpoints.py
+-rw-r--r--   0        0        0      741 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/betfair_parser/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/betfair_parser/spec/__init__.py
+-rw-r--r--   0        0        0       85 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/betfair_parser/spec/accounts/__init__.py
+-rw-r--r--   0        0        0     2929 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/betfair_parser/spec/accounts/enums.py
+-rw-r--r--   0        0        0     3177 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/betfair_parser/spec/accounts/operations.py
+-rw-r--r--   0        0        0    11161 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/betfair_parser/spec/accounts/type_definitions.py
+-rw-r--r--   0        0        0       84 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/betfair_parser/spec/betting/__init__.py
+-rw-r--r--   0        0        0    21951 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/betting/enums.py
+-rw-r--r--   0        0        0     9634 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/betting/listings.py
+-rw-r--r--   0        0        0      134 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/betting/operations.py
+-rw-r--r--   0        0        0     8860 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/betting/orders.py
+-rw-r--r--   0        0        0    32756 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/betting/type_definitions.py
+-rw-r--r--   0        0        0      238 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/common/__init__.py
+-rw-r--r--   0        0        0     9826 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/common/enums.py
+-rw-r--r--   0        0        0     6202 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/common/messages.py
+-rw-r--r--   0        0        0     1526 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/common/type_definitions.py
+-rw-r--r--   0        0        0      279 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/common/types.py
+-rw-r--r--   0        0        0     2773 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/heartbeat.py
+-rw-r--r--   0        0        0     8653 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/identity.py
+-rw-r--r--   0        0        0     3662 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/navigation.py
+-rw-r--r--   0        0        0     3172 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/race_status.py
+-rw-r--r--   0        0        0      399 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/streaming/__init__.py
+-rw-r--r--   0        0        0     5989 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/streaming/mcm.py
+-rw-r--r--   0        0        0     2247 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/streaming/ocm.py
+-rw-r--r--   0        0        0     2507 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/streaming/status.py
+-rw-r--r--   0        0        0     2319 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/strenums.py
+-rw-r--r--   0        0        0      902 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/util.py
+-rw-r--r--   0        0        0     1731 2023-06-01 21:25:32.448697 betfair_parser-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 betfair_parser-0.3.0/PKG-INFO
```

### Comparing `betfair_parser-0.2.6/betfair_parser/core.py` & `betfair_parser-0.3.0/betfair_parser/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 import bz2
 import tarfile
+import typing
 
 import fsspec
 import msgspec
 
-from betfair_parser.spec.streaming import STREAM_DECODER, STREAM_MESSAGE
+from betfair_parser.spec.streaming import stream_decode
 
 
-def parse(line: bytes) -> STREAM_MESSAGE:
-    return STREAM_DECODER.decode(line)
+def iter_file(fsspec_url: str):
+    with fsspec.open(fsspec_url, compression="infer") as f:
+        yield from iter_stream(f)
 
 
-def iter_parse(file_like):
+def iter_tar_file(tar_file: str, file_path: str):
+    tf = tarfile.open(tar_file)
+    assert file_path in tf.getnames(), f"Can't find `{file_path}` in {tf.getnames()[:5]}... "
+    f = tf.extractfile(file_path)
+    assert f is not None
+    if file_path.endswith("bz2"):
+        f = bz2.open(f)
+    yield from iter_stream(f)  # type: ignore
+
+
+def iter_stream(file_like: typing.BinaryIO):
     for line in file_like:
         try:
-            data = parse(line)
+            data = stream_decode(line)
         except (msgspec.DecodeError, msgspec.ValidationError) as e:
             print("ERR", e)
             print(msgspec.json.decode(line))
             raise e
         yield data
-
-
-def read_file(fsspec_url: str):
-    with fsspec.open(fsspec_url, compression="infer") as f:
-        yield from iter_parse(f)
-
-
-def read_tar_file(tar_file: str, file_path: str):
-    tf = tarfile.open(tar_file)
-    assert file_path in tf.getnames(), f"Can't find `{file_path}` in {tf.getnames()[:5]}... "
-    f = tf.extractfile(file_path)
-    if file_path.endswith("bz2"):
-        f = bz2.open(f)
-    yield from iter_parse(f)
```

### Comparing `betfair_parser-0.2.6/betfair_parser/spec/accounts/enums.py` & `betfair_parser-0.3.0/betfair_parser/spec/accounts/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.6/betfair_parser/spec/accounts/operations.py` & `betfair_parser-0.3.0/betfair_parser/spec/accounts/operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 from typing import Optional
 
+from betfair_parser.exceptions import AccountAPINGException
 from betfair_parser.spec.accounts.enums import IncludeItem, Wallet
 from betfair_parser.spec.accounts.type_definitions import (
     AccountDetailsResponse,
     AccountFundsResponse,
     AccountStatementReport,
     CurrencyRate,
 )
-from betfair_parser.spec.common import APIException, BaseMessage, Request, Response, TimeRange
-from betfair_parser.spec.error import AccountAPIExceptionCode
+from betfair_parser.spec.common import EndpointType, Params, Request, Response, TimeRange
 
 
-AccountAPIException = APIException[AccountAPIExceptionCode]
+class AccountRequest(Request, frozen=True):
+    endpoint_type = EndpointType.ACCOUNTS
+    throws = AccountAPINGException  # type: ignore
 
 
-class _GetAccountFundsParams(BaseMessage, frozen=True):
+class _GetAccountFundsParams(Params, frozen=True):
     wallet: Optional[Wallet] = None  # Name of the wallet in question. Global wallet is returned by default
 
 
-class GetAccountFunds(Request, kw_only=True, frozen=True):
+class GetAccountFunds(AccountRequest, kw_only=True, frozen=True):
     """Returns the available to bet amount, exposure and commission information."""
 
     method = "AccountAPING/v1.0/getAccountFunds"
     params: _GetAccountFundsParams
     return_type = Response[AccountFundsResponse]
-    throws = AccountAPIException
 
 
-class GetAccountDetails(Request, kw_only=True, frozen=True):
+class GetAccountDetails(AccountRequest, kw_only=True, frozen=True):
     """Returns the details relating your account, including your discount rate and Betfair point balance."""
 
     method = "AccountAPING/v1.0/getAccountDetails"
     return_type = Response[AccountDetailsResponse]
-    throws = AccountAPIException
 
 
-class _GetAccountStatementParams(BaseMessage, frozen=True):
+class _GetAccountStatementParams(Params, frozen=True):
     locale: Optional[str] = None  # The language to be used where applicable. Defaults to account settings
     from_record: Optional[int] = None  # Specifies the first record that will be returned, defaults to 0
     record_count: Optional[int] = None  # Specifies the maximum number of records to be returned. Maximum 100
 
     # Return items with an itemDate within this date range. Both from and to date times are inclusive.
     # If from is not specified then the oldest available items will be in range. If to is not specified
     # then the latest items will be in range. nb. This itemDataRange is currently only applied when
     # includeItem is set to ALL or not specified, else items are NOT bound by itemDate.
     # Please note:  You can only retrieve account statement items for the last 90 days.
     item_date_range: Optional[TimeRange] = None
     include_item: Optional[IncludeItem] = None  # Which items to include, if not specified then defaults to ALL.
     wallet: Optional[Wallet] = None  # Which wallet to return statementItems for. Defaults to UK
 
 
-class GetAccountStatement(Request, kw_only=True, frozen=True):
+class GetAccountStatement(AccountRequest, kw_only=True, frozen=True):
+    """Return the account statement. Essentially a large list of your last profits and losses."""
+
     method = "AccountAPING/v1.0/getAccountStatement"
     params: _GetAccountStatementParams
     return_type = Response[AccountStatementReport]
-    throws = AccountAPIException
 
 
-class _ListCurrencyRatesParams(BaseMessage, frozen=True):
+class _ListCurrencyRatesParams(Params, frozen=True):
     from_currency: Optional[str] = None  # The currency from which the rates are computed. Only GBP for now.
 
 
-class ListCurrencyRates(Request, kw_only=True, frozen=True):
+class ListCurrencyRates(AccountRequest, kw_only=True, frozen=True):
     """Returns a list of currency rates based on given currency. Updates only once per hour."""
 
     method = "AccountAPING/v1.0/listCurrencyRates"
     params: _ListCurrencyRatesParams
     return_type = Response[list[CurrencyRate]]
-    throws = AccountAPIException
```

### Comparing `betfair_parser-0.2.6/betfair_parser/spec/accounts/type_definitions.py` & `betfair_parser-0.3.0/betfair_parser/spec/accounts/type_definitions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.6/betfair_parser/spec/betting/enums.py` & `betfair_parser-0.3.0/betfair_parser/spec/betting/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from betfair_parser.spec.common import EventTypeIdCode  # noqa for reimport
 from betfair_parser.strenums import DocumentedEnum, StrEnum, auto, doc
 
 
 class MarketProjection(DocumentedEnum):
     COMPETITION = doc("If not selected then the competition will not be returned with marketCatalogue")
     EVENT = doc("If not selected then the event will not be returned with marketCatalogue")
     EVENT_TYPE = doc("If not selected then the eventType will not be returned with marketCatalogue")
@@ -367,7 +368,47 @@
     PAYOUT = doc("The total payout requested on a LimitOrder")
 
 
 class PriceLadderType(DocumentedEnum):
     CLASSIC = doc("Price ladder increments traditionally used for Odds Markets.")
     FINEST = doc("Price ladder with the finest available increment, traditionally used for Asian Handicap markets.")
     LINE_RANGE = doc("Price ladder used for LINE markets. Refer to MarketLineRangeInfo for more details.")
+
+
+class MarketTypeCode(StrEnum):
+    """This is not a complete list, but only a selection of some popular options for direct access.
+
+    A full list can be retrieved from the API using ListMarketTypes.
+    """
+
+    ALT_TOTAL_GOALS = auto()
+    ANTEPOST_WIN = auto()
+    ASIAN_HANDICAP = auto()
+    BOTH_TEAMS_TO_SCORE = auto()
+    COMBINED_TOTAL = auto()
+    CORRECT_SCORE = auto()
+    EACH_WAY = auto()
+    EXACTA = auto()
+    FORECAST = auto()
+    HANDICAP = auto()
+    MATCH_BET = auto()
+    MATCH_ODDS = auto()
+    NUMBER_OF_SETS = auto()
+    OTHER_PLACE = auto()
+    OUTRIGHT_WINNER = auto()
+    OVER_UNDER_05 = auto()
+    OVER_UNDER_25 = auto()
+    PLACE = auto()
+    PLAYER_A_WIN_A_SET = auto()
+    PLAYER_B_WIN_A_SET = auto()
+    QUARTER_WINNER = auto()
+    QUINELLA = auto()
+    RACE_WIN_DIST = auto()
+    SEASON_SPECIALS = auto()
+    SET_BETTING = auto()
+    SET_CORRECT_SCORE = auto()
+    SET_WINNER = auto()
+    TOURNAMENT_WINNER = auto()
+    TRAP_CHALLENGE = auto()
+    UNUSED = auto()
+    WIN = auto()
+    WITHOUT_FAV = auto()
```

### Comparing `betfair_parser-0.2.6/betfair_parser/spec/betting/listings.py` & `betfair_parser-0.3.0/betfair_parser/spec/betting/listings.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,111 +17,109 @@
     MarketFilter,
     MarketProfitAndLoss,
     MarketTypeResult,
     PriceProjection,
     TimeRangeResult,
     VenueResult,
 )
-from betfair_parser.spec.common import BaseMessage, BetId, Date, MarketId, Request, Response, SelectionId
+from betfair_parser.spec.common import BetId, Date, EndpointType, MarketId, Params, Request, Response, SelectionId
 
 
-class _ListingParams(BaseMessage, frozen=True):
+class ListingRequest(Request, frozen=True):
+    endpoint_type = EndpointType.BETTING
+
+
+class _ListingParams(Params, frozen=True):
     filter: MarketFilter
     locale: Optional[str] = None
 
 
-class ListCompetitions(Request, kw_only=True, frozen=True):
+class ListCompetitions(ListingRequest, kw_only=True, frozen=True):
     """
     Returns a list of Competitions (i.e., World Cup 2013) associated with the markets selected by
     the MarketFilter. Currently only Football markets have an associated competition.
     """
 
     method = "SportsAPING/v1.0/listCompetitions"
     params: _ListingParams
     return_type = Response[list[CompetitionResult]]
 
 
-class ListCountries(Request, kw_only=True, frozen=True):
+class ListCountries(ListingRequest, kw_only=True, frozen=True):
     """
     Returns a list of Countries associated with the markets selected by the MarketFilter.
     """
 
     method = "SportsAPING/v1.0/listCountries"
     params: _ListingParams
     return_type = Response[list[CountryCodeResult]]
 
 
-class ListEvents(Request, kw_only=True, frozen=True):
+class ListEvents(ListingRequest, kw_only=True, frozen=True):
     """
     Returns a list of Events (i.e, Reading vs. Man United) associated with the markets selected
     by the MarketFilter.
     """
 
     method = "SportsAPING/v1.0/listEvents"
     params: _ListingParams
     return_type = Response[list[EventResult]]
 
 
-class ListEventTypes(Request, kw_only=True, frozen=True):
+class ListEventTypes(ListingRequest, kw_only=True, frozen=True):
     """
     Returns a list of Event Types (i.e. Sports) associated with the markets selected by the
     MarketFilter.
     """
 
     method = "SportsAPING/v1.0/listEventTypes"
     params: _ListingParams
     return_type = Response[list[EventTypeResult]]
 
 
-class ListMarketTypes(Request, kw_only=True, frozen=True):
+class ListMarketTypes(ListingRequest, kw_only=True, frozen=True):
     """
     Returns a list of market types (i.e. MATCH_ODDS, NEXT_GOAL) associated with the markets selected
     by the MarketFilter. The market types are always the same, regardless of locale.
     """
 
     method = "SportsAPING/v1.0/listMarketTypes"
     params: _ListingParams
     return_type = Response[list[MarketTypeResult]]
 
 
-class ListVenues(Request, kw_only=True, frozen=True):
+class ListVenues(ListingRequest, kw_only=True, frozen=True):
     """
     Returns a list of Venues (i.e. Cheltenham, Ascot) associated with the markets selected by the
     MarketFilter. Currently, only Horse Racing markets are associated with a Venue.
     """
 
     method = "SportsAPING/v1.0/listVenues"
     params: _ListingParams
     return_type = Response[list[VenueResult]]
 
 
 # More complex listings
 
 
-class _ListMarketBookParams(BaseMessage, frozen=True):
+class _ListMarketBookParams(Params, frozen=True):
     market_ids: list[str]  # One or more market ids
-    price_projection: Optional[
-        PriceProjection
-    ] = None  # The projection of price data you want to receive in the response
+    price_projection: Optional[PriceProjection] = None  # The desired projection of price data
     order_projection: Optional[OrderProjection] = None  # The orders you want to receive in the response
     match_projection: Optional[MatchProjection] = None  # If you ask for orders, specifies the representation of matches
     include_overall_position: Optional[bool] = None  # If you ask for orders, returns matches for each selection
-    partition_matched_by_strategy_ref: Optional[
-        bool
-    ] = None  # Returns the breakdown of matches by strategy for each selection
+    partition_matched_by_strategy_ref: Optional[bool] = None  # Breakdown of matches by strategy for each selection
     customer_strategy_refs: Optional[set[str]] = None
     currency_code: Optional[str] = None  # A Betfair standard currency code
     locale: Optional[str] = None  # The language used for the response
-    matched_since: Optional[
-        Date
-    ] = None  # Restricts to orders with at least one fragment matched since the specified date
-    bet_ids: Optional[set[BetId]] = None  # Restricts to orders with the specified bet IDs
+    matched_since: Optional[Date] = None  # Only orders with at least one fragment matched since the specified date
+    bet_ids: Optional[set[BetId]] = None  # Only orders with the specified bet IDs
 
 
-class ListMarketBook(Request, kw_only=True, frozen=True):
+class ListMarketBook(ListingRequest, kw_only=True, frozen=True):
     """
     Returns a list of dynamic data about markets. Dynamic data includes prices, the status of the
     market, the status of selections, the traded volume, and the status of any orders you have
     placed in the market.
 
     Please note: Separate requests should be made for OPEN & CLOSED markets. Request that include
     both OPEN & CLOSED markets will only return those markets that are OPEN.
@@ -138,90 +136,91 @@
     """
 
     method = "SportsAPING/v1.0/listMarketBook"
     params: _ListMarketBookParams
     return_type = Response[list[MarketBook]]
 
 
-class _ListMarketCatalogueParams(BaseMessage, kw_only=True, frozen=True):
+class _ListMarketCatalogueParams(Params, kw_only=True, frozen=True):
     filter: MarketFilter  # The filter to select desired markets
     market_projection: Optional[set[MarketProjection]] = None  # The type and amount of data returned about the market
     sort: Optional[MarketSort] = None  # The order of the results, defaults to RANK
     max_results: int  # Limit on the total number of results returned
     locale: Optional[str] = None  # The language used for the response
 
 
-class ListMarketCatalogue(Request, kw_only=True, frozen=True):
+class ListMarketCatalogue(ListingRequest, kw_only=True, frozen=True):
     """
     Returns a list of information about published (ACTIVE/SUSPENDED) markets that does not change
     (or changes very rarely). You use listMarketCatalogue to retrieve the name of the market, the
     names of selections and other information about markets.  Market Data Request Limits apply to
     requests made to listMarketCatalogue.
 
     Please note: listMarketCatalogue does not return markets that are CLOSED.
     """
 
     method = "SportsAPING/v1.0/listMarketCatalogue"
     params: _ListMarketCatalogueParams
     return_type = Response[list[MarketCatalogue]]
 
 
-class _ListMarketProfitAndLossParams(BaseMessage, frozen=True):
+ListMarketCatalog = ListMarketCatalogue  # allow both spellings
+
+
+class _ListMarketProfitAndLossParams(Params, frozen=True):
     market_ids: set[MarketId]  # List of markets to calculate profit and loss
     include_settled_bets: Optional[bool] = False  # Option to include settled bets (partially settled markets only)
     include_bsp_bets: Optional[bool] = False  # Option to include BSP bets
     net_of_commission: Optional[bool] = False  # Option to return profit and loss net of users current commission rate
 
 
-class ListMarketProfitAndLoss(Request, kw_only=True, frozen=True):
+class ListMarketProfitAndLoss(ListingRequest, kw_only=True, frozen=True):
     """Returns a list of Countries associated with the markets selected by the MarketFilter."""
 
     method = "SportsAPING/v1.0/listMarketProfitAndLoss"
     params: _ListMarketProfitAndLossParams
     return_type = Response[list[MarketProfitAndLoss]]
 
 
-class _ListRunnerBookParams(BaseMessage, frozen=True):
+class _ListRunnerBookParams(Params, frozen=True):
     market_id: MarketId  # The unique id for the market
     selection_id: SelectionId  # The unique id for the selection in the market
     handicap: Optional[float] = None  # The handicap associated with the runner in case of Asian handicap market
     price_projection: Optional[PriceProjection] = None
     order_projection: Optional[OrderProjection] = None
     match_projection: Optional[MatchProjection] = None  # If you ask for orders, specifies the representation of matches
     include_overall_position: Optional[bool] = None  # If you ask for orders, returns matches for each selection
-    partition_matched_by_strategy_ref: Optional[
-        bool
-    ] = None  # Return a breakdown of matches by strategy for each selection
+    partition_matched_by_strategy_ref: Optional[bool] = None  # Return a breakdown of matches by strategy
     customer_strategy_refs: Optional[set[str]] = None
     currency_code: Optional[str] = None  # A Betfair standard currency code
     locale: Optional[str] = None  # The language used for the response
     matched_since: Optional[Date] = None  # Restricts to orders with at least one fragment matched since specified date
     bet_ids: Optional[set[BetId]] = None  # Restricts to orders with the specified bet IDs
 
 
-class ListRunnerBook(Request, kw_only=True, frozen=True):
+class ListRunnerBook(ListingRequest, kw_only=True, frozen=True):
     """
     Returns a list of dynamic data about a market and a specified runner. Dynamic data includes
     prices, the status of the market, the status of selections, the traded volume, and the status
     of any orders you have placed in the market..
     """
 
     method = "SportsAPING/v1.0/listRunnerBook"
     params: _ListRunnerBookParams
     return_type = Response[list[MarketBook]]
 
 
-class _ListTimeRangesParams(BaseMessage, frozen=True):
+class _ListTimeRangesParams(Params, frozen=True):
     # The filter to select desired markets. All markets that match the criteria in the filter are selected.
     filter: MarketFilter
     # The granularity of time periods that correspond to markets selected by the market filter.
     granularity: TimeGranularity
 
 
-class ListTimeRanges(Request, kw_only=True, frozen=True):
+class ListTimeRanges(ListingRequest, kw_only=True, frozen=True):
     """
     Returns a list of time ranges in the granularity specified in the request (i.e. 3PM to 4PM,
     Aug 14th to Aug 15th) associated with the markets selected by the MarketFilter.
     """
 
     method = "SportsAPING/v1.0/listTimeRanges"
     params: _ListTimeRangesParams
```

### Comparing `betfair_parser-0.2.6/betfair_parser/spec/betting/orders.py` & `betfair_parser-0.3.0/betfair_parser/spec/betting/orders.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,38 +14,43 @@
     ReplaceExecutionReport,
     ReplaceInstruction,
     RunnerId,
     UpdateExecutionReport,
     UpdateInstruction,
 )
 from betfair_parser.spec.common import (
-    BaseMessage,
     BetId,
     CustomerOrderRef,
     CustomerRef,
     CustomerStrategyRef,
+    EndpointType,
     EventId,
     EventTypeId,
     MarketId,
+    Params,
     Request,
     Response,
     TimeRange,
 )
 
 
-class _PlaceOrdersParams(BaseMessage, frozen=True):
+class OrderRequest(Request, frozen=True):
+    endpoint_type = EndpointType.BETTING
+
+
+class _PlaceOrdersParams(Params, frozen=True):
     market_id: str
     instructions: list[PlaceInstruction]
     customer_ref: Optional[CustomerRef] = None
     market_version: Optional[MarketVersion] = None
     customer_strategy_ref: Optional[CustomerStrategyRef] = None
     async_: Optional[bool] = msgspec.field(name="async", default=False)
 
 
-class PlaceOrders(Request, kw_only=True, frozen=True):
+class PlaceOrders(OrderRequest, kw_only=True, frozen=True):
     """Place new orders into market.
 
     Please note that additional bet sizing rules apply to bets placed into the Italian Exchange.
 
     In normal circumstances the placeOrders is an atomic operation. PLEASE NOTE: if the
     'Best Execution' features is switched off, placeOrders can return ‘PROCESSED_WITH_ERRORS’
     meaning that some bets can be rejected and other placed when submitted in the same
@@ -53,53 +58,53 @@
     """
 
     method = "SportsAPING/v1.0/placeOrders"
     params: _PlaceOrdersParams
     return_type = Response[PlaceExecutionReport]
 
 
-class _CancelOrdersParams(BaseMessage, frozen=True):
+class _CancelOrdersParams(Params, frozen=True):
     market_id: Optional[str] = None
     instructions: Optional[list[CancelInstruction]] = None
     customer_ref: Optional[CustomerRef] = None
 
 
-class CancelOrders(Request, kw_only=True, frozen=True):
+class CancelOrders(OrderRequest, kw_only=True, frozen=True):
     """
     Cancel all bets OR cancel all bets on a market OR fully or partially cancel particular
     orders on a market. Only LIMIT orders can be cancelled or partially cancelled once placed.
     """
 
     method = "SportsAPING/v1.0/cancelOrders"
     params: _CancelOrdersParams
     return_type = Response[CancelExecutionReport]
 
 
-class _ReplaceOrdersParams(BaseMessage, frozen=True):
+class _ReplaceOrdersParams(Params, frozen=True):
     market_id: str
     instructions: list[ReplaceInstruction]
     customer_ref: Optional[CustomerRef] = None
     market_version: Optional[MarketVersion] = None
     async_: Optional[bool] = msgspec.field(name="async", default=False)
 
 
-class ReplaceOrders(Request, kw_only=True, frozen=True):
+class ReplaceOrders(OrderRequest, kw_only=True, frozen=True):
     """
     This operation is logically a bulk cancel followed by a bulk place. The cancel is completed
     first then the new orders are placed. The new orders will be placed atomically in that they
     will all be placed or none will be placed. In the case where the new orders cannot be placed
     the cancellations will not be rolled back. See ReplaceInstruction.
     """
 
     method = "SportsAPING/v1.0/replaceOrders"
     params: _ReplaceOrdersParams
     return_type = Response[ReplaceExecutionReport]
 
 
-class _ListClearedOrdersParams(BaseMessage, frozen=True):
+class _ListClearedOrdersParams(Params, frozen=True):
     bet_status: BetStatus  # Restricts the results to the specified status.
     event_type_ids: Optional[set[EventTypeId]] = None  # Restricts the results to the specified Event Type IDs.
     event_ids: Optional[set[EventId]] = None  # Restricts the results to the specified Event IDs.
     market_ids: Optional[set[MarketId]] = None  # Restricts the results to the specified market IDs.
     runner_ids: Optional[set[RunnerId]] = None  # Restricts the results to the specified Runners.
     bet_ids: Optional[set[BetId]] = None  # Restricts the results to the specified bet IDs, maximum 1000 betIds
     customer_order_refs: Optional[set[CustomerOrderRef]] = None
@@ -118,15 +123,15 @@
     group_by: Optional[GroupBy] = None
     include_item_description: Optional[bool] = None
     locale: Optional[str] = None  # The language used for the itemDescription, defaults to account settings
     from_record: Optional[int] = None  # Specifies the first record that will be returned. Records start at index zero.
     record_count: Optional[int] = None  # Number of records from the index position 'fromRecord', maximum 1000
 
 
-class ListClearedOrders(Request, kw_only=True, frozen=True):
+class ListClearedOrders(OrderRequest, kw_only=True, frozen=True):
     """
     Returns a list of settled bets based on the bet status, ordered by settled date. To retrieve
     more than 1000 records, you need to make use of the fromRecord and recordCount parameters.
 
     By default the service will return all available data for the last 90 days (see Best Practice
     note below).  The fields available at each roll-up are available here
 
@@ -137,15 +142,15 @@
     """
 
     method = "SportsAPING/v1.0/listClearedOrders"
     params: _ListClearedOrdersParams
     return_type = Response[ClearedOrderSummaryReport]
 
 
-class _ListCurrentOrdersParams(BaseMessage, frozen=True):
+class _ListCurrentOrdersParams(Params, frozen=True):
     """
     Parameters for retrieving a list of current orders.
     """
 
     bet_ids: Optional[set[BetId]] = None  # Restricts the results to the specified bet IDs
     market_ids: Optional[set[str]] = None  # Restricts the results to the specified market IDs
     order_projection: Optional[OrderProjection] = None  # Restricts the results to the specified order status
@@ -155,15 +160,15 @@
     order_by: Optional[OrderBy] = None  # Specifies how the results will be ordered
     sort_dir: Optional[SortDir] = None  # Specifies the direction the results will be sorted in
     from_record: Optional[int] = None  # Specifies the first record that will be returned
     record_count: Optional[int] = None  # Specifies how many records will be returned
     include_item_description: Optional[bool] = None
 
 
-class ListCurrentOrders(Request, kw_only=True, frozen=True):
+class ListCurrentOrders(OrderRequest, kw_only=True, frozen=True):
     """
     Returns a list of your current orders. Optionally you can filter and sort your current orders
     using the various parameters, setting none of the parameters will return all of your current
     orders up to a maximum of 1000 bets, ordered BY_BET and sorted EARLIEST_TO_LATEST. To retrieve
     more than 1000 orders, you need to make use of the fromRecord and recordCount parameters.
 
     Best Practice:
@@ -175,19 +180,19 @@
     """
 
     method = "SportsAPING/v1.0/listCurrentOrders"
     params: _ListCurrentOrdersParams
     return_type = Response[CurrentOrderSummaryReport]
 
 
-class _UpdateOrdersParams(BaseMessage, frozen=True):
+class _UpdateOrdersParams(Params, frozen=True):
     market_id: str  # The market id these orders are to be placed on
     instructions: list[UpdateInstruction]  # The limit of update instructions per request is 60
     customer_ref: Optional[CustomerRef] = None
 
 
-class UpdateOrders(Request, kw_only=True, frozen=True):
+class UpdateOrders(OrderRequest, kw_only=True, frozen=True):
     """Update non-exposure changing fields."""
 
     method = "SportsAPING/v1.0/updateOrders"
     params: _UpdateOrdersParams
     return_type = Response[UpdateExecutionReport]
```

### Comparing `betfair_parser-0.2.6/betfair_parser/spec/betting/type_definitions.py` & `betfair_parser-0.3.0/betfair_parser/spec/betting/type_definitions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional
 
 import msgspec
 
+from betfair_parser.endpoints import SILKS
 from betfair_parser.spec.betting.enums import (
     BetTargetType,
     ExecutionReportErrorCode,
     ExecutionReportStatus,
     InstructionReportErrorCode,
     InstructionReportStatus,
     MarketBettingType,
@@ -26,15 +27,17 @@
     CustomerOrderRef,
     CustomerRef,
     CustomerStrategyRef,
     Date,
     EventId,
     EventTypeId,
     ExchangeId,
+    FloatStr,
     Handicap,
+    IntStr,
     MarketId,
     MatchId,
     OrderStatus,
     OrderType,
     Price,
     SelectionId,
     Size,
@@ -99,36 +102,34 @@
 
 
 class TimeRangeResult(BaseMessage, frozen=True):
     time_range: Optional[TimeRange] = None
     market_count: Optional[int] = None  # Count of markets associated with this TimeRange
 
 
-class MarketFilter(BaseMessage, frozen=True):
+class MarketFilter(BaseMessage, omit_defaults=True, frozen=True):
     text_query: Optional[str] = None  # Restrict markets by any text associated with the Event name
     exchange_ids: Optional[set[ExchangeId]] = None  # DEPRECATED
     event_type_ids: Optional[set[EventTypeId]] = None  # Restrict markets by event type associated with the market
     event_ids: Optional[set[EventId]] = None  # Restrict markets by the event id associated with the market
-    competition_ids: Optional[
-        set[CompetitionId]
-    ] = None  # Restrict markets by the competitions associated with the market
+    competition_ids: Optional[set[CompetitionId]] = None  # Restrict markets by the competitions
     market_ids: Optional[set[MarketId]] = None  # Restrict markets by the market id associated with the market
     venues: Optional[set[Venue]] = None  # Restrict markets by the venue associated with the market
     bsp_only: Optional[bool] = None  # Restrict to bsp markets only if True or non-bsp markets if False
 
     # Restrict to markets that will turn in play if True or will not turn in play if False
     turn_in_play_enabled: Optional[bool] = None
 
     # Restrict to markets that are currently in play if True or are not currently in play if False
     in_play_only: Optional[bool] = None
     market_betting_types: Optional[set[MarketBettingType]] = None  # Match the betting type of the market
     market_countries: Optional[set[CountryCode]] = None  # Match the specified country or countries
     market_type_codes: Optional[set[str]] = None  # Restrict to markets that match the type of the market
     market_start_time: Optional[TimeRange] = None  # Restrict to markets with a market start time range
-    with_orders: Optional[set[str]] = None  # Restrict to markets that I have one or more orders in these status
+    with_orders: Optional[set[str]] = None  # Markets that have one or more orders of defined OrderStatus
     race_types: Optional[set[str]] = None  # Restrict by race type
 
 
 class MarketLineRangeInfo(BaseMessage, frozen=True):
     """Market Line and Range Info"""
 
     max_unit_value: float  # Maximum value for the outcome, in market units
@@ -229,35 +230,82 @@
     each_way_divisor: Optional[float] = None  # Divisor for EACH_WAY market type
     clarifications: Optional[str] = None  # Additional information regarding the market
     line_range_info: Optional[MarketLineRangeInfo] = None  # Line range info for line markets
     race_type: Optional[str] = None  # External identifier of a race type
     price_ladder_description: Optional[PriceLadderDescription] = None  # Details about the price ladder in use
 
 
+# TODO: Some fields in the meta data should be country codes. Unfortunately, sometimes they contain
+#       erroneous data that fails verification. This should be switched to CountryCode as soon as there is
+#       some more fine-grained error handling possible in msgspec. Related issue:
+#       https://github.com/jcrist/msgspec/issues/420
+_MetaCountryCode = str  # CountryCode
+
+
+class RunnerMetaData(BaseMessage, frozen=True, omit_defaults=True, rename="upper"):
+    # Yes, this is the only type definition, that has (mostly) uppered key names
+    """
+    Runner metadata as defined in the API as additional information.
+    https://docs.developer.betfair.com/display/1smk3cen4v3lu3yomq5qye0ni/Additional+Information
+    """
+
+    weight_units: Optional[str] = None  # The unit of weight used.
+    adjusted_rating: Optional[IntStr] = None  # Race-specific ratings that reflect weights allocated in the race
+    dam_year_born: Optional[IntStr] = None  # The year the horse’s mother's birth
+    days_since_last_run: Optional[IntStr] = None  # The number of days since the horse last ran
+    wearing: Optional[str] = None  # Any extra equipment the horse is wearing
+    damsire_year_born: Optional[IntStr] = None  # Year in which the horse's grandfather was born on its mother's side
+    sire_bred: Optional[_MetaCountryCode] = None  # The country where the horse's father was bred
+    trainer_name: Optional[str] = None  # The name of the horse's trainer
+    stall_draw: Optional[IntStr] = None  # The stall number the horse is starting from
+    sex_type: Optional[str] = None  # The sex of the horse
+    owner_name: Optional[str] = None  # The owner of the horse
+    sire_name: Optional[str] = None  # The name of the horse's father
+    forecastprice_numerator: Optional[IntStr] = None  # The forecast price numerator
+    forecastprice_denominator: Optional[IntStr] = None  # The forecast price denominator
+    jockey_claim: Optional[IntStr] = None  # Reduction in the weight that the horse carries for a particular jockey
+    weight_value: Optional[FloatStr] = None  # The weight of the horse
+    dam_name: Optional[str] = None  # The name of the horse's mother
+    age: Optional[IntStr] = None  # The age of the horse
+    colour_type: Optional[str] = None  # The colour of the horse
+    damsire_bred: Optional[_MetaCountryCode] = None  # The country where the horse's grandfather was born
+    damsire_name: Optional[str] = None  # The name of the horse's grandfather
+    sire_year_born: Optional[IntStr] = None  # The year the horse's father was born
+    official_rating: Optional[IntStr] = None  # The horses official rating
+    form: Optional[str] = None  # The horses recent form
+    bred: Optional[_MetaCountryCode] = None  # The country in which the horse was born
+    runner_id: Optional[IntStr] = msgspec.field(name="runnerId", default=None)  # The runnerId for the horse
+    jockey_name: Optional[str] = None  # Name of the jockey. This field will contain 'Reserve' if its a reserve runner
+    dam_bred: Optional[_MetaCountryCode] = None  # The country where the horse's mother was born
+    colours_description: Optional[str] = None  # The textual description of the jockey silk
+    colours_filename: Optional[str] = None  # Image representing the jockey silk
+    cloth_number: Optional[IntStr] = None  # The number on the saddle-cloth
+    cloth_number_alpha: Optional[str] = None  # The number on the saddle cloth for US paired runners, e.g. "1A"
+
+    @property
+    def colours_url(self):
+        if self.colours_filename:
+            return SILKS + self.colours_filename
+
+
 class RunnerCatalog(BaseMessage, frozen=True):
     """Information about the Runners (selections) in a market"""
 
     selection_id: int  # The unique id for the selection
     runner_name: str  # The name of the runner
 
     # The handicap applies to market with the MarketBettingType ASIAN_HANDICAP_SINGLE_LINE
     # & ASIAN_HANDICAP_DOUBLE_LINE only
     handicap: float
     sort_priority: Optional[int] = None  # This is marked as REQUIRED in the API doc, but omitted sometimes
-    metadata: Optional[dict[str, Optional[str]]] = None  # Metadata associated with the runner
+    metadata: Optional[RunnerMetaData] = None  # Metadata associated with the runner
 
     @property
-    def runner_id(self):
-        # TODO: Careful, selectionId is simply a number for a certain string. It's not
-        #       uniquely identifying a team or a certain horse.
-        if self.selection_id:
-            return self.selection_id
-        elif self.metadata.get("runner_id"):
-            return int(self.metadata.get("runner_id"))
-        return None
+    def name(self):
+        return self.runner_name
 
 
 class Runner(BaseMessage, frozen=True):
     """The dynamic data about runners in a market"""
 
     selection_id: int  # The unique id of the runner (selection)
     handicap: float  # The handicap
@@ -266,15 +314,15 @@
     last_price_traded: Optional[float] = None  # The price of the most recent bet matched on this selection
     total_matched: Optional[float] = None  # The total amount matched on this runner
     removal_date: Optional[Date] = None  # If date and time the runner was removed
     sp: Optional[StartingPrices] = None  # The BSP related prices for this runner
     ex: Optional[ExchangePrices] = None  # The Exchange prices available for this runner
     orders: Optional[list[Order]] = None  # List of orders in the market
     matches: Optional[list[Match]] = None  # List of matches (i.e., orders that have been fully or partially executed)
-    matches_by_strategy: Optional[dict[str, Match]] = None  # List of matches for each strategy, ordered by matched data
+    matches_by_strategy: Optional[dict[str, list[Match]]] = None  # All matches for each strategy, sort by matched data
 
 
 class MarketCatalogue(BaseMessage, frozen=True):
     market_id: MarketId  # The unique identifier for the market
     market_name: str  # The name of the market
     market_start_time: Optional[Date] = None  # Only returned when the MARKET_START_TIME enum is requested
     description: Optional[MarketDescription] = None  # Details about the market
@@ -399,15 +447,18 @@
     price_size: PriceSize  # The price and size of the bet
     bsp_liability: Size  # The liability of a given BSP bet
     side: Side  # BACK/LAY
     status: OrderStatus  # The status of the order
     persistence_type: PersistenceType  # What to do with the order at turn-in-play
     order_type: OrderType  # BSP Order type
     placed_date: Date  # The date the bet was placed
-    matched_date: Date  # The date of the last matched bet fragment
+
+    # The date of the last matched bet fragment.
+    # Mandatory according to documentation, but optional in reality
+    matched_date: Optional[Date] = None
     average_price_matched: Optional[Price] = None  # The average price matched at
     size_matched: Optional[Size] = None
     size_remaining: Optional[Size] = None
     size_lapsed: Optional[Size] = None
     size_cancelled: Optional[Size] = None
     size_voided: Optional[Size] = None
     regulator_auth_code: Optional[str] = None
@@ -420,15 +471,15 @@
 class CurrentOrderSummaryReport(BaseMessage, frozen=True):
     """A container representing search results"""
 
     current_orders: list[CurrentOrderSummary]  # The list of current orders returned by the query
     more_available: bool  # Indicates whether there are further result items beyond this page
 
 
-class LimitOrder(BaseMessage, frozen=True):
+class LimitOrder(BaseMessage, omit_defaults=True, frozen=True):
     """Place a new LIMIT order (simple exchange bet for immediate execution)"""
 
     size: Size
     price: Price
     persistence_type: PersistenceType
     time_in_force: Optional[TimeInForce] = None
     min_fill_size: Optional[Size] = None
@@ -500,15 +551,15 @@
 
 
 class CancelInstructionReport(BaseMessage, kw_only=True, frozen=True):
     status: InstructionReportStatus  # Whether the command succeeded or failed
     error_code: Optional[InstructionReportErrorCode] = None  # Cause of failure, or null if command succeeds
     instruction: Optional[CancelInstruction] = None  # The instruction that was requested
     size_cancelled: Optional[float] = None  # The API states, that this is mandatory, but it's skipped in case of error
-    cancelled_date: Optional[Date] = None
+    cancelled_date: Optional[Date] = None  # The API states, that this is mandatory, but it's skipped in case of error
 
 
 class CancelExecutionReport(BaseMessage, kw_only=True, frozen=True):
     customer_ref: Optional[CustomerRef] = None  # Echo of the customerRef if passed
     status: ExecutionReportStatus
     error_code: Optional[ExecutionReportErrorCode] = None
     market_id: Optional[MarketId] = None  # Echo of marketId passed
@@ -557,15 +608,15 @@
     best_prices_depth: Optional[int] = None  # The maximum number of prices to return on each side for each runner
     rollup_model: Optional[RollupModel] = None  # The model to use when rolling up available sizes
     rollup_limit: Optional[int] = None  # The volume limit to use when rolling up returned sizes
     rollup_liability_threshold: Optional[float] = None  # Only applicable when rollupModel is MANAGED_LIABILITY
     rollup_liability_factor: Optional[int] = None  # Only applicable when rollupModel is MANAGED_LIABILITY
 
 
-class PriceProjection(BaseMessage, frozen=True):
+class PriceProjection(BaseMessage, omit_defaults=True, frozen=True):
     """Selection criteria of the returning price data"""
 
     price_data: Optional[set[PriceData]] = None  # The basic price data you want to receive in the response
 
     # Options to alter the default representation of best offer prices
     ex_best_offers_overrides: Optional[ExBestOffersOverrides] = None
     virtualise: Optional[bool] = None  # Indicates if the returned prices should include virtual prices
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `betfair_parser-0.2.6/betfair_parser/spec/navigation.py` & `betfair_parser-0.3.0/betfair_parser/spec/navigation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,36 @@
 import re
-from typing import ClassVar, Literal, Optional, Union
+from typing import Literal, Optional, Union
 
-import msgspec
-
-from betfair_parser.spec.common import BaseMessage, Date, Request, decode, encode
-from betfair_parser.spec.constants import Locale
+from betfair_parser.spec.common import BaseMessage, BaseResponse, Date, EndpointType, IntStr, Request
 
 
 def tag_func(s: str):
     """
     >>> tag_func("EventType")
     'EVENT_TYPE'
 
     >>> tag_func("Group")
     'GROUP'
     """
     return re.sub(r"(?<!^)(?=[A-Z])", "_", s).upper()
 
 
-class _NavigationParams(BaseMessage, kw_only=True, frozen=True):
-    locale: Locale
-
-
-class NavigationRequest(Request, kw_only=True, frozen=True):
-    """
-    Navigation requests - https://docs.developer.betfair.com/display/1smk3cen4v3lu3yomq5qye0ni/Navigation+Data+For+Applications
-    """
-
-    METHOD_TEMPLATE: ClassVar[str] = "/betting/rest/v1/{locale}/navigation/menu.json"
-    params: _NavigationParams
-    method: str = METHOD_TEMPLATE.format(locale=Locale.English.value)
-
-    @classmethod
-    def with_locale(cls, params: _NavigationParams, locale: Locale):
-        method = cls.METHOD_TEMPLATE.format(locale=locale.value)
-        return msgspec.structs.replace(cls(params=params), method=method)
-
-
 class Market(BaseMessage, tag=tag_func, frozen=True):
     name: str
     id: str
     exchange_id: str
     market_type: str
-    market_start_time: str
+    market_start_time: Date
     number_of_winners: Union[int, str]
 
 
 class Event(BaseMessage, tag=tag_func, frozen=True):
     name: str
-    id: str
+    id: IntStr
     country_code: str
     children: list[Union["Group", "Event", Market]]
 
 
 class Race(BaseMessage, tag=tag_func, frozen=True):
     name: str
     id: str
@@ -67,79 +45,99 @@
     name: str
     id: str
     children: list[Union["Group", Event]]
 
 
 class EventType(BaseMessage, tag=tag_func, frozen=True):
     name: str
-    id: str
+    id: IntStr
     children: list[Union[Group, Event, Race]]
 
 
-class Navigation(BaseMessage, frozen=True):
-    """Navigation"""
+class Navigation(BaseResponse, frozen=True):
+    """Navigation root"""
 
     type: Literal["GROUP"]
     name: Literal["ROOT"]
     id: int
     children: list[EventType]
 
+    @property
+    def result(self):
+        # Play along with ordinary RPC Response objects
+        return self
+
+
+class Menu(Request, kw_only=True, frozen=True):
+    """Navigation requests
+
+    https://docs.developer.betfair.com/display/1smk3cen4v3lu3yomq5qye0ni/Navigation+Data+For+Applications
+    """
+
+    endpoint_type = EndpointType.NAVIGATION
+    method = ""
+    id: int = 0
+    return_type = Navigation  # type: ignore
+
 
 class FlattenedMarket(BaseMessage, kw_only=True, frozen=True, rename=None):
     event_type_name: str
-    event_type_id: str
+    event_type_id: IntStr
     event_name: Optional[str] = None
     event_id: Optional[str] = None
     event_country_code: Optional[str] = None
     market_name: str
     market_id: str
     market_exchange_id: str
     market_market_type: str
-    market_market_start_time: str
+    market_market_start_time: Date
     market_number_of_winners: Union[int, str]
     group_name: Optional[str] = None
     group_id: Optional[str] = None
     race_name: Optional[str] = None
     race_id: Optional[str] = None
     race_country_code: Optional[str] = None
     race_venue: Optional[str] = None
-    race_start_time: Optional[str] = None
+    race_start_time: Optional[Date] = None
     race_race_number: Optional[str] = None
 
 
-def navigation_to_flatten_markets(navigation: Navigation, **filters) -> list[FlattenedMarket]:
-    flattened = flatten_tree(decode(encode(navigation), type=Navigation), **filters)
-    return decode(encode(flattened), type=list[FlattenedMarket])
-
-
-def flatten_tree(navigation: dict, **filters):
-    """
-    Flatten a nested dict into a list of dicts with each nested level combined
-    into a single dict.
-    """
-    results = []
-    ignore_keys = ("type", "children")
+def flatten_nav_tree(navigation: Navigation, **filters) -> list[FlattenedMarket]:
+    return list(filter_flattened(flattened_nav_iter(navigation), **filters))
 
-    def _filter(k, v):
-        if isinstance(v, str):
-            return k == v
-        if isinstance(v, (tuple, list)):
-            return k in v
-        raise TypeError
-
-    def flatten(nav_item, depth: Optional[int] = None):
-        depth = depth or 0
-        node_type = tag_func(nav_item.__class__.__name__).lower()
-        data = {f"{node_type}_{k}": v for k, v in nav_item.to_dict().items() if k not in ignore_keys}
-        if hasattr(nav_item, "children"):
-            for child in nav_item.children:
-                for child_data in flatten(child, depth=depth + 1):
-                    if depth == 0:
-                        if all(_filter(child_data[k], v) for k, v in filters.items()):
-                            results.append(child_data)
-                    else:
-                        yield {**data, **child_data}
-        else:
-            yield data
 
-    list(flatten(navigation))
-    return results
+def _filter(k, v):
+    if isinstance(v, str):
+        return k == v
+    if isinstance(v, (tuple, list)):
+        return k in v
+    raise TypeError
+
+
+def filter_flattened(nav_iter, **filters):
+    for flattened in nav_iter:
+        if all(_filter(getattr(flattened, k), v) for k, v in filters.items()):
+            yield flattened
+
+
+def flattened_nav_iter(node, **context):
+    node_type_name = tag_func(node.__class__.__name__).lower()
+    context[node_type_name] = node
+    if isinstance(node, Market):
+        flattened = _flattened_from_context(context)
+        yield flattened
+    else:
+        for child in node.children:
+            for flattened in flattened_nav_iter(child, **context):
+                yield flattened
+
+
+def _flattened_from_context(ctx):
+    ctx.pop("navigation")
+    return FlattenedMarket(
+        **{
+            f"{node_type}_{k}": v
+            for node_type, nav_item in ctx.items()
+            for k, v in nav_item.to_dict().items()
+            if k not in ("type", "children")
+        }
+    )
```

### Comparing `betfair_parser-0.2.6/betfair_parser/spec/race_status.py` & `betfair_parser-0.3.0/betfair_parser/spec/race_status.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from betfair_parser.spec.common import BaseMessage, Date, Request, Response
+from betfair_parser.spec.common import BaseMessage, Date, EndpointType, Params, Request, Response
 from betfair_parser.strenums import DocumentedEnum, doc
 
 
 class RaceStatus(DocumentedEnum):
     DORMANT = doc("There is no data available for this race.")
     DELAYED = doc("The start of the race has been delayed")
     PARADING = doc("The horses/greyhounds are in the parade ring")
@@ -36,24 +36,26 @@
     UNEXPECTED_ERROR = doc("An unexpected error occurred retrieving score data")
     LIVE_DATA_TEMPORARILY_UNAVAILABLE = doc(
         "Live Data feed for this event/match is temporarily unavailable, data could potentially be stale"
     )
 
 
 class RaceDetails(BaseMessage, kw_only=True, frozen=True):
-    meeting_Id: str  # The unique Id for the meeting equivalent to the eventId as returned by listEvents
-    race_id: str  # The unique Id for the race in the format meetingId.raceTime (hhmm)
-    race_status: RaceStatus  # The current status of the race.
-    last_updated: Date  # This is the time the data was last updated
-    sequence: int  # This is the unique identifier associated to each update of the data
+    # Even as these items are marked as mandatory, they seem to be missing a lot
+    meeting_id: Optional[str] = None  # The unique Id for the meeting as returned by listEvents
+    race_id: Optional[str] = None  # The unique Id for the race in the format meetingId.raceTime (hhmm)
+    race_status: Optional[RaceStatus] = None  # The current status of the race.
+    last_updated: Optional[Date] = None  # This is the time the data was last updated
+    sequence: Optional[int] = None  # This is the unique identifier associated to each update of the data
     response_code: ResponseCode
 
 
-class _ListRaceDetailsParams(BaseMessage, frozen=True):
+class _ListRaceDetailsParams(Params, frozen=True):
     meeting_ids: Optional[set[str]] = None  # Restricts the results to the specified meeting IDs.
     race_ids: Optional[set[str]] = None  # Restricts the results to the specified race IDs.
 
 
 class ListRaceDetail(Request, kw_only=True, frozen=True):
+    endpoint_type = EndpointType.SCORES
     method = "ScoresAPING/v1.0/listRaceDetails"
     params: _ListRaceDetailsParams
     return_type = Response[list[RaceDetails]]
```

### Comparing `betfair_parser-0.2.6/betfair_parser/spec/streaming/mcm.py` & `betfair_parser-0.3.0/betfair_parser/spec/streaming/mcm.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from typing import List, Literal, Optional, Union
+from typing import Annotated, List, Literal, Optional, Union
+
+import msgspec
 
 from betfair_parser.spec.betting.enums import MarketStatus, RunnerStatus
 from betfair_parser.spec.betting.type_definitions import PriceLadderDescription
-from betfair_parser.spec.common import BaseMessage, Date
-from betfair_parser.spec.constants import EVENT_TYPE_TO_NAME
+from betfair_parser.spec.common import BaseMessage, Date, EventTypeIdCode, RegulatorCode
 
 
 class RunnerValues(BaseMessage, frozen=True):
     """
     https://docs.developer.betfair.com/display/1smk3cen4v3lu3yomq5qye0ni/Exchange+Stream+API
     """
 
@@ -76,15 +77,15 @@
     in_play: bool
     cross_matching: bool
     runners_voidable: bool
     number_of_active_runners: int
     bet_delay: int
     status: MarketStatus
     runners: List[Runner]
-    regulators: List[str]
+    regulators: List[RegulatorCode]
     name: Optional[str] = None
     open_date: Optional[str] = None
     timezone: Optional[str] = None
     venue: Optional[str] = None
     version: Optional[int] = None
     country_code: Optional[str] = None
     discount_allowed: Optional[bool] = None
@@ -92,82 +93,37 @@
     price_ladder_definition: Optional[Union[str, PriceLadderDescription]] = None
     settled_time: Optional[Date] = None
     key_line_definition: Optional[KeyLineDefinition] = None
     each_way_divisor: Optional[float] = None
 
     @property
     def event_type_name(self) -> str:
-        return EVENT_TYPE_TO_NAME[self.event_type_id]
-
-
-class AvailableToBack(BaseMessage, array_like=True, frozen=True):
-    """AvailableToBack"""
-
-    price: float
-    volume: float
-
-
-class AvailableToLay(BaseMessage, array_like=True, frozen=True):
-    """AvailableToLay"""
-
-    price: float
-    volume: float
-
-
-class BestAvailableToBack(BaseMessage, array_like=True, frozen=True):
-    """BestAvailableToBack"""
-
-    level: int
-    price: float
-    volume: float
-
+        return EventTypeIdCode(int(self.event_type_id)).name
 
-class BestAvailableToLay(BaseMessage, array_like=True, frozen=True):
-    """BestAvailableToLay"""
 
-    level: int
+class _PriceVolume(BaseMessage, array_like=True, frozen=True):
     price: float
     volume: float
 
 
-class BestDisplayAvailableToBack(BaseMessage, array_like=True, frozen=True):
-    """BestDisplayAvailableToBack"""
-
+class _LevelPriceVolume(BaseMessage, array_like=True, frozen=True):
     level: int
     price: float
     volume: float
 
 
-class BestDisplayAvailableToLay(BaseMessage, array_like=True, frozen=True):
-    """BestDisplayAvailableToLay"""
-
-    level: int
-    price: float
-    volume: float
-
-
-class Trade(BaseMessage, array_like=True, frozen=True):
-    """Trade"""
-
-    price: float
-    volume: float
-
-
-class StartingPriceBack(BaseMessage, array_like=True, frozen=True):
-    """StartingPriceBack"""
-
-    price: float
-    volume: float
-
-
-class StartingPriceLay(BaseMessage, array_like=True, frozen=True):
-    """StartingPriceLay"""
-
-    price: float
-    volume: float
+AvailableToBack = Annotated[_PriceVolume, msgspec.Meta(title="AvailableToBack")]
+AvailableToLay = Annotated[_PriceVolume, msgspec.Meta(title="AvailableToLay")]
+BestAvailableToBack = Annotated[_LevelPriceVolume, msgspec.Meta(title="BestAvailableToBack")]
+BestAvailableToLay = Annotated[_LevelPriceVolume, msgspec.Meta(title="BestAvailableToLay")]
+BestDisplayAvailableToBack = Annotated[_LevelPriceVolume, msgspec.Meta(title="BestDisplayAvailableToBack")]
+BestDisplayAvailableToLay = Annotated[_LevelPriceVolume, msgspec.Meta(title="BestDisplayAvailableToLay")]
+Trade = Annotated[_PriceVolume, msgspec.Meta(title="Trade")]
+StartingPriceBack = Annotated[_PriceVolume, msgspec.Meta(title="StartingPriceBack")]
+StartingPriceLay = Annotated[_PriceVolume, msgspec.Meta(title="StartingPriceLay")]
 
 
 class RunnerChange(BaseMessage, frozen=True):
     """
     https://docs.developer.betfair.com/display/1smk3cen4v3lu3yomq5qye0ni/Exchange+Stream+API
     """
```

### Comparing `betfair_parser-0.2.6/betfair_parser/spec/streaming/ocm.py` & `betfair_parser-0.3.0/betfair_parser/spec/streaming/ocm.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.6/betfair_parser/spec/streaming/status.py` & `betfair_parser-0.3.0/betfair_parser/spec/streaming/status.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,20 +35,24 @@
     UNEXPECTED_ERROR = doc("Failure code returned when an internal error occurred on the server")
     CONNECTION_FAILED = doc("Failure code used when the client / server connection is terminated")
 
 
 class Connection(BaseMessage, tag_field="op", tag=str.lower, frozen=True):
     """Connection Message"""
 
-    connectionId: str
+    connection_id: str
 
 
 class Status(BaseMessage, tag_field="op", tag=str.lower, frozen=True):
     """Status Message"""
 
     status_code: Literal["SUCCESS", "FAILURE"]
     connection_closed: bool
     id: Optional[int] = None
     connections_available: Optional[int] = None
     connection_id: Optional[str] = None
     error_code: Optional[StatusErrorCode] = None
     error_message: Optional[str] = None
+
+    @property
+    def is_error(self):
+        return self.status_code != "SUCCESS"
```

### Comparing `betfair_parser-0.2.6/betfair_parser/strenums.py` & `betfair_parser-0.3.0/betfair_parser/strenums.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,21 @@
     True
     """
 
     def _generate_next_value_(key, start, count, last_values):
         return key
 
 
+class LowerStrEnum(StrEnum):
+    """Like StrEnum, but have lowered values."""
+
+    def _generate_next_value_(key, start, count, last_values):
+        return key.lower()
+
+
 class doc(auto):
     """Auto-generated enum field with docstring
 
     doc("docstring") replaces auto() for DocumentedEnums. A value
     can be set using doc(value=..., docstring=...), otherwise the
     same value as for auto() is calculated.
 
@@ -63,18 +70,18 @@
     def __new__(cls, val):
         member = object.__new__(cls)
         if isinstance(val, doc):
             member._value_ = val._value
             member.__doc__ = val.__doc__
         else:
             # also handle ordinary or auto() values
-            member._value = val
+            member._value = val  # type: ignore
             member.__doc__ = None
         return member
 
     def _generate_next_value_(key, start, count, last_values):
         return key
 
     def __str__(self):
         if self.__doc__:
-            return f"{super().__str__()}: {self.__doc__}"
-        return super().__str__()
+            return f"{self.name}: {self.__doc__}"
+        return self.name
```

