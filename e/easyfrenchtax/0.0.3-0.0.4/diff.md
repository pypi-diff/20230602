# Comparing `tmp/easyfrenchtax-0.0.3.tar.gz` & `tmp/easyfrenchtax-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyfrenchtax-0.0.3.tar", last modified: Wed May 24 20:46:41 2023, max compression
+gzip compressed data, was "easyfrenchtax-0.0.4.tar", last modified: Fri Jun  2 20:58:45 2023, max compression
```

## Comparing `easyfrenchtax-0.0.3.tar` & `easyfrenchtax-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-05-24 20:46:41.010088 easyfrenchtax-0.0.3/
--rw-r--r--   0 hadrien    (501) staff       (20)     1069 2021-12-17 08:32:37.000000 easyfrenchtax-0.0.3/LICENSE
--rw-r--r--   0 hadrien    (501) staff       (20)     2557 2023-05-24 20:46:41.010172 easyfrenchtax-0.0.3/PKG-INFO
--rw-r--r--   0 hadrien    (501) staff       (20)     1824 2022-06-07 08:55:19.000000 easyfrenchtax-0.0.3/README.md
--rw-r--r--   0 hadrien    (501) staff       (20)      103 2021-12-17 08:19:56.000000 easyfrenchtax-0.0.3/pyproject.toml
--rw-r--r--   0 hadrien    (501) staff       (20)      853 2023-05-24 20:46:41.010483 easyfrenchtax-0.0.3/setup.cfg
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-05-24 20:46:41.005089 easyfrenchtax-0.0.3/src/
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-05-24 20:46:41.006778 easyfrenchtax-0.0.3/src/easyfrenchtax/
--rw-r--r--   0 hadrien    (501) staff       (20)      100 2022-06-09 10:23:03.000000 easyfrenchtax-0.0.3/src/easyfrenchtax/__init__.py
--rw-r--r--   0 hadrien    (501) staff       (20)    23113 2023-05-19 21:32:02.000000 easyfrenchtax-0.0.3/src/easyfrenchtax/stock_helper.py
--rw-r--r--   0 hadrien    (501) staff       (20)    27735 2023-05-24 20:40:18.000000 easyfrenchtax-0.0.3/src/easyfrenchtax/tax_simulator.py
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-05-24 20:46:41.007549 easyfrenchtax-0.0.3/src/easyfrenchtax.egg-info/
--rw-r--r--   0 hadrien    (501) staff       (20)     2557 2023-05-24 20:46:41.000000 easyfrenchtax-0.0.3/src/easyfrenchtax.egg-info/PKG-INFO
--rw-r--r--   0 hadrien    (501) staff       (20)      480 2023-05-24 20:46:41.000000 easyfrenchtax-0.0.3/src/easyfrenchtax.egg-info/SOURCES.txt
--rw-r--r--   0 hadrien    (501) staff       (20)        1 2023-05-24 20:46:41.000000 easyfrenchtax-0.0.3/src/easyfrenchtax.egg-info/dependency_links.txt
--rw-r--r--   0 hadrien    (501) staff       (20)       18 2023-05-24 20:46:41.000000 easyfrenchtax-0.0.3/src/easyfrenchtax.egg-info/requires.txt
--rw-r--r--   0 hadrien    (501) staff       (20)       14 2023-05-24 20:46:41.000000 easyfrenchtax-0.0.3/src/easyfrenchtax.egg-info/top_level.txt
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-05-24 20:46:41.009892 easyfrenchtax-0.0.3/tests/
--rw-r--r--   0 hadrien    (501) staff       (20)     5482 2022-06-10 11:22:52.000000 easyfrenchtax-0.0.3/tests/test_capital_tax.py
--rw-r--r--   0 hadrien    (501) staff       (20)    11040 2022-11-27 06:14:06.000000 easyfrenchtax-0.0.3/tests/test_fiscal_advantages.py
--rw-r--r--   0 hadrien    (501) staff       (20)     5387 2022-06-09 13:40:59.000000 easyfrenchtax-0.0.3/tests/test_income_tax.py
--rw-r--r--   0 hadrien    (501) staff       (20)     8783 2022-06-10 11:29:26.000000 easyfrenchtax-0.0.3/tests/test_rental_tax.py
--rw-r--r--   0 hadrien    (501) staff       (20)    11717 2023-05-19 21:32:02.000000 easyfrenchtax-0.0.3/tests/test_stock_helper.py
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-06-02 20:58:45.124373 easyfrenchtax-0.0.4/
+-rw-r--r--   0 hadrien    (501) staff       (20)     1069 2021-12-17 08:32:37.000000 easyfrenchtax-0.0.4/LICENSE
+-rw-r--r--   0 hadrien    (501) staff       (20)     2557 2023-06-02 20:58:45.124444 easyfrenchtax-0.0.4/PKG-INFO
+-rw-r--r--   0 hadrien    (501) staff       (20)     1824 2022-06-07 08:55:19.000000 easyfrenchtax-0.0.4/README.md
+-rw-r--r--   0 hadrien    (501) staff       (20)      103 2021-12-17 08:19:56.000000 easyfrenchtax-0.0.4/pyproject.toml
+-rw-r--r--   0 hadrien    (501) staff       (20)      853 2023-06-02 20:58:45.124714 easyfrenchtax-0.0.4/setup.cfg
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-06-02 20:58:45.121005 easyfrenchtax-0.0.4/src/
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-06-02 20:58:45.122417 easyfrenchtax-0.0.4/src/easyfrenchtax/
+-rw-r--r--   0 hadrien    (501) staff       (20)      100 2022-06-09 10:23:03.000000 easyfrenchtax-0.0.4/src/easyfrenchtax/__init__.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    21521 2023-06-02 20:57:43.000000 easyfrenchtax-0.0.4/src/easyfrenchtax/stock_helper.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    27735 2023-06-02 20:57:34.000000 easyfrenchtax-0.0.4/src/easyfrenchtax/tax_simulator.py
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-06-02 20:58:45.123052 easyfrenchtax-0.0.4/src/easyfrenchtax.egg-info/
+-rw-r--r--   0 hadrien    (501) staff       (20)     2557 2023-06-02 20:58:45.000000 easyfrenchtax-0.0.4/src/easyfrenchtax.egg-info/PKG-INFO
+-rw-r--r--   0 hadrien    (501) staff       (20)      480 2023-06-02 20:58:45.000000 easyfrenchtax-0.0.4/src/easyfrenchtax.egg-info/SOURCES.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)        1 2023-06-02 20:58:45.000000 easyfrenchtax-0.0.4/src/easyfrenchtax.egg-info/dependency_links.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)       18 2023-06-02 20:58:45.000000 easyfrenchtax-0.0.4/src/easyfrenchtax.egg-info/requires.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)       14 2023-06-02 20:58:45.000000 easyfrenchtax-0.0.4/src/easyfrenchtax.egg-info/top_level.txt
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-06-02 20:58:45.124248 easyfrenchtax-0.0.4/tests/
+-rw-r--r--   0 hadrien    (501) staff       (20)     5482 2022-06-10 11:22:52.000000 easyfrenchtax-0.0.4/tests/test_capital_tax.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    11040 2022-11-27 06:14:06.000000 easyfrenchtax-0.0.4/tests/test_fiscal_advantages.py
+-rw-r--r--   0 hadrien    (501) staff       (20)     5387 2022-06-09 13:40:59.000000 easyfrenchtax-0.0.4/tests/test_income_tax.py
+-rw-r--r--   0 hadrien    (501) staff       (20)     8783 2022-06-10 11:29:26.000000 easyfrenchtax-0.0.4/tests/test_rental_tax.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    11721 2023-06-02 20:57:43.000000 easyfrenchtax-0.0.4/tests/test_stock_helper.py
```

### Comparing `easyfrenchtax-0.0.3/LICENSE` & `easyfrenchtax-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.3/PKG-INFO` & `easyfrenchtax-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyfrenchtax
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simulator of French taxes
 Home-page: https://github.com/had/easyfrenchtax
 Author: Hadrien Hamel
 Author-email: hadrien.hamel@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/had/easyfrenchtax/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyfrenchtax-0.0.3/README.md` & `easyfrenchtax-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.3/setup.cfg` & `easyfrenchtax-0.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = easyfrenchtax
-version = 0.0.3
+version = 0.0.4
 author = Hadrien Hamel
 author_email = hadrien.hamel@gmail.com
 license = MIT
 description = A simulator of French taxes
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/had/easyfrenchtax
```

### Comparing `easyfrenchtax-0.0.3/src/easyfrenchtax/stock_helper.py` & `easyfrenchtax-0.0.4/src/easyfrenchtax/stock_helper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from datetime import date, datetime
 from dateutil.relativedelta import relativedelta
 from currency_converter import CurrencyConverter
-from collections import defaultdict, namedtuple
+from collections import defaultdict
 import csv
 import glob
 
 
 @dataclass
 class StockGroup:
     owner: int  # taxpayer 1 or 2, typically, for tax statements
@@ -17,15 +17,15 @@
     acq_date: date
     plan_name: str
 
 
 @dataclass
 class RsuPlan:
     name: str
-    grant_date: date
+    approval_date: date
     taxation_scheme: str
     stock_symbol: str
     currency: str
 
 
 @dataclass
 class SaleEvent:
@@ -44,30 +44,27 @@
 
 
 class StockHelper:
     rsu_plans: dict[str, RsuPlan]
     rsus: dict[str, list[StockGroup]]  # TODO integrate list of RSUs to RsuPlan
     espp_stocks: dict[str, list[StockGroup]]
     stock_sales: dict[int, list[SaleEvent]]
-    weighted_average_prices: dict[tuple[str, date], float]
 
     def __init__(self):
         self.rsu_plans = {}
         self.rsus = defaultdict(list)
         self.espp_stocks = defaultdict(list)
         self.stock_options = defaultdict(list)
         self.stock_sales = defaultdict(list)
-        self.weighted_average_prices = {}  # "prix moyen pondéré" in euro ; keyed by a tuple (plan_name, acq_date)
 
     # TODO: this seems unused, consider removing
     def reset(self, stock_types: list[str] = ("espp", "stockoption", "rsu"), symbols: list[str] = None) -> None:
         for sales in self.stock_sales.values():
             sales[:] = [s for s in sales if
                         (symbols and s.symbol not in symbols) or (s.stock_type not in stock_types)]
-        self.weighted_average_prices.clear()
         stock_types_mapping = {
             "espp": self.espp_stocks,
             "stockoption": self.stock_options,
             "rsu": self.rsus
         }
         for stock_type in [stock_types_mapping[st] for st in stock_types]:
             if not symbols:
@@ -90,32 +87,35 @@
         for symbol, stockoptions in self.stock_options.items():
             for stockoption in stockoptions:
                 summary[symbol]["StockOption"] += stockoption.count
         return summary
 
     # ----- RSU related load functions ------
     @staticmethod
-    def _determine_rsu_plans_type(grant_date: date) -> str:
-        if grant_date <= date(2012, 9, 27):
+    def _determine_rsu_plans_type(approval_date: date) -> str:
+        if approval_date <= date(2012, 9, 27):
             return "2007"  # TODO replace with an enum
-        elif grant_date <= date(2015, 8, 8):
+        elif approval_date <= date(2015, 8, 8):
             return "2012"
-        elif grant_date <= date(2017, 1, 1):
+        elif approval_date <= date(2017, 1, 1):
             return "2015"
-        elif grant_date <= date(2018, 1, 1):
+        elif approval_date <= date(2018, 1, 1):
             return "2017"
         else:
             return "2018"
 
-    def rsu_plan(self, name: str, grant_date: date, symbol: str, currency: str) -> None:
+    ## IMPORTANT! approval_date here is used to determine the taxation scheme
+    # (Macron I, Macron II, etc.) so it needs to be the date where the plan was
+    # approved by the shareholders, NOT the grant date.
+    def rsu_plan(self, name: str, approval_date: date, symbol: str, currency: str) -> None:
         if name not in self.rsu_plans:
             self.rsu_plans[name] = RsuPlan(
                 name=name,
-                grant_date=grant_date,
-                taxation_scheme=StockHelper._determine_rsu_plans_type(grant_date),
+                approval_date=approval_date,
+                taxation_scheme=StockHelper._determine_rsu_plans_type(approval_date),
                 stock_symbol=symbol,
                 currency=currency
             )
 
     def rsu_vesting(self, owner: int, symbol: str, plan_name: str, count: int, acq_date: date, acq_price: float,
                     currency: str = None) -> None:
         if not currency:
@@ -188,37 +188,14 @@
                         self.rsu_vesting(owner, symbol, plan_name, acq_count, acq_date, acq_price, currency)
                     elif stock_type == "ESPP":
                         self.add_espp(owner, symbol, acq_count, acq_date, acq_price, currency)
                     elif stock_type == "StockOption":
                         self.add_stockoptions(owner, symbol, plan_name, acq_count, acq_date, acq_price, currency)
 
     ####### stock selling related load functions #######
-    def compute_weighted_average_prices(self, symbol: str, up_to: date):
-        # There are complex rules of computing weighted average price (WAP, or PMP in French), see:
-        # https://bofip.impots.gouv.fr/bofip/3619-PGP.html/identifiant=BOI-RPPM-PVBMI-20-10-20-40-20191220#Regle_du_prix_moyen_pondere_10
-        # Basically, we need to compute a weighted average of all *available* stock, up to the provided date (sell date)
-        # When some stocks have already been part of a computation for a previous sell event, we re-use the then
-        # computed WAP (aka PMP), and update it.
-        total = 0
-        count = 0
-        rsu_up_to_date = [r for r in self.rsus[symbol] if r.acq_date < up_to]
-        for acq in rsu_up_to_date:
-            # get WAP, fallback on acq_price_eur if it's the first time we're computing it
-            price = self.weighted_average_prices.get((acq.plan_name, acq.acq_date),
-                                                     acq.acq_price_eur)
-            acq_count = acq.available
-            total += acq_count * price
-            count += acq_count
-        if count == 0:
-            return -1
-        weighted_average_price = total / count
-        for acq in rsu_up_to_date:
-            # upsert the newly computed weighted average price
-            self.weighted_average_prices[(acq.plan_name, acq.acq_date)] = weighted_average_price
-        return weighted_average_price
 
     def sell_stockoptions(self, symbol: str, nb_stocks: int, sell_date: date, sell_price: float, fees: float,
                           currency: str = "EUR"):
         if nb_stocks == 0:
             return
         sell_details = []
         sell_price_eur = round(cc.convert(sell_price, currency, "EUR", date=sell_date), 2)
@@ -260,93 +237,95 @@
                   currency: str = "EUR"):
         if nb_stocks == 0:
             return
         sell_details = []
         sell_price_eur = round(cc.convert(sell_price, currency, "EUR", date=sell_date), 2)
         to_sell = nb_stocks
         stocks_before_sell_date = [r for r in self.espp_stocks[symbol] if r.acq_date < sell_date]
-        total_acquisition_price = 0
         for i, acq in enumerate(stocks_before_sell_date):
             if acq.available == 0:
                 continue
             sell_from_acq = min(to_sell, acq.available)
-            sell_details.append({
-                "plan_name": acq.plan_name,
-                "count": sell_from_acq,
-                "acq_price": acq.acq_price,  # keep price in original currency here
-                "acq_date": acq.acq_date
-            })
-            total_acquisition_price += acq.acq_price_eur * sell_from_acq
-            # update the rsu data with new availability (tuples are immutable, so replace with new one)
             self.espp_stocks[symbol][i].available = acq.available - sell_from_acq
             to_sell -= sell_from_acq
+            self.stock_sales[sell_date.year].append(SaleEvent(
+                symbol=symbol,
+                stock_type="espp",
+                nb_stocks_sold=sell_from_acq,
+                unit_acquisition_price=round(acq.acq_price_eur, 2),
+                sell_date=sell_date,
+                sell_price_eur=sell_price_eur,
+                sell_details=[{
+                    "plan_name": acq.plan_name,
+                    "count": sell_from_acq,
+                    "acq_price": acq.acq_price,  # keep price in original currency here
+                    "acq_date": acq.acq_date
+                }],
+                selling_fees=0  # not sure how to handle this
+            ))
             if to_sell == 0:
                 break
         if to_sell > 0:
             print(f"WARNING: You are trying to sell more stocks ({nb_stocks}) than you have")
             return (0, 0, [])
-        average_acquisition_price = total_acquisition_price / (nb_stocks - to_sell)
-        self.stock_sales[sell_date.year].append(SaleEvent(
-            symbol=symbol,
-            stock_type="espp",
-            nb_stocks_sold=nb_stocks - to_sell,
-            unit_acquisition_price=round(average_acquisition_price, 2),
-            sell_date=sell_date,
-            sell_price_eur=sell_price_eur,
-            sell_details=sell_details,
-            selling_fees=round(cc.convert(fees, currency, "EUR", date=sell_date), 2)
-        ))
-        return ((nb_stocks - to_sell), average_acquisition_price, sell_details)
+        return (nb_stocks - to_sell)
 
-    # TODO differentiate by stock_symbol
     def sell_rsus(self, symbol: str, nb_stocks: int, sell_date: date, sell_price: float, fees: float,
-                  currency: str = "EUR"):
+                  currency: str = "EUR") -> int:
         if nb_stocks == 0:
-            return
+            return 0
         sell_details = []
         sell_price_eur = round(cc.convert(sell_price, currency, "EUR", date=sell_date), 2)
         to_sell = nb_stocks
-        # we need to compute weighted average prices of our stocks up to the sell date, for future tax accounting
-        weighted_average_price = self.compute_weighted_average_prices(symbol, up_to=sell_date)
 
         # Acquisitions are sorted by date, this is the rule set by the tax office (FIFO, or PEPS="premier entré premier
         # sorti"); we only keep stocks acquired *before* the sell date, in case we input a sell event in the middle of
         # acquisitions.
         rsu_before_sell_date = [r for r in self.rsus[symbol] if r.acq_date < sell_date]
         if not rsu_before_sell_date:
             # no rsu for that date
-            return (0, 0, [])
+            return 0
         for i, acq in enumerate(rsu_before_sell_date):
             if acq.available == 0:
                 continue
             sell_from_acq = min(to_sell, acq.available)
-            sell_details.append({
-                "plan_name": acq.plan_name,
-                "count": sell_from_acq,
-                "acq_price": acq.acq_price,  # keep price in original currency here
-                "acq_date": acq.acq_date
-            })
+            self.stock_sales[sell_date.year].append(SaleEvent(
+                symbol=symbol,
+                stock_type="rsu",
+                nb_stocks_sold=sell_from_acq,
+                unit_acquisition_price=round(acq.acq_price_eur, 2),
+                sell_date=sell_date,
+                sell_price_eur=sell_price_eur,
+                sell_details=[{
+                    "plan_name": acq.plan_name,
+                    "count": sell_from_acq,
+                    "acq_price": acq.acq_price,  # keep price in original currency here
+                    "acq_price_currency": "TODO",  # TODO
+                    "acq_date": acq.acq_date
+                }],
+                selling_fees=0  # not sure how to handle this
+            ))
             # update the rsu data with new availability (tuples are immutable, so replace with new one)
             self.rsus[symbol][i].available = acq.available - sell_from_acq
             to_sell -= sell_from_acq
             if to_sell == 0:
                 break
         if to_sell > 0:
             print(f"WARNING: You are trying to sell more stocks ({nb_stocks}) than you have ({to_sell})")
-        self.stock_sales[sell_date.year].append(SaleEvent(
-            symbol=symbol,
-            stock_type="rsu",
-            nb_stocks_sold=nb_stocks - to_sell,
-            unit_acquisition_price=round(weighted_average_price, 2),
-            sell_date=sell_date,
-            sell_price_eur=sell_price_eur,
-            sell_details=sell_details,
-            selling_fees=round(cc.convert(fees, currency, "EUR", date=sell_date), 2)
-        ))
-        return ((nb_stocks - to_sell), weighted_average_price, sell_details)
+        # self.stock_sales[sell_date.year].append(SaleEvent(
+        #     symbol=symbol,
+        #     stock_type="rsu",
+        #     nb_stocks_sold=nb_stocks - to_sell,
+        #     unit_acquisition_price=-1,
+        #     sell_date=sell_date,
+        #     sell_price_eur=sell_price_eur,
+        #     sell_details=sell_details,
+        #     selling_fees=round(cc.convert(fees, currency, "EUR", date=sell_date), 2)
+        # ))
+        return (nb_stocks - to_sell)
 
     ####### tax computation functions #######
 
     # the bible of acquisition and capital gain tax (version 2021):
     # https://www.impots.gouv.fr/portail/www2/fichiers/documentation/brochure/ir_2021/pdf_som/09-plus_values_141a158.pdf
     def compute_acquisition_gain_tax(self, year: int):
         sell_events = self.stock_sales[year]
@@ -371,19 +350,20 @@
                             f"Owner must be 1 or 2, not {sale_detail['owner']} (type={type(sale_detail['owner'])}")
             elif sale.stock_type == "rsu":
                 # acquisition gain only applies to RSU
                 sell_date = sale.sell_date
                 sell_date_minus_2y = sell_date + relativedelta(years=-2)
                 sell_date_minus_8y = sell_date + relativedelta(years=-8)
                 for sale_detail in sale.sell_details:
-                    plan_name = sale_detail["plan_name"]
-                    taxation_scheme = self.rsu_plans[plan_name].taxation_scheme
+                    rsu_plan = self.rsu_plans[sale_detail["plan_name"]]
+                    taxation_scheme = rsu_plan.taxation_scheme
+                    plan_currency = rsu_plan.currency
                     acq_date = sale_detail["acq_date"]
-                    usd_eur = cc.convert(1, "USD", "EUR",
-                                         date=acq_date)  # TODO: fetch actual currency instead of hardcoding USD here
+                    usd_eur = cc.convert(1, plan_currency, "EUR",
+                                         date=acq_date)
                     gain_eur = sale_detail["count"] * sale_detail["acq_price"] * usd_eur
                     # gain tax
                     if taxation_scheme == "2015" or taxation_scheme == "2017":
                         # 50% rebates btw 2 and 8y retention, 65% above 8y
                         if acq_date <= sell_date_minus_8y:
                             taxable_gain += gain_eur * 0.35
                             rebates += gain_eur * 0.65
@@ -423,15 +403,15 @@
             sell_event_report = {}
             sell_event_report["selling_date_512"] = sale.sell_date
             sell_event_report["sell_price_514"] = sale.sell_price_eur
             sell_event_report["sold_stock_units_515"] = sale.nb_stocks_sold
             global_selling_proceeds = sale.sell_price_eur * sale.nb_stocks_sold
             sell_event_report["global_selling_proceeds_516"] = round(global_selling_proceeds)
             sell_event_report["selling_fees_517"] = round(sale.selling_fees)
-            net_selling_proceeds = global_selling_proceeds - sale.selling_fees
+            net_selling_proceeds = round(global_selling_proceeds - sale.selling_fees)
             sell_event_report["net_selling_proceeds_518"] = net_selling_proceeds
             sell_event_report["unit_acquisition_price_520"] = sale.unit_acquisition_price
             global_acquisition_cost = round(sale.unit_acquisition_price * sale.nb_stocks_sold)
             sell_event_report["global_acquisition_cost_521"] = global_acquisition_cost
             sell_event_report["acquisition_fees_522"] = 0  # TODO: check how to report this, if we need to support it
             total_acquisition_cost = global_acquisition_cost + sell_event_report["acquisition_fees_522"]
             sell_event_report["total_acquisition_cost_523"] = total_acquisition_cost
```

### Comparing `easyfrenchtax-0.0.3/src/easyfrenchtax/tax_simulator.py` & `easyfrenchtax-0.0.4/src/easyfrenchtax/tax_simulator.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.3/src/easyfrenchtax.egg-info/PKG-INFO` & `easyfrenchtax-0.0.4/src/easyfrenchtax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyfrenchtax
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simulator of French taxes
 Home-page: https://github.com/had/easyfrenchtax
 Author: Hadrien Hamel
 Author-email: hadrien.hamel@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/had/easyfrenchtax/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyfrenchtax-0.0.3/tests/test_capital_tax.py` & `easyfrenchtax-0.0.4/tests/test_capital_tax.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.3/tests/test_fiscal_advantages.py` & `easyfrenchtax-0.0.4/tests/test_fiscal_advantages.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.3/tests/test_income_tax.py` & `easyfrenchtax-0.0.4/tests/test_income_tax.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.3/tests/test_rental_tax.py` & `easyfrenchtax-0.0.4/tests/test_rental_tax.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.3/tests/test_stock_helper.py` & `easyfrenchtax-0.0.4/tests/test_stock_helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,139 +1,150 @@
+from collections.abc import Callable
+
 import pytest
 from src.easyfrenchtax import StockHelper
 from datetime import date
 from currency_converter import CurrencyConverter
 
 
 @pytest.fixture
 def stock_helper_with_plan():
     stock_helper = StockHelper()
-    stock_helper.rsu_plan("RSU JUN 16", date(2016, 6, 28), "CAKE", "USD")
-    stock_helper.rsu_vesting(1, "CAKE", "RSU JUN 16", 240, date(2018, 6, 29), 20)
-    stock_helper.rsu_vesting(1, "CAKE", "RSU JUN 16", 10, date(2018, 7, 30), 18)
-    stock_helper.rsu_vesting(1, "CAKE", "RSU JUN 16", 10, date(2018, 8, 28), 19)
-    stock_helper.rsu_vesting(1, "CAKE", "RSU JUN 16", 10, date(2018, 9, 28), 14)
-    stock_helper.rsu_vesting(1, "CAKE", "RSU JUN 16", 10, date(2018, 10, 29), 15)
-    stock_helper.rsu_vesting(1, "CAKE", "RSU JUN 16", 10, date(2018, 11, 28), 14)
-    stock_helper.rsu_vesting(1, "CAKE", "RSU JUN 16", 10, date(2018, 12, 28), 19)
-    stock_helper.rsu_vesting(1, "CAKE", "RSU JUN 16", 10, date(2019, 1, 28), 23)
-    stock_helper.rsu_vesting(1, "CAKE", "RSU JUN 16", 10, date(2019, 2, 28), 24)
-    stock_helper.add_espp(1, "BUD", 500, date(2019, 1, 15), 22, "USD")
+    stock_helper.rsu_plan("Cake1", date(2016, 6, 28), "CAKE", "USD")
+    stock_helper.rsu_vesting(1, "CAKE", "Cake1", 240, date(2018, 6, 29), 20)
+    stock_helper.rsu_vesting(1, "CAKE", "Cake1", 10, date(2018, 7, 30), 18)
+    stock_helper.rsu_vesting(1, "CAKE", "Cake1", 10, date(2018, 8, 28), 19)
+    stock_helper.rsu_vesting(1, "CAKE", "Cake1", 10, date(2018, 9, 28), 14)
+    stock_helper.rsu_vesting(1, "CAKE", "Cake1", 10, date(2018, 10, 29), 15)
+    stock_helper.rsu_vesting(1, "CAKE", "Cake1", 10, date(2018, 11, 28), 14)
+    stock_helper.rsu_vesting(1, "CAKE", "Cake1", 10, date(2018, 12, 28), 19)
+    stock_helper.rsu_vesting(1, "CAKE", "Cake1", 10, date(2019, 1, 28), 23)
+    stock_helper.rsu_vesting(1, "CAKE", "Cake1", 10, date(2019, 2, 28), 24)
+    stock_helper.rsu_plan("Pineapple", date(2016, 6, 29), "PZZA", "USD")
+    stock_helper.rsu_vesting(1, "PZZA", "Pineapple", 313, date(2020, 12, 28), 20.84)
+    stock_helper.rsu_vesting(1, "PZZA", "Pineapple", 312, date(2021, 3, 28), 27.44)
+    stock_helper.rsu_vesting(1, "PZZA", "Pineapple", 313, date(2021, 6, 28), 37.25)
+    stock_helper.rsu_plan("Pepperoni", date(2017, 7, 28), "PZZA", "USD")
+    stock_helper.rsu_vesting(1, "PZZA", "Pepperoni", 398, date(2020, 12, 16), 18.75)
+    stock_helper.rsu_vesting(1, "PZZA", "Pepperoni", 133, date(2021, 1, 26), 19.13)
+    stock_helper.add_espp(1, "BUD", 200, date(2019, 1, 15), 22, "USD")
+    stock_helper.add_espp(1, "BUD", 300, date(2019, 7, 15), 19, "USD")
     stock_helper.add_stockoptions(1, "PZZA", "SO", 150, date(2018, 1, 15), 5, "USD")
     return stock_helper
 
 
 @pytest.fixture
-def convert_fn():
+def convert_fn() -> Callable[[float, str, str, date], float]:
     cc = CurrencyConverter(fallback_on_wrong_date=True)
     return cc.convert
 
 
 def test_summary(stock_helper_with_plan):
     summary = stock_helper_with_plan.summary()
     assert set(summary.keys()) == {"CAKE", "BUD", "PZZA"}
     assert set(summary["CAKE"].keys()) == {"RSU"}
     assert summary["CAKE"]["RSU"] == 320
     assert set(summary["BUD"].keys()) == {"ESPP"}
     assert summary["BUD"]["ESPP"] == 500
-    assert set(summary["PZZA"].keys()) == {"StockOption"}
+    assert set(summary["PZZA"].keys()) == {"StockOption", "RSU"}
     assert summary["PZZA"]["StockOption"] == 150
 
 
-def test_weighted_average_price(stock_helper_with_plan):
-    weighted_average_price = stock_helper_with_plan.compute_weighted_average_prices("CAKE", date(2018, 7, 1))
-    rsu_under_test = stock_helper_with_plan.rsus["CAKE"][0]
-    wap_price = stock_helper_with_plan.weighted_average_prices[(rsu_under_test.plan_name, rsu_under_test.acq_date)]
-    assert rsu_under_test.acq_price_eur == wap_price, \
-        "weighted average price is computed on 1st element only, should be equal to original price"
-    assert weighted_average_price == rsu_under_test.acq_price_eur, \
-        "returned value should also match the original price"
-    assert len(stock_helper_with_plan.weighted_average_prices) == 1, \
-        "weighted average price should NOT be computed for the next elements"
-
-
-def test_selling_rsus(stock_helper_with_plan):
+def test_rsu_sale(stock_helper_with_plan):
     assert sum([r.available for r in stock_helper_with_plan.rsus["CAKE"]]) == 320
-    final_count_1, _, _ = stock_helper_with_plan.sell_rsus("CAKE", 200, date(2019, 6, 3), sell_price=22, fees=0,
-                                                           currency="USD")
+    final_count_1 = stock_helper_with_plan.sell_rsus("CAKE", 200, date(2019, 6, 3), sell_price=22, fees=0,
+                                                     currency="USD")
     assert final_count_1 == 200
     assert stock_helper_with_plan.rsus["CAKE"][0].available == 40
     assert all([r.available == 10 for r in stock_helper_with_plan.rsus["CAKE"][1:]])
-    final_count_2, _, _ = stock_helper_with_plan.sell_rsus("CAKE", 200, date(2019, 6, 3), sell_price=22, fees=0,
-                                                           currency="USD")
+    final_count_2 = stock_helper_with_plan.sell_rsus("CAKE", 200, date(2019, 6, 3), sell_price=22, fees=0,
+                                                     currency="USD")
     assert final_count_2 == 120, "Cannot sell more than we have"
 
 
-def test_selling_too_many_rsus(stock_helper_with_plan):
-    assert sum([r.available for r in stock_helper_with_plan.rsus["CAKE"]]) == 320
-    final_count, _, _ = stock_helper_with_plan.sell_rsus("CAKE", 400, date(2019, 6, 3), sell_price=22, fees=0,
-                                                         currency="USD")
-    assert final_count == 320, "Cannot sell more than we have"
-
-
-def test_acquisition_gain_tax(stock_helper_with_plan):
+def test_rsu_acquisition_gain_tax(stock_helper_with_plan):
     stock_helper_with_plan.sell_rsus("CAKE", 200, date(2019, 1, 16),
                                      sell_price=22, fees=0, currency="USD")
     taxes = stock_helper_with_plan.compute_acquisition_gain_tax(2019)
     assert taxes["taxable_acquisition_gain_1TZ"] == 3431
     assert taxes["acquisition_gain_50p_rebates_1WZ"] == 0
     assert taxes["acquisition_gain_rebates_1UZ"] == 0
     assert taxes["exercise_gain_1_1TT"] == 0
     assert taxes["exercise_gain_2_1UT"] == 0
 
 
-def test_acquisition_gain_tax_rebates(stock_helper_with_plan):
+def test_rsu_acquisition_gain_tax_rebates(stock_helper_with_plan):
     stock_helper_with_plan.sell_rsus("CAKE", 200, date(2021, 8, 2),
                                      sell_price=28, fees=0, currency="USD")
     taxes = stock_helper_with_plan.compute_acquisition_gain_tax(2021)
     assert taxes["taxable_acquisition_gain_1TZ"] == 1716
     assert taxes["acquisition_gain_50p_rebates_1WZ"] == 0
     assert taxes["acquisition_gain_rebates_1UZ"] == 1716
     assert taxes["exercise_gain_1_1TT"] == 0
     assert taxes["exercise_gain_2_1UT"] == 0
 
 
-def test_bofip_case():
-    # example from:
-    # https://bofip.impots.gouv.fr/bofip/3619-PGP.html/identifiant=BOI-RPPM-PVBMI-20-10-20-40-20191220#Regle_du_prix_moyen_pondere_10
-    stock_helper = StockHelper()
-    stock_helper.rsu_plan("Test", date(2013, 1, 1), "X", "EUR")
-    # plan_name, acq_count, acq_date, acq_price, currency = None
-    year_N = 2010
-    stock_helper.rsu_vesting(1, "TEST", "Test", 100, date(year_N, 1, 1), 95)
-    stock_helper.rsu_vesting(1, "TEST", "Test", 200, date(year_N + 2, 1, 1), 105)
-    stock_helper.rsu_vesting(1, "TEST", "Test", 100, date(year_N + 3, 1, 1), 107)
-    _, weighted_average_price_1, _ = stock_helper.sell_rsus("TEST", 150, date(year_N + 7, 1, 1), 110, 0)
-    capital_gain_tax_1 = stock_helper.compute_capital_gain_tax(year_N + 7)
-    assert weighted_average_price_1 == 103
-    assert capital_gain_tax_1["2042C"]["capital_gain_3VG"] == 1050
-    assert sum([r.available for r in stock_helper.rsus["TEST"]]) == 250
-    stock_helper.rsu_vesting(1, "TEST", "Test", 50, date(year_N + 8, 9, 1), 100)
-    stock_helper.rsu_vesting(1, "TEST", "Test", 300, date(year_N + 8, 11, 1), 107.50)
-    _, weighted_average_price_2, _ = stock_helper.sell_rsus("TEST", 200, date(year_N + 9, 1, 1), 108, 0)
-    capital_gain_tax_2 = stock_helper.compute_capital_gain_tax(year_N + 9)
-    assert weighted_average_price_2 == 105
-    assert capital_gain_tax_2["2042C"]["capital_gain_3VG"] == 600
-    assert sum([r.available for r in stock_helper.rsus["TEST"]]) == 400
+def test_rsu_capital_gain_simple(stock_helper_with_plan):
+    final_count = stock_helper_with_plan.sell_rsus("CAKE", 200, date(2021, 8, 2),
+                                                   sell_price=28, fees=0, currency="USD")
+    assert final_count == 200
+    report = stock_helper_with_plan.compute_capital_gain_tax(2021)
+    assert True
 
 
-def test_espp_sale(stock_helper_with_plan, convert_fn):
+def test_rsu_example(stock_helper_with_plan):
+    final_count = stock_helper_with_plan.sell_rsus("PZZA", 844, date(2021, 2, 12),
+                                                   sell_price=31.52, fees=0, currency="USD")
+    assert final_count == 844
+    report_ag = stock_helper_with_plan.compute_acquisition_gain_tax(2021)
+    assert report_ag['taxable_acquisition_gain_1TZ'] == 13556
+    report_cg = stock_helper_with_plan.compute_capital_gain_tax(2021)
+    report_2042C = report_cg['2042C']
+    report_2074 = report_cg['2074']
+    assert report_2042C['capital_gain_3VG'] == 8413
+    assert len(report_2074) == 3
+    assert report_2074[0]['sold_stock_units_515'] == 398
+    assert report_2074[0]['global_acquisition_cost_521'] == 6121
+    assert report_2074[0]['global_selling_proceeds_516'] == 10360
+    assert report_2074[1]['sold_stock_units_515'] == 313
+    assert report_2074[1]['global_acquisition_cost_521'] == 5340
+    assert report_2074[1]['global_selling_proceeds_516'] == 8147
+    assert report_2074[2]['sold_stock_units_515'] == 133
+    assert report_2074[2]['global_acquisition_cost_521'] == 2095
+    assert report_2074[2]['global_selling_proceeds_516'] == 3462
+    stock_helper_with_plan.helper_capital_gain_tax(report_cg)
+
+
+def test_espp_sale(convert_fn):
+    stock_helper = StockHelper()
+    stock_helper.add_espp(1, "BUD", 200, date(2019, 1, 15), 22, "USD")
+    stock_helper.add_espp(1, "BUD", 300, date(2019, 7, 15), 19, "USD")
     sell_price = 28
-    final_count, unit_acquisition_price, sell = stock_helper_with_plan.sell_espp("BUD", 200, date(2021, 8, 2),
-                                                                                 sell_price=sell_price, fees=0,
-                                                                                 currency="USD")
-    agt = stock_helper_with_plan.compute_acquisition_gain_tax(2021)
-    cgt = stock_helper_with_plan.compute_capital_gain_tax(2021)
+    final_count = stock_helper.sell_espp("BUD", 300, date(2021, 8, 2), sell_price=sell_price, fees=0, currency="USD")
+    assert final_count == 300
 
-    sell_price_eur = convert_fn(sell_price, "USD", "EUR", date(2021, 8, 2))
-    assert final_count == 200
-    assert unit_acquisition_price == stock_helper_with_plan.espp_stocks["BUD"][0].acq_price_eur
-    assert not any(agt.values()), "ESPP should not yield acquisition gain (thus no acquisition gain tax)"
-    expected_capital_gain = round(200 * (round(sell_price_eur, 2) - round(unit_acquisition_price, 2)))
-    assert cgt["2042C"]["capital_gain_3VG"] == expected_capital_gain, \
+    report_ag = stock_helper.compute_acquisition_gain_tax(2021)
+    assert not any(report_ag.values()), "ESPP should not yield acquisition gain (thus no acquisition gain tax)"
+
+    report_cg = stock_helper.compute_capital_gain_tax(2021)
+    report_2042C = report_cg['2042C']
+    report_2074 = report_cg['2074']
+
+    acq_price_eur_1 = round(convert_fn(22, "USD", "EUR", date(2019, 1, 15)), 2)
+    acq_price_eur_2 = round(convert_fn(19, "USD", "EUR", date(2019, 7, 15)), 2)
+    sell_price_eur = round(convert_fn(sell_price, "USD", "EUR", date(2021, 8, 2)), 2)
+    assert report_2074[0]['sold_stock_units_515'] == 200
+    assert report_2074[0]['sell_price_514'] == sell_price_eur
+    assert report_2074[1]['sold_stock_units_515'] == 100
+    assert report_2074[1]['sell_price_514'] == sell_price_eur
+    expected_capital_gain = round(
+        200 * (round(sell_price_eur, 2) - round(acq_price_eur_1, 2)) +
+        100 * (round(sell_price_eur, 2) - round(acq_price_eur_2, 2)), 2
+    )
+    assert report_2042C["capital_gain_3VG"] == expected_capital_gain, \
         "Capital gain tax should be compliant"
 
 
 def test_stockoptions_sale(stock_helper_with_plan, convert_fn):
     sell_price = 40
     final_count, _, sell = stock_helper_with_plan.sell_stockoptions("PZZA", 50, date(2021, 8, 2), sell_price=sell_price,
                                                                     fees=0, currency="USD")
@@ -149,56 +160,56 @@
     assert not any(cgt["2042C"].values()), \
         "Stock options 'exercise and sell' should not yield capital gain (thus no capital gain tax)"
     assert len(cgt["2074"]) == 0, \
         "Stock options 'exercise and sell' should not yield capital gain (thus no capital gain tax)"
 
 
 def test_reset_all(stock_helper_with_plan):
-    # CAKE=240 ; BUD=500 ; PZZA=150
+    # CAKE=240 ; BUD=200 ; PZZA=150
     stock_helper_with_plan.sell_rsus("CAKE", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
     stock_helper_with_plan.sell_espp("BUD", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
     stock_helper_with_plan.sell_stockoptions("PZZA", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
     stock_helper_with_plan.reset()
     assert stock_helper_with_plan.rsus["CAKE"][0].available == 240
-    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 500
+    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 200
     assert stock_helper_with_plan.stock_options["PZZA"][0].available == 150
     assert len(stock_helper_with_plan.stock_sales[2021]) == 0
 
 
 def test_reset_by_stocktype(stock_helper_with_plan):
-    # CAKE=240 ; BUD=500 ; PZZA=150
+    # CAKE=240 ; BUD=200 ; PZZA=150
     stock_helper_with_plan.sell_rsus("CAKE", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
     stock_helper_with_plan.sell_espp("BUD", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
     stock_helper_with_plan.sell_stockoptions("PZZA", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
     assert stock_helper_with_plan.rsus["CAKE"][0].available == 190
-    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 450
+    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 150
     assert stock_helper_with_plan.stock_options["PZZA"][0].available == 100
     stock_helper_with_plan.reset(stock_types=["espp"])
     assert stock_helper_with_plan.rsus["CAKE"][0].available == 190
-    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 500
+    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 200
     assert stock_helper_with_plan.stock_options["PZZA"][0].available == 100
     stock_helper_with_plan.reset(stock_types=["stockoption"])
     assert stock_helper_with_plan.rsus["CAKE"][0].available == 190
-    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 500
+    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 200
     assert stock_helper_with_plan.stock_options["PZZA"][0].available == 150
     stock_helper_with_plan.reset(stock_types=["rsu"])
     assert stock_helper_with_plan.rsus["CAKE"][0].available == 240
-    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 500
+    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 200
     assert stock_helper_with_plan.stock_options["PZZA"][0].available == 150
 
 
 def test_reset_by_symbol(stock_helper_with_plan):
-    # CAKE=240 ; BUD=500 ; PZZA=150
+    # CAKE=240 ; BUD=200 ; PZZA=150
     stock_helper_with_plan.sell_rsus("CAKE", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
     stock_helper_with_plan.sell_espp("BUD", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
     stock_helper_with_plan.sell_stockoptions("PZZA", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
     assert stock_helper_with_plan.rsus["CAKE"][0].available == 190
-    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 450
+    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 150
     assert stock_helper_with_plan.stock_options["PZZA"][0].available == 100
     stock_helper_with_plan.reset(symbols=["CAKE", "PZZA"])
     assert stock_helper_with_plan.rsus["CAKE"][0].available == 240
-    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 450
+    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 150
     assert stock_helper_with_plan.stock_options["PZZA"][0].available == 150
     stock_helper_with_plan.reset(symbols=["BUD"])
     assert stock_helper_with_plan.rsus["CAKE"][0].available == 240
-    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 500
+    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 200
     assert stock_helper_with_plan.stock_options["PZZA"][0].available == 150
```

