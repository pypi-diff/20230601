# Comparing `tmp/betwatch-1.0.5.tar.gz` & `tmp/betwatch-1.0.6.tar.gz`

## Comparing `betwatch-1.0.5.tar` & `betwatch-1.0.6.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-1.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 betwatch-1.0.5/Makefile
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.0.5/.github/dependabot.yml
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 betwatch-1.0.5/.github/workflows/test.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-1.0.5/betwatch/__about__.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 betwatch-1.0.5/betwatch/__init__.py
--rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 betwatch-1.0.5/betwatch/client.py
--rw-r--r--   0        0        0    26499 2020-02-02 00:00:00.000000 betwatch-1.0.5/betwatch/client_async.py
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 betwatch-1.0.5/betwatch/queries.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.0.5/betwatch/types/__init__.py
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 betwatch-1.0.5/betwatch/types/bookmakers.py
--rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 betwatch-1.0.5/betwatch/types/filters.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 betwatch-1.0.5/betwatch/types/markets.py
--rw-r--r--   0        0        0    12489 2020-02-02 00:00:00.000000 betwatch-1.0.5/betwatch/types/race.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.0.5/betwatch/types/updates.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 betwatch-1.0.5/examples/get_race_prices.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 betwatch-1.0.5/examples/get_race_prices_async.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 betwatch-1.0.5/examples/get_races.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 betwatch-1.0.5/examples/get_races_async.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 betwatch-1.0.5/examples/subscriptions.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 betwatch-1.0.5/examples/update_rated_prices.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.0.5/tests/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 betwatch-1.0.5/tests/test_check_last_updated.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 betwatch-1.0.5/tests/test_get_race.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 betwatch-1.0.5/tests/test_get_race_async.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 betwatch-1.0.5/tests/test_get_races.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 betwatch-1.0.5/tests/test_get_races_async.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 betwatch-1.0.5/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.0.5/LICENSE.txt
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.0.5/README.md
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 betwatch-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 betwatch-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-1.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 betwatch-1.0.6/Makefile
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.0.6/.github/dependabot.yml
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 betwatch-1.0.6/.github/workflows/test.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-1.0.6/betwatch/__about__.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 betwatch-1.0.6/betwatch/__init__.py
+-rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 betwatch-1.0.6/betwatch/client.py
+-rw-r--r--   0        0        0    27637 2020-02-02 00:00:00.000000 betwatch-1.0.6/betwatch/client_async.py
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 betwatch-1.0.6/betwatch/queries.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.0.6/betwatch/types/__init__.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 betwatch-1.0.6/betwatch/types/bookmakers.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 betwatch-1.0.6/betwatch/types/exceptions.py
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 betwatch-1.0.6/betwatch/types/filters.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 betwatch-1.0.6/betwatch/types/markets.py
+-rw-r--r--   0        0        0    12482 2020-02-02 00:00:00.000000 betwatch-1.0.6/betwatch/types/race.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.0.6/betwatch/types/updates.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 betwatch-1.0.6/examples/get_race_prices.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 betwatch-1.0.6/examples/get_race_prices_async.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 betwatch-1.0.6/examples/get_races.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 betwatch-1.0.6/examples/get_races_async.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 betwatch-1.0.6/examples/subscriptions.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 betwatch-1.0.6/examples/update_rated_prices.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.0.6/tests/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 betwatch-1.0.6/tests/test_check_last_updated.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 betwatch-1.0.6/tests/test_get_race.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 betwatch-1.0.6/tests/test_get_race_async.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 betwatch-1.0.6/tests/test_get_races.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 betwatch-1.0.6/tests/test_get_races_async.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 betwatch-1.0.6/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.0.6/LICENSE.txt
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.0.6/README.md
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 betwatch-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 betwatch-1.0.6/PKG-INFO
```

### Comparing `betwatch-1.0.5/.github/workflows/test.yml` & `betwatch-1.0.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.5/betwatch/__init__.py` & `betwatch-1.0.6/betwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.5/betwatch/client.py` & `betwatch-1.0.6/betwatch/client.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.5/betwatch/client_async.py` & `betwatch-1.0.6/betwatch/client_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     Bookmaker,
     BookmakerMarket,
     Race,
     RaceProjection,
     RaceUpdate,
     SubscriptionUpdate,
 )
+from betwatch.types.exceptions import NotEntitledError
 from betwatch.types.filters import RacesFilter
 from betwatch.types.updates import SelectionData
 
 
 class BetwatchAsyncClient:
     def __init__(
         self,
@@ -348,14 +349,24 @@
                             try:
                                 err = task.exception()
                                 if err:
                                     logging.warning(f"Subscription task closed: {err}")
                                     # reset the connection
                                     if self._websocket_session:
                                         await self.disconnect()
+
+                                    # if the user is not entitled to the data, don't retry
+                                    # check if err is of type NotEntitledError
+                                    if isinstance(err, NotEntitledError):
+                                        logging.warning(
+                                            "You are not entitled to subscriptions. Please contact api@betwatch.com to upgrade your API key."
+                                        )
+                                        del d[key]
+                                        continue
+
                             except asyncio.InvalidStateError:
                                 pass
 
                             logging.warning(
                                 f"Retrying subscription task for {key if key else 'all races'}"
                             )
 
@@ -502,14 +513,20 @@
                             result["priceUpdates"], List[BookmakerMarket]
                         ),
                     )
 
                     self._subscription_queue.put_nowait(update)
         except TransportError as e:
             logging.debug(f"Error subscribing to bookmaker updates: {e}")
+
+            # check if the user is entitled to this data
+            if "does not have access" in e.args[0]:
+                raise NotEntitledError(
+                    "API key is not entitled to websocket subscriptions"
+                ) from e
         except asyncio.CancelledError:
             await self.unsubscribe_bookmaker_updates(race_id)
             return
         except Exception as e:
             logging.debug(f"Error subscribing to bookmaker updates: {e}")
 
     async def unsubscribe_betfair_updates(self, race_id: str):
@@ -572,14 +589,20 @@
                             result["betfairUpdates"], List[BetfairMarket]
                         ),
                     )
                     self._subscription_queue.put_nowait(update)
 
         except TransportError as e:
             logging.debug(f"Error subscribing to betfair updates: {e}")
+
+            # check if the user is entitled to this data
+            if "does not have access" in e.args[0]:
+                raise NotEntitledError(
+                    "API key is not entitled to websocket subscriptions"
+                ) from e
         except asyncio.CancelledError:
             await self.unsubscribe_betfair_updates(race_id)
             return
 
     async def unsubscribe_race_updates(self, date_from: str, date_to: str):
         if (date_from, date_to) not in self._subscriptions_updates:
             logging.info(f"Not subscribed to races updates for {date_from} - {date_to}")
```

### Comparing `betwatch-1.0.5/betwatch/queries.py` & `betwatch-1.0.6/betwatch/queries.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.5/betwatch/types/bookmakers.py` & `betwatch-1.0.6/betwatch/types/bookmakers.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,21 +84,21 @@
     THUNDERBET = "Thunderbet"
     ESKANDERBET = "EskanderBet"
     SPORTCHAMPS = "SportChamps"
     SURGE = "Surge"
 
     def __str__(self):
         return self.value
-    
+
     def __repr__(self):
         return self.value
-    
+
     def __eq__(self, other):
         if isinstance(other, Bookmaker):
             return self.value == other.value
         elif isinstance(other, str):
             return self.value == other
         else:
             return False
-        
+
     def __hash__(self):
         return hash(self.value)
```

### Comparing `betwatch-1.0.5/betwatch/types/filters.py` & `betwatch-1.0.6/betwatch/types/filters.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.5/betwatch/types/markets.py` & `betwatch-1.0.6/betwatch/types/markets.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.5/betwatch/types/race.py` & `betwatch-1.0.6/betwatch/types/race.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,14 +267,15 @@
             return o.isoformat()
         elif isinstance(o, timedelta):
             return (datetime.min + o).time().isoformat()
         elif isinstance(o, Enum):
             return o.value
         return super().default(o)
 
+
 @dataclass
 class Race:
     id: str
 
     status: Optional[RaceStatus] = None
 
     runners: Optional[List[Runner]] = None
@@ -318,15 +319,15 @@
             if self.start_time
             else ""
         )
 
         if self.meeting is None:
             return f"R{self.number} [{st}]"
         return f"({self.meeting.type}) {self.meeting.track} R{self.number}{st}"
-    
+
     def __repr__(self) -> str:
         return str(self)
 
     def get_bookmaker_link(
         self, bookmaker: Union[Bookmaker, str]
     ) -> Optional[RaceLink]:
         """Returns the link for the given bookmaker"""
@@ -336,15 +337,15 @@
 
         if not self.links:
             return None
         for link in self.links:
             if link.bookmaker == bookmaker:
                 return link
         return None
-    
+
     def to_dict(self) -> dict:
         return json.loads(json.dumps(self, cls=EnhancedJSONEncoder))
 
     def get_runners_by_price(
         self,
         market_type: MarketPriceType,
         bookmakers: Optional[List[Bookmaker]] = None,
```

### Comparing `betwatch-1.0.5/examples/get_race_prices.py` & `betwatch-1.0.6/examples/get_race_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.5/examples/get_race_prices_async.py` & `betwatch-1.0.6/examples/get_race_prices_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.5/examples/get_races.py` & `betwatch-1.0.6/examples/get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.5/examples/get_races_async.py` & `betwatch-1.0.6/examples/get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.5/examples/subscriptions.py` & `betwatch-1.0.6/examples/subscriptions.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.5/examples/update_rated_prices.py` & `betwatch-1.0.6/examples/update_rated_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.5/tests/test_get_race.py` & `betwatch-1.0.6/tests/test_get_race.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.5/tests/test_get_race_async.py` & `betwatch-1.0.6/tests/test_get_race_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.5/tests/test_get_races.py` & `betwatch-1.0.6/tests/test_get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.5/tests/test_get_races_async.py` & `betwatch-1.0.6/tests/test_get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.5/.gitignore` & `betwatch-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.5/LICENSE.txt` & `betwatch-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.5/README.md` & `betwatch-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.5/pyproject.toml` & `betwatch-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.5/PKG-INFO` & `betwatch-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betwatch
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python package for interacting with the Betwatch.com API
 Project-URL: Documentation, https://github.com/betwatch/betwatch-sdk-python#readme
 Project-URL: Issues, https://github.com/betwatch/betwatch-sdk-python/issues
 Project-URL: Source, https://github.com/betwatch/betwatch-sdk-python
 Project-URL: Betwatch.com, https://betwatch.com
 Author-email: Jamie Watts <jamie@betwatch.com>
 License-File: LICENSE.txt
```

