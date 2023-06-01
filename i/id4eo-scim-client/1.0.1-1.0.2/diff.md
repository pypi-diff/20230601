# Comparing `tmp/id4eo-scim-client-1.0.1.tar.gz` & `tmp/id4eo-scim-client-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "id4eo-scim-client-1.0.1.tar", last modified: Thu Mar 16 16:23:06 2023, max compression
+gzip compressed data, was "dist/id4eo-scim-client-1.0.2.tar", last modified: Thu Jun  1 16:21:07 2023, max compression
```

## Comparing `id4eo-scim-client-1.0.1.tar` & `id4eo-scim-client-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 16:23:06.217395 id4eo-scim-client-1.0.1/
--rw-rw-rw-   0        0        0      506 2023-03-16 16:23:06.217395 id4eo-scim-client-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2923 2022-11-09 15:37:32.000000 id4eo-scim-client-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-16 16:23:06.211394 id4eo-scim-client-1.0.1/id4eo_scim/
--rw-rw-rw-   0        0        0      343 2022-09-22 16:06:28.000000 id4eo-scim-client-1.0.1/id4eo_scim/__init__.py
--rw-rw-rw-   0        0        0    28404 2022-10-19 15:02:10.000000 id4eo-scim-client-1.0.1/id4eo_scim/id4eo_scim.py
--rw-rw-rw-   0        0        0     3213 2022-09-22 16:06:28.000000 id4eo-scim-client-1.0.1/id4eo_scim/main.py
-drwxrwxrwx   0        0        0        0 2023-03-16 16:23:06.216395 id4eo-scim-client-1.0.1/id4eo_scim_client.egg-info/
--rw-rw-rw-   0        0        0      506 2023-03-16 16:23:06.000000 id4eo-scim-client-1.0.1/id4eo_scim_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-03-16 16:23:06.000000 id4eo-scim-client-1.0.1/id4eo_scim_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 16:23:06.000000 id4eo-scim-client-1.0.1/id4eo_scim_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-03-16 16:23:06.000000 id4eo-scim-client-1.0.1/id4eo_scim_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-03-16 16:23:06.218395 id4eo-scim-client-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      756 2023-03-16 16:09:54.000000 id4eo-scim-client-1.0.1/setup.py
+drwxr-xr-x   0 alvl       (508) gsc4eo    (1001)        0 2023-06-01 16:21:07.000000 id4eo-scim-client-1.0.2/
+drwxr-xr-x   0 alvl       (508) gsc4eo    (1001)        0 2023-06-01 16:21:07.000000 id4eo-scim-client-1.0.2/id4eo_scim/
+-rw-r--r--   0 alvl       (508) gsc4eo    (1001)      338 2023-05-24 15:13:31.000000 id4eo-scim-client-1.0.2/id4eo_scim/__init__.py
+-rw-r--r--   0 alvl       (508) gsc4eo    (1001)    28837 2023-06-01 16:18:56.000000 id4eo-scim-client-1.0.2/id4eo_scim/id4eo_scim.py
+-rw-r--r--   0 alvl       (508) gsc4eo    (1001)     3147 2023-05-24 15:13:31.000000 id4eo-scim-client-1.0.2/id4eo_scim/main.py
+drwxr-xr-x   0 alvl       (508) gsc4eo    (1001)        0 2023-06-01 16:21:07.000000 id4eo-scim-client-1.0.2/id4eo_scim_client.egg-info/
+-rw-r--r--   0 alvl       (508) gsc4eo    (1001)      532 2023-06-01 16:21:07.000000 id4eo-scim-client-1.0.2/id4eo_scim_client.egg-info/PKG-INFO
+-rw-r--r--   0 alvl       (508) gsc4eo    (1001)      259 2023-06-01 16:21:07.000000 id4eo-scim-client-1.0.2/id4eo_scim_client.egg-info/SOURCES.txt
+-rw-r--r--   0 alvl       (508) gsc4eo    (1001)        1 2023-06-01 16:21:07.000000 id4eo-scim-client-1.0.2/id4eo_scim_client.egg-info/dependency_links.txt
+-rw-r--r--   0 alvl       (508) gsc4eo    (1001)       11 2023-06-01 16:21:07.000000 id4eo-scim-client-1.0.2/id4eo_scim_client.egg-info/top_level.txt
+-rw-r--r--   0 alvl       (508) gsc4eo    (1001)     2842 2023-05-24 15:13:31.000000 id4eo-scim-client-1.0.2/README.md
+-rw-r--r--   0 alvl       (508) gsc4eo    (1001)       79 2023-06-01 16:21:07.000000 id4eo-scim-client-1.0.2/setup.cfg
+-rw-r--r--   0 alvl       (508) gsc4eo    (1001)      738 2023-06-01 16:21:06.000000 id4eo-scim-client-1.0.2/setup.py
+-rw-r--r--   0 alvl       (508) gsc4eo    (1001)      532 2023-06-01 16:21:07.000000 id4eo-scim-client-1.0.2/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `id4eo-scim-client-1.0.1/README.md` & `id4eo-scim-client-1.0.2/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-<p align="center">
-  <h3 align="center">id4eo_scim</h3>
-  <p align="center">
-    Auxiliary Python3 library that allows a client to dynamically register with Gluu and access SCIM endpoints to get/add/edit/remove user attributes
-  </p>
-</p>
-
-## Table of Contents
-
-- [Setup this template!](#setup-this-template)
-- [Table of Contents](#table-of-contents)
-- [About The Project](#about-the-project)
-  - [Built With](#built-with)
-- [Getting Started](#getting-started)
-  - [Prerequisites](#prerequisites)
-  - [Installation](#installation)
-  - [Testing](#testing)
-- [Documentation & Usage](#documentation--usage)
-- [Roadmap](#roadmap)
-- [Contributing](#contributing)
-- [License](#license)
-- [Contact](#contact)
-- [Acknowledgements](#acknowledgements)
-
-## About The Project
-
-This is an auxiliary Python3 library to allow a client to dynamically register with Gluu. At the same time, it allows to get all user attributes, and also add/edit/remove specific attributes, by using SCIM endpointsWith both OAuth and UMA tokens.
-
-### Built With
-
-- [Python](https://www.python.org//)
-- [PyTest](https://docs.pytest.org)
-- [YAML](https://yaml.org/)
-- [Travis CI](https://travis-ci.com/)
-
-### Prerequisites
-
-- [Python 3](https://www.python.org//)
-- [Pip](https://pip.pypa.io/en/stable/)
-- [Requests](https://pypi.org/project/requests/)
-- [Pyjwkest](https://pypi.org/project/pyjwkest/)
-- [Pycrypto](https://pypi.org/project/pycrypto/)
-
-### Installation
-
-Download the library using pip
-
-```sh
-pip install id4eo-scim-client
-```
-
-Enable Test Mode in Gluu by following these procedures: [Protection using Test Mode](https://gluu.org/docs/gluu-server/3.1.6/user-management/scim2/#protection-using-test-mode)
-Disable Test Mode and Enable UMA by following these procedures: [Protection using UMA](https://gluu.org/docs/gluu-server/3.1.6/user-management/scim2/#protection-using-uma)
-
-## Documentation & Usage
-
-The component documentation can be found at https://eoepca.github.io/um-common-scim-client/.
-
-For example usages, check main.py
-
-## Roadmap
-
-See the [open issues](https://github.com/EOEPCA/um-common-scim-client/issues) for a list of proposed features (and known issues).
-
-## Contributing
-
-Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.
-
-1. Fork the Project
-2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
-3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
-4. Push to the Branch (`git push origin feature/AmazingFeature`)
-5. Open a Pull Request
-
-## License
-
-Distributed under the Apache-2.0 License. See `LICENSE` for more information.
-
-## Acknowledgements
-
-- README.md is based on [this template](https://github.com/othneildrew/Best-README-Template) by [Othneil Drew](https://github.com/othneildrew).
+<p align="center">
+  <h3 align="center">id4eo_scim</h3>
+  <p align="center">
+    Auxiliary Python3 library that allows a client to dynamically register with Gluu and access SCIM endpoints to get/add/edit/remove user attributes
+  </p>
+</p>
+
+## Table of Contents
+
+- [Setup this template!](#setup-this-template)
+- [Table of Contents](#table-of-contents)
+- [About The Project](#about-the-project)
+  - [Built With](#built-with)
+- [Getting Started](#getting-started)
+  - [Prerequisites](#prerequisites)
+  - [Installation](#installation)
+  - [Testing](#testing)
+- [Documentation & Usage](#documentation--usage)
+- [Roadmap](#roadmap)
+- [Contributing](#contributing)
+- [License](#license)
+- [Contact](#contact)
+- [Acknowledgements](#acknowledgements)
+
+## About The Project
+
+This is an auxiliary Python3 library to allow a client to dynamically register with Gluu. At the same time, it allows to get all user attributes, and also add/edit/remove specific attributes, by using SCIM endpointsWith both OAuth and UMA tokens.
+
+### Built With
+
+- [Python](https://www.python.org//)
+- [PyTest](https://docs.pytest.org)
+- [YAML](https://yaml.org/)
+- [Travis CI](https://travis-ci.com/)
+
+### Prerequisites
+
+- [Python 3](https://www.python.org//)
+- [Pip](https://pip.pypa.io/en/stable/)
+- [Requests](https://pypi.org/project/requests/)
+- [Pyjwkest](https://pypi.org/project/pyjwkest/)
+- [Pycrypto](https://pypi.org/project/pycrypto/)
+
+### Installation
+
+Download the library using pip
+
+```sh
+pip install id4eo-scim-client
+```
+
+Enable Test Mode in Gluu by following these procedures: [Protection using Test Mode](https://gluu.org/docs/gluu-server/3.1.6/user-management/scim2/#protection-using-test-mode)
+Disable Test Mode and Enable UMA by following these procedures: [Protection using UMA](https://gluu.org/docs/gluu-server/3.1.6/user-management/scim2/#protection-using-uma)
+
+## Documentation & Usage
+
+The component documentation can be found at https://eoepca.github.io/um-common-scim-client/.
+
+For example usages, check main.py
+
+## Roadmap
+
+See the [open issues](https://github.com/EOEPCA/um-common-scim-client/issues) for a list of proposed features (and known issues).
+
+## Contributing
+
+Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.
+
+1. Fork the Project
+2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
+3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
+4. Push to the Branch (`git push origin feature/AmazingFeature`)
+5. Open a Pull Request
+
+## License
+
+Distributed under the Apache-2.0 License. See `LICENSE` for more information.
+
+## Acknowledgements
+
+- README.md is based on [this template](https://github.com/othneildrew/Best-README-Template) by [Othneil Drew](https://github.com/othneildrew).
```

### Comparing `id4eo-scim-client-1.0.1/id4eo_scim/id4eo_scim.py` & `id4eo-scim-client-1.0.2/id4eo_scim/id4eo_scim.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,577 +1,633 @@
-import requests
-import json
-import sys
-import base64
-import time
-import traceback
-import urllib
-import logging
-import datetime
-from jwkest.jws import JWS
-from jwkest.jwk import RSAKey, import_rsa_key_from_file, load_jwks_from_url, import_rsa_key
-from jwkest.jwk import load_jwks
-from Crypto.PublicKey import RSA
-from WellKnownHandler import WellKnownHandler, TYPE_SCIM, TYPE_OIDC, KEY_SCIM_USER_ENDPOINT, KEY_OIDC_TOKEN_ENDPOINT, KEY_OIDC_REGISTRATION_ENDPOINT, KEY_OIDC_SUPPORTED_AUTH_METHODS_TOKEN_ENDPOINT
-
-
-# token Endpoint Auth Methods
-# TODO: Check against WellKnownHandler's permitted auths
-ENDPOINT_AUTH_CLIENT_BASIC = "client_secret_basic"
-ENDPOINT_AUTH_CLIENT_POST = "client_secret_post"
-ENDPOINT_AUTH_CLIENT_SECRET_JWT = "client_secret_jwt"
-ENDPOINT_AUTH_CLIENT_PRIVATE_KEY_JWT = "private_key_jwt"
-ENDPOINT_AUTH_CLIENT_TLS = "tls_client_auth"
-ENDPOINT_AUTH_CLIENT_TLS_SELF_SIGNED = "self_signed_tls_client_auth"
-
-class ID4EO_Scim:
-
-    def __init__(self, host, clientID=None, clientSecret=None, jks_private_path=None, jks_public_path=None, kid=None):
-        self.client_id = clientID
-        self.client_secret = clientSecret
-        self.jks_private_path = jks_private_path
-        self.jks_public_path = jks_public_path
-        self._kid = kid if kid != None else "RSA1"
-        self.access_token = None
-        self.authRetries = 3
-        self.usingJWT = 0 if self.jks_private_path == None or self.jks_public_path == None else 1
-
-        if "https://" in host or "http://" in host:
-            self.wkh = WellKnownHandler(host, secure=False)
-        else:
-            self.wkh = WellKnownHandler("https://"+host, secure=False)
-
-        self.__SCIM_USERS_ENDPOINT = self.wkh.get(TYPE_SCIM, KEY_SCIM_USER_ENDPOINT)
-        self.__TOKEN_ENDPOINT = self.wkh.get(TYPE_OIDC, KEY_OIDC_TOKEN_ENDPOINT)
-        self.__REGISTER_ENDPOINT = self.wkh.get(TYPE_OIDC, KEY_OIDC_REGISTRATION_ENDPOINT)
-
-    def __generateRSAKeyPair(self):
-        _rsakey = RSA.generate(2048)
-        self._private_key = _rsakey.exportKey()
-        self._public_key = _rsakey.publickey().exportKey()
-
-        file_out = open(self.jks_private_path, "wb")
-        file_out.write(self._private_key)
-        file_out.close()
-
-        file_out = open(self.jks_public_path, "wb")
-        file_out.write(self._public_key)
-        file_out.close()
-
-        return
-
-    def __getRSAPrivateKey(self):
-        return self._private_key
-
-    def __getRSAPublicKey(self):
-        return self._public_key
-
-    def registerClient(self, clientName, grantTypes, redirectURIs, logoutURI, responseTypes, scopes, token_endpoint_auth_method, useJWT=0, sectorIdentifier=None, subject_type=None, access_token_as_jwt=False):
-        logging.info("Registering new client...")
-        headers = { 'content-type': "application/scim+json"}
-        if useJWT == 1:
-            self.__generateRSAKeyPair()
-            self.usingJWT = 1
-        payload = self.clientPayloadCreation(clientName, grantTypes, redirectURIs, logoutURI, responseTypes, scopes, sectorIdentifier, token_endpoint_auth_method, useJWT, subject_type, access_token_as_jwt)
-        res = requests.post(self.__REGISTER_ENDPOINT, data=payload, headers=headers, verify=False)
-        matrix = res.json()
-        self.client_id = matrix['client_id']
-        self.client_secret = matrix['client_secret']
-        logging.info("New client " + clientName + " successfully created!")
-        return matrix
-
-    def __create_jwt(self):
-        if self.jks_private_path != None:
-            _rsajwk = RSAKey(kid=self._kid, key=import_rsa_key_from_file(self.jks_private_path))
-        else:
-            _rsajwk = RSAKey(kid=self._kid, key=import_rsa_key(self.__getRSAPrivateKey()))
-        _payload = { 
-                    "iss": self.client_id,
-                    "sub": self.client_id,
-                    "aud": self.__TOKEN_ENDPOINT,
-                    "jti": datetime.datetime.today().strftime('%Y%m%d%s'),
-                    "exp": int(time.time())+3600
-                }
-        _jws = JWS(_payload, alg="RS256")
-        logging.info(str(_payload))
-        logging.info(str(_jws))
-        return _jws.sign_compact(keys=[_rsajwk])
-
-    def __getUMAAccessToken(self, ticket, jwt):
-        logging.info("UMA Token invalid, generating new one...")
-        if self.client_id == None:
-            logging.info("No client id found, please register first.")
-            return None
-        headers = { 'content-type': "application/x-www-form-urlencoded", 'cache-control': "no-cache" }
-        payload = {'grant_type' : "urn:ietf:params:oauth:grant-type:uma-ticket", 'client_id' : self.client_id, 'client_assertion_type': "urn:ietf:params:oauth:client-assertion-type:jwt-bearer", 'ticket': ticket, 'client_assertion': jwt }
-        msg = "Host unreachable"
-        status = 404
-        logging.info("Requesting UMA token")
-        logging.info("url " + self.__TOKEN_ENDPOINT)
-        logging.info("payload " + str(payload))
-        logging.info("headers " + str(headers))
-        try:
-            res = requests.post(self.__TOKEN_ENDPOINT, data=payload, headers=headers, verify=False)
-            status = res.status_code
-            logging.info("Get UMA Token reply code: " + str(status))
-            if status == 200:
-                self.access_token = res.json()["access_token"]
-        except:
-            logging.info("Get UMA Token: Exception occured!")
-            logging.info(traceback.format_exc())
-        return
-
-    def __getOAuthAccessToken(self, credentials):
-        logging.info("OAuth Token invalid, generating new one...")
-        if credentials == None:
-            logging.info("No client id or secret found, please register first.")
-            return None
-        headers = { 'content-type': "application/x-www-form-urlencoded", 'Authorization' : credentials }
-        payload = {'grant_type' : 'client_credentials'}
-        try:
-            res = requests.post(self.__TOKEN_ENDPOINT, headers=headers, data=payload, verify=False)
-            status = res.status_code
-            logging.info("Get OAuth Token reply code: " + str(status))
-            if status == 200:
-                self.access_token = res.json()["access_token"]
-        except:
-            logging.info("Get OAuth Token: Exception occured!")
-            logging.info(traceback.format_exc())
-        return
-
-    def createOAuthCredentials(self, client_id, client_secret):
-        message = client_id + ':' + client_secret
-        message_bytes = message.encode('utf-8')
-        base64_bytes = base64.b64encode(message_bytes)
-        base64_message = base64_bytes.decode('utf-8')
-        credentials = 'Basic ' + base64_message
-        return credentials
-
-    def createBearerToken(self, token):
-        return 'Bearer ' + token
- 
-    def __getUserInum(self, userID):
-        logging.info("Fetching User INUM for user " + userID + "...")
-        logging.info(self.usingJWT)
-        if self.access_token != None:
-            headers = { 'content-type': "application/x-www-form-urlencoded", 'Authorization' : self.createBearerToken(self.access_token)}
-        else:
-            headers = { 'content-type': 'application/x-www-form-urlencoded', 'Authorization': self.createBearerToken('0')}
-        msg = "Host unreachable"
-        status = 404
-        query = "userName eq \"" + userID +"\""
-        payload = { 'filter' : query }
-        url = self.__SCIM_USERS_ENDPOINT 
-        try:
-            res = requests.get(url, headers=headers, params=payload, verify=False)
-            status = res.status_code
-            msg = res.text
-            logging.info("Get User INUM reply code: " + str(status))
-        except:
-            logging.info("Get User INUM: Exception occured!")
-            logging.info(traceback.format_exc())
-        if self.authRetries == 0:
-            logging.info("Maximum number of attempts reached, re-register client.")
-            self.authRetries = 3
-            return "0"
-        if status == 401:
-            if self.usingJWT == 1:
-                self.__getUMAAccessToken(res.headers["WWW-Authenticate"].split("ticket=")[1], self.__create_jwt())
-            else:
-                self.__getOAuthAccessToken(self.createOAuthCredentials(self.client_id, self.client_secret))
-            self.authRetries -= 1
-            return self.__getUserInum(userID)
-        elif status == 500:
-            self.access_token = None
-            return self.__getUserInum(userID)
-        user = (res.json())['Resources']
-        logging.info("User INUM found!")
-        self.authRetries = 3
-        return user[0]['id']
-
-
-    def __getUserInumByEmail(self, userEmail):
-        logging.info("Fetching User INUM for user with email " + userEmail + "...")
-        if self.access_token != None:
-            headers = { 'content-type': "application/x-www-form-urlencoded", 'Authorization' : self.createBearerToken(self.access_token)}
-        else:
-            headers = { 'content-type': 'application/x-www-form-urlencoded', 'Authorization': self.createBearerToken('0')}
-        msg = "Host unreachable"
-        status = 404
-        query = "emails.value eq \"" + userEmail +"\""
-        payload = { 'filter' : query }
-        url = self.__SCIM_USERS_ENDPOINT 
-        try:
-            res = requests.get(url, headers=headers, params=payload, verify=False)
-            status = res.status_code
-            msg = res.text
-            logging.info("Get User INUM by Email reply code: " + str(status))
-        except:
-            logging.info("Get User INUM by Email: Exception occured!")
-            logging.info(traceback.format_exc())
-        if self.authRetries == 0:
-            logging.info("Maximum number of attempts reached, re-register client.")
-            self.authRetries = 3
-            return "0"
-        if status == 401:
-            if self.usingJWT == 1:
-                self.__getUMAAccessToken(res.headers["WWW-Authenticate"].split("ticket=")[1], self.__create_jwt())
-            else:
-                self.__getOAuthAccessToken(self.createOAuthCredentials(self.client_id, self.client_secret))
-            self.authRetries -= 1
-            return self.__getUserInumByEmail(userEmail)
-        elif status == 500:
-            self.access_token = None
-            return self.__getUserInumByEmail(userEmail)
-        user = (res.json())['Resources']
-        logging.info("User INUM found!")
-        self.authRetries = 3
-        return user[0]['id']
-
-    def get_users_by_query(self, query):
-        logging.info("Fetching User INUMs for users with query " + query + "...")
-        logging.info("access_token " + str(self.access_token))
-        if self.access_token != None:
-            headers = { 'content-type': "application/x-www-form-urlencoded", 'Authorization' : self.createBearerToken(self.access_token)}
-        else:
-            headers = { 'content-type': 'application/x-www-form-urlencoded', 'Authorization': self.createBearerToken('0')}
-        msg = "Host unreachable"
-        status = 404
-        payload = { 'filter' : query }
-        url = self.__SCIM_USERS_ENDPOINT
-        logging.info("headers " + str(headers))
-        logging.info("payload " + str(payload))
-        logging.info("url " + url)
-        try:
-            res = requests.get(url, headers=headers, params=payload, verify=False)
-            status = res.status_code
-            msg = res.text
-            logging.info("Get User INUM by query reply code: " + str(status))
-        except:
-            logging.info("Get User INUM by query: Exception occured!")
-            logging.info(traceback.format_exc())
-        if self.authRetries == 0:
-            logging.info("Maximum number of attempts reached, re-register client.")
-            self.authRetries = 3
-            return "0"
-        if status == 401:
-            if self.usingJWT == 1:
-                self.__getUMAAccessToken(res.headers["WWW-Authenticate"].split("ticket=")[1], self.__create_jwt())
-            else:
-                self.__getOAuthAccessToken(self.createOAuthCredentials(self.client_id, self.client_secret))
-            self.authRetries -= 1
-            return self.get_users_by_query(query)
-        elif status == 500:
-            self.access_token = None
-            return self.get_users_by_query(query)
-        if ( 'Resources' not in res.json()) :
-            return "1"
-        users = (res.json())['Resources']
-        logging.info("User INUM found!")
-        self.authRetries = 3
-        return users
-
-    def createUser(self, scim_body):
-        if self.client_id == None:
-            logging.info("No client id found, please register first.")
-            return None
-        url = self.__SCIM_USERS_ENDPOINT
-        if self.access_token != None:
-            headers = { 'Authorization' : self.createBearerToken(self.access_token)}
-        else:
-            headers = { 'Authorization': self.createBearerToken('0')}
-        msg = "Host unreachable"
-        status = 404
-        try:
-            res = requests.post(url, headers=headers, json=scim_body, verify=False)
-            status = res.status_code
-            msg = res.text
-            logging.info("User creation reply code: " + str(status))
-        except:
-            logging.info("User creation: Exception occured!")
-            logging.info(traceback.format_exc())
-        if self.authRetries == 0:
-            logging.info("Maximum number of attempts reached, re-register client.")
-            self.authRetries = 3
-            return "0"
-        if status == 401:
-            if self.usingJWT == 1:
-                self.__getUMAAccessToken(res.headers["WWW-Authenticate"].split("ticket=")[1], self.__create_jwt())
-            else:
-                self.__getOAuthAccessToken(self.createOAuthCredentials(self.client_id, self.client_secret))
-            self.authRetries -= 1
-            return self.createUser(scim_body)
-        elif status == 500:
-            self.access_token = None
-            return self.createUser(scim_body)
-        logging.info("User created.")
-        self.authRetries = 3
-        return res.json(), status
-
-
-    def getUserAttributes(self, userID):
-        logging.info("Fetching user " + userID + " attributes...")
-        if self.client_id == None:
-            logging.info("No client id found, please register first.")
-            return None
-        url = self.__SCIM_USERS_ENDPOINT + "/" + self.__getUserInum(userID)
-        if self.access_token != None:
-            headers = { 'content-type': "application/x-www-form-urlencoded", 'Authorization' : self.createBearerToken(self.access_token)}
-        else:
-            headers = { 'content-type': 'application/x-www-form-urlencoded', 'Authorization': self.createBearerToken('0')}
-        msg = "Host unreachable"
-        status = 404
-        try:
-            res = requests.get(url, headers=headers, verify=False)
-            status = res.status_code
-            msg = res.text
-            logging.info("Get User Attributes reply code: " + str(status))
-        except:
-            logging.info("Get User Attributes: Exception occured!")
-            logging.info(traceback.format_exc())
-        if self.authRetries == 0:
-            logging.info("Maximum number of attempts reached, re-register client.")
-            self.authRetries = 3
-            return "0"
-        if status == 401:
-            if self.usingJWT == 1:
-                self.__getUMAAccessToken(res.headers["WWW-Authenticate"].split("ticket=")[1], self.__create_jwt())
-            else:
-                self.__getOAuthAccessToken(self.createOAuthCredentials(self.client_id, self.client_secret))
-            self.authRetries -= 1
-            return self.getUserAttributes(userID)
-        elif status == 500:
-            self.access_token = None
-            return self.getUserAttributes(userID)
-        logging.info("User attributes found, returning.")
-        self.authRetries = 3
-        return res.json()
-
-    def addUserAttribute(self, userID, attributePath, newValue):
-        logging.info("Adding attribute " + attributePath + ", with value " + newValue + " to user " + userID)
-        if self.client_id == None:
-            logging.info("No client id found, please register first.")
-            return None
-        url = self.__SCIM_USERS_ENDPOINT + "/" + self.__getUserInum(userID)
-        if self.access_token != None:
-            headers = { 'content-type': "application/scim+json", 'Authorization' : self.createBearerToken(self.access_token)}
-        else:
-            headers = { 'content-type': 'application/x-www-form-urlencoded', 'Authorization': self.createBearerToken('0')}
-        operation = "{ \"op\":\"add\", \"path\": \"" + attributePath + "\", \"value\":\"" + newValue + "\"}"
-        payload = "{ \"Operations\" : [" + operation + "]}"
-        msg = "Host unreachable"
-        status = 404
-        try:
-            res = requests.patch(url, data=payload, headers=headers, verify=False)
-            status = res.status_code
-            msg = res.text
-            logging.info("Add User Attribute reply code: " + str(status))
-        except:
-            logging.info("Add User Attribute: Exception occured!")
-            logging.info(traceback.format_exc())
-        if self.authRetries == 0:
-            logging.info("Maximum number of attempts reached, re-register client.")
-            self.authRetries = 3
-            return "0"
-        if status == 401:
-            if self.usingJWT == 1:
-                self.__getUMAAccessToken(res.headers["WWW-Authenticate"].split("ticket=")[1], self.__create_jwt())
-            else:
-                self.__getOAuthAccessToken(self.createOAuthCredentials(self.client_id, self.client_secret))
-            self.authRetries -= 1
-            return self.addUserAttribute(userID, attributePath, newValue)
-        elif status == 500:
-            self.access_token = None
-            return self.addUserAttribute(userID, attributePath, newValue)
-        logging.info("Attribute successfully added.")
-        self.authRetries = 3
-        return status
-
-    def editUserAttribute(self, userID, attributePath, newValue):
-        logging.info("Editing user " + userID + "'s attribute " + attributePath)
-        if self.client_id == None:
-            logging.info("No client id found, please register first.")
-            return None
-        url = self.__SCIM_USERS_ENDPOINT + "/" + self.__getUserInum(userID)
-        if self.access_token != None:
-            headers = { 'content-type': "application/scim+json", 'Authorization' : self.createBearerToken(self.access_token)}
-        else:
-            headers = { 'content-type': 'application/x-www-form-urlencoded', 'Authorization': self.createBearerToken('0')}
-        operation = "{ \"op\":\"replace\", \"path\": \"" + attributePath + "\", \"value\":\"" + newValue + "\"}"
-        payload = "{ \"Operations\" : [" + operation + "]}"
-        msg = "Host unreachable"
-        status = 404
-        try:
-            res = requests.patch(url, data=payload, headers=headers, verify=False)
-            status = res.status_code
-            msg = res.text
-            logging.info("Edit User Attribute reply code: " + str(status))
-        except:
-            logging.info("Edit User Attribute: Exception occured!")
-            logging.info(traceback.format_exc())
-        if self.authRetries == 0:
-            logging.info("Maximum number of attempts reached, re-register client.")
-            self.authRetries = 3
-            return 401
-        if status == 401:
-            if self.usingJWT == 1:
-                self.__getUMAAccessToken(res.headers["WWW-Authenticate"].split("ticket=")[1], self.__create_jwt())
-            else:
-                self.__getOAuthAccessToken(self.createOAuthCredentials(self.client_id, self.client_secret))
-            self.authRetries -= 1
-            return self.editUserAttribute(userID, attributePath, newValue)
-        elif status == 500:
-            self.access_token = None
-            return self.editUserAttribute(userID, attributePath, newValue)
-        self.authRetries = 3
-        return status
-
-    def editUserMultiValueAttribute(self, userID, attributePath, newValue):
-        logging.info("Editing user " + userID + "'s mutli value attribute " + attributePath)
-        if self.client_id == None:
-            logging.info("No client id found, please register first.")
-            return None
-        url = self.__SCIM_USERS_ENDPOINT + "/" + self.__getUserInum(userID)
-        if self.access_token != None:
-            headers = { 'content-type': "application/scim+json", 'Authorization' : self.createBearerToken(self.access_token)}
-        else:
-            headers = { 'content-type': 'application/x-www-form-urlencoded', 'Authorization': self.createBearerToken('0')}
-        operation = "{ \"op\":\"replace\", \"path\": \"" + attributePath + "\", \"value\":" + newValue + "}"
-        payload = "{ \"Operations\" : [" + operation + "]}"
-        msg = "Host unreachable"
-        status = 404
-        try:
-            res = requests.patch(url, data=payload, headers=headers, verify=False)
-            status = res.status_code
-            msg = res.text
-            logging.info("Edit User Attribute reply code: " + str(status))
-        except:
-            logging.info("Edit User Attribute: Exception occured!")
-            logging.info(traceback.format_exc())
-        if self.authRetries == 0:
-            logging.info("Maximum number of attempts reached, re-register client.")
-            self.authRetries = 3
-            return 401
-        if status == 401:
-            if self.usingJWT == 1:
-                self.__getUMAAccessToken(res.headers["WWW-Authenticate"].split("ticket=")[1], self.__create_jwt())
-            else:
-                self.__getOAuthAccessToken(self.createOAuthCredentials(self.client_id, self.client_secret))
-            self.authRetries -= 1
-            return self.editUserMultiValueAttribute(userID, attributePath, newValue)
-        elif status == 500:
-            self.access_token = None
-            return self.editUserMultiValueAttribute(userID, attributePath, newValue)
-        self.authRetries = 3
-        return status
-
-    def removeUserAttribute(self, userID, attributePath):
-        logging.info("Removing user " + userID + "'s attribute " + attributePath)
-        if self.client_id == None:
-            logging.info("No client id found, please register first.")
-            return None
-        url = self.__SCIM_USERS_ENDPOINT + "/" + self.__getUserInum(userID)
-        if self.access_token != None:
-            headers = { 'content-type': "application/scim+json", 'Authorization' : self.createBearerToken(self.access_token)}
-        else:
-            headers = { 'content-type': 'application/x-www-form-urlencoded', 'Authorization': self.createBearerToken('0')}
-        operation = "{ \"op\":\"remove\", \"path\": \"" + attributePath + "\"}"
-        payload = "{ \"Operations\" : [" + operation + "]}"
-        msg = "Host unreachable"
-        status = 404
-        try:
-            res = requests.patch(url, data=payload, headers=headers, verify=False)
-            status = res.status_code
-            msg = res.text
-            logging.info("Remove User Attribute reply code: " + str(status))
-        except:
-            logging.info("Remove User Attribute: Exception occured!")
-            logging.info(traceback.format_exc())
-        if self.authRetries == 0:
-            logging.info("Maximum number of attempts reached, re-register client.")
-            self.authRetries = 3
-            return 401
-        if status == 401:
-            if self.usingJWT == 1:
-                self.__getUMAAccessToken(res.headers["WWW-Authenticate"].split("ticket=")[1], self.__create_jwt())
-            else:
-                self.__getOAuthAccessToken(self.createOAuthCredentials(self.client_id, self.client_secret))
-            self.authRetries -= 1
-            return self.removeUserAttribute(userID, attributePath)
-        elif status == 500:
-            self.access_token = None
-            return self.removeUserAttribute(userID, attributePath)
-        self.authRetries = 3
-        return status
-
-    def deleteUser(self, userEmail):
-        logging.info("Deleting user with email " + userEmail)
-        if self.client_id == None:
-            logging.info("No client id found, please register first.")
-            return None
-        url = self.__SCIM_USERS_ENDPOINT + "/" + self.__getUserInumByEmail(userEmail)
-        if self.access_token != None:
-            headers = { 'content-type': "application/x-www-form-urlencoded", 'Authorization' : self.createBearerToken(self.access_token)}
-        else:
-            headers = { 'content-type': 'application/x-www-form-urlencoded', 'Authorization': self.createBearerToken('0')}
-        msg = "Host unreachable"
-        status = 404
-        try:
-            res = requests.delete(url, headers=headers, verify=False)
-            status = res.status_code
-            msg = res.text
-            logging.info("Delete User reply code: " + str(status))
-        except:
-            logging.info("Delete User: Exception occured!")
-            logging.info(traceback.format_exc())
-        if self.authRetries == 0:
-            logging.info("Maximum number of attempts reached, re-register client.")
-            self.authRetries = 3
-            return 0
-        if status == 401:
-            if self.usingJWT == 1:
-                self.__getUMAAccessToken(res.headers["WWW-Authenticate"].split("ticket=")[1], self.__create_jwt())
-            else:
-                self.__getOAuthAccessToken(self.createOAuthCredentials(self.client_id, self.client_secret))
-            self.authRetries -= 1
-            return self.getUserAttributes(userEmail)
-        elif status == 500:
-            self.access_token = None
-            return self.getUserAttributes(userEmail)
-        logging.info("User deleted.")
-        self.authRetries = 3
-        return status
-
-    def clientPayloadCreation(self, clientName, grantTypes, redirectURIs, logoutURI, responseTypes, scopes, sectorIdentifier, token_endpoint_auth_method, useJWT=0, subject_type=None, access_token_as_jwt=False):
-        # Check the auth method is allowed by Auth Server.
-        # Since this value can change dynamically, we check it each time this function is called.
-        allowed_auth_methods = self.wkh.get(TYPE_OIDC, KEY_OIDC_SUPPORTED_AUTH_METHODS_TOKEN_ENDPOINT)
-        if token_endpoint_auth_method not in allowed_auth_methods:
-            raise Exception("Auth method '"+token_endpoint_auth_method+"' is not currently allowed by Auth Server: "+str(allowed_auth_methods))
-
-        payload = "{ \"client_name\": \"" + clientName + "\", \"grant_types\":["
-        for grant in grantTypes:
-            payload += "\"" + grant.strip() + "\", "
-        payload = payload[:-2] + "], \"redirect_uris\" : ["
-        for uri in redirectURIs:
-            payload += "\"" + uri.strip() + "\", "
-        payload = payload[:-2] + "], \"post_logout_redirect_uris\": [\""+ logoutURI +"\"], \"scope\": \""
-        for scope in scopes:
-            payload += scope.strip() + " "
-        payload = payload[:-1] + "\", "
-        if sectorIdentifier is not None:
-            payload += "\"sector_identifier_uri\": "
-            payload += "\"" + sectorIdentifier.strip() + "\", "
-            payload = payload[:-2] + ", "
-        payload += "\"response_types\": [  "
-        for response in responseTypes:
-            payload += "\"" + response.strip() + "\",  "
-        payload = payload[:-2] + "]"
-        if useJWT == 1:
-            payload += ", \"jwks\": {\"keys\": [ " + str(RSAKey(kid=self._kid, key=import_rsa_key(self.__getRSAPublicKey()))) + "]}"
-        payload += ", \"token_endpoint_auth_method\": \""+token_endpoint_auth_method+"\""
-        if subject_type:
-            payload += ", \"subject_type\": \""+subject_type+"\""
-        if access_token_as_jwt:
-            payload += ", \"access_token_as_jwt\": \"true\""
-        payload += "}"
-        return payload
+import requests
+import json
+import sys
+import base64
+import time
+import traceback
+import urllib
+import logging
+import datetime
+from jwkest.jws import JWS
+from jwkest.jwk import RSAKey, import_rsa_key_from_file, load_jwks_from_url, import_rsa_key
+from jwkest.jwk import load_jwks
+from Crypto.PublicKey import RSA
+from WellKnownHandler import WellKnownHandler, TYPE_SCIM, TYPE_OIDC, KEY_SCIM_USER_ENDPOINT, KEY_OIDC_TOKEN_ENDPOINT, \
+    KEY_OIDC_REGISTRATION_ENDPOINT, KEY_OIDC_SUPPORTED_AUTH_METHODS_TOKEN_ENDPOINT
+
+# token Endpoint Auth Methods
+# TODO: Check against WellKnownHandler's permitted auths
+ENDPOINT_AUTH_CLIENT_BASIC = "client_secret_basic"
+ENDPOINT_AUTH_CLIENT_POST = "client_secret_post"
+ENDPOINT_AUTH_CLIENT_SECRET_JWT = "client_secret_jwt"
+ENDPOINT_AUTH_CLIENT_PRIVATE_KEY_JWT = "private_key_jwt"
+ENDPOINT_AUTH_CLIENT_TLS = "tls_client_auth"
+ENDPOINT_AUTH_CLIENT_TLS_SELF_SIGNED = "self_signed_tls_client_auth"
+
+
+class ID4EO_Scim:
+
+    def __init__(self, host, clientID=None, clientSecret=None, jks_private_path=None, jks_public_path=None, kid=None):
+        self.client_id = clientID
+        self.client_secret = clientSecret
+        self.jks_private_path = jks_private_path
+        self.jks_public_path = jks_public_path
+        self._kid = kid if kid != None else "RSA1"
+        self.access_token = None
+        self.authRetries = 3
+        self.usingJWT = 0 if self.jks_private_path == None or self.jks_public_path == None else 1
+
+        if "https://" in host or "http://" in host:
+            self.wkh = WellKnownHandler(host, secure=False)
+        else:
+            self.wkh = WellKnownHandler("https://" + host, secure=False)
+
+        self.__SCIM_USERS_ENDPOINT = self.wkh.get(TYPE_SCIM, KEY_SCIM_USER_ENDPOINT)
+        self.__TOKEN_ENDPOINT = self.wkh.get(TYPE_OIDC, KEY_OIDC_TOKEN_ENDPOINT)
+        self.__REGISTER_ENDPOINT = self.wkh.get(TYPE_OIDC, KEY_OIDC_REGISTRATION_ENDPOINT)
+
+    def __generateRSAKeyPair(self):
+        _rsakey = RSA.generate(2048)
+        self._private_key = _rsakey.exportKey()
+        self._public_key = _rsakey.publickey().exportKey()
+
+        file_out = open(self.jks_private_path, "wb")
+        file_out.write(self._private_key)
+        file_out.close()
+
+        file_out = open(self.jks_public_path, "wb")
+        file_out.write(self._public_key)
+        file_out.close()
+
+        return
+
+    def __getRSAPrivateKey(self):
+        return self._private_key
+
+    def __getRSAPublicKey(self):
+        return self._public_key
+
+    def registerClient(self, clientName, grantTypes, redirectURIs, logoutURI, responseTypes, scopes,
+                       token_endpoint_auth_method, useJWT=0, sectorIdentifier=None, subject_type=None,
+                       access_token_as_jwt=False):
+        logging.info("Registering new client...")
+        headers = {'content-type': "application/scim+json"}
+        if useJWT == 1:
+            self.__generateRSAKeyPair()
+            self.usingJWT = 1
+        payload = self.clientPayloadCreation(clientName, grantTypes, redirectURIs, logoutURI, responseTypes, scopes,
+                                             sectorIdentifier, token_endpoint_auth_method, useJWT, subject_type,
+                                             access_token_as_jwt)
+        res = requests.post(self.__REGISTER_ENDPOINT, data=payload, headers=headers, verify=False)
+        matrix = res.json()
+        self.client_id = matrix['client_id']
+        self.client_secret = matrix['client_secret']
+        logging.info("New client " + clientName + " successfully created!")
+        return matrix
+
+    def __create_jwt(self):
+        if self.jks_private_path != None:
+            _rsajwk = RSAKey(kid=self._kid, key=import_rsa_key_from_file(self.jks_private_path))
+        else:
+            _rsajwk = RSAKey(kid=self._kid, key=import_rsa_key(self.__getRSAPrivateKey()))
+        _payload = {
+            "iss": self.client_id,
+            "sub": self.client_id,
+            "aud": self.__TOKEN_ENDPOINT,
+            "jti": datetime.datetime.today().strftime('%Y%m%d%s'),
+            "exp": int(time.time()) + 3600
+        }
+        _jws = JWS(_payload, alg="RS256")
+        logging.info(str(_payload))
+        logging.info(str(_jws))
+        return _jws.sign_compact(keys=[_rsajwk])
+
+    def __getUMAAccessToken(self, ticket, jwt):
+        logging.info("UMA Token invalid, generating new one...")
+        if self.client_id == None:
+            logging.info("No client id found, please register first.")
+            return None
+        headers = {'content-type': "application/x-www-form-urlencoded", 'cache-control': "no-cache"}
+        payload = {'grant_type': "urn:ietf:params:oauth:grant-type:uma-ticket", 'client_id': self.client_id,
+                   'client_assertion_type': "urn:ietf:params:oauth:client-assertion-type:jwt-bearer", 'ticket': ticket,
+                   'client_assertion': jwt}
+        msg = "Host unreachable"
+        status = 404
+        logging.info("Requesting UMA token")
+        logging.info("url " + self.__TOKEN_ENDPOINT)
+        logging.info("payload " + str(payload))
+        logging.info("headers " + str(headers))
+        try:
+            res = requests.post(self.__TOKEN_ENDPOINT, data=payload, headers=headers, verify=False)
+            status = res.status_code
+            logging.info("Get UMA Token reply code: " + str(status))
+            if status == 200:
+                self.access_token = res.json()["access_token"]
+        except:
+            logging.info("Get UMA Token: Exception occured!")
+            logging.info(traceback.format_exc())
+        return
+
+    def __getOAuthAccessToken(self, credentials):
+        logging.info("OAuth Token invalid, generating new one...")
+        if credentials == None:
+            logging.info("No client id or secret found, please register first.")
+            return None
+        headers = {'content-type': "application/x-www-form-urlencoded", 'Authorization': credentials}
+        payload = {'grant_type': 'client_credentials'}
+        try:
+            res = requests.post(self.__TOKEN_ENDPOINT, headers=headers, data=payload, verify=False)
+            status = res.status_code
+            logging.info("Get OAuth Token reply code: " + str(status))
+            if status == 200:
+                self.access_token = res.json()["access_token"]
+        except:
+            logging.info("Get OAuth Token: Exception occured!")
+            logging.info(traceback.format_exc())
+        return
+
+    def createOAuthCredentials(self, client_id, client_secret):
+        message = client_id + ':' + client_secret
+        message_bytes = message.encode('utf-8')
+        base64_bytes = base64.b64encode(message_bytes)
+        base64_message = base64_bytes.decode('utf-8')
+        credentials = 'Basic ' + base64_message
+        return credentials
+
+    def createBearerToken(self, token):
+        return 'Bearer ' + token
+
+    def __getUserInum(self, userID):
+        logging.info("Fetching User INUM for user " + userID + "...")
+        logging.info("Using JWT: " + str(self.usingJWT == 1))
+        if self.access_token != None:
+            headers = {'content-type': "application/x-www-form-urlencoded",
+                       'Authorization': self.createBearerToken(self.access_token)}
+        else:
+            headers = {'content-type': 'application/x-www-form-urlencoded',
+                       'Authorization': self.createBearerToken('0')}
+        msg = "Host unreachable"
+        status = 404
+        query = "userName eq \"" + userID + "\""
+        payload = {'filter': query}
+        url = self.__SCIM_USERS_ENDPOINT
+        try:
+            res = requests.get(url, headers=headers, params=payload, verify=False)
+            status = res.status_code
+            msg = res.text
+            logging.info("Get User INUM reply code: " + str(status))
+        except:
+            logging.info("Get User INUM: Exception occured!")
+            logging.info(traceback.format_exc())
+        if self.authRetries == 0:
+            logging.info("Maximum number of attempts reached, re-register client.")
+            self.authRetries = 3
+            return "0"
+        if status == 401:
+            if self.usingJWT == 1:
+                self.__getUMAAccessToken(res.headers["WWW-Authenticate"].split("ticket=")[1], self.__create_jwt())
+            else:
+                self.__getOAuthAccessToken(self.createOAuthCredentials(self.client_id, self.client_secret))
+            self.authRetries -= 1
+            return self.__getUserInum(userID)
+        elif status == 500:
+            self.access_token = None
+            return self.__getUserInum(userID)
+        user = (res.json())['Resources']
+        logging.info("User INUM found!")
+        self.authRetries = 3
+        return user[0]['id']
+
+    def __getUserInumByEmail(self, userEmail):
+        logging.info("Fetching User INUM for user with email " + userEmail + "...")
+        if self.access_token != None:
+            headers = {'content-type': "application/x-www-form-urlencoded",
+                       'Authorization': self.createBearerToken(self.access_token)}
+        else:
+            headers = {'content-type': 'application/x-www-form-urlencoded',
+                       'Authorization': self.createBearerToken('0')}
+        msg = "Host unreachable"
+        status = 404
+        query = "emails.value eq \"" + userEmail + "\""
+        payload = {'filter': query}
+        url = self.__SCIM_USERS_ENDPOINT
+        try:
+            res = requests.get(url, headers=headers, params=payload, verify=False)
+            status = res.status_code
+            msg = res.text
+            logging.info("Get User INUM by Email reply code: " + str(status))
+        except:
+            logging.info("Get User INUM by Email: Exception occured!")
+            logging.info(traceback.format_exc())
+        if self.authRetries == 0:
+            logging.info("Maximum number of attempts reached, re-register client.")
+            self.authRetries = 3
+            return "0"
+        if status == 401:
+            if self.usingJWT == 1:
+                self.__getUMAAccessToken(res.headers["WWW-Authenticate"].split("ticket=")[1], self.__create_jwt())
+            else:
+                self.__getOAuthAccessToken(self.createOAuthCredentials(self.client_id, self.client_secret))
+            self.authRetries -= 1
+            return self.__getUserInumByEmail(userEmail)
+        elif status == 500:
+            self.access_token = None
+            return self.__getUserInumByEmail(userEmail)
+        user = (res.json())['Resources']
+        logging.info("User INUM found!")
+        self.authRetries = 3
+        return user[0]['id']
+
+    def get_users_by_query(self, query):
+        logging.info("Fetching User INUMs for users with query " + query + "...")
+        logging.info("access_token " + str(self.access_token))
+        if self.access_token != None:
+            headers = {'content-type': "application/x-www-form-urlencoded",
+                       'Authorization': self.createBearerToken(self.access_token)}
+        else:
+            headers = {'content-type': 'application/x-www-form-urlencoded',
+                       'Authorization': self.createBearerToken('0')}
+        msg = "Host unreachable"
+        status = 404
+        payload = {'filter': query}
+        url = self.__SCIM_USERS_ENDPOINT
+        logging.info("headers " + str(headers))
+        logging.info("payload " + str(payload))
+        logging.info("url " + url)
+        try:
+            res = requests.get(url, headers=headers, params=payload, verify=False)
+            status = res.status_code
+            msg = res.text
+            logging.info("Get User INUM by query reply code: " + str(status))
+        except:
+            logging.info("Get User INUM by query: Exception occured!")
+            logging.info(traceback.format_exc())
+        if self.authRetries == 0:
+            logging.info("Maximum number of attempts reached, re-register client.")
+            self.authRetries = 3
+            return "0"
+        if status == 401:
+            if self.usingJWT == 1:
+                self.__getUMAAccessToken(res.headers["WWW-Authenticate"].split("ticket=")[1], self.__create_jwt())
+            else:
+                self.__getOAuthAccessToken(self.createOAuthCredentials(self.client_id, self.client_secret))
+            self.authRetries -= 1
+            return self.get_users_by_query(query)
+        elif status == 500:
+            self.access_token = None
+            return self.get_users_by_query(query)
+        if ('Resources' not in res.json()):
+            return "1"
+        users = (res.json())['Resources']
+        logging.info("User INUM found!")
+        self.authRetries = 3
+        return users
+
+    def createUser(self, scim_body):
+        if self.client_id == None:
+            logging.info("No client id found, please register first.")
+            return None
+        url = self.__SCIM_USERS_ENDPOINT
+        if self.access_token != None:
+            headers = {'Authorization': self.createBearerToken(self.access_token)}
+        else:
+            headers = {'Authorization': self.createBearerToken('0')}
+        msg = "Host unreachable"
+        status = 404
+        try:
+            res = requests.post(url, headers=headers, json=scim_body, verify=False)
+            status = res.status_code
+            msg = res.text
+            logging.info("User creation reply code: " + str(status))
+        except:
+            logging.info("User creation: Exception occured!")
+            logging.info(traceback.format_exc())
+        if self.authRetries == 0:
+            logging.info("Maximum number of attempts reached, re-register client.")
+            self.authRetries = 3
+            return "0"
+        if status == 401:
+            if self.usingJWT == 1:
+                self.__getUMAAccessToken(res.headers["WWW-Authenticate"].split("ticket=")[1], self.__create_jwt())
+            else:
+                self.__getOAuthAccessToken(self.createOAuthCredentials(self.client_id, self.client_secret))
+            self.authRetries -= 1
+            return self.createUser(scim_body)
+        elif status == 500:
+            self.access_token = None
+            return self.createUser(scim_body)
+        logging.info("User created.")
+        self.authRetries = 3
+        return res.json(), status
+
+    def getUserAttributes(self, userID):
+        logging.info("Fetching user " + userID + " attributes...")
+        if self.client_id == None:
+            logging.info("No client id found, please register first.")
+            return None
+        url = self.__SCIM_USERS_ENDPOINT + "/" + self.__getUserInum(userID)
+        if self.access_token != None:
+            headers = {'content-type': "application/x-www-form-urlencoded",
+                       'Authorization': self.createBearerToken(self.access_token)}
+        else:
+            headers = {'content-type': 'application/x-www-form-urlencoded',
+                       'Authorization': self.createBearerToken('0')}
+        msg = "Host unreachable"
+        status = 404
+        try:
+            res = requests.get(url, headers=headers, verify=False)
+            status = res.status_code
+            msg = res.text
+            logging.info("Get User Attributes reply code: " + str(status))
+        except:
+            logging.info("Get User Attributes: Exception occured!")
+            logging.info(traceback.format_exc())
+        if self.authRetries == 0:
+            logging.info("Maximum number of attempts reached, re-register client.")
+            self.authRetries = 3
+            return "0"
+        if status == 401:
+            if self.usingJWT == 1:
+                self.__getUMAAccessToken(res.headers["WWW-Authenticate"].split("ticket=")[1], self.__create_jwt())
+            else:
+                self.__getOAuthAccessToken(self.createOAuthCredentials(self.client_id, self.client_secret))
+            self.authRetries -= 1
+            return self.getUserAttributes(userID)
+        elif status == 500:
+            self.access_token = None
+            return self.getUserAttributes(userID)
+        logging.info("User attributes found, returning.")
+        self.authRetries = 3
+        return res.json()
+
+    def addUserAttribute(self, userID, attributePath, newValue):
+        logging.info("Adding attribute " + attributePath + ", with value " + newValue + " to user " + userID)
+        if self.client_id == None:
+            logging.info("No client id found, please register first.")
+            return None
+        url = self.__SCIM_USERS_ENDPOINT + "/" + self.__getUserInum(userID)
+        headers = {
+            'content-type': "application/scim+json",
+            'Authorization': self.createBearerToken(self.access_token if self.access_token is not None else '0')
+        }
+        payload = {
+            "Operations": [
+                {
+                    "op": "add",
+                    "path": attributePath,
+                    "value": newValue
+                }
+            ]
+        }
+        status = 404
+        try:
+            logging.info("URL: " + str(url))
+            logging.info("Payload: " + json.dumps(payload, indent=2))
+            logging.info("Headers: " + json.dumps(headers, indent=2))
+            res = requests.patch(url, data=json.dumps(payload), headers=headers, verify=False)
+            status = res.status_code
+            msg = res.text
+            logging.info("Add User Attribute reply code: " + str(status))
+            logging.info("Add User Attribute reply message: " + str(msg))
+        except:
+            logging.info("Add User Attribute: Exception occured!")
+            logging.info(traceback.format_exc())
+        if self.authRetries == 0:
+            logging.info("Maximum number of attempts reached, re-register client.")
+            self.authRetries = 3
+            return "0"
+        if status == 401:
+            if self.usingJWT == 1:
+                self.__getUMAAccessToken(res.headers["WWW-Authenticate"].split("ticket=")[1], self.__create_jwt())
+            else:
+                self.__getOAuthAccessToken(self.createOAuthCredentials(self.client_id, self.client_secret))
+            self.authRetries -= 1
+            return self.addUserAttribute(userID, attributePath, newValue)
+        elif status == 500:
+            self.access_token = None
+            return self.addUserAttribute(userID, attributePath, newValue)
+        logging.info("Attribute successfully added.")
+        self.authRetries = 3
+        return status
+
+    def editUserAttribute(self, userID, attributePath, newValue):
+        logging.info("Editing user " + userID + "'s attribute " + attributePath)
+        if self.client_id == None:
+            logging.info("No client id found, please register first.")
+            return None
+        url = self.__SCIM_USERS_ENDPOINT + "/" + self.__getUserInum(userID)
+        headers = {
+            'content-type': "application/scim+json",
+            'Authorization': self.createBearerToken(self.access_token if self.access_token is not None else '0')
+        }
+        payload = {
+            "Operations": [
+                {
+                    "op": "replace",
+                    "path": attributePath,
+                    "value": newValue
+                }
+            ]
+        }
+        status = 404
+        try:
+            logging.info("URL: " + str(url))
+            logging.info("Payload: " + json.dumps(payload, indent=2))
+            logging.info("Headers: " + json.dumps(headers, indent=2))
+            res = requests.patch(url, data=json.dumps(payload), headers=headers, verify=False)
+            status = res.status_code
+            msg = res.text
+            logging.info("Edit User Attribute reply code: " + str(status))
+            logging.info("Edit User Attribute message: " + str(msg))
+        except:
+            logging.info("Edit User Attribute: Exception occured!")
+            logging.info(traceback.format_exc())
+        if self.authRetries == 0:
+            logging.info("Maximum number of attempts reached, re-register client.")
+            self.authRetries = 3
+            return 401
+        if status == 401:
+            if self.usingJWT == 1:
+                self.__getUMAAccessToken(res.headers["WWW-Authenticate"].split("ticket=")[1], self.__create_jwt())
+            else:
+                self.__getOAuthAccessToken(self.createOAuthCredentials(self.client_id, self.client_secret))
+            self.authRetries -= 1
+            return self.editUserAttribute(userID, attributePath, newValue)
+        elif status == 500:
+            self.access_token = None
+            return self.editUserAttribute(userID, attributePath, newValue)
+        self.authRetries = 3
+        return status
+
+    def editUserMultiValueAttribute(self, userID, attributePath, newValue):
+        logging.info("Editing user " + userID + "'s mutli value attribute " + attributePath)
+        if self.client_id == None:
+            logging.info("No client id found, please register first.")
+            return None
+        url = self.__SCIM_USERS_ENDPOINT + "/" + self.__getUserInum(userID)
+        headers = {
+            'content-type': "application/scim+json",
+            'Authorization': self.createBearerToken(self.access_token if self.access_token is not None else '0')
+        }
+        payload = {
+            "Operations": [
+                {
+                    "op": "replace",
+                    "path": attributePath,
+                    "value": newValue
+                }
+            ]
+        }
+        status = 404
+        try:
+            logging.info("URL: " + str(url))
+            logging.info("Payload: " + json.dumps(payload, indent=2))
+            logging.info("Headers: " + json.dumps(headers, indent=2))
+            res = requests.patch(url, data=json.dumps(payload), headers=headers, verify=False)
+            status = res.status_code
+            msg = res.text
+            logging.info("Edit User Attribute reply code: " + str(status))
+            logging.info("Edit User Attribute message: " + str(msg))
+        except:
+            logging.info("Edit User Attribute: Exception occured!")
+            logging.info(traceback.format_exc())
+        if self.authRetries == 0:
+            logging.info("Maximum number of attempts reached, re-register client.")
+            self.authRetries = 3
+            return 401
+        if status == 401:
+            if self.usingJWT == 1:
+                self.__getUMAAccessToken(res.headers["WWW-Authenticate"].split("ticket=")[1], self.__create_jwt())
+            else:
+                self.__getOAuthAccessToken(self.createOAuthCredentials(self.client_id, self.client_secret))
+            self.authRetries -= 1
+            return self.editUserMultiValueAttribute(userID, attributePath, newValue)
+        elif status == 500:
+            self.access_token = None
+            return self.editUserMultiValueAttribute(userID, attributePath, newValue)
+        self.authRetries = 3
+        return status
+
+    def removeUserAttribute(self, userID, attributePath):
+        logging.info("Removing user " + userID + "'s attribute " + attributePath)
+        if self.client_id == None:
+            logging.info("No client id found, please register first.")
+            return None
+        url = self.__SCIM_USERS_ENDPOINT + "/" + self.__getUserInum(userID)
+        headers = {
+            'content-type': "application/scim+json",
+            'Authorization': self.createBearerToken(self.access_token if self.access_token is not None else '0')
+        }
+        payload = {
+            "Operations": [
+                {
+                    "op": "remove",
+                    "path": attributePath
+                }
+            ]
+        }
+        status = 404
+        try:
+            res = requests.patch(url, data=payload, headers=headers, verify=False)
+            status = res.status_code
+            msg = res.text
+            logging.info("Remove User Attribute reply code: " + str(status))
+            logging.info("Remove User Attribute message: " + str(msg))
+        except:
+            logging.info("Remove User Attribute: Exception occured!")
+            logging.info(traceback.format_exc())
+        if self.authRetries == 0:
+            logging.info("Maximum number of attempts reached, re-register client.")
+            self.authRetries = 3
+            return 401
+        if status == 401:
+            if self.usingJWT == 1:
+                self.__getUMAAccessToken(res.headers["WWW-Authenticate"].split("ticket=")[1], self.__create_jwt())
+            else:
+                self.__getOAuthAccessToken(self.createOAuthCredentials(self.client_id, self.client_secret))
+            self.authRetries -= 1
+            return self.removeUserAttribute(userID, attributePath)
+        elif status == 500:
+            self.access_token = None
+            return self.removeUserAttribute(userID, attributePath)
+        self.authRetries = 3
+        return status
+
+    def deleteUser(self, userEmail):
+        logging.info("Deleting user with email " + userEmail)
+        if self.client_id == None:
+            logging.info("No client id found, please register first.")
+            return None
+        url = self.__SCIM_USERS_ENDPOINT + "/" + self.__getUserInumByEmail(userEmail)
+        if self.access_token != None:
+            headers = {'content-type': "application/x-www-form-urlencoded",
+                       'Authorization': self.createBearerToken(self.access_token)}
+        else:
+            headers = {'content-type': 'application/x-www-form-urlencoded',
+                       'Authorization': self.createBearerToken('0')}
+        msg = "Host unreachable"
+        status = 404
+        try:
+            res = requests.delete(url, headers=headers, verify=False)
+            status = res.status_code
+            msg = res.text
+            logging.info("Delete User reply code: " + str(status))
+        except:
+            logging.info("Delete User: Exception occured!")
+            logging.info(traceback.format_exc())
+        if self.authRetries == 0:
+            logging.info("Maximum number of attempts reached, re-register client.")
+            self.authRetries = 3
+            return 0
+        if status == 401:
+            if self.usingJWT == 1:
+                self.__getUMAAccessToken(res.headers["WWW-Authenticate"].split("ticket=")[1], self.__create_jwt())
+            else:
+                self.__getOAuthAccessToken(self.createOAuthCredentials(self.client_id, self.client_secret))
+            self.authRetries -= 1
+            return self.getUserAttributes(userEmail)
+        elif status == 500:
+            self.access_token = None
+            return self.getUserAttributes(userEmail)
+        logging.info("User deleted.")
+        self.authRetries = 3
+        return status
+
+    def clientPayloadCreation(self, clientName, grantTypes, redirectURIs, logoutURI, responseTypes, scopes,
+                              sectorIdentifier, token_endpoint_auth_method, useJWT=0, subject_type=None,
+                              access_token_as_jwt=False):
+        # Check the auth method is allowed by Auth Server.
+        # Since this value can change dynamically, we check it each time this function is called.
+        allowed_auth_methods = self.wkh.get(TYPE_OIDC, KEY_OIDC_SUPPORTED_AUTH_METHODS_TOKEN_ENDPOINT)
+        if token_endpoint_auth_method not in allowed_auth_methods:
+            raise Exception(
+                "Auth method '" + token_endpoint_auth_method + "' is not currently allowed by Auth Server: " + str(
+                    allowed_auth_methods))
+
+        payload = "{ \"client_name\": \"" + clientName + "\", \"grant_types\":["
+        for grant in grantTypes:
+            payload += "\"" + grant.strip() + "\", "
+        payload = payload[:-2] + "], \"redirect_uris\" : ["
+        for uri in redirectURIs:
+            payload += "\"" + uri.strip() + "\", "
+        payload = payload[:-2] + "], \"post_logout_redirect_uris\": [\"" + logoutURI + "\"], \"scope\": \""
+        for scope in scopes:
+            payload += scope.strip() + " "
+        payload = payload[:-1] + "\", "
+        if sectorIdentifier is not None:
+            payload += "\"sector_identifier_uri\": "
+            payload += "\"" + sectorIdentifier.strip() + "\", "
+            payload = payload[:-2] + ", "
+        payload += "\"response_types\": [  "
+        for response in responseTypes:
+            payload += "\"" + response.strip() + "\",  "
+        payload = payload[:-2] + "]"
+        if useJWT == 1:
+            payload += ", \"jwks\": {\"keys\": [ " + str(
+                RSAKey(kid=self._kid, key=import_rsa_key(self.__getRSAPublicKey()))) + "]}"
+        payload += ", \"token_endpoint_auth_method\": \"" + token_endpoint_auth_method + "\""
+        if subject_type:
+            payload += ", \"subject_type\": \"" + subject_type + "\""
+        if access_token_as_jwt:
+            payload += ", \"access_token_as_jwt\": \"true\""
+        payload += "}"
+        return payload
```

### Comparing `id4eo-scim-client-1.0.1/id4eo_scim/main.py` & `id4eo-scim-client-1.0.2/id4eo_scim/main.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-#!/usr/bin/env python3
-from id4eo_scim import ID4EO_Scim, ENDPOINT_AUTH_CLIENT_POST, ENDPOINT_AUTH_CLIENT_PRIVATE_KEY_JWT
-import logging
-# *** Use this for auto-contained examples ***
-
-def main():
-    logging.getLogger().setLevel(logging.INFO)
-
-    #Determine Gluu host address
-    gluuHost = "https://demoexample.gluu.org"
-
-    #Initiate class
-    scim_client = ID4EO_Scim(host=gluuHost)
-
-    #Initiate class with an existing user (INUM), specifying the location of their private RSA key file and kid (key ID) for UMA purposes
-    #When no kid is provided, default value "RSA1" is used
-    #scim_client = EOEPCA_Scim(host=gluuHost, clientID="", clientSecret="", jks_path="", kid="")
-
-    #Register a new client, returns client information in JSON format
-    clientName="TestClient"
-    grantTypes=["client_credentials", "urn:ietf:params:oauth:grant-type:uma-ticket", "password", "implicit"]
-    redirectURIs=["https://demoexample.gluu.org/web_ui/oauth/callback"]
-    logoutURI="https://demoexample.gluu.org/logout"
-    responseTypes=[]
-    #Sector identifier is OPTIONAL field
-    #Redirect URIs MUST be contained in Sector Identifier, if this is used
-    sectorIdentifier="https://demoexample.gluu.org/oxauth/sectoridentifier/9b473868-fa96-4fd1-a662-76e3663c9726"
-    #sectorIdentifiers=None
-    #OpenID scope examples
-    scopes=["openid", "oxd", "permission"]
-    #UMA scope example
-    #scopes=["https://demoexample.gluu.org/oxauth/restv1/uma/scopes/scim_access"]
-    #Register call, with useJWK=1 if JWK is being used
-    #clientJSON = scim_client.registerClient(clientName=clientName, grantTypes=grantTypes, redirectURIs=redirectURIs, logoutURI=logoutURI, responseTypes=responseTypes, scopes=scopes, token_endpoint_auth_method= ENDPOINT_AUTH_CLIENT_POST)
-    clientJSON = scim_client.registerClient(clientName=clientName, grantTypes=grantTypes, redirectURIs=redirectURIs, logoutURI=logoutURI, responseTypes=responseTypes, scopes=scopes, sectorIdentifier=sectorIdentifier, token_endpoint_auth_method= ENDPOINT_AUTH_CLIENT_POST)
-    #clientJSON = scim_client.registerClient(clientName=clientName, grantTypes=grantTypes, redirectURIs=redirectURIs, logoutURI=logoutURI, responseTypes=responseTypes, scopes=scopes, token_endpoint_auth_method= ENDPOINT_AUTH_CLIENT_PRIVATE_KEY_JWT , useJWK=1)
-    print(clientJSON)
-
-    #User to which we want to obtain all attributes
-    userID = "test@test.com"
-
-    #Get user attributes
-    attributes = scim_client.getUserAttributes(userID=userID)
-    print(attributes)
-
-    #Add a new attribute
-    attributePath="name.middleName"
-    newValue="Middle"
-    scim_client.addUserAttribute(userID=userID, attributePath=attributePath, newValue=newValue)
-    
-    #Modify an attribute
-    attributePath="name.familyName"
-    newValue="Last"
-    scim_client.editUserAttribute(userID=userID, attributePath=attributePath, newValue=newValue)
-
-    #Remove an attribute
-    attributePath="name.middleName"
-    scim_client.removeUserAttribute(userID=userID, attributePath=attributePath)
-    
-    #Delete user
-    reply = scim_client.deleteUser(userID=userID)
-    print(reply)
-
-if __name__ == "__main__":
-     
-    main()
+#!/usr/bin/env python3
+from id4eo_scim import ID4EO_Scim, ENDPOINT_AUTH_CLIENT_POST, ENDPOINT_AUTH_CLIENT_PRIVATE_KEY_JWT
+import logging
+# *** Use this for auto-contained examples ***
+
+def main():
+    logging.getLogger().setLevel(logging.INFO)
+
+    #Determine Gluu host address
+    gluuHost = "https://demoexample.gluu.org"
+
+    #Initiate class
+    scim_client = ID4EO_Scim(host=gluuHost)
+
+    #Initiate class with an existing user (INUM), specifying the location of their private RSA key file and kid (key ID) for UMA purposes
+    #When no kid is provided, default value "RSA1" is used
+    #scim_client = EOEPCA_Scim(host=gluuHost, clientID="", clientSecret="", jks_path="", kid="")
+
+    #Register a new client, returns client information in JSON format
+    clientName="TestClient"
+    grantTypes=["client_credentials", "urn:ietf:params:oauth:grant-type:uma-ticket", "password", "implicit"]
+    redirectURIs=["https://demoexample.gluu.org/web_ui/oauth/callback"]
+    logoutURI="https://demoexample.gluu.org/logout"
+    responseTypes=[]
+    #Sector identifier is OPTIONAL field
+    #Redirect URIs MUST be contained in Sector Identifier, if this is used
+    sectorIdentifier="https://demoexample.gluu.org/oxauth/sectoridentifier/9b473868-fa96-4fd1-a662-76e3663c9726"
+    #sectorIdentifiers=None
+    #OpenID scope examples
+    scopes=["openid", "oxd", "permission"]
+    #UMA scope example
+    #scopes=["https://demoexample.gluu.org/oxauth/restv1/uma/scopes/scim_access"]
+    #Register call, with useJWK=1 if JWK is being used
+    #clientJSON = scim_client.registerClient(clientName=clientName, grantTypes=grantTypes, redirectURIs=redirectURIs, logoutURI=logoutURI, responseTypes=responseTypes, scopes=scopes, token_endpoint_auth_method= ENDPOINT_AUTH_CLIENT_POST)
+    clientJSON = scim_client.registerClient(clientName=clientName, grantTypes=grantTypes, redirectURIs=redirectURIs, logoutURI=logoutURI, responseTypes=responseTypes, scopes=scopes, sectorIdentifier=sectorIdentifier, token_endpoint_auth_method= ENDPOINT_AUTH_CLIENT_POST)
+    #clientJSON = scim_client.registerClient(clientName=clientName, grantTypes=grantTypes, redirectURIs=redirectURIs, logoutURI=logoutURI, responseTypes=responseTypes, scopes=scopes, token_endpoint_auth_method= ENDPOINT_AUTH_CLIENT_PRIVATE_KEY_JWT , useJWK=1)
+    print(clientJSON)
+
+    #User to which we want to obtain all attributes
+    userID = "test@test.com"
+
+    #Get user attributes
+    attributes = scim_client.getUserAttributes(userID=userID)
+    print(attributes)
+
+    #Add a new attribute
+    attributePath="name.middleName"
+    newValue="Middle"
+    scim_client.addUserAttribute(userID=userID, attributePath=attributePath, newValue=newValue)
+    
+    #Modify an attribute
+    attributePath="name.familyName"
+    newValue="Last"
+    scim_client.editUserAttribute(userID=userID, attributePath=attributePath, newValue=newValue)
+
+    #Remove an attribute
+    attributePath="name.middleName"
+    scim_client.removeUserAttribute(userID=userID, attributePath=attributePath)
+    
+    #Delete user
+    reply = scim_client.deleteUser(userID=userID)
+    print(reply)
+
+if __name__ == "__main__":
+     
+    main()
```

### Comparing `id4eo-scim-client-1.0.1/setup.py` & `id4eo-scim-client-1.0.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import setuptools
-
-setuptools.setup(
-  name = 'id4eo-scim-client',
-  version = '1.0.1',
-  author = 'ID4EO',
-  author_email = 'joao.matos@elecnor.es',
-  description = 'Python library to interact with SCIM protocol',
-  url = 'https://stash.elecnor-deimos.com/projects/GSC4EO/repos/id4eo/browse/src/scim-client',
-  packages=setuptools.find_packages(),
-  license='apache-2.0',
-  keywords = ['SCIM', 'Client', 'ID4EO','user','management'],
-  classifiers=[
-    'Development Status :: 3 - Alpha',                      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
-    'Intended Audience :: Developers',
-    'Topic :: Software Development :: Build Tools',
-  ],
-  python_requires='>=3.6',
+import setuptools
+
+setuptools.setup(
+  name = 'id4eo-scim-client',
+  version = '1.0.2',
+  author = 'ID4EO',
+  author_email = 'joao.matos@elecnor.es',
+  description = 'Python library to interact with SCIM protocol',
+  url = 'https://stash.elecnor-deimos.com/projects/GSC4EO/repos/id4eo/browse/src/scim-client',
+  packages=setuptools.find_packages(),
+  license='apache-2.0',
+  keywords = ['SCIM', 'Client', 'ID4EO','user','management'],
+  classifiers=[
+    'Development Status :: 3 - Alpha',                      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
+    'Intended Audience :: Developers',
+    'Topic :: Software Development :: Build Tools',
+  ],
+  python_requires='>=3.6',
 )
```

