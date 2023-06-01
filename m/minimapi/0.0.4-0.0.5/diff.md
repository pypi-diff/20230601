# Comparing `tmp/minimapi-0.0.4.tar.gz` & `tmp/minimapi-0.0.5.tar.gz`

## Comparing `minimapi-0.0.4.tar` & `minimapi-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 minimapi-0.0.4/build.sh
--rw-r--r--   0        0        0    19873 2020-02-02 00:00:00.000000 minimapi-0.0.4/minimapi.png
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 minimapi-0.0.4/src/minimapi/__init__.py
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 minimapi-0.0.4/src/minimapi/minimapi.py
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 minimapi-0.0.4/src/minimapi/sanitizer.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 minimapi-0.0.4/src/minimapi/auth_modules/bearer.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 minimapi-0.0.4/src/minimapi/auth_modules/ecdsa.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 minimapi-0.0.4/src/minimapi/auth_modules/jwt.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 minimapi-0.0.4/src/minimapi/auth_modules/none.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 minimapi-0.0.4/src/minimapi/data_types/date.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 minimapi-0.0.4/src/minimapi/data_types/email.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 minimapi-0.0.4/src/minimapi/data_types/number.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 minimapi-0.0.4/src/minimapi/data_types/password.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 minimapi-0.0.4/src/minimapi/data_types/pbkdf2.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 minimapi-0.0.4/src/minimapi/data_types/sha256.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 minimapi-0.0.4/src/minimapi/data_types/text.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 minimapi-0.0.4/src/minimapi/data_types/totp.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 minimapi-0.0.4/src/minimapi/data_types/url.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 minimapi-0.0.4/src/minimapi/database_connectors/pysondb.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 minimapi-0.0.4/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 minimapi-0.0.4/LICENSE
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 minimapi-0.0.4/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 minimapi-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 minimapi-0.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 minimapi-0.0.5/build.sh
+-rw-r--r--   0        0        0    19873 2020-02-02 00:00:00.000000 minimapi-0.0.5/minimapi.png
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/__init__.py
+-rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/minimapi.py
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/sanitizer.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/auth_modules/bearer.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/auth_modules/ecdsa.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/auth_modules/jwt.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/auth_modules/none.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/data_types/date.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/data_types/email.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/data_types/number.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/data_types/password.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/data_types/pbkdf2.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/data_types/sha256.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/data_types/text.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/data_types/totp.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/data_types/url.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/database_connectors/pysondb.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 minimapi-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 minimapi-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 minimapi-0.0.5/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 minimapi-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 minimapi-0.0.5/PKG-INFO
```

### Comparing `minimapi-0.0.4/minimapi.png` & `minimapi-0.0.5/minimapi.png`

 * *Files identical despite different names*

### Comparing `minimapi-0.0.4/src/minimapi/minimapi.py` & `minimapi-0.0.5/src/minimapi/minimapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 			return send_from_directory(self.path+'/'+static_path, path)
 
 
 	def add_routes(self):
 
 		@self.app.route('/api/auth', methods=['POST'])
 		def login():
-			request_data = self.sanitizer.sanitize_request('auth', request.json)
+			request_data = self.sanitizer.sanitize_request('credential', request.json)
 			if request_data:
 				return self.auth.login(request_data)
 			return 'Bad request', 400
 
 		@self.app.route('/api/auth', methods=['DELETE'])
 		@self.auth.check
 		def logout():
```

### Comparing `minimapi-0.0.4/src/minimapi/sanitizer.py` & `minimapi-0.0.5/src/minimapi/sanitizer.py`

 * *Files identical despite different names*

### Comparing `minimapi-0.0.4/src/minimapi/auth_modules/ecdsa.py` & `minimapi-0.0.5/src/minimapi/auth_modules/ecdsa.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,32 +15,32 @@
 		self.database = database
 
 	def check(self, function):
 		@wraps(function)
 		def wrapper(*args,**kargs):
 			try:
 				auth_data = request.headers.get('Authorization').split('.')
-				if self.database.read('auth',id=auth_data[0]):
-					public_key = self.database.read('auth',id=auth_data[0])[0]['public_key']
+				if self.database.read('credential',id=auth_data[0]):
+					public_key = self.database.read('credential',id=auth_data[0])[0]['public_key']
 					signature_checker = ecdsa.VerifyingKey.from_string(bytes.fromhex(public_key), curve=CURVE, hashfunc=HASH_FUNCTION)
 					timestamp = str(int(datetime.utcnow().timestamp()))
 					payload = ((auth_data[2]+request.method+request.full_path.strip('?')).encode('utf-8')+request.data)
 					if signature_checker.verify(bytes.fromhex(auth_data[1]), payload) and (abs(int(timestamp) - int(auth_data[2])) <= MAX_TIMESTAMP_GAP):
 						return function(*args,**kargs)
 			except:
 				pass
 			return '', 401
 		return wrapper
 
 	def login(self, request_data):
 		public_key = request_data["public_key"]
 		del request_data["public_key"]
-		results = self.database.read('auth', **request_data)
+		results = self.database.read('credential', **request_data)
 		if len(results) == 1:
-			self.database.update('auth', results[0]['id'], public_key=public_key)
+			self.database.update('credential', results[0]['id'], public_key=public_key)
 			return jsonify({'id':results[0]['id']})
 		return '', 401
 
 	def logout(self, request):
 		auth_id = request.headers.get('Authorization').split('.')[0]
-		self.database.update('auth', auth_id, {'public_key': None})
+		self.database.update('credential', auth_id, {'public_key': None})
 		return '', 204
```

### Comparing `minimapi-0.0.4/src/minimapi/auth_modules/jwt.py` & `minimapi-0.0.5/src/minimapi/auth_modules/jwt.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 		self.secret = urandom(JWT_SECRET_SIZE)
 
 	def check(self, function):
 		@wraps(function)
 		def wrapper(*args,**kargs):
 			try:
 				auth_data = jwt.decode(request.headers.get('Authorization'), self.secret, algorithms=[JWT_ALGO])
-				if self.database.read('auth',id=auth_data['ID']):
+				if self.database.read('credential',id=auth_data['ID']):
 					return function(*args,**kargs)
 			except:
 				pass
 			return '', 401
 		return wrapper
 
 	def login(self, request_data):
-		results = self.database.read('auth', **request_data)
+		results = self.database.read('credential', **request_data)
 		if len(results) == 1:
 			return jsonify({'token': jwt.encode({"ID": results[0]['id'], "exp": datetime.now(tz=timezone.utc)+timedelta(minutes=JWT_EXPIRATION_IN_MIN)}, self.secret, algorithm=JWT_ALGO)})
 		return '', 401
 
 	def logout(self, request):
 		return '', 404
```

### Comparing `minimapi-0.0.4/src/minimapi/data_types/pbkdf2.py` & `minimapi-0.0.5/src/minimapi/data_types/pbkdf2.py`

 * *Files identical despite different names*

### Comparing `minimapi-0.0.4/src/minimapi/database_connectors/pysondb.py` & `minimapi-0.0.5/src/minimapi/database_connectors/pysondb.py`

 * *Files identical despite different names*

### Comparing `minimapi-0.0.4/LICENSE` & `minimapi-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `minimapi-0.0.4/README.md` & `minimapi-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `minimapi-0.0.4/pyproject.toml` & `minimapi-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "minimapi"
-version = "0.0.4"
+version = "0.0.5"
 description = "Easy and simple REST API from model"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
   'flask >= 2.2.0',
   'pysondb >= 1.6.7',
   'pyjwt >= 2.6.0',
```

### Comparing `minimapi-0.0.4/PKG-INFO` & `minimapi-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minimapi
-Version: 0.0.4
+Version: 0.0.5
 Summary: Easy and simple REST API from model
 Project-URL: Homepage, https://github.com/minimapi/minimapi
 Project-URL: Bug Tracker, https://github.com/minimapi/minimapi/issues
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
```

