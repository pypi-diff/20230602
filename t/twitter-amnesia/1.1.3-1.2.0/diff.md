# Comparing `tmp/twitter_amnesia-1.1.3-py3-none-any.whl.zip` & `tmp/twitter_amnesia-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,15 @@
-Zip file size: 19386 bytes, number of entries: 10
--rw-r--r--  2.0 unx       42 b- defN 19-Dec-07 03:09 twitter_amnesia/__init__.py
--rw-r--r--  2.0 unx     4388 b- defN 19-Dec-07 03:09 twitter_amnesia/arg_parsing.py
--rw-r--r--  2.0 unx     4918 b- defN 19-Dec-07 03:09 twitter_amnesia/helpers.py
--rw-r--r--  2.0 unx     3937 b- defN 19-Dec-07 03:09 twitter_amnesia/main.py
--rw-r--r--  2.0 unx    35149 b- defN 19-Dec-07 03:09 twitter_amnesia-1.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     3522 b- defN 19-Dec-07 03:09 twitter_amnesia-1.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 19-Dec-07 03:09 twitter_amnesia-1.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       58 b- defN 19-Dec-07 03:09 twitter_amnesia-1.1.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       21 b- defN 19-Dec-07 03:09 twitter_amnesia-1.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      862 b- defN 19-Dec-07 03:09 twitter_amnesia-1.1.3.dist-info/RECORD
-10 files, 52989 bytes uncompressed, 17898 bytes compressed:  66.2%
+Zip file size: 20798 bytes, number of entries: 13
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-02 03:16 twitter_amnesia/__init__.py
+-rw-r--r--  2.0 unx      202 b- defN 23-Jun-02 03:16 twitter_amnesia/__main__.py
+-rw-r--r--  2.0 unx     1448 b- defN 23-Jun-02 03:16 twitter_amnesia/arg_parsing.py
+-rw-r--r--  2.0 unx     2850 b- defN 23-Jun-02 03:16 twitter_amnesia/configuration_parser.py
+-rw-r--r--  2.0 unx     4918 b- defN 23-Jun-02 03:16 twitter_amnesia/helpers.py
+-rw-r--r--  2.0 unx     3738 b- defN 23-Jun-02 03:16 twitter_amnesia/main.py
+-rw-r--r--  2.0 unx      139 b- defN 23-Jun-02 03:16 twitter_amnesia/version.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jun-02 03:16 twitter_amnesia-1.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3128 b- defN 23-Jun-02 03:16 twitter_amnesia-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 03:16 twitter_amnesia-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-02 03:16 twitter_amnesia-1.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-02 03:16 twitter_amnesia-1.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1123 b- defN 23-Jun-02 03:16 twitter_amnesia-1.2.0.dist-info/RECORD
+13 files, 52903 bytes uncompressed, 18898 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -1,31 +1,40 @@
 Filename: twitter_amnesia/__init__.py
 Comment: 
 
+Filename: twitter_amnesia/__main__.py
+Comment: 
+
 Filename: twitter_amnesia/arg_parsing.py
 Comment: 
 
+Filename: twitter_amnesia/configuration_parser.py
+Comment: 
+
 Filename: twitter_amnesia/helpers.py
 Comment: 
 
 Filename: twitter_amnesia/main.py
 Comment: 
 
-Filename: twitter_amnesia-1.1.3.dist-info/LICENSE
+Filename: twitter_amnesia/version.py
+Comment: 
+
+Filename: twitter_amnesia-1.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: twitter_amnesia-1.1.3.dist-info/METADATA
+Filename: twitter_amnesia-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: twitter_amnesia-1.1.3.dist-info/WHEEL
+Filename: twitter_amnesia-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: twitter_amnesia-1.1.3.dist-info/entry_points.txt
+Filename: twitter_amnesia-1.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: twitter_amnesia-1.1.3.dist-info/top_level.txt
+Filename: twitter_amnesia-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: twitter_amnesia-1.1.3.dist-info/RECORD
+Filename: twitter_amnesia-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## twitter_amnesia/__init__.py

 * *Ordering differences only*

```diff
@@ -1,3 +1,3 @@
 __all__ = ["main"]
 
-from .main import main
+from .main import main
```

## twitter_amnesia/arg_parsing.py

```diff
@@ -1,162 +1,59 @@
+"""
+Define the command line arguments and the parser for it.
 
-import argparse
-import re
-import pathlib
-
-consumer_key_re = re.compile(r'([a-zA-Z1-9]+)')
-consumer_secret_re = re.compile(r'([a-zA-Z1-9]+)')
-access_token_key_re = re.compile(r'([0-9]+-[a-zA-Z1-9]+)')
-access_token_secret_re = re.compile(r'([a-zA-Z1-9]+)')
-
-protection_tag_re = re.compile(r'(\[[\w]+\])')
-
-
-def validate_unsigned_int_non_zero(value):
-    if isinstance(value, int) and value > 0:
-        return value
-    else:
-        raise argparse.ArgumentTypeError(
-            f"Invalid alue. Must be int and bigger than 0 (current value {value})"
-        )
-
-
-def validate_consumer_key(token):
-    if consumer_key_re.match(token):
-        return token
-    else:
-        raise argparse.ArgumentTypeError(
-            f"Invalid consumer key token -> {token}"
-        )
-
-
-def validate_consumer_secret(token):
-    if consumer_secret_re.match(token):
-        return token
-    else:
-        raise argparse.ArgumentTypeError(
-            f"Invalid consumer secret token -> {token}"
-        )
-
-
-def validate_access_token_key(token):
-    if access_token_key_re.match(token):
-        return token
-    else:
-        raise argparse.ArgumentTypeError(
-            f"Invalid consumer secret token -> {token}"
-        )
-
-
-def validate_access_token_secret(token):
-    if access_token_secret_re.match(token):
-        return token
-    else:
-        raise argparse.ArgumentTypeError(
-            f"Invalid consumer secret token -> {token}"
-        )
-
-
-def validate_protection_tag(protection_tag):
-    if protection_tag_re.match(protection_tag):
-        return protection_tag
-    else:
-        raise argparse.ArgumentTypeError(
-            f"Invalid protection tag -> {protection_tag} - Can only contain alphabetic or numeric values and have the format [customTag]."
-        )
-
-
-def validate_directory_attribute(directory_location):
-    if type(directory_location) is str:
-        directory_location = pathlib.Path(directory_location)
-        if directory_location.exists():
-            if directory_location.is_dir():
-                return directory_location
-            else:
-                raise argparse.ArgumentTypeError(
-                    "Directory location must point to a directory"
-                )
-        else:
-            raise argparse.ArgumentTypeError(
-                "Directory location must exist."
-            )
-
-    raise argparse.ArgumentTypeError(
-        f"Invalid directory attribute -> {directory_location}. Must be a valid directory location."
-    )
-
+"""
+from argparse import ArgumentParser, ArgumentTypeError,  Namespace
+from pathlib import Path
 
-def parse_arguments():
 
-    parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "-l", "--logLevel",
-        help="Logging Level (default: %(default)s)",
-        type=str,
-        choices=["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"],
-        default="INFO"
-    )
-
-    parser.add_argument(
-        "-d", "--days",
-        help="Tweets older than %(default)d days (default value)",
-        type=validate_unsigned_int_non_zero,
-        default=0
-    )
-
-    parser.add_argument(
-        "-m", "--months",
-        help="Tweets older than %(default)d months (default value)",
-        type=validate_unsigned_int_non_zero,
-        default=1
-    )
+__all__ = [
+    "parse_arguments"
+]
 
-    parser.add_argument(
-        "-y", "--years",
-        help="Tweets older than %(default)d years (default value)",
-        type=validate_unsigned_int_non_zero,
-        default=0
-    )
 
-    parser.add_argument(
-        "-t", "--protection_tag",
-        help="Protection Tag (default: %(default)s)",
-        type=validate_protection_tag,
-        default="[P]"
-    )
+def _validate_config_file_location(file_location):
+    if isinstance(file_location, str):
+        file_location = Path(file_location)
+        if file_location.exists():
+            if file_location.is_file():
+                return file_location
+            else:
+                raise ArgumentTypeError(
+                    "Location must point to a file"
+                )
+        else:
+            raise ArgumentTypeError(
+                "File must exist."
+            )
 
-    parser.add_argument(
-        "-f", "--saving_directory",
-        help="Directory location to where deleted tweets are exported (default: %(default)s)",
-        type=validate_directory_attribute,
-        default=None
+    raise ArgumentTypeError(
+        f"Invalid configuration file location [{file_location}]. Must be a valid file location."
     )
 
-    parser.add_argument(
-        "-ck", "--consumer_key",
-        help="Consumer Key",
-        required=True,
-        type=validate_consumer_key
-    )
+def parse_arguments() -> Namespace:
+    """
+    Return the parsed arguments
+    """
 
-    parser.add_argument(
-        "-cs", "--consumer_secret",
-        help="Consumer Secret",
-        required=True,
-        type=validate_consumer_secret
+    parser = ArgumentParser(
+        prog="twitter_amnesia",
+        description=" Twitter Amnesia Service"
     )
 
     parser.add_argument(
-        "-tk", "--token_key",
-        help="Access Token Key",
+        "-c",
+        "--configuration_file",
+        help="YAML Configuration file to be used.",
+        type=_validate_config_file_location,
         required=True,
-        type=validate_access_token_key
     )
 
     parser.add_argument(
-        "-ts", "--token_secret",
-        help="Access Token Secret",
-        required=True,
-        type=validate_access_token_secret
+        "-l", "--logLevel",
+        help="Logging Level (default: %(default)s)",
+        type=str,
+        choices=["INFO", "WARNING", "ERROR", "CRITICAL"],
+        default="INFO"
     )
 
     return parser.parse_args()
```

## twitter_amnesia/main.py

```diff
@@ -1,105 +1,105 @@
 """
 Twitter Amnesia
 
 A service which can be deployed to erase tweets older than a specific date and not marked with a custom tag
 """
 
-import logging
-import sys
 import datetime
-from datetime import *
+import logging
 import pickle
+import sys
+from datetime import datetime, timezone
 
-import twitter
-from dateutil.relativedelta import *
-from dateutil import parser
+import rfc3339
+from dateutil.relativedelta import relativedelta
+from pytwitter import Api
 
-from twitter_amnesia.helpers import custom_logging_callback, logger_module_name
 from twitter_amnesia.arg_parsing import parse_arguments
+from twitter_amnesia.configuration_parser import load_configurations
+from twitter_amnesia.helpers import custom_logging_callback, logger_module_name
 
 # Initialize Exception Hook
 sys.excepthook = (lambda tp, val, tb: custom_logging_callback(logging.getLogger(), logging.ERROR, tp, val, tb))
 
 
 # Initialize logger for this module
-__log_format = '[{asctime:^s}][{levelname:^8s}]: {message:s}'
-__log_format_debug = '[{asctime:^s}][{levelname:^8s}][{name:s}|{funcName:s}|{lineno:d}]: {message:s}'
-__log_datefmt = '%Y/%m/%d|%H:%M:%S (%Z)'
-__log = logging.getLogger(logger_module_name(__file__))
+_LOG_FORMAT = '[{asctime:^s}][{levelname:^8s}]: {message:s}'
+_LOG_FORMAT_DEBUG = '[{asctime:^s}][{levelname:^8s}][{name:s}|{funcName:s}|{lineno:d}]: {message:s}'
+_LOG_DATE_FORMAT = '%Y/%m/%d|%H:%M:%S (%Z)'
+_log = logging.getLogger(logger_module_name(__file__))
 
 
 def main():
-    try:
-        parsed_args = parse_arguments()
-        if sys.flags.debug:
-            logging.basicConfig(format=__log_format_debug, datefmt=__log_datefmt, style='{', level=logging.DEBUG)
-        else:
-            logging.basicConfig(format=__log_format, datefmt=__log_datefmt, style='{', level=parsed_args.logLevel)
-
-        if sys.flags.debug:
-            __log.debug(
-                ''.join(['CLI arguments: ']+list(
-                                ('  {:s}: {:s}'.format(
-                                    str(key), str(data)
-                                ) for (key, data) in vars(parsed_args).items())
-                            )
-                        )
-            )
-
-        date_until = datetime.now() - relativedelta(
-            days=parsed_args.days,
-            months=parsed_args.months,
-            years=parsed_args.years
+    """
+    The main entry point for this service
+    """
+
+    parsed_args = parse_arguments()
+    if sys.flags.debug:
+        logging.basicConfig(format=_LOG_FORMAT_DEBUG, datefmt=_LOG_DATE_FORMAT, style='{', level=logging.DEBUG)
+    else:
+        logging.basicConfig(format=_LOG_FORMAT, datefmt=_LOG_DATE_FORMAT, style='{', level=parsed_args.logLevel)
+
+    if sys.flags.debug:
+        _log.debug(
+            ''.join(['CLI arguments: ']+list((f'  {key:s}: {data:s}' for (key, data) in vars(parsed_args).items())))
         )
 
-        __log.warning(
-            "Tweets created before {:s} will be deleted.".format(date_until.strftime("%Y-%m-%d"))
-        )
 
-        api = twitter.Api(
-            consumer_key=parsed_args.consumer_key,
-            consumer_secret=parsed_args.consumer_secret,
-            access_token_key=parsed_args.token_key,
-            access_token_secret=parsed_args.token_secret,
-            sleep_on_rate_limit=False
-        )
-        this_user_credentials = api.VerifyCredentials()
-        __log.info(
-            f"Name: {this_user_credentials.name:s}; Screen Name: {this_user_credentials.screen_name:s}"
-        )
-        removed_tweets_counter = 0
-
-        statuses = api.GetUserTimeline(trim_user=True, count=1)
-        if len(statuses):
-            __log.info("Retrieving first status in timeline")
-        while len(statuses):
-            max_id = statuses[-1].id
-            for status in statuses:
-                if parsed_args.protection_tag in status.text[0:len(parsed_args.protection_tag)]:
-                    __log.info(f"Tweet with ID {status.id:d} skipped. Protection tag present.")
-                    continue
-                elif date_until.astimezone() <= parser.parse(status.created_at).astimezone():
-                    __log.info(f"Tweet with ID {status.id:d} skipped. Not old enough to be removed.")
-                    continue
-                else:
-                    if parsed_args.saving_directory:
-                        __log.info(f"Saving tweet with ID {status.id:d}.")
-                        with open(f"{parsed_args.saving_directory}/{status.id:d}", "wb") as file:
-                            pickle.dump(status.AsDict(), file)
-
-                    api.DestroyStatus(status.id)
-                    removed_tweets_counter += 1
-                    __log.warning(f"Tweet {status.id:d} deleted.")
-            statuses = api.GetUserTimeline(trim_user=True, max_id=max_id-1, count=200)
-        __log.info(f"Total number of deleted tweets: {removed_tweets_counter:d}.")
-
-    except Exception:
-        custom_logging_callback(__log, logging.ERROR, *sys.exc_info())
-        exit(-1)
-
-    __log.info("It's done!")
+    service_configurations = load_configurations(parsed_args.configuration_file)
+    username = service_configurations.twitter_configurations.username
+    storage_location = service_configurations.storage_location
+    protection_tag = service_configurations.protection_tag
+    date_until = (datetime.now(timezone.utc) - relativedelta(days=service_configurations.days_to_expire))
+
+    _log.info(
+        "Tweeter Amnesia Service Configs: "
+        f"Username [{storage_location}]; "
+        f"Protection Tag [{storage_location}]; "
+        f"Storage Location [{protection_tag}]; "
+        f"Deleting Tweets created before than [{date_until.strftime('%Y/%m/%d %H:%M:%S'):s}]"
+    )
+
+    api = Api(
+        bearer_token=service_configurations.twitter_configurations.bearer_token,
+        sleep_on_rate_limit=False
+    )
+
+    response = api.get_user(username=username)
+    user_id = response.data.id
+    _log.info(f"Username is [{username}] with User ID [{user_id}]")
+
+    continue_fecthing = True
+    search_parameters = {
+        "user_id": user_id,
+        "end_time": rfc3339.rfc3339(date_until),
+        "tweet_fields": "id,text,created_at"
+    }
+
+    removed_tweets_counter = 0
+    while continue_fecthing:
+        response = api.get_timelines(**search_parameters)
+
+        for tweet in response.data:
+            if protection_tag in tweet.text:
+                _log.info(f"Tweet with ID [{tweet.id}] skipped. Protection tag present.")
+                continue
+            else:
+                if storage_location:
+                    _log.info(f"Saving tweet with ID [{tweet.id}].")
+                    with open(f"{storage_location}/{tweet.id}", "wb") as file:
+                        pickle.dump(tweet.__dict__, file)
+
+                api.delete_tweet(tweet.id)
+                removed_tweets_counter += 1
+                _log.warning(f"Tweet [{tweet.id}] deleted.")
+
+        continue_fecthing = response.meta.next_token
+        search_parameters = {
+            "user_id": user_id,
+            "tweet_fields": "id,text,created_at",
+            "pagination_token": response.meta.next_token
+        }
+    _log.info(f"Total number of deleted tweets is [{removed_tweets_counter:d}].")
+    _log.info("It's done!")
     exit(0)
-
-
-if __name__ == '__main__':
-    main()
```

## Comparing `twitter_amnesia-1.1.3.dist-info/LICENSE` & `twitter_amnesia-1.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

