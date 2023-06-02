# Comparing `tmp/twitter-api-client-0.8.4.tar.gz` & `tmp/twitter-api-client-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.8.4.tar", last modified: Fri Jun  2 03:04:19 2023, max compression
+gzip compressed data, was "twitter-api-client-0.8.5.tar", last modified: Fri Jun  2 17:06:28 2023, max compression
```

## Comparing `twitter-api-client-0.8.4.tar` & `twitter-api-client-0.8.5.tar`

### file list

```diff
@@ -1,37 +1,19 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-02 03:04:19.553220 twitter-api-client-0.8.4/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)    10964 2023-06-02 03:04:19.553220 twitter-api-client-0.8.4/PKG-INFO
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-02 03:04:19.551220 twitter-api-client-0.8.4/protonmail/
--rw-r--r--   0 x         (1000) x         (1000)       78 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    24269 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/api.py
--rw-r--r--   0 x         (1000) x         (1000)     5579 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/cert_pinning.py
--rw-r--r--   0 x         (1000) x         (1000)     1589 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     1029 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/exceptions.py
--rw-r--r--   0 x         (1000) x         (1000)     1397 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/logger.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-02 03:04:19.551220 twitter-api-client-0.8.4/protonmail/metadata/
--rw-r--r--   0 x         (1000) x         (1000)      106 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/metadata/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)     1225 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/metadata/_base.py
--rw-r--r--   0 x         (1000) x         (1000)     3432 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/metadata/textfile_metadata.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-02 03:04:19.551220 twitter-api-client-0.8.4/protonmail/srp/
--rw-r--r--   0 x         (1000) x         (1000)      172 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/srp/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)     9305 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/srp/_ctsrp.py
--rw-r--r--   0 x         (1000) x         (1000)     4426 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/srp/_pysrp.py
--rw-r--r--   0 x         (1000) x         (1000)      684 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/srp/pmhash.py
--rw-r--r--   0 x         (1000) x         (1000)     1482 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/srp/util.py
--rw-r--r--   0 x         (1000) x         (1000)      962 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/utils.py
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-02 03:04:19.553220 twitter-api-client-0.8.4/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)    12852 2023-06-02 03:02:38.000000 twitter-api-client-0.8.4/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-02 03:04:19.552220 twitter-api-client-0.8.4/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    22968 2023-06-02 01:49:12.000000 twitter-api-client-0.8.4/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    28454 2023-06-02 01:49:12.000000 twitter-api-client-0.8.4/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     7350 2023-06-02 01:49:12.000000 twitter-api-client-0.8.4/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    27552 2023-06-02 01:49:12.000000 twitter-api-client-0.8.4/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     5960 2023-06-02 01:50:23.000000 twitter-api-client-0.8.4/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     9198 2023-06-02 01:49:12.000000 twitter-api-client-0.8.4/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-02 03:04:19.553220 twitter-api-client-0.8.4/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)    10964 2023-06-02 03:04:19.000000 twitter-api-client-0.8.4/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      740 2023-06-02 03:04:19.000000 twitter-api-client-0.8.4/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-02 03:04:19.000000 twitter-api-client-0.8.4/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)      130 2023-06-02 03:04:19.000000 twitter-api-client-0.8.4/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)       19 2023-06-02 03:04:19.000000 twitter-api-client-0.8.4/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-02 17:06:28.543697 twitter-api-client-0.8.5/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.8.5/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)    11223 2023-06-02 17:06:28.543697 twitter-api-client-0.8.5/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-02 17:06:28.543697 twitter-api-client-0.8.5/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)    13056 2023-06-02 17:03:22.000000 twitter-api-client-0.8.5/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-02 17:06:28.543697 twitter-api-client-0.8.5/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-05-28 16:24:21.000000 twitter-api-client-0.8.5/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    23264 2023-06-02 17:01:02.000000 twitter-api-client-0.8.5/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    28454 2023-06-02 01:49:12.000000 twitter-api-client-0.8.5/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     7410 2023-06-02 17:01:01.000000 twitter-api-client-0.8.5/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    27552 2023-06-02 17:05:12.000000 twitter-api-client-0.8.5/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     5960 2023-06-02 01:50:23.000000 twitter-api-client-0.8.5/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     9348 2023-06-02 17:01:02.000000 twitter-api-client-0.8.5/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-02 17:06:28.543697 twitter-api-client-0.8.5/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)    11223 2023-06-02 17:06:28.000000 twitter-api-client-0.8.5/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-02 17:06:28.000000 twitter-api-client-0.8.5/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-02 17:06:28.000000 twitter-api-client-0.8.5/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-02 17:06:28.000000 twitter-api-client-0.8.5/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-02 17:06:28.000000 twitter-api-client-0.8.5/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.8.4/LICENSE` & `twitter-api-client-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.4/PKG-INFO` & `twitter-api-client-0.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.8.4
+Version: 0.8.5
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
@@ -351,14 +351,17 @@
         'filter': SpaceCategory.Live,
         'query': 'foo bar'
     }
 ])
 ```
 
 ### Automated Solvers
+
+> **Currently removed** due to issues running on Mac. Code has been commented out for now. Cloning the repo, adding the proton mail package, and uncommenting the code referencing `protonmail` can be used as a temporary workaround to re-enable this feature.
+
 To set up automated email confirmation/verification solvers, add your Proton Mail credentials below as shown.
 This removes the need to manually solve email challenges via the web app. These credentials can be used in `Scraper`, `Account`, and `Search` constructors.
 
 E.g.
 
 ```python
 from twitter.scraper import Scraper
```

### Comparing `twitter-api-client-0.8.4/protonmail/api.py` & `twitter-api-client-0.8.5/twitter/scraper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,708 +1,612 @@
-import base64
-import json
-
-import sys
-import gnupg
-import requests
-
-"""
-When using alternative routing, we want to verify as little data as possible. Thus we'll
-end up relying mostly on tls key pinning. If we don't disable warnings, a warning will be
-constantly popping on the terminal informing the user about it.
-https://urllib3.readthedocs.io/en/latest/advanced-usage.html#ssl-warnings
-"""
-import urllib3
-
-urllib3.disable_warnings()
-
-from concurrent.futures import ThreadPoolExecutor
-
-
-from .cert_pinning import TLSPinningAdapter
-from .constants import (ALT_HASH_DICT, DEFAULT_TIMEOUT, DNS_HOSTS,
-                        ENCODED_URLS, SRP_MODULUS_KEY,
-                        SRP_MODULUS_KEY_FINGERPRINT)
-from .exceptions import (ConnectionTimeOutError, NetworkError,
-                         NewConnectionError, ProtonAPIError, TLSPinningError,
-                         UnknownConnectionError, MissingDepedencyError)
-from .logger import CustomLogger
-from .metadata import MetadataBackend
-from .srp import User as PmsrpUser
-
-
-class Session:
-    """A Proton Session.
-
-    Provides public key pinning, fetch alternative routes and connect to
-    Proton API in a authenticated manner, dump and load sessions.
-
-    All this is possible since it serves as a wrapper for `<Requests>`
-
-    Basic Usage:
-
-      >>> import proton
-      >>> s = proton.Session("https://url-to-api.ch")
-      >>> s.enable_alternative_routing = True
-      >>> s.api_request("/api/endpoint")
-      <Response [200]>
-    """
-    _base_headers = {
-        "x-pm-apiversion": "3",
-        "Accept": "application/vnd.protonmail.v1+json"
-    }
-    __force_skip_alternative_routing = False
+import asyncio
+import logging.config
+import math
+import platform
+import random
+from concurrent.futures import ThreadPoolExecutor, as_completed
+
+import aiofiles
+import httpx
+import websockets
+from httpx import AsyncClient, Limits, ReadTimeout, URL
+from tqdm import tqdm
+from tqdm.asyncio import tqdm_asyncio
+
+from .constants import *
+from .login import login
+from .util import *
+
+try:
+    if get_ipython().__class__.__name__ == 'ZMQInteractiveShell':
+        import nest_asyncio
+
+        nest_asyncio.apply()
+except:
+    ...
+
+if platform.system() != 'Windows':
+    try:
+        import uvloop
+
+        uvloop.install()
+    except ImportError as e:
+        ...
+
+
+class Scraper:
+    def __init__(self, email: str = None, username: str = None, password: str = None, session: Client = None, **kwargs):
+        self.guest = False
+        self.logger = self.init_logger(kwargs.get('log_config', False))
+        self.session = self.validate_session(email, username, password, session, **kwargs)
+        self.save = kwargs.get('save', True)
+        self.debug = kwargs.get('debug', 0)
+        self.out_path = Path('data')
+        self.api = 'https://twitter.com/i/api/graphql'
 
     @staticmethod
-    def load(
-        dump, log_dir_path, cache_dir_path,
-        tls_pinning=True, timeout=DEFAULT_TIMEOUT,
-        proxies=None
-    ):
-        """Load session from file/keyring.
-
-        This should load the output generated by dump().
-
-        Args:
-            log_dir_path (str): path to desired logging directory
-            cache_dir_path (str): path to desired cache directory
-            tls_pinning (bool): tls pinning
-            timeout (tuple|int|float): How long to wait for the server to send
-            data before giving up.
-            proxies (dict): desired proxies
-
-        Returns:
-            proton.Session
-        """
-        api_url = dump["api_url"]
-        appversion = dump["appversion"]
-        user_agent = dump["User-Agent"]
-        cookies = dump.get("cookies", {})
-        s = Session(
-            api_url=api_url,
-            log_dir_path=log_dir_path,
-            cache_dir_path=cache_dir_path,
-            appversion=appversion,
-            user_agent=user_agent,
-            tls_pinning=tls_pinning,
-            timeout=timeout,
-            proxies=proxies
-        )
-        requests.utils.add_dict_to_cookiejar(s.s.cookies, cookies)
-        s._session_data = dump["session_data"]
-        if s.UID is not None:
-            s.s.headers["x-pm-uid"] = s.UID
-            s.s.headers["Authorization"] = "Bearer " + s.AccessToken
-        return s
-
-    def dump(self):
-        """Dump session.
-
-        If you want to reuse the session, then dump it and store the values
-        somewhere safe.
-
-        Returns:
-            dict
-        """
-        return {
-            "api_url": self.__api_url,
-            "appversion": self.__appversion,
-            "User-Agent": self.__user_agent,
-            "cookies": self.s.cookies.get_dict(),
-            "session_data": self._session_data
-        }
-
-    def __init__(
-        self, api_url, log_dir_path, cache_dir_path,
-        appversion="Other", user_agent="None",
-        tls_pinning=True, ClientSecret=None, timeout=DEFAULT_TIMEOUT,
-        proxies=None
-    ):
-        """Constructs a new Session object.
-
-        Args:
-            api_url (string): URL for the new Session object
-            appversion (string): version for the new Session object
-            user_agent (string): user agent for the new Session` object
-            should be in the following syntax:
-                - Linux based -> ClientName/client.version (Linux; Distro/distro_version)
-                - Non-linux based -> ClientName/client.version (OS)
-            tls_pinning (bool): wether tls pinning should be enabled for the new
-                Session object.
-            ClientSecret (string): secret token for the new Session object that
-                is added to the payload with key `ClientSecret`. [OPTIONAL]
-            timeout (int|float|tuple): How long to wait for the server to send
-                data before giving up. [OPTIONAL]
-            proxies (dict): proxies to be used by the new Session object.
-                This is mutually exclusive with `tls_pinning`. [OPTIONAL]
-        """
-        self.__api_url = api_url
-        self.__appversion = appversion
-        self.__user_agent = user_agent
-        self.__clientsecret = ClientSecret
-        self.__timeout = timeout
-        self.__tls_pinning_enabled = tls_pinning
-        self._logger = CustomLogger()
-        self._logger.set_log_path(log_dir_path)
-        self._logger = self._logger.logger
-        self.__metadata = MetadataBackend.get_backend()
-        self.__metadata.cache_dir_path = cache_dir_path
-        self.__metadata.logger = self._logger
-        self.__allow_alternative_routing = None
-
-        # Verify modulus
-        self.__gnupg = gnupg.GPG()
-        self.__gnupg.import_keys(SRP_MODULUS_KEY)
-
-        self._session_data = {}
-
-        self.s = requests.Session()
-
-        if proxies and self.__tls_pinning_enabled:
-            raise RuntimeError("Not allowed to add proxies while TLS Pinning is enabled")
-
-        self.s.proxies = proxies
-
-        if self.__tls_pinning_enabled:
-            self.s.mount(self.__api_url, TLSPinningAdapter())
-
-        self.s.headers["x-pm-appversion"] = appversion
-        self.s.headers["User-Agent"] = user_agent
-
-    def api_request(
-        self, endpoint,
-        jsondata=None, additional_headers=None,
-        method=None, params=None, _skip_alt_routing_for_api_check=False
-    ):
-        """Make API request.
-
-        Args:
-            endpoint (string): API endpoint.
-            jsondata (json): json to send in the body.
-            additional_headers (dict): additional (dictionary of) headers to send.
-            method (string): get|post|put|delete|patch.
-            params (dict|tuple): URL parameters to append to the URL. If a dictionary or
-                list of tuples ``[(key, value)]`` is provided, form-encoding will
-                take place.
-            _skip_alt_routing_for_api_check (bool): used to temporarly skip alt routing.
-
-        Returns:
-            requests.Response
-        """
-        if self.__allow_alternative_routing is None:
-            msg = "Alternative routing has not been configured before making API requests. " \
-                "Please either enable or disable it before making any requests."
-            self._logger.info(msg)
-            raise RuntimeError(msg)
-
-        fct = self.s.post
-
-        if method is None:
-            if jsondata is None:
-                fct = self.s.get
-            else:
-                fct = self.s.post
-        else:
-            fct = {
-                "get": self.s.get,
-                "post": self.s.post,
-                "put": self.s.put,
-                "delete": self.s.delete,
-                "patch": self.s.patch
-            }.get(method.lower())
-
-        if fct is None:
-            raise ValueError("Unknown method: {}".format(method))
-
-        _url = self.__api_url
-        _verify = True
-
-        if not self.__metadata.try_original_url(
-            self.__allow_alternative_routing,
-            self.__force_skip_alternative_routing
-        ):
-            _url = self.__metadata.get_alternative_url()
-            _verify = False
-
-        request_params = {
-            "url": _url,
-            "endpoint": endpoint,
-            "headers": additional_headers,
-            "json": jsondata,
-            "timeout": self.__timeout,
-            "verify": _verify,
-            "params": params
-        }
-
-        exception_class = None
-        exception_msg = None
-
-        try:
-            response = self.__make_request(fct, **request_params)
-        except (
-            NewConnectionError,
-            ConnectionTimeOutError,
-            TLSPinningError,
-        ) as e:
-            self._logger.exception(e)
-            exc_type, *_ = sys.exc_info()
-            exception_class = exc_type
-            exception_msg = e
-        except (Exception, requests.exceptions.BaseHTTPError) as e:
-            self._logger.exception(e)
-            raise UnknownConnectionError(e)
-
-        if exception_class and (not self.__allow_alternative_routing or _skip_alt_routing_for_api_check or self.__force_skip_alternative_routing): # noqa
-            self._logger.info("{}: {}".format(exception_class, exception_msg))
-            raise exception_class(exception_msg)
-        elif (
-            exception_class in [NewConnectionError, ConnectionTimeOutError, TLSPinningError]
-            and not self._is_api_reacheable()
-        ):
-            response = self.__try_with_alt_routing(fct, **request_params)
-
-        try:
-            status_code = response.status_code
-        except: # noqa
-            status_code = False
-
-        try:
-            json_error = False
-            response = response.json()
-        except json.decoder.JSONDecodeError as e:
-            json_error = e
-
-        if json_error and status_code != 200:
-            self._logger.exception(json_error)
-            raise ProtonAPIError(
-                {
-                    "Code": response.status_code,
-                    "Error": response.reason,
-                    "Headers": response.headers
-                }
-            )
-
-        # This check is needed for routers or any other clients that will ask for other
-        # data that is not provided in json format, such as when asking /vpn/config for
-        # a .ovpn template
-        try:
-            if response["Code"] not in [1000, 1001]:
-                if response["Code"] == 9001:
-                    self.__captcha_token = response["Details"]["HumanVerificationToken"]
-                elif response["Code"] == 12087:
-                    del self.human_verification_token
-
-                raise ProtonAPIError(response)
-        except TypeError as e:
-            if status_code != 200:
-                raise TypeError(e)
-
-        return response
-
-    def __try_with_alt_routing(self, fct, **request_params):
-        alternative_routes = self.get_alternative_routes_from_dns()
-
-        request_params["verify"] = False
-        response = None
+    def init_logger(cfg: dict) -> Logger:
+        if cfg:
+            logging.config.dictConfig(cfg)
+            return logging.getLogger(__name__)
+        return logger
 
-        for route in alternative_routes:
-            _alt_url = "https://{}".format(route)
-            request_params["url"] = _alt_url
+    def validate_session(self, *args, **kwargs):
+        email, username, password, session = args
+        if session and all(session.cookies.get(c) for c in {'ct0', 'auth_token'}):
+            # authenticated session provided
+            return session
+        if not session:
+            # no session provided, login to authenticate
+            return login(email, username, password, **kwargs)
+        self.logger.warning(f'\n{RED}WARNING: This is a guest session, '
+                            f'some endpoints cannot be accessed.{RESET}\n')
+        self.guest = True
+        return session
 
-            if self.__tls_pinning_enabled:
-                self.s.mount(_alt_url, TLSPinningAdapter(ALT_HASH_DICT))
+    def users(self, screen_names: list[str], **kwargs) -> list[dict]:
+        return self._run(Operation.UserByScreenName, screen_names, **kwargs)
 
-            self._logger.info("Trying {}".format(_alt_url))
-            try:
-                response = self.__make_request(fct, **request_params)
-            except Exception as e: # noqa
-                self._logger.exception(e)
-                continue
-            else:
-                self._logger.info("Storing alternative route: {}".format(_alt_url))
-                self.__metadata.store_alternative_route(_alt_url)
-                break
-
-        if not response:
-            self._logger.info("Possible network error, unable to reach API")
-            raise NetworkError("Network error")
-
-        return response
+    def tweets_by_id(self, tweet_ids: list[int], **kwargs) -> list[dict]:
+        return self._run(Operation.TweetResultByRestId, tweet_ids, **kwargs)
 
-    def __make_request(self, fct, **kwargs):
-        _endpoint = kwargs.pop("endpoint")
-        _url = kwargs["url"]
+    def tweets_details(self, tweet_ids: list[int], **kwargs) -> list[dict]:
+        return self._run(Operation.TweetDetail, tweet_ids, **kwargs)
 
-        kwargs["url"] = _url + _endpoint
-        try:
-            ret = fct(**kwargs)
-        except requests.exceptions.ConnectionError as e:
-            raise NewConnectionError(e)
-        except requests.exceptions.Timeout as e:
-            raise ConnectionTimeOutError(e)
-        except TLSPinningError as e:
-            raise TLSPinningError(e)
-        except (Exception, requests.exceptions.BaseHTTPError) as e:
-            raise UnknownConnectionError(e)
-
-        return ret
-
-    def _is_api_reacheable(self):
-        try:
-            self.api_request("/tests/ping", _skip_alt_routing_for_api_check=True)
-        except (NewConnectionError, ConnectionTimeOutError, TLSPinningError) as e:
-            self._logger.exception(e)
-            return False
+    def tweets(self, user_ids: list[int], **kwargs) -> list[dict]:
+        return self._run(Operation.UserTweets, user_ids, **kwargs)
 
-        return True
+    def tweets_and_replies(self, user_ids: list[int], **kwargs) -> list[dict]:
+        return self._run(Operation.UserTweetsAndReplies, user_ids, **kwargs)
 
-    def verify_modulus(self, armored_modulus):
-        # gpg.decrypt verifies the signature too, and returns the parsed data.
-        # By using gpg.verify the data is not returned
-        verified = self.__gnupg.decrypt(armored_modulus)
+    def media(self, user_ids: list[int], **kwargs) -> list[dict]:
+        return self._run(Operation.UserMedia, user_ids, **kwargs)
 
-        if not (verified.valid and verified.fingerprint.lower() == SRP_MODULUS_KEY_FINGERPRINT):
-            raise ValueError("Invalid modulus")
+    def likes(self, user_ids: list[int], **kwargs) -> list[dict]:
+        return self._run(Operation.Likes, user_ids, **kwargs)
 
-        return base64.b64decode(verified.data.strip())
+    def followers(self, user_ids: list[int], **kwargs) -> list[dict]:
+        return self._run(Operation.Followers, user_ids, **kwargs)
 
-    def authenticate(self, username, password):
-        """Authenticate user against API.
+    def following(self, user_ids: list[int], **kwargs) -> list[dict]:
+        return self._run(Operation.Following, user_ids, **kwargs)
 
-        Args:
-            username (string): proton account username
-            password (string): proton account password
+    def favoriters(self, tweet_ids: list[int], **kwargs) -> list[dict]:
+        return self._run(Operation.Favoriters, tweet_ids, **kwargs)
 
-        Returns:
-            dict
+    def retweeters(self, tweet_ids: list[int], **kwargs) -> list[dict]:
+        return self._run(Operation.Retweeters, tweet_ids, **kwargs)
 
-        The returning dict contains the Scope of the account. This allows
-        to identify if the account is locked, has unpaid invoices, etc.
+    def profile_spotlights(self, screen_names: list[str], **kwargs) -> list[dict]:
         """
-        self.logout()
-
-        payload = {"Username": username}
-        if self.__clientsecret:
-            payload["ClientSecret"] = self.__clientsecret
-
-        info_response = self.api_request("/auth/info", payload)
-
-        modulus = self.verify_modulus(info_response["Modulus"])
-        server_challenge = base64.b64decode(info_response["ServerEphemeral"])
-        salt = base64.b64decode(info_response["Salt"])
-        version = info_response["Version"]
-
-        usr = PmsrpUser(password, modulus)
-        client_challenge = usr.get_challenge()
-        client_proof = usr.process_challenge(salt, server_challenge, version)
-
-        if client_proof is None:
-            raise ValueError("Invalid challenge")
-
-        # Send response
-        payload = {
-            "Username": username,
-            "ClientEphemeral": base64.b64encode(client_challenge).decode(
-                "utf8"
-            ),
-            "ClientProof": base64.b64encode(client_proof).decode("utf8"),
-            "SRPSession": info_response["SRPSession"],
-        }
-        if self.__clientsecret:
-            payload["ClientSecret"] = self.__clientsecret
-
-        auth_response = self.api_request("/auth", payload)
-
-        if "ServerProof" not in auth_response:
-            raise ValueError("Invalid password")
-
-        usr.verify_session(base64.b64decode(auth_response["ServerProof"]))
-        if not usr.authenticated():
-            raise ValueError("Invalid server proof")
-
-        self._session_data = {
-            "UID": auth_response["UID"],
-            "AccessToken": auth_response["AccessToken"],
-            "RefreshToken": auth_response["RefreshToken"],
-            "PasswordMode": auth_response["PasswordMode"],
-            "Scope": auth_response["Scope"].split(),
-        }
-
-        if self.UID is not None:
-            self.s.headers["x-pm-uid"] = self.UID
-            self.s.headers["Authorization"] = "Bearer " + self.AccessToken
-
-        return self.Scope
-
-    def provide_2fa(self, code):
-        """Provide Two Factor Authentication Code to the API.
-
-        Args:
-            code (string): string of ints
-
-        Returns:
-            dict
-
-        The returning dict contains the Scope of the account. This allows
-        to identify if the account is locked, has unpaid invoices, etc.
+        This endpoint is included for completeness only. It returns very few data points.
+        Use the batched query `users_by_ids` instead if you wish to pull user profile data.
         """
-        ret = self.api_request("/auth/2fa", {"TwoFactorCode": code})
-        self._session_data["Scope"] = ret["Scope"]
+        return self._run(Operation.ProfileSpotlightsQuery, screen_names, **kwargs)
 
-        return self.Scope
-
-    def logout(self):
-        """Logout from API."""
-        if self._session_data:
-            self.api_request("/auth", method="DELETE")
-            del self.s.headers["Authorization"]
-            del self.s.headers["x-pm-uid"]
-            self._session_data = {}
-
-    def refresh(self):
-        """Refresh tokens.
-
-        Refresh AccessToken with a valid RefreshToken.
-        If the RefreshToken is invalid then the user will have to
-        re-authenticate.
+    def users_by_id(self, user_ids: list[int], **kwargs) -> list[dict]:
         """
-        refresh_response = self.api_request(
-            "/auth/refresh",
-            {
-                "ResponseType": "token",
-                "GrantType": "refresh_token",
-                "RefreshToken": self.RefreshToken,
-                "RedirectURI": "http://protonmail.ch"
-            }
-        )
-        self._session_data["AccessToken"] = refresh_response["AccessToken"]
-        self._session_data["RefreshToken"] = refresh_response["RefreshToken"]
-        self.s.headers["Authorization"] = "Bearer " + self.AccessToken
-
-    def get_alternative_routes_from_dns(self, callback=None):
-        """Get alternative routes to circumvent firewalls and API restrictions.
-
-        Args:
-            callback (func): a callback method to be called.
-                Might be usefull for multi-threading. [OPTIONAL]
-
-        This method leverages the power of ThreadPoolExecutor to async
-        check if the provided dns hosts can be reached, and if so, collect the
-        alternatives routes provided by them.
-        The encoded url are done sync because most often one of the two should work,
-        as it should provide the data as quick as possible.
-
-        If callback is passed then the method does not return any value, otherwise it
-        returns a set().
+        This endpoint is included for completeness only.
+        Use the batched query `users_by_ids` instead if you wish to pull user profile data.
         """
+        return self._run(Operation.UserByRestId, user_ids, **kwargs)
 
-        try:
-            from dns import message
-            from dns.rdatatype import TXT
-        except ImportError as e:
-            self._logger.exception(e)
-            raise MissingDepedencyError(
-                "Could not find dnspython package. "
-                "Please either install the missing package or disable "
-                "alternative routing."
-            )
+    def tweet_stats(self, user_ids: list[int], **kwargs) -> list[dict]:
+        return self._run(Operation.TweetStats, user_ids, **kwargs)
 
-        routes = set()
+    def users_by_rest_ids(self, user_ids: list[int], **kwargs) -> list[dict]:
+        return self._run(Operation.UsersByRestIds, batch_ids(user_ids), **kwargs)
 
-        for encoded_url in ENCODED_URLS:
-            dns_query, dns_encoded_data = self.__generate_dns_message(encoded_url)
-            dns_hosts_response = []
+    def recommended_users(self, user_ids: list[int] = None, **kwargs) -> dict:
+        if user_ids:
+            contexts = [{"context": orjson.dumps({"contextualUserId": x}).decode()} for x in user_ids]
+        else:
+            contexts = [{'context': None}]
+        return self._run(Operation.ConnectTabTimeline, contexts, **kwargs)
 
-            host_and_dns = [(host, dns_encoded_data) for host in DNS_HOSTS]
+    def download_media(self, ids: list[int], photos: bool = True, videos: bool = True) -> None:
+        tweets = self.tweets_by_id(ids)
+        urls = []
+        for tweet in tweets:
+            tweet_ids = find_key(tweet, 'id_str')
+            tweet_id = tweet_ids[0]
+            url = f'https://twitter.com/i/status/{tweet_id}'  # `i` evaluates to screen_name
+            media = [y for x in find_key(tweet, 'media') for y in x]
+            if photos:
+                photo_urls = list({u for m in media if 'ext_tw_video_thumb' not in (u := m['media_url_https'])})
+                [urls.append([url, photo]) for photo in photo_urls]
+            if videos:
+                video_urls = [x['variants'] for m in media if (x := m.get('video_info'))]
+                hq_videos = {sorted(v, key=lambda d: d.get('bitrate', 0))[-1]['url'] for v in video_urls}
+                [urls.append([url, video]) for video in hq_videos]
+
+        with tqdm(total=len(urls), desc='downloading media') as pbar:
+            with ThreadPoolExecutor(max_workers=32) as e:
+                for future in as_completed(e.submit(self._download, x, y) for x, y in urls):
+                    future.result()
+                    pbar.update()
+
+    def _download(self, post_url: str, cdn_url: str, path: str = 'media', chunk_size: int = 4096) -> None:
+        (self.out_path / 'media').mkdir(parents=True, exist_ok=True)
+        name = urlsplit(post_url).path.replace('/', '_')[1:]
+        ext = urlsplit(cdn_url).path.split('/')[-1]
+        try:
+            with httpx.stream('GET', cdn_url, headers=self.session.headers, cookies=self.session.cookies) as r:
+                with open(f'{path}/{name}_{ext}', 'wb') as f:
+                    for chunk in r.iter_bytes(chunk_size=chunk_size):
+                        f.write(chunk)
+        except Exception as e:
+            self.logger.error(f'[{RED}error{RESET}] Failed to download media: {post_url} {e}')
 
-            with ThreadPoolExecutor(max_workers=len(DNS_HOSTS)) as executor:
-                dns_hosts_response = list(
-                    executor.map(self.__query_for_dns_data, host_and_dns, timeout=20)
-                )
-                dns_hosts_response = [dns_url for dns_url in dns_hosts_response if dns_url]
+    def trends(self) -> dict:
+        """Get trends for all UTC offsets"""
 
-            if len(dns_hosts_response) == 0:
-                continue
+        def get_trends(offset: str, url: str, headers: dict):
+            try:
+                headers['x-twitter-utcoffset'] = offset
+                r = self.session.get(url, headers=headers)
+                trends = find_key(r.json(), 'item')
+                return {t['content']['trend']['name']: t for t in trends}
+            except Exception as e:
+                self.logger.error('Failed to get trends', e)
+
+        headers = get_headers(self.session)
+        url = set_qs('https://twitter.com/i/api/2/guide.json', trending_params)
+        offsets = [f"{str(i).zfill(3)}00" if i < 0 else f"+{str(i).zfill(2)}00" for i in range(-12, 15)]
+        trends = {}
+        with tqdm(total=len(offsets), desc='downloading trends') as pbar:
+            with ThreadPoolExecutor(max_workers=32) as e:
+                for future in as_completed(e.submit(get_trends, o, url, headers) for o in offsets):
+                    trends |= future.result()
+                    pbar.update()
+
+        path = self.out_path / 'raw/trends'
+        path.mkdir(parents=True, exist_ok=True)
+        (path / f'{time.time_ns()}.json').write_text(
+            orjson.dumps(trends, option=orjson.OPT_INDENT_2).decode(),
+            encoding='utf-8'
+        )
+        return trends
 
-            for response in dns_hosts_response:
-                routes = self.__extract_dns_answer(response, dns_query)
+    def spaces(self, *, rooms: list[str] = None, search: list[dict] = None, audio: bool = False, chat: bool = False,
+               **kwargs) -> list[dict]:
+        if rooms:
+            spaces = self._run(Operation.AudioSpaceById, rooms, **kwargs)
+        else:
+            res = self._run(Operation.AudioSpaceSearch, search, **kwargs)
+            search_results = set(find_key(res, 'rest_id'))
+            spaces = self._run(Operation.AudioSpaceById, search_results, **kwargs)
+        if audio or chat:
+            return self._get_space_data(spaces, audio, chat)
+        return spaces
+
+    def _get_space_data(self, spaces: list[dict], audio=True, chat=True):
+        streams = self._check_streams(spaces)
+        chat_data = None
+        if chat:
+            temp = []  # get necessary keys instead of passing large dicts
+            for stream in filter(lambda x: x['stream'], streams):
+                meta = stream['space']['data']['audioSpace']['metadata']
+                if meta['state'] not in {SpaceState.Running, SpaceState.NotStarted}:
+                    temp.append({
+                        'rest_id': meta['rest_id'],
+                        'chat_token': stream['stream']['chatToken'],
+                        'media_key': meta['media_key'],
+                        'state': meta['state'],
+                    })
+            chat_data = self._get_chat_data(temp)
+        if audio:
+            temp = []
+            for stream in streams:
+                if stream.get('stream'):
+                    chunks = self._get_chunks(stream['stream']['source']['location'])
+                    temp.append({
+                        'rest_id': stream['space']['data']['audioSpace']['metadata']['rest_id'],
+                        'chunks': chunks,
+                    })
+            self._download_audio(temp)
+        return chat_data
+
+    async def _get_stream(self, client: AsyncClient, media_key: str) -> dict | None:
+        params = {
+            'client': 'web',
+            'use_syndication_guest_id': 'false',
+            'cookie_set_host': 'twitter.com',
+        }
+        url = f'https://twitter.com/i/api/1.1/live_video_stream/status/{media_key}'
+        try:
+            r = await client.get(url, params=params)
+            return r.json()
+        except Exception as e:
+            self.logger.error(f'stream not available for playback\n{e}')
+
+    async def _init_chat(self, client: AsyncClient, chat_token: str) -> dict:
+        payload = {'chat_token': chat_token}  # stream['chatToken']
+        url = 'https://proxsee.pscp.tv/api/v2/accessChatPublic'
+        r = await client.post(url, json=payload)
+        return r.json()
 
-            if len(routes) > 0:
+    async def _get_chat(self, client: AsyncClient, endpoint: str, access_token: str, cursor: str = '') -> list[dict]:
+        payload = {
+            'access_token': access_token,
+            'cursor': cursor,
+            'limit': 1000,  # or 0
+            'since': None,
+            'quick_get': True,
+        }
+        url = f"{endpoint}/chatapi/v1/history"
+        r = await client.post(url, json=payload)
+        data = r.json()
+        res = [data]
+        while cursor := data.get('cursor'):
+            try:
+                r = await client.post(url, json=payload | {'cursor': cursor})
+                if r.status_code == 503:
+                    # not our fault, service error, something went wrong with the stream
+                    break
+                data = r.json()
+                res.append(data)
+            except ReadTimeout as e:
+                self.logger.debug(f'End of chat data\n{e}')
                 break
 
-        if not callback:
-            return routes
-
-        callback(routes)
+        parsed = []
+        for r in res:
+            messages = r.get('messages', [])
+            for msg in messages:
+                try:
+                    msg['payload'] = orjson.loads(msg.get('payload', '{}'))
+                    msg['payload']['body'] = orjson.loads(msg['payload'].get('body'))
+                except Exception as e:
+                    self.logger.error(f'Failed to parse chat message\n{e}')
+            parsed.extend(messages)
+        return parsed
 
-    def __generate_dns_message(self, encoded_url):
-        """Generate DNS message object.
-
-        Args:
-            encoded_url (string): encoded url as per documentation
-
-        Returns:
-            tuple():
-                dns_query (dns.message.Message): output of dns.message.make_query
-                base64_dns_message (base64): encode bytes
-        """
-        from dns import message
-        from dns.rdatatype import TXT
-
-        dns_query = message.make_query(encoded_url, TXT)
-        dns_wire = dns_query.to_wire()
-        base64_dns_message = base64.urlsafe_b64encode(dns_wire).rstrip(b"=")
-
-        return dns_query, base64_dns_message
-
-    def __query_for_dns_data(self, dns_settings):
-        """Query DNS host for data.
-
-        Args:
-            dns_settings (tuple):
-                host_url (str): http/https url
-                dns_encoded_data (str): base64 output
-                generate by __generate_dns_message()
-
-        This method uses requests.get to query the url
-        for dns data.
-
-        Returns:
-            bytes: content of the response
-        """
-        dns_host, dns_encoded_data = dns_settings[0], dns_settings[1]
+    def _get_chunks(self, location: str) -> list[str]:
         try:
-            response = requests.get(
-                dns_host,
-                headers={"accept": "application/dns-message"},
-                timeout=(3.05, 16.95),
-                params={"dns": dns_encoded_data}
+            url = URL(location)
+            stream_type = url.params.get('type')
+            r = self.session.get(
+                url=location,
+                params={'type': stream_type},
+                headers={'authority': url.host}
             )
+            # don't need an m3u8 parser
+            chunks = re.findall('\n(chunk_.*)\n', r.text, flags=re.I)
+            url = '/'.join(location.split('/')[:-1])
+            return [f'{url}/{chunk}' for chunk in chunks]
+        except Exception as e:
+            self.logger.error(f'Failed to get chunks\n{e}')
+
+    def _get_chat_data(self, keys: list[dict]) -> list[dict]:
+        async def get(c: AsyncClient, key: dict) -> dict:
+            info = await self._init_chat(c, key['chat_token'])
+            chat = await self._get_chat(c, info['endpoint'], info['access_token'])
+            if self.save:
+                (self.out_path / 'raw' / f"chat_{key['rest_id']}.json").write_bytes(orjson.dumps(chat))
+            return {
+                'space': key['rest_id'],
+                'chat': chat,
+                'info': info,
+            }
 
-            if response.status_code == 404:
-                return
-        except Exception as e: # noqa
-            return
-
-        return response.content
-
-    def __extract_dns_answer(self, query_content, dns_query):
-        """Extract alternative URL from dns message.
-
-        Args:
-            query_content (bytes): content of the response
-            dns_query (dns.message.Message): output of dns.message.make_query
-
-        Returns:
-            set(): alternative routes for API
-        """
-        from dns import message
-        r = message.from_wire(
-            query_content,
-            keyring=dns_query.keyring,
-            request_mac=dns_query.request_mac,
-            one_rr_per_rrset=False,
-            ignore_trailing=False
-        )
-        routes = set()
-        for route in r.answer:
-            routes = set([str(url).strip("\"") for url in route])
-
-        return routes
-
-    @property
-    def captcha_url(self):
-        return "{}/core/v4/captcha?Token={}".format(
-            self.__api_url, self.__captcha_token
-        )
-
-    @property
-    def enable_alternative_routing(self):
-        """Alternative routing getter."""
-        return self.__allow_alternative_routing
-
-    @enable_alternative_routing.setter
-    def enable_alternative_routing(self, newvalue):
-        """Alternative routing setter.
-
-        If you would like to enable/disable alternative routing
-        before making any requests, this should be set to the desired
-        value.
-
-        Args:
-            newvalue (bool)
-        """
-        if self.__allow_alternative_routing != bool(newvalue):
-            self.__allow_alternative_routing = bool(newvalue)
-
-    @property
-    def force_skip_alternative_routing(self):
-        """Force skip alternative routing getter."""
-        return self.__force_skip_alternative_routing
-
-    @force_skip_alternative_routing.setter
-    def force_skip_alternative_routing(self, newvalue):
-        """Force skip alternative routing setter.
-
-        Alternative routing is normally used when the usual API is not
-        reacheable. In certain cases, such as when connected to the VPN,
-        the usual API should be reacheable as the connection is tunneled,
-        thus there is not need to reach for the alternative routes and the
-        usual API is preffered to be used, for security and reliability.
-
-        Args:
-            newvalue (bool)
-        """
-        self.__force_skip_alternative_routing = bool(newvalue)
+        async def process():
+            limits = Limits(max_connections=100, max_keepalive_connections=10)
+            headers = self.session.headers if self.guest else get_headers(self.session)
+            cookies = self.session.cookies
+            async with AsyncClient(limits=limits, headers=headers, cookies=cookies, timeout=20) as c:
+                return await tqdm_asyncio.gather(*(get(c, key) for key in keys), desc='downloading chat')
+
+        return asyncio.run(process())
+
+    def _download_audio(self, data: list[dict]) -> None:
+        async def get(s: AsyncClient, chunk: str, rest_id: str) -> tuple:
+            r = await s.get(chunk)
+            return rest_id, r
+
+        async def process(data: list[dict]) -> list:
+            limits = Limits(max_connections=100, max_keepalive_connections=10)
+            headers = self.session.headers if self.guest else get_headers(self.session)
+            cookies = self.session.cookies
+            async with AsyncClient(limits=limits, headers=headers, cookies=cookies, timeout=20) as c:
+                tasks = []
+                for d in data:
+                    tasks.extend([get(c, chunk, d['rest_id']) for chunk in d['chunks']])
+                return await tqdm_asyncio.gather(*tasks, desc='downloading audio')
+
+        chunks = asyncio.run(process(data))
+        streams = {}
+        [streams.setdefault(_id, []).append(chunk) for _id, chunk in chunks]
+        # ensure chunks are in correct order
+        for k, v in streams.items():
+            streams[k] = sorted(v, key=lambda x: int(re.findall('_(\d+)_\w\.aac$', x.url.path)[0]))
+        out = self.out_path / 'audio'
+        out.mkdir(parents=True, exist_ok=True)
+        for space_id, chunks in streams.items():
+            # 1hr ~= 50mb
+            with open(out / f'{space_id}.aac', 'wb') as fp:
+                [fp.write(c.content) for c in chunks]
+
+    def _check_streams(self, keys: list[dict]) -> list[dict]:
+        async def get(c: AsyncClient, space: dict) -> dict:
+            media_key = space['data']['audioSpace']['metadata']['media_key']
+            stream = await self._get_stream(c, media_key)
+            return {'space': space, 'stream': stream}
+
+        async def process():
+            limits = Limits(max_connections=100, max_keepalive_connections=10)
+            headers = self.session.headers if self.guest else get_headers(self.session)
+            cookies = self.session.cookies
+            async with AsyncClient(limits=limits, headers=headers, cookies=cookies, timeout=20) as c:
+                return await asyncio.gather(*(get(c, key) for key in keys))
+
+        return asyncio.run(process())
+
+    def _run(self, operation: tuple[dict, str, str], queries: set | list[int | str | dict], **kwargs):
+        keys, qid, name = operation
+        save = kwargs.pop('save', True)
+        op = kwargs.pop('res', 'json')
+
+        ops = {
+            None: lambda x: x,  # return raw response
+            'json': lambda x: list(filter(None, (get_json(r, name, save, **kwargs) for r in x))),
+            'text': lambda x: [r.text for r in x],
+        }
 
-    @property
-    def human_verification_token(self):
-        return (
-            self.s.headers.get("X-PM-Human-Verification-Token-Type", None),
-            self.s.headers.get("X-PM-Human-Verification-Token", None)
-        )
+        # stay within rate-limits
+        if (l := len(queries)) > 500:
+            self.logger.warning(f'Got {l} queries, truncating to first 500.')
+            queries = list(queries)[:500]
+
+        if all(isinstance(q, dict) for q in queries):
+            return ops[op](asyncio.run(self._process(operation, list(queries), **kwargs)))
+
+        # queries are of type set | list[int|str], need to convert to list[dict]
+        _queries = [{k: q} for q in queries for k, v in keys.items()]
+        res = ops[op](asyncio.run(self._process(operation, _queries, **kwargs)))
+        return res.pop() if kwargs.get('cursor') else flatten(res)
+
+    async def _query(self, c: AsyncClient, operation: tuple, **kwargs) -> Response:
+        keys, qid, name = operation
+        params = {
+            'variables': Operation.default_variables | keys | kwargs,
+            'features': Operation.default_features,
+        }
+        url = f'https://twitter.com/i/api/graphql/{qid}/{name}'
+        r = await c.get(url, params=build_params(params))
+        if self.debug:
+            log(self.logger, self.debug, r)
+        if self.save:
+            save_json(r, self.out_path, name, **kwargs)
+        return r
+
+    async def _process(self, operation: tuple, queries: list[dict], **kwargs):
+        limits = Limits(max_connections=100, max_keepalive_connections=10)
+        headers = self.session.headers if self.guest else get_headers(self.session)
+        cookies = self.session.cookies
+        async with AsyncClient(limits=limits, headers=headers, cookies=cookies, timeout=20) as c:
+            return await tqdm_asyncio.gather(
+                *(self._paginate(c, operation, **q, **kwargs) for q in queries),
+                desc=operation[-1],
+            )
 
-    @human_verification_token.setter
-    def human_verification_token(self, newtuplevalue):
-        """Set human verification token:
+    async def _paginate(self, client: AsyncClient, operation: tuple, **kwargs):
+        limit = kwargs.pop('limit', math.inf)
+        cursor = kwargs.pop('cursor', None)
+        is_resuming = False
+        dups = 0
+        DUP_LIMIT = 3
+        if cursor:
+            is_resuming = True
+            res = []
+            ids = set()
+        else:
+            try:
+                r = await self._query(client, operation, **kwargs)
+                initial_data = r.json()
+                res = [r]
+                ids = set(find_key(initial_data, 'rest_id'))
+                cursor = get_cursor(initial_data)
+            except Exception as e:
+                self.logger.error('Failed to get initial pagination data', e)
+                return
+        while (dups < DUP_LIMIT) and cursor:
+            prev_len = len(ids)
+            if prev_len >= limit:
+                break
+            try:
+                r = await self._query(client, operation, cursor=cursor, **kwargs)
+                data = r.json()
+            except Exception as e:
+                self.logger.error('Failed to get pagination data', e)
+                return
+            cursor = get_cursor(data)
+            ids |= set(find_key(data, 'rest_id'))
+            if self.debug:
+                self.logger.debug(f'cursor: {cursor}\tunique results: {len(ids)}')
+            if prev_len == len(ids):
+                dups += 1
+            res.append(r)
+        if is_resuming:
+            return res, cursor
+        return res
+
+    async def _space_listener(self, chat: dict, frequency: int):
+        rand_color = lambda: random.choice([RED, GREEN, RESET, BLUE, CYAN, MAGENTA, YELLOW])
+        uri = f"wss://{URL(chat['endpoint']).host}/chatapi/v1/chatnow"
+        with open('chatlog.jsonl', 'ab') as fp:
+            async with websockets.connect(uri) as ws:
+                await ws.send(orjson.dumps({
+                    "payload": orjson.dumps({"access_token": chat['access_token']}).decode(),
+                    "kind": 3
+                }).decode())
+                await ws.send(orjson.dumps({
+                    "payload": orjson.dumps({
+                        "body": orjson.dumps({
+                            "room": chat['room_id']
+                        }).decode(),
+                        "kind": 1
+                    }).decode(),
+                    "kind": 2
+                }).decode())
+
+                prev_message = ''
+                prev_user = ''
+                while True:
+                    msg = await ws.recv()
+                    temp = orjson.loads(msg)
+                    kind = temp.get('kind')
+                    if kind == 1:
+                        signature = temp.get('signature')
+                        payload = orjson.loads(temp.get('payload'))
+                        payload['body'] = orjson.loads(payload.get('body'))
+                        res = {
+                            'kind': kind,
+                            'payload': payload,
+                            'signature': signature,
+                        }
+                        fp.write(orjson.dumps(res) + b'\n')
+                        body = payload['body']
+                        message = body.get('body')
+                        user = body.get('username')
+                        # user_id = body.get('user_id')
+                        final = body.get('final')
+
+                        if frequency == 1:
+                            if final:
+                                if user != prev_user:
+                                    print()
+                                    print(f"({rand_color()}{user}{RESET})")
+                                    prev_user = user
+                                # print(message, end=' ')
+                                print(message)
+
+                        # dirty
+                        if frequency == 2:
+                            if user and (not final):
+                                if user != prev_user:
+                                    print()
+                                    print(f"({rand_color()}{user}{RESET})")
+                                    prev_user = user
+                                new_message = re.sub(f'^({prev_message})', '', message, flags=re.I).strip()
+                                if len(new_message) < 100:
+                                    print(new_message, end=' ')
+                                    prev_message = message
+
+    async def _get_live_chats(self, client: Client, spaces: list[dict]):
+        async def get(c: AsyncClient, space: dict) -> list[dict]:
+            media_key = space['data']['audioSpace']['metadata']['media_key']
+            r = await c.get(
+                url=f'https://twitter.com/i/api/1.1/live_video_stream/status/{media_key}',
+                params={
+                    'client': 'web',
+                    'use_syndication_guest_id': 'false',
+                    'cookie_set_host': 'twitter.com',
+                })
+            r = await c.post(
+                url='https://proxsee.pscp.tv/api/v2/accessChatPublic',
+                json={'chat_token': r.json()['chatToken']}
+            )
+            return r.json()
 
-        Args:
-            newtuplevalue (tuple): (token_type, token_value)
-        """
-        self.s.headers["X-PM-Human-Verification-Token-Type"] = newtuplevalue[0]
-        self.s.headers["X-PM-Human-Verification-Token"] = newtuplevalue[1]
+        limits = Limits(max_connections=100)
+        async with AsyncClient(headers=client.headers, limits=limits, timeout=30) as c:
+            return await tqdm_asyncio.gather(*(get(c, _id) for _id in spaces), desc='getting live transcripts')
+
+    def space_live_transcript(self, room: str, frequency: int = 1):
+        async def get(spaces: list[dict]):
+            client = init_session()
+            chats = await self._get_live_chats(client, spaces)
+            await asyncio.gather(*(self._space_listener(c, frequency) for c in chats))
+
+        spaces = self.spaces(rooms=[room])
+        asyncio.run(get(spaces))
+
+    def spaces_live(self, rooms: list[str]):
+        chunk_idx = lambda chunk: re.findall('_(\d+)_\w\.aac', chunk)[0]
+        sort_chunks = lambda chunks: sorted(chunks, key=lambda x: int(chunk_idx(x)))
+        parse_chunks = lambda txt: re.findall('\n(chunk_.*)\n', txt, flags=re.I)
 
-    @human_verification_token.deleter
-    def human_verification_token(self):
-        # Safest to use .pop() as it will onyl attempt to remove the key by name
-        # while del can also remove the whole dict (in case of code/programming error)
-        # Thus to prevent this, pop() is used.
+        async def get_m3u8(client: AsyncClient, space: dict) -> dict:
+            try:
+                media_key = space['data']['audioSpace']['metadata']['media_key']
+                r = await client.get(
+                    url=f'https://twitter.com/i/api/1.1/live_video_stream/status/{media_key}',
+                    params={'client': 'web', 'use_syndication_guest_id': 'false', 'cookie_set_host': 'twitter.com'}
+                )
+                data = r.json()
+                room = data['shareUrl'].split('/')[-1]
+                return {"url": data['source']['location'], "room": room}
+            except Exception as e:
+                room = space['data']['audioSpace']['metadata']['rest_id']
+                self.logger.error(f'Failed to get stream info for https://twitter.com/i/spaces/{room}\n{e}')
 
-        try:
-            self.s.headers.pop("X-PM-Human-Verification-Token-Type")
-        except (KeyError, IndexError):
-            pass
+        async def get_chunks(client: AsyncClient, url: str) -> list[str]:
+            try:
+                url = URL(url)
+                r = await client.get(
+                    url=url,
+                    params={'type': url.params.get('type')},
+                    headers={'authority': url.host}
+                )
+                base = '/'.join(str(url).split('/')[:-1])
+                return [f'{base}/{c}' for c in parse_chunks(r.text)]
+            except Exception as e:
+                self.logger.error(f'Failed to get chunks\n{e}')
+
+        async def poll_space(client: AsyncClient, space: dict) -> dict | None:
+            curr = 0
+            lim = 10
+            all_chunks = set()
+            playlist = await get_m3u8(client, space)
+            if not playlist: return
+            chunks = await get_chunks(client, playlist['url'])
+            if not chunks: return
+            out = self.out_path / 'live'
+            out.mkdir(parents=True, exist_ok=True)
+            async with aiofiles.open(out / f'{playlist["room"]}.aac', 'wb') as fp:
+                while curr < lim:
+                    chunks = await get_chunks(client, playlist['url'])
+                    if not chunks:
+                        return {'space': space, 'chunks': sort_chunks(all_chunks)}
+                    new_chunks = set(chunks) - all_chunks
+                    all_chunks |= new_chunks
+                    for c in sort_chunks(new_chunks):
+                        try:
+                            self.logger.debug(f"write: chunk [{chunk_idx(c)}]\t{c}")
+                            r = await client.get(c)
+                            await fp.write(r.content)
+                        except Exception as e:
+                            self.logger.error(f'Failed to write chunk {c}\n{e}')
+                    curr = 0 if new_chunks else curr + 1
+                    # wait for new chunks. dynamic playlist is updated every 2-3 seconds
+                    await asyncio.sleep(random.random() + 1.5)
+            return {'space': space, 'chunks': sort_chunks(all_chunks)}
+
+        async def process(spaces: list[dict]):
+            limits = Limits(max_connections=100)
+            headers, cookies = self.session.headers, self.session.cookies
+            async with AsyncClient(limits=limits, headers=headers, cookies=cookies, timeout=20) as c:
+                return await asyncio.gather(*(poll_space(c, space) for space in spaces))
 
-        try:
-            self.s.headers.pop("X-PM-Human-Verification-Token")
-        except (KeyError, IndexError):
-            pass
-
-    @property
-    def UID(self):
-        return self._session_data.get("UID", None)
-
-    @property
-    def AccessToken(self):
-        return self._session_data.get("AccessToken", None)
-
-    @property
-    def RefreshToken(self):
-        return self._session_data.get("RefreshToken", None)
-
-    @property
-    def PasswordMode(self):
-        return self._session_data.get("PasswordMode", None)
-
-    @property
-    def Scope(self):
-        return self._session_data.get("Scope", [])
+        spaces = self.spaces(rooms=rooms)
+        return asyncio.run(process(spaces))
```

### Comparing `twitter-api-client-0.8.4/setup.py` & `twitter-api-client-0.8.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,24 +5,20 @@
 install_requires = [
     "aiofiles",
     "websockets",
     "nest_asyncio",
     "httpx",
     "tqdm",
     "orjson",
-    "bcrypt",
-    "python-gnupg",
-    "pyopenssl",
-    "requests",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.8.4",
+    version="0.8.5",
     python_requires=">=3.10.10",
     description="Twitter API",
     long_description=dedent('''
     
     ## Implementation of Twitter's v1, v2, and GraphQL APIs
 
     Tools include: [Scraping](#scraping), [Account Automation](#automation), [Search](#search)
@@ -362,14 +358,17 @@
             'filter': SpaceCategory.Live,
             'query': 'foo bar'
         }
     ])
     ```
     
     ### Automated Solvers
+    
+    > **Currently removed** due to issues running on Mac. Code has been commented out for now. Cloning the repo, adding the proton mail package, and uncommenting the code referencing `protonmail` can be used as a temporary workaround to re-enable this feature.
+    
     To set up automated email confirmation/verification solvers, add your Proton Mail credentials below as shown.
     This removes the need to manually solve email challenges via the web app. These credentials can be used in `Scraper`, `Account`, and `Search` constructors.
     
     E.g.
     
     ```python
     from twitter.scraper import Scraper
```

### Comparing `twitter-api-client-0.8.4/twitter/account.py` & `twitter-api-client-0.8.5/twitter/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,40 @@
 import hashlib
 import logging.config
 import math
 import mimetypes
+import platform
 import random
 from copy import deepcopy
 from datetime import datetime
 from string import ascii_letters
 from uuid import uuid1, getnode
 
 from tqdm import tqdm
 
 from .constants import *
 from .login import login
 from .util import *
 
+try:
+    if get_ipython().__class__.__name__ == 'ZMQInteractiveShell':
+        import nest_asyncio
+
+        nest_asyncio.apply()
+except:
+    ...
+
+if platform.system() != 'Windows':
+    try:
+        import uvloop
+
+        uvloop.install()
+    except ImportError as e:
+        ...
+
 
 class Account:
 
     def __init__(self, email: str = None, username: str = None, password: str = None, session: Client = None, **kwargs):
         self.logger = self.init_logger(kwargs.get('log_config', False))
         self.session = self.validate_session(email, username, password, session, **kwargs)
         self.gql_url = 'https://twitter.com/i/api/graphql'
```

### Comparing `twitter-api-client-0.8.4/twitter/constants.py` & `twitter-api-client-0.8.5/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.4/twitter/login.py` & `twitter-api-client-0.8.5/twitter/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import time
 
 from httpx import Client
 from .constants import GREEN, YELLOW, RED, BOLD, RESET
-from .util import find_key, get_confirmation_code, get_inbox, init_protonmail_session
+from .util import find_key  # ,get_confirmation_code, get_inbox, init_protonmail_session
 
 
 def update_token(client: Client, key: str, url: str, **kwargs) -> Client:
     caller_name = sys._getframe(1).f_code.co_name
     try:
         headers = {
             'x-guest-token': client.cookies.get('guest_token', ''),
@@ -105,51 +105,52 @@
                     "text": client.cookies.get('email'),
                     "link": "next_link"
                 }
             }]
     })
 
 
-def solve_confirmation_challenge(client: Client, email: str, password: str) -> Client:
-    proton_session = init_protonmail_session(email, password)
-    inbox = get_inbox(proton_session)
-    confirmation_code = get_confirmation_code(inbox)
-    print(f'{confirmation_code = }')
-    return update_token(client, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', json={
-        "flow_token": client.cookies.get('flow_token'),
-        'subtask_inputs': [
-            {
-                'subtask_id': 'LoginAcid',
-                'enter_text': {
-                    'text': confirmation_code,
-                    'link': 'next_link',
-                },
-            },
-        ],
-    })
+# def solve_confirmation_challenge(client: Client, email: str, password: str) -> Client:
+#     proton_session = init_protonmail_session(email, password)
+#     inbox = get_inbox(proton_session)
+#     confirmation_code = get_confirmation_code(inbox)
+#     print(f'{confirmation_code = }')
+#     return update_token(client, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', json={
+#         "flow_token": client.cookies.get('flow_token'),
+#         'subtask_inputs': [
+#             {
+#                 'subtask_id': 'LoginAcid',
+#                 'enter_text': {
+#                     'text': confirmation_code,
+#                     'link': 'next_link',
+#                 },
+#             },
+#         ],
+#     })
 
 
 def execute_login_flow(client: Client) -> Client | None:
     client = init_guest_token(client)
     for fn in [flow_start, flow_instrumentation, flow_username, flow_password, flow_duplication_check]:
         client = fn(client)
 
     # solve email challenge
     if client.cookies.get('confirm_email') == 'true':
         client = confirm_email(client)
 
-    # solve confirmation challenge (Proton Mail only)
-    if client.cookies.get('confirmation_code') == 'true':
-        if not client.protonmail:
-            print(f'[{RED}warning{RESET}] Please check your email for a confirmation code'
-                  f' and log in again using the web app. If you wish to automatically solve'
-                  f' email confirmation challenges, add a Proton Mail account in your account settings')
-            return
-        time.sleep(10)  # todo: just poll the inbox until it arrives instead of waiting
-        client = solve_confirmation_challenge(client, *client.protonmail.values())
+    # # solve confirmation challenge (Proton Mail only)
+    # if client.cookies.get('confirmation_code') == 'true':
+    #     if not client.protonmail:
+    #         print(f'[{RED}warning{RESET}] Please check your email for a confirmation code'
+    #               f' and log in again using the web app. If you wish to automatically solve'
+    #               f' email confirmation challenges, add a Proton Mail account in your account settings')
+    #         return
+    #     time.sleep(10)  # todo: just poll the inbox until it arrives instead of waiting
+    #     client = solve_confirmation_challenge(client, *client.protonmail.values())
+
     return client
 
 
 def login(email: str, username: str, password: str, **kwargs) -> Client:
     client = Client(
         cookies={
             "email": email,
@@ -161,15 +162,17 @@
         headers={
             'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
             'content-type': 'application/json',
             'user-agent': 'Mozilla/5.0 (Linux; Android 11; Nokia G20) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.88 Mobile Safari/537.36',
             'x-twitter-active-user': 'yes',
             'x-twitter-client-language': 'en',
         })
-    client.protonmail = kwargs.get('protonmail')
+
+    # client.protonmail = kwargs.get('protonmail')
+
     client = execute_login_flow(client)
     if kwargs.get('debug', True):
         if not client or client.cookies.get('flow_errors') == 'true':
             print(f'[{RED}error{RESET}] {BOLD}{username}{RESET} login failed')
         else:
             print(f'[{GREEN}success{RESET}] {BOLD}{username}{RESET} login success')
     return client
```

### Comparing `twitter-api-client-0.8.4/twitter/search.py` & `twitter-api-client-0.8.5/twitter/search.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.4/twitter/util.py` & `twitter-api-client-0.8.5/twitter/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 import time
 from logging import Logger
 from pathlib import Path
 from urllib.parse import urlsplit, urlencode, urlunsplit, parse_qs, quote
 
 import orjson
-import protonmail
+# import protonmail
 from httpx import Response, Client
 
 from .constants import GREEN, MAGENTA, RED, RESET
 
 
 def init_session():
     client = Client(headers={
@@ -146,94 +146,94 @@
             for k in obj:
                 L.extend(helper(obj[k], key, []))
         return L
 
     return helper(obj, key, [])
 
 
-def init_protonmail_session(email: str, password: str) -> protonmail.api.Session:
-    """
-    Create an authenticated Proton Mail session
-
-    @param email: your email. Can also use username
-    @param password: your password
-    @return: Proton Mail Session object
-    """
-    cwd = Path.cwd()
-    log_dir_path = cwd / 'protonmail_log'
-    cache_dir_path = cwd / 'protonmail_cache'
-    try:
-        session = protonmail.api.Session(
-            api_url="https://api.protonmail.ch",
-            log_dir_path=log_dir_path,
-            cache_dir_path=cache_dir_path,
-            user_agent="Ubuntu_20.04",
-            tls_pinning=False,
-        )
-        session.enable_alternative_routing = False
-        session.authenticate(email, password)
-        return session
-    except Exception as e:
-        print('Failed to initialize Proton Mail Session:', e)
-
-
-def get_inbox(session: protonmail.api.Session) -> dict:
-    """
-    Get inbox
-
-    @param session: Proton Mail Session object
-    @return: inbox data
-    """
-    try:
-        return session.api_request(
-            "/api/mail/v4/conversations",
-            method="GET",
-            params={
-                'Page': 0,
-                'PageSize': 50,
-                'Limit': 100,
-                'LabelID': 0,
-                'Sort': 'Time',
-                'Desc': 1,
-            }
-        )
-    except Exception as e:
-        print('Failed to get inbox:', e)
-
-
-def get_verification_code(inbox: dict) -> str:
-    """
-    Get Twitter verification code from inbox.
-
-    Crude implementation. Subject line contains verification code, no need to decrypt message body.
-
-    @param inbox: inbox data
-    @return: Twitter verification code
-    """
-    try:
-        expr = '(\w+) is your Twitter verification code'
-        return list(filter(len, (re.findall(expr, conv['Subject']) for conv in inbox['Conversations'])))[0][0]
-    except Exception as e:
-        print('Failed to get Twitter verification code:', e)
-
-
-def get_confirmation_code(inbox: dict) -> str:
-    """
-    Get Twitter confirmation code from inbox.
-
-    Crude implementation. Subject line contains confirmation code, no need to decrypt message body.
-
-    @param inbox: inbox data
-    @return: Twitter confirmation code
-    """
-    try:
-        expr = 'Your Twitter confirmation code is (\w+)'
-        return list(filter(len, (re.findall(expr, conv['Subject']) for conv in inbox['Conversations'])))[0][0]
-    except Exception as e:
-        print('Failed to get Twitter confirmation code:', e)
+# def init_protonmail_session(email: str, password: str) -> protonmail.api.Session:
+#     """
+#     Create an authenticated Proton Mail session
+#
+#     @param email: your email. Can also use username
+#     @param password: your password
+#     @return: Proton Mail Session object
+#     """
+#     cwd = Path.cwd()
+#     log_dir_path = cwd / 'protonmail_log'
+#     cache_dir_path = cwd / 'protonmail_cache'
+#     try:
+#         session = protonmail.api.Session(
+#             api_url="https://api.protonmail.ch",
+#             log_dir_path=log_dir_path,
+#             cache_dir_path=cache_dir_path,
+#             user_agent="Ubuntu_20.04",
+#             tls_pinning=False,
+#         )
+#         session.enable_alternative_routing = False
+#         session.authenticate(email, password)
+#         return session
+#     except Exception as e:
+#         print('Failed to initialize Proton Mail Session:', e)
+#
+#
+# def get_inbox(session: protonmail.api.Session) -> dict:
+#     """
+#     Get inbox
+#
+#     @param session: Proton Mail Session object
+#     @return: inbox data
+#     """
+#     try:
+#         return session.api_request(
+#             "/api/mail/v4/conversations",
+#             method="GET",
+#             params={
+#                 'Page': 0,
+#                 'PageSize': 50,
+#                 'Limit': 100,
+#                 'LabelID': 0,
+#                 'Sort': 'Time',
+#                 'Desc': 1,
+#             }
+#         )
+#     except Exception as e:
+#         print('Failed to get inbox:', e)
+#
+#
+# def get_verification_code(inbox: dict) -> str:
+#     """
+#     Get Twitter verification code from inbox.
+#
+#     Crude implementation. Subject line contains verification code, no need to decrypt message body.
+#
+#     @param inbox: inbox data
+#     @return: Twitter verification code
+#     """
+#     try:
+#         expr = '(\w+) is your Twitter verification code'
+#         return list(filter(len, (re.findall(expr, conv['Subject']) for conv in inbox['Conversations'])))[0][0]
+#     except Exception as e:
+#         print('Failed to get Twitter verification code:', e)
+#
+#
+# def get_confirmation_code(inbox: dict) -> str:
+#     """
+#     Get Twitter confirmation code from inbox.
+#
+#     Crude implementation. Subject line contains confirmation code, no need to decrypt message body.
+#
+#     @param inbox: inbox data
+#     @return: Twitter confirmation code
+#     """
+#     try:
+#         expr = 'Your Twitter confirmation code is (\w+)'
+#         return list(filter(len, (re.findall(expr, conv['Subject']) for conv in inbox['Conversations'])))[0][0]
+#     except Exception as e:
+#         print('Failed to get Twitter confirmation code:', e)
 
 
 def log(logger: Logger, level: int, r: Response):
     def stat(r, txt, data):
         if level >= 1:
             logger.debug(f'{r.url.path}')
         if level >= 2:
```

### Comparing `twitter-api-client-0.8.4/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.8.5/twitter_api_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.8.4
+Version: 0.8.5
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
@@ -351,14 +351,17 @@
         'filter': SpaceCategory.Live,
         'query': 'foo bar'
     }
 ])
 ```
 
 ### Automated Solvers
+
+> **Currently removed** due to issues running on Mac. Code has been commented out for now. Cloning the repo, adding the proton mail package, and uncommenting the code referencing `protonmail` can be used as a temporary workaround to re-enable this feature.
+
 To set up automated email confirmation/verification solvers, add your Proton Mail credentials below as shown.
 This removes the need to manually solve email challenges via the web app. These credentials can be used in `Scraper`, `Account`, and `Search` constructors.
 
 E.g.
 
 ```python
 from twitter.scraper import Scraper
```

