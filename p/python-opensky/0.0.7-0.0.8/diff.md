# Comparing `tmp/python_opensky-0.0.7.tar.gz` & `tmp/python_opensky-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_opensky-0.0.7.tar", max compression
+gzip compressed data, was "python_opensky-0.0.8.tar", max compression
```

## Comparing `python_opensky-0.0.7.tar` & `python_opensky-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1077 2023-05-23 20:15:17.557045 python_opensky-0.0.7/LICENSE.md
--rw-r--r--   0        0        0     5328 2023-05-23 20:15:17.557045 python_opensky-0.0.7/README.md
--rw-r--r--   0        0        0     3659 2023-05-23 20:15:43.549260 python_opensky-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      444 2023-05-23 20:15:17.557045 python_opensky-0.0.7/src/python_opensky/__init__.py
--rw-r--r--   0        0        0      849 2023-05-23 20:15:17.557045 python_opensky-0.0.7/src/python_opensky/const.py
--rw-r--r--   0        0        0      384 2023-05-23 20:15:17.561045 python_opensky-0.0.7/src/python_opensky/exceptions.py
--rw-r--r--   0        0        0     3573 2023-05-23 20:15:17.561045 python_opensky-0.0.7/src/python_opensky/models.py
--rw-r--r--   0        0        0    12059 2023-05-23 20:15:17.561045 python_opensky-0.0.7/src/python_opensky/opensky.py
--rw-r--r--   0        0        0        0 2023-05-23 20:15:17.561045 python_opensky-0.0.7/src/python_opensky/py.typed
--rw-r--r--   0        0        0     6580 1970-01-01 00:00:00.000000 python_opensky-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-01 11:43:00.841027 python_opensky-0.0.8/LICENSE.md
+-rw-r--r--   0        0        0     5328 2023-06-01 11:43:00.841027 python_opensky-0.0.8/README.md
+-rw-r--r--   0        0        0     3659 2023-06-01 11:43:15.744941 python_opensky-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      444 2023-06-01 11:43:00.845028 python_opensky-0.0.8/src/python_opensky/__init__.py
+-rw-r--r--   0        0        0      849 2023-06-01 11:43:00.845028 python_opensky-0.0.8/src/python_opensky/const.py
+-rw-r--r--   0        0        0      384 2023-06-01 11:43:00.845028 python_opensky-0.0.8/src/python_opensky/exceptions.py
+-rw-r--r--   0        0        0     3573 2023-06-01 11:43:00.845028 python_opensky-0.0.8/src/python_opensky/models.py
+-rw-r--r--   0        0        0     9203 2023-06-01 11:43:00.845028 python_opensky-0.0.8/src/python_opensky/opensky.py
+-rw-r--r--   0        0        0        0 2023-06-01 11:43:00.845028 python_opensky-0.0.8/src/python_opensky/py.typed
+-rw-r--r--   0        0        0     6580 1970-01-01 00:00:00.000000 python_opensky-0.0.8/PKG-INFO
```

### Comparing `python_opensky-0.0.7/LICENSE.md` & `python_opensky-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python_opensky-0.0.7/README.md` & `python_opensky-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `python_opensky-0.0.7/pyproject.toml` & `python_opensky-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python_opensky"
-version = "0.0.7"
+version = "0.0.8"
 description = "Asynchronous Python client for Opensky API."
 authors = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 maintainers = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/joostlek/python-opensky"
 repository = "https://github.com/joostlek/python-opensky"
@@ -24,31 +24,31 @@
     { include = "python_opensky", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = ">=3.0.0"
 yarl = ">=1.6.0"
-pydantic = "1.10.7"
+pydantic = "1.10.8"
 
 [tool.poetry.group.dev.dependencies]
 aresponses = "2.1.6"
 black = "23.3.0"
 blacken-docs = "1.13.0"
 codespell = "2.2.4"
 covdefaults = "2.3.0"
-coverage = {version = "7.2.5", extras = ["toml"]}
+coverage = {version = "7.2.7", extras = ["toml"]}
 mypy = "1.3.0"
 pre-commit = "3.3.2"
 pre-commit-hooks = "4.4.0"
 pylint = "2.17.4"
 pytest = "7.3.1"
 pytest-asyncio = "0.21.0"
-pytest-cov = "4.0.0"
-ruff = "0.0.269"
+pytest-cov = "4.1.0"
+ruff = "0.0.270"
 safety = "2.4.0b1"
 yamllint = "1.32.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/joostlek/python-opensky/issues"
 Changelog = "https://github.com/joostlek/python-opensky/releases"
```

### Comparing `python_opensky-0.0.7/src/python_opensky/const.py` & `python_opensky-0.0.8/src/python_opensky/const.py`

 * *Files identical despite different names*

### Comparing `python_opensky-0.0.7/src/python_opensky/models.py` & `python_opensky-0.0.8/src/python_opensky/models.py`

 * *Files identical despite different names*

### Comparing `python_opensky-0.0.7/src/python_opensky/opensky.py` & `python_opensky-0.0.8/src/python_opensky/opensky.py`

 * *Files 25% similar despite different names*

```diff
@@ -218,135 +218,63 @@
             "position_source",
             "category",
         ]
 
         return dict(zip(keys, state, strict=True))
 
     @staticmethod
-    # pylint: disable=too-many-locals
-    def calculate_point(
+    def get_bounding_box(
         latitude: float,
         longitude: float,
-        distance: float,
-        degrees: float,
-    ) -> tuple[float, float]:
-        """Calculate a point from an origin point, direction in degrees and distance."""
-        # ruff: noqa: N806
-        # pylint: disable=invalid-name
-        pi_d4 = math.atan(1.0)
-        two_pi = pi_d4 * 8.0
-        latitude = latitude * pi_d4 / 45.0
-        longitude = longitude * pi_d4 / 45.0
-        degrees = degrees * pi_d4 / 45.0
-        if degrees < 0.0:
-            degrees = degrees + two_pi
-        if degrees > two_pi:
-            degrees = degrees - two_pi
-        axis_a = 6378137
-        flattening = 1 / 298.257223563
-        axis_b = axis_a * (1.0 - flattening)
-        tan_u1 = (1 - flattening) * math.tan(latitude)
-        u1 = math.atan(tan_u1)
-        sigma1 = math.atan2(tan_u1, math.cos(degrees))
-        sinalpha = math.cos(u1) * math.sin(degrees)
-        cosalpha_sq = 1.0 - sinalpha * sinalpha
-        u2 = cosalpha_sq * (axis_a * axis_a - axis_b * axis_b) / (axis_b * axis_b)
-        A = 1.0 + (u2 / 16384) * (4096 + u2 * (-768 + u2 * (320 - 175 * u2)))
-        B = (u2 / 1024) * (256 + u2 * (-128 + u2 * (74 - 47 * u2)))
-        # Starting with the approx
-        sigma = distance / (axis_b * A)
-        last_sigma = 2.0 * sigma + 2.0  # something impossible
-
-        # Iterate the following 3 eqs until no sig change in sigma
-        # two_sigma_m , delta_sigma
-        while abs((last_sigma - sigma) / sigma) > 1.0e-9:
-            two_sigma_m = 2 * sigma1 + sigma
-            delta_sigma = (
-                B
-                * math.sin(sigma)
-                * (
-                    math.cos(two_sigma_m)
-                    + (B / 4)
-                    * (
-                        math.cos(sigma)
-                        * (
-                            -1
-                            + 2 * math.pow(math.cos(two_sigma_m), 2)
-                            - (B / 6)
-                            * math.cos(two_sigma_m)
-                            * (-3 + 4 * math.pow(math.sin(sigma), 2))
-                            * (-3 + 4 * math.pow(math.cos(two_sigma_m), 2))
-                        )
-                    )
-                )
-            )
-            last_sigma = sigma
-            sigma = (distance / (axis_b * A)) + delta_sigma
-        phi2 = math.atan2(
-            (
-                math.sin(u1) * math.cos(sigma)
-                + math.cos(u1) * math.sin(sigma) * math.cos(degrees)
-            ),
-            (
-                (1 - flattening)
-                * math.sqrt(
-                    math.pow(sinalpha, 2)
-                    + pow(
-                        math.sin(u1) * math.sin(sigma)
-                        - math.cos(u1) * math.cos(sigma) * math.cos(degrees),
-                        2,
-                    ),
-                )
-            ),
+        radius: float,
+    ) -> BoundingBox:
+        """Get bounding box from radius and a point."""
+        half_side_in_km = abs(radius) / 1000
+
+        lat = math.radians(latitude)
+        lon = math.radians(longitude)
+
+        approx_earth_radius = 6371
+        hypotenuse_distance = math.sqrt(2 * (math.pow(half_side_in_km, 2)))
+
+        lat_min = math.asin(
+            math.sin(lat) * math.cos(hypotenuse_distance / approx_earth_radius)
+            + math.cos(lat)
+            * math.sin(hypotenuse_distance / approx_earth_radius)
+            * math.cos(225 * (math.pi / 180)),
         )
-        lembda = math.atan2(
-            (math.sin(sigma) * math.sin(degrees)),
-            (
-                math.cos(u1) * math.cos(sigma)
-                - math.sin(u1) * math.sin(sigma) * math.cos(degrees)
-            ),
+        lon_min = lon + math.atan2(
+            math.sin(225 * (math.pi / 180))
+            * math.sin(hypotenuse_distance / approx_earth_radius)
+            * math.cos(lat),
+            math.cos(hypotenuse_distance / approx_earth_radius)
+            - math.sin(lat) * math.sin(lat_min),
         )
-        C = (flattening / 16) * cosalpha_sq * (4 + flattening * (4 - 3 * cosalpha_sq))
-        omega = lembda - (1 - C) * flattening * sinalpha * (
-            sigma
-            + C
-            * math.sin(sigma)
-            * (
-                math.cos(two_sigma_m)
-                + C * math.cos(sigma) * (-1 + 2 * math.pow(math.cos(two_sigma_m), 2))
-            )
+
+        lat_max = math.asin(
+            math.sin(lat) * math.cos(hypotenuse_distance / approx_earth_radius)
+            + math.cos(lat)
+            * math.sin(hypotenuse_distance / approx_earth_radius)
+            * math.cos(45 * (math.pi / 180)),
         )
-        lembda2 = longitude + omega
-        math.atan2(
-            sinalpha,
-            (
-                -math.sin(u1) * math.sin(sigma)
-                + math.cos(u1) * math.cos(sigma) * math.cos(degrees)
-            ),
+        lon_max = lon + math.atan2(
+            math.sin(45 * (math.pi / 180))
+            * math.sin(hypotenuse_distance / approx_earth_radius)
+            * math.cos(lat),
+            math.cos(hypotenuse_distance / approx_earth_radius)
+            - math.sin(lat) * math.sin(lat_max),
         )
-        phi2 = phi2 * 45.0 / pi_d4
-        lembda2 = lembda2 * 45.0 / pi_d4
-        return phi2, lembda2
 
-    @staticmethod
-    def get_bounding_box(
-        latitude: float,
-        longitude: float,
-        radius: float,
-    ) -> BoundingBox:
-        """Get bounding box from radius and a point."""
-        north = OpenSky.calculate_point(latitude, longitude, radius, 0)
-        east = OpenSky.calculate_point(latitude, longitude, radius, 90)
-        south = OpenSky.calculate_point(latitude, longitude, radius, 180)
-        west = OpenSky.calculate_point(latitude, longitude, radius, 270)
+        rad2deg = math.degrees
+
         return BoundingBox(
-            min_latitude=min(north[0], south[0]) + latitude,
-            max_latitude=max(north[0], south[0]) + latitude,
-            min_longitude=min(east[1], west[1]) + longitude,
-            max_longitude=max(east[1], west[1]) + longitude,
+            min_latitude=rad2deg(lat_min),
+            max_latitude=rad2deg(lat_max),
+            min_longitude=rad2deg(lon_min),
+            max_longitude=rad2deg(lon_max),
         )
 
     async def close(self) -> None:
         """Close open client session."""
         if self.session and self._close_session:
             await self.session.close()
```

### Comparing `python_opensky-0.0.7/PKG-INFO` & `python_opensky-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-opensky
-Version: 0.0.7
+Version: 0.0.8
 Summary: Asynchronous Python client for Opensky API.
 Home-page: https://github.com/joostlek/python-opensky
 License: MIT
 Keywords: opensky,api,async,client
 Author: Joost Lekkerkerker
 Author-email: joostlek@outlook.com
 Maintainer: Joost Lekkerkerker
@@ -16,15 +16,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp (>=3.0.0)
-Requires-Dist: pydantic (==1.10.7)
+Requires-Dist: pydantic (==1.10.8)
 Requires-Dist: yarl (>=1.6.0)
 Project-URL: Bug Tracker, https://github.com/joostlek/python-opensky/issues
 Project-URL: Changelog, https://github.com/joostlek/python-opensky/releases
 Project-URL: Documentation, https://github.com/joostlek/python-opensky
 Project-URL: Repository, https://github.com/joostlek/python-opensky
 Description-Content-Type: text/markdown
```

