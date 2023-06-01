# Comparing `tmp/cvxsimulator-0.4.0.tar.gz` & `tmp/cvxsimulator-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.4.0.tar", max compression
+gzip compressed data, was "cvxsimulator-0.4.1.tar", max compression
```

## Comparing `cvxsimulator-0.4.0.tar` & `cvxsimulator-0.4.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11375 2023-05-30 15:25:14.769701 cvxsimulator-0.4.0/LICENSE
--rw-r--r--   0        0        0     5064 2023-05-30 15:25:14.769701 cvxsimulator-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-05-30 15:25:14.845701 cvxsimulator-0.4.0/cvx/simulator/__init__.py
--rw-r--r--   0        0        0    14005 2023-05-30 15:25:14.845701 cvxsimulator-0.4.0/cvx/simulator/builder.py
--rw-r--r--   0        0        0     1552 2023-05-30 15:25:14.845701 cvxsimulator-0.4.0/cvx/simulator/grid.py
--rw-r--r--   0        0        0     1163 2023-05-30 15:25:14.845701 cvxsimulator-0.4.0/cvx/simulator/metrics.py
--rw-r--r--   0        0        0     1422 2023-05-30 15:25:14.845701 cvxsimulator-0.4.0/cvx/simulator/month.py
--rw-r--r--   0        0        0    17965 2023-05-30 15:25:14.845701 cvxsimulator-0.4.0/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      514 2023-05-30 15:25:14.845701 cvxsimulator-0.4.0/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      608 2023-05-30 15:25:39.242008 cvxsimulator-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5651 1970-01-01 00:00:00.000000 cvxsimulator-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11375 2023-06-01 22:20:45.829135 cvxsimulator-0.4.1/LICENSE
+-rw-r--r--   0        0        0     5064 2023-06-01 22:20:45.829135 cvxsimulator-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-01 22:20:45.913135 cvxsimulator-0.4.1/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0    14009 2023-06-01 22:20:45.913135 cvxsimulator-0.4.1/cvx/simulator/builder.py
+-rw-r--r--   0        0        0     1553 2023-06-01 22:20:45.913135 cvxsimulator-0.4.1/cvx/simulator/grid.py
+-rw-r--r--   0        0        0     1148 2023-06-01 22:20:45.913135 cvxsimulator-0.4.1/cvx/simulator/metrics.py
+-rw-r--r--   0        0        0     1457 2023-06-01 22:20:45.913135 cvxsimulator-0.4.1/cvx/simulator/month.py
+-rw-r--r--   0        0        0    19235 2023-06-01 22:20:45.913135 cvxsimulator-0.4.1/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      512 2023-06-01 22:20:45.913135 cvxsimulator-0.4.1/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      608 2023-06-01 22:21:10.857277 cvxsimulator-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5651 1970-01-01 00:00:00.000000 cvxsimulator-0.4.1/PKG-INFO
```

### Comparing `cvxsimulator-0.4.0/LICENSE` & `cvxsimulator-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.4.0/README.md` & `cvxsimulator-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.4.0/cvx/simulator/builder.py` & `cvxsimulator-0.4.1/cvx/simulator/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     prices: a pandas Series object containing the stock prices of the current portfolio state
     position: a pandas Series object containing the current holdings of the portfolio
     cash: the amount of cash available in the portfolio.
 
     By default, prices and position are set to None, while cash is set to 1 million.
     These attributes can be updated and accessed through setter and getter methods
     """
+
     prices: pd.Series = None
     position: pd.Series = None
     cash: float = 1e6
 
     @property
     def value(self):
         """
@@ -79,15 +80,15 @@
         as the product of the current position and the current stock prices,
         divided by the net asset value of the portfolio (as computed by the nav method).
         Note that this weighting represents the fraction of the portfolio value allocated to a particular asset.
         If the portfolio weighting cannot be computed due to missing positions,
         then a series of zeroes with the same size as the prices attribute is returned instead.
         """
         try:
-            return (self.prices * self.position)/self.nav
+            return (self.prices * self.position) / self.nav
         except TypeError:
             return 0 * self.prices
 
     @property
     def leverage(self):
         """
         The `leverage` method computes the leverage of the portfolio,
@@ -129,23 +130,23 @@
         cash: the new amount of cash in the portfolio after any trades and trading costs are applied.
 
         Note that the method does not return any value: instead,
         it updates the internal state of the _State instance.
         """
         if self.position is None:
             self.position = 0.0 * position
-            #trades = position
-        #else:
+            # trades = position
+        # else:
         trades = position - self.position
 
         self.position = position
         self.cash -= (trades * self.prices).sum()
 
         if model is not None:
-            self.cash -= model.eval(self.prices,  trades=trades, **kwargs).sum()
+            self.cash -= model.eval(self.prices, trades=trades, **kwargs).sum()
 
         return self
 
 
 def builder(prices, weights=None, initial_cash=1e6, trading_cost_model=None):
     """The builder function creates an instance of the _Builder class, which
     is used to construct a portfolio of assets. The function takes in a pandas
@@ -160,18 +161,24 @@
     set_weights method of the _Builder object. The final output is the
     constructed _Builder object."""
 
     assert isinstance(prices, pd.DataFrame)
     assert prices.index.is_monotonic_increasing
     assert prices.index.is_unique
 
-    stocks = pd.DataFrame(index=prices.index, columns=prices.columns, data=0.0, dtype=float)
-
-    builder = _Builder(stocks=stocks, prices=prices.ffill(), initial_cash=float(initial_cash),
-                    trading_cost_model=trading_cost_model)
+    stocks = pd.DataFrame(
+        index=prices.index, columns=prices.columns, data=0.0, dtype=float
+    )
+
+    builder = _Builder(
+        stocks=stocks,
+        prices=prices.ffill(),
+        initial_cash=float(initial_cash),
+        trading_cost_model=trading_cost_model,
+    )
 
     if weights is not None:
         for t, state in builder:
             builder.set_weights(time=t[-1], weights=weights.loc[t[-1]])
 
     return builder
 
@@ -197,37 +204,37 @@
         that can only be performed after the object is fully initialized. __post_init__
         is called automatically after the object initialization.
         """
         self._state.cash = self.initial_cash
 
     @property
     def index(self):
-        """ A property that returns the index of the portfolio,
+        """A property that returns the index of the portfolio,
         which is the time period for which the portfolio data is available.
 
         Returns: pd.Index: A pandas index representing the
         time period for which the portfolio data is available.
 
         Notes: The function extracts the index of the prices dataframe,
         which represents the time periods for which data is available for the portfolio.
         The resulting index will be a pandas index object
-        with the same length as the number of rows in the prices dataframe. """
+        with the same length as the number of rows in the prices dataframe."""
 
         return self.prices.index
 
     @property
     def assets(self):
-        """ A property that returns a list of the assets held by the portfolio.
+        """A property that returns a list of the assets held by the portfolio.
 
         Returns: list: A list of the assets held by the portfolio.
 
         Notes: The function extracts the column names of the prices dataframe,
         which correspond to the assets held by the portfolio.
         The resulting list will contain the names of all assets
-        held by the portfolio, without any duplicates. """
+        held by the portfolio, without any duplicates."""
         return self.prices.columns
 
     def set_weights(self, time, weights):
         """
         Set the position via weights (e.g. fractions of the nav)
 
         :param time: time
@@ -294,34 +301,36 @@
         assert isinstance(position, pd.Series)
         assert set(position.index).issubset(set(self.assets))
 
         self.stocks.loc[time, position.index] = position
         self._state.update(position, model=self.trading_cost_model)
 
     def __getitem__(self, time):
-        """ The __getitem__ method retrieves the stock data for a specific time in the dataframe.
+        """The __getitem__ method retrieves the stock data for a specific time in the dataframe.
         It returns the stock data for that time. The method takes one input parameter:
 
         time: the time index for which to retrieve the stock data
         Returns: stock data for the input time
 
         Note that the input time must be in the index of the dataframe, otherwise a KeyError will be raised.
         """
         return self.stocks.loc[time]
 
     def build(self):
-        """ A function that creates a new instance of the EquityPortfolio
+        """A function that creates a new instance of the EquityPortfolio
         class based on the internal state of the Portfolio builder object.
 
         Returns: EquityPortfolio: A new instance of the EquityPortfolio class
         with the attributes (prices, stocks, initial_cash, trading_cost_model) as specified in the Portfolio builder.
 
         Notes: The function simply creates a new instance of the EquityPortfolio
         class with the attributes (prices, stocks, initial_cash, trading_cost_model) equal
         to the corresponding attributes in the Portfolio builder object.
-        The resulting EquityPortfolio object will have the same state as the Portfolio builder from which it was built. """
-
-        return EquityPortfolio(prices=self.prices,
-                               stocks=self.stocks,
-                               initial_cash=self.initial_cash,
-                               trading_cost_model=self.trading_cost_model)
+        The resulting EquityPortfolio object will have the same state as the Portfolio builder from which it was built.
+        """
 
+        return EquityPortfolio(
+            prices=self.prices,
+            stocks=self.stocks,
+            initial_cash=self.initial_cash,
+            trading_cost_model=self.trading_cost_model,
+        )
```

### Comparing `cvxsimulator-0.4.0/cvx/simulator/grid.py` & `cvxsimulator-0.4.1/cvx/simulator/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pandas as pd
 import numpy as np
 
+
 def iron_frame(frame, rule):
     """
     The iron_frame function takes a pandas DataFrame
     and keeps it constant on a coarser grid.
 
     :param frame: The frame to be ironed
     :param rule: The rule to be used for the construction of the grid
```

### Comparing `cvxsimulator-0.4.0/cvx/simulator/metrics.py` & `cvxsimulator-0.4.1/cvx/simulator/metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 
 @dataclass(frozen=True)
 class Metrics:
     """
     Metrics class for a portfolio
     """
+
     daily_profit: pd.Series
     days_per_year: int = 252
 
     def __post_init__(self):
         # check there are no NaNs in the profit series
         assert not self.daily_profit.isnull().values.any()
         assert self.days_per_year > 0
@@ -40,9 +41,8 @@
 
     @property
     def sr_profit(self):
         """
         Computes the Sharpe ratio of daily profits
         """
         # print(self.mean_profit)
-        return self.mean_profit * np.sqrt(self.days_per_year) \
-               / self.std_profit
+        return self.mean_profit * np.sqrt(self.days_per_year) / self.std_profit
```

### Comparing `cvxsimulator-0.4.0/cvx/simulator/month.py` & `cvxsimulator-0.4.1/cvx/simulator/month.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from __future__ import annotations
 
 import calendar
 
 import numpy as np
 import pandas as pd
 
+
 def _compound(rets):
     """
     Helper function for compounded return calculation.
     """
     return (1.0 + rets).prod() - 1.0
 
 
@@ -27,23 +28,27 @@
         DataFrame with monthly returns, their STDev and YTD.
     """
 
     # Works better in the first month
     # Compute all the intramonth-returns, instead of reapplying some monthly resampling of the NAV
     returns = returns.dropna()
 
-    return_monthly = returns.groupby([returns.index.year, returns.index.month]).apply(
-        _compound
-    ).unstack(level=1)
+    return_monthly = (
+        returns.groupby([returns.index.year, returns.index.month])
+        .apply(_compound)
+        .unstack(level=1)
+    )
 
     # make sure all months are in the table!
     frame = pd.DataFrame(index=return_monthly.index, columns=range(1, 13), data=np.NaN)
     frame[return_monthly.columns] = return_monthly
 
-    frame = frame.rename(columns={month: calendar.month_abbr[month] for month in frame.columns})
+    frame = frame.rename(
+        columns={month: calendar.month_abbr[month] for month in frame.columns}
+    )
 
     ytd = frame.apply(_compound, axis=1)
     frame["STDev"] = np.sqrt(12) * frame.std(axis=1)
     # make sure that you don't include the column for the STDev in your computation
     frame["YTD"] = ytd
     frame.index.name = "Year"
     frame.columns.name = None
```

### Comparing `cvxsimulator-0.4.0/cvx/simulator/portfolio.py` & `cvxsimulator-0.4.1/cvx/simulator/portfolio.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,25 @@
 
 def diff(portfolio1, portfolio2, initial_cash=1e6, trading_cost_model=None):
     # check both portfolios are on the same price grid
     pd.testing.assert_frame_equal(portfolio1.prices, portfolio2.prices)
 
     stocks = portfolio1.stocks - portfolio2.stocks
 
-    return EquityPortfolio(prices=portfolio1.prices, stocks=stocks, initial_cash=initial_cash, trading_cost_model=trading_cost_model)
+    return EquityPortfolio(
+        prices=portfolio1.prices,
+        stocks=stocks,
+        initial_cash=initial_cash,
+        trading_cost_model=trading_cost_model,
+    )
 
 
 @dataclass(frozen=True)
 class EquityPortfolio:
-    """ A class that represents an equity portfolio
+    """A class that represents an equity portfolio
     and contains dataframes for prices and stock holdings,
     as well as optional parameters for trading cost models
     and initial cash values.
 
     Attributes:
         prices (pd.DataFrame): A pandas dataframe representing
         the prices of various assets held by the portfolio over time.
@@ -43,75 +48,76 @@
 
     prices: pd.DataFrame
     stocks: pd.DataFrame
     trading_cost_model: TradingCostModel = None
     initial_cash: float = 1e6
 
     def __post_init__(self):
-        """ A class method that performs input validation after object initialization.
+        """A class method that performs input validation after object initialization.
         Notes: The post_init method is called after an instance of the EquityPortfolio class has been initialized,
         and performs a series of input validation checks to ensure that the prices
         and stocks dataframes are in the expected format
         with no duplicates or missing data,
         and that the stocks dataframe represents valid equity positions
         for the assets held in the portfolio.
         Specifically, the method checks that both the prices and stocks dataframes
         have a monotonic increasing and unique index,
         and that the index and columns of the stocks dataframe are subsets
         of the index and columns of the prices dataframe, respectively.
-        If any of these checks fail, an assertion error will be raised. """
+        If any of these checks fail, an assertion error will be raised."""
 
         assert self.prices.index.is_monotonic_increasing
         assert self.prices.index.is_unique
         assert self.stocks.index.is_monotonic_increasing
         assert self.stocks.index.is_unique
 
         assert set(self.stocks.index).issubset(set(self.prices.index))
         assert set(self.stocks.columns).issubset(set(self.prices.columns))
 
     @property
     def index(self):
-        """ A property that returns the index of the EquityPortfolio instance,
+        """A property that returns the index of the EquityPortfolio instance,
         which is the time period for which the portfolio data is available.
 
         Returns: pd.Index: A pandas index representing the time period for which the
         portfolio data is available.
 
         Notes: The function extracts the index of the prices dataframe,
         which represents the time periods for which data is available for the portfolio.
         The resulting index will be a pandas index object with the same length
         as the number of rows in the prices dataframe."""
         return self.prices.index
 
     @property
     def assets(self):
-        """ A property that returns a list of the assets held by the EquityPortfolio object.
+        """A property that returns a list of the assets held by the EquityPortfolio object.
 
         Returns: list: A list of the assets held by the EquityPortfolio object.
 
         Notes: The function extracts the column names of the prices dataframe,
         which correspond to the assets held by the EquityPortfolio object.
-        The resulting list will contain the names of all assets held by the portfolio, without any duplicates. """
+        The resulting list will contain the names of all assets held by the portfolio, without any duplicates.
+        """
         return self.prices.columns
 
     @property
     def weights(self):
-        """ A property that returns a pandas dataframe representing
+        """A property that returns a pandas dataframe representing
         the weights of various assets in the portfolio.
 
         Returns: pd.DataFrame: A pandas dataframe representing the weights
         of various assets in the portfolio.
 
         Notes: The function calculates the weights of various assets
         in the portfolio by dividing the equity positions
         for each asset (as represented in the equity dataframe)
         by the total portfolio value (as represented in the nav dataframe).
         Both dataframes are assumed to have the same dimensions.
         The resulting dataframe will show the relative weight
-        of each asset in the portfolio at each point in time. """
+        of each asset in the portfolio at each point in time."""
         return self.equity.apply(lambda x: x / self.nav)
 
     def __getitem__(self, time):
         """The `__getitem__` method retrieves the stock data for a specific time in the dataframe.
         It returns the stock data for that time.
 
         The method takes one input parameter:
@@ -122,112 +128,118 @@
 
         Note that the input time must be in the index of the dataframe,
         otherwise a KeyError will be raised."""
         return self.stocks.loc[time]
 
     @property
     def trading_costs(self):
-        """ A property that returns a pandas dataframe
+        """A property that returns a pandas dataframe
         representing the trading costs incurred by the portfolio due to trades made.
 
         Returns: pd.DataFrame: A pandas dataframe representing the trading
         costs incurred by the portfolio due to trades made.
 
         Notes: The function calculates the trading costs using the specified
         trading cost model (if available) and the prices and trading
         data represented by the prices and trades_stocks
         dataframes, respectively. If no trading cost model is provided,
         a dataframe with all zeros will be returned.
         The resulting dataframe will have the same dimensions as
         the prices and trades_stocks dataframes,
-        showing the trading costs incurred at each point in time for each asset traded. """
+        showing the trading costs incurred at each point in time for each asset traded.
+        """
         if self.trading_cost_model is None:
             return 0.0 * self.prices
 
         return self.trading_cost_model.eval(self.prices, self.trades_stocks)
 
     @property
     def equity(self) -> pd.DataFrame:
-        """ A property that returns a pandas dataframe
+        """A property that returns a pandas dataframe
         representing the equity positions of the portfolio,
         which is the value of each asset held by the portfolio.
         Returns: pd.DataFrame: A pandas dataframe representing
         the equity positions of the portfolio.
 
         Notes: The function calculates the equity of the portfolio
         by multiplying the current prices of each asset
         by the number of shares held by the portfolio.
         The resulting values are filled forward to account
         for any missing data or NaN values.
         The equity dataframe will have the same dimensions
-        as the prices and stocks dataframes. """
+        as the prices and stocks dataframes."""
 
         return (self.prices * self.stocks).ffill()
 
     @property
     def trades_stocks(self) -> pd.DataFrame:
-        """ A property that returns a pandas dataframe representing the trades made in the portfolio in terms of stocks.
+        """A property that returns a pandas dataframe representing the trades made in the portfolio in terms of stocks.
 
         Returns: pd.DataFrame: A pandas dataframe representing the trades made in the portfolio in terms of stocks.
 
         Notes: The function calculates the trades made by the portfolio by taking
         the difference between the current and previous values of the stocks dataframe.
         The resulting values will represent the number of shares of each asset
         bought or sold by the portfolio at each point in time.
         The resulting dataframe will have the same dimensions
-        as the stocks dataframe, with NaN values filled with zeros. """
+        as the stocks dataframe, with NaN values filled with zeros."""
         t = self.stocks.diff()
         t.loc[self.index[0]] = self.stocks.loc[self.index[0]]
         return t.fillna(0.0)
 
     @property
     def trades_currency(self) -> pd.DataFrame:
-        """ A property that returns a pandas dataframe representing the trades made in the portfolio in terms of currency.
+        """A property that returns a pandas dataframe representing the trades made in the portfolio in terms of currency.
 
         Returns: pd.DataFrame: A pandas dataframe representing the trades made in the portfolio in terms of currency.
 
         Notes: The function calculates the trades made in currency by multiplying
         the number of shares of each asset bought or sold (as represented in the trades_stocks dataframe)
         with the current prices of each asset (as represented in the prices dataframe).
         Uses pandas ffill() method to forward fill NaN values in the prices dataframe.
-        The resulting dataframe will have the same dimensions as the stocks and prices dataframes. """
+        The resulting dataframe will have the same dimensions as the stocks and prices dataframes.
+        """
         return self.trades_stocks * self.prices.ffill()
 
     @property
     def turnover(self) -> pd.DataFrame:
         return self.trades_currency.abs()
 
     @property
     def cash(self) -> pd.Series:
-        """ A property that returns a pandas series representing the cash on hand in the portfolio.
+        """A property that returns a pandas series representing the cash on hand in the portfolio.
 
         Returns: pd.Series: A pandas series representing the cash on hand in the portfolio.
 
         Notes: The function calculates the cash available in the portfolio by subtracting
         the sum of trades currency and cumulative trading costs from the initial cash value specified
         when constructing the object. Uses pandas cumsum() method
         to calculate the cumulative sum of trading costs and
         trades currency along the time axis.
         The resulting series will show how much money is available for further trades at each point in time.
         """
-        return self.initial_cash - self.trades_currency.sum(axis=1).cumsum() - self.trading_costs.sum(axis=1).cumsum()
+        return (
+            self.initial_cash
+            - self.trades_currency.sum(axis=1).cumsum()
+            - self.trading_costs.sum(axis=1).cumsum()
+        )
 
     @property
     def nav(self) -> pd.Series:
-        """ Returns a pandas series representing the total value
+        """Returns a pandas series representing the total value
         of the portfolio's investments and cash.
 
         Returns: pd.Series: A pandas series representing the
                             total value of the portfolio's investments and cash.
         """
         return self.equity.sum(axis=1) + self.cash
 
     @property
     def profit(self) -> pd.Series:
-        """ A property that returns a pandas series representing the
+        """A property that returns a pandas series representing the
         profit gained or lost in the portfolio based on changes in asset prices.
 
         Returns: pd.Series: A pandas series representing the profit
         gained or lost in the portfolio based on changes in asset prices.
 
         Notes: The calculation is based on the difference between
         the previous and current prices of the assets in the portfolio,
@@ -236,103 +248,141 @@
 
         price_changes = self.prices.ffill().diff()
         previous_stocks = self.stocks.shift(1).fillna(0.0)
         return (previous_stocks * price_changes).dropna(axis=0, how="all").sum(axis=1)
 
     @property
     def highwater(self) -> pd.Series:
-        """ A function that returns a pandas series representing
+        """A function that returns a pandas series representing
         the high-water mark of the portfolio, which is the highest point
         the portfolio value has reached over time.
 
         Returns: pd.Series: A pandas series representing the
         high-water mark of the portfolio.
 
         Notes: The function performs a rolling computation based on
         the cumulative maximum of the portfolio's value over time,
         starting from the beginning of the time period being considered.
         Min_periods argument is set to 1 to include the minimum period of one day.
-        The resulting series will show the highest value the portfolio has reached at each point in time. """
+        The resulting series will show the highest value the portfolio has reached at each point in time.
+        """
         return self.nav.expanding(min_periods=1).max()
 
     @property
     def drawdown(self) -> pd.Series:
-        """ A property that returns a pandas series representing the
+        """A property that returns a pandas series representing the
         drawdown of the portfolio, which measures the decline
         in the portfolio's value from its (previously) highest
         point to its current point.
 
         Returns: pd.Series: A pandas series representing the
         drawdown of the portfolio.
 
         Notes: The function calculates the ratio of the portfolio's current value
         vs. its current high-water-mark and then subtracting the result from 1.
         A positive drawdown means the portfolio is currently worth
-        less than its high-water mark. A drawdown of 0.1 implies that the nav is currently 0.9 times the high-water mark """
+        less than its high-water mark. A drawdown of 0.1 implies that the nav is currently 0.9 times the high-water mark
+        """
         return 1.0 - self.nav / self.highwater
 
     def __mul__(self, scalar):
-        """ A method that allows multiplication of the EquityPortfolio object with a scalar constant.
+        """A method that allows multiplication of the EquityPortfolio object with a scalar constant.
 
         Args: scalar: A scalar constant that multiplies the number of shares
         of each asset held in the EquityPortfolio object.
 
         Returns: EquityPortfolio: A new EquityPortfolio object multiplied by the scalar constant.
 
         Notes: The mul method allows multiplication of an EquityPortfolio object
         with a scalar constant to increase or decrease
         the number of shares held for each asset in the portfolio accordingly.
         The method returns a new EquityPortfolio object with the same prices
         and trading cost model as the original object,
         and with the number of shares for each asset multiplied by the scalar constant
         (as represented in the stocks dataframe).
         Additionally, the initial cash value is multiplied
-        by the scalar to maintain the same cash-to-equity ratio as the original portfolio. """
+        by the scalar to maintain the same cash-to-equity ratio as the original portfolio.
+        """
         assert scalar > 0
-        return EquityPortfolio(prices=self.prices, stocks=self.stocks * scalar, initial_cash=self.initial_cash * scalar, trading_cost_model=self.trading_cost_model)
+        return EquityPortfolio(
+            prices=self.prices,
+            stocks=self.stocks * scalar,
+            initial_cash=self.initial_cash * scalar,
+            trading_cost_model=self.trading_cost_model,
+        )
 
     def __rmul__(self, scalar):
-        """ A method that allows multiplication of the EquityPortfolio object with a scalar constant in a reversed order.
+        """A method that allows multiplication of the EquityPortfolio object with a scalar constant in a reversed order.
 
         Args: scalar: A scalar constant that multiplies the EquityPortfolio object in a reversed order.
 
         Returns: EquityPortfolio: A new EquityPortfolio object multiplied by the scalar constant.
 
         Notes: The rmul method allows multiplication of a scalar
         constant with an EquityPortfolio object in a reversed order"""
         return self.__mul__(scalar)
 
-    # def __sub__(self, other):
-    #     return self.__add__(-1 * other)
-
     def __add__(self, port_new):
+        """
+        A method that allows addition of two EquityPortfolio objects.
+        """
+        # check if the other object is an EquityPortfolio object
         assert isinstance(port_new, EquityPortfolio)
 
-        assets = self.assets.union(port_new.assets)
-        index = self.index.union(port_new.index)
+        # make sure the prices are aligned for overlapping points
+        prices_left = self.prices.combine_first(port_new.prices)
+        prices_right = port_new.prices.combine_first(self.prices)
+        pd.testing.assert_frame_equal(prices_left, prices_right)
 
-        left = pd.DataFrame(index=index, columns=assets)
-        left.update(self.stocks)
-        # this is a problem...
-        left = left.fillna(0.0)
-
-        right = pd.DataFrame(index=index, columns=assets)
-        right.update(port_new.stocks)
-        right = right.fillna(0.0)
+        # bring both portfolios to the finer grid
+        left = self.reset_prices(prices=prices_left)
+        right = port_new.reset_prices(prices=prices_left)
+
+        # just make sure the left and right portfolio are now on exactly the same grid
+        pd.testing.assert_index_equal(left.index, right.index)
+
+        # add the stocks
+        positions = left.stocks.add(right.stocks, fill_value=0.0)
+
+        # make sure the trading cost models are the same
+        return EquityPortfolio(
+            prices=prices_right,
+            stocks=positions,
+            initial_cash=self.initial_cash + port_new.initial_cash,
+            trading_cost_model=self.trading_cost_model,
+        )
 
-        positions = left + right
+    def reset_prices(self, prices):
+        """
+        A method that constructs an EquityPortfolio object using finer prices.
+        """
+        # extract the relevant columns from prices
+        p = prices[self.assets]
 
-        prices_left = self.prices.combine_first(port_new.prices)
-        prices_right = port_new.prices.combine_first(self.prices)
+        # the prices need to contain the original index
+        assert set(self.index).issubset(set(prices.index))
 
-        pd.testing.assert_frame_equal(prices_left, prices_right)
+        # build a frame for the stocks
+        stocks = pd.DataFrame(index=prices.index, columns=self.assets)
 
-        return EquityPortfolio(prices=prices_right, stocks=positions,
-                               initial_cash=self.initial_cash + port_new.initial_cash,
-                               trading_cost_model=self.trading_cost_model)
+        # only forward fill stocks on the subgrid induced by the original index
+        sub = stocks.truncate(before=self.index[0], after=self.index[-1])
+        sub.update(self.stocks)
+        sub = sub.ffill()
+
+        # outside the original index, the stocks are zero
+        stocks.update(sub)
+        stocks = stocks.fillna(0.0)
+
+        return EquityPortfolio(
+            prices=p,
+            stocks=stocks,
+            initial_cash=self.initial_cash,
+            trading_cost_model=self.trading_cost_model,
+        )
 
     def truncate(self, before=None, after=None):
         """
         The truncate method truncates the prices DataFrame, stocks DataFrame
         and the cash series of an EquityPortfolio object.
         The method also optionally accepts a before and/or after argument
         to specify a date range for truncation.
@@ -347,18 +397,20 @@
 
         Note that this method does not modify the original EquityPortfolio object,
         but rather returns a new object.
         :param before:
         :param after:
         :return:
         """
-        return EquityPortfolio(prices=self.prices.truncate(before=before, after=after),
-                               stocks=self.stocks.truncate(before=before, after=after),
-                               trading_cost_model=self.trading_cost_model,
-                               initial_cash=self.nav.truncate(before=before, after=after).values[0])
+        return EquityPortfolio(
+            prices=self.prices.truncate(before=before, after=after),
+            stocks=self.stocks.truncate(before=before, after=after),
+            trading_cost_model=self.trading_cost_model,
+            initial_cash=self.nav.truncate(before=before, after=after).values[0],
+        )
 
     # @property
     # def start(self):
     #     """first index with a profit that is not zero"""
     #     return self.profit.ne(0).idxmax()
 
     def resample(self, rule):
@@ -370,11 +422,13 @@
 
         Note that the resample method does not modify the original EquityPortfolio object,
         but rather returns a new object.
         """
         # iron out the stocks index
         stocks = iron_frame(self.stocks, rule=rule)
 
-        return EquityPortfolio(prices=self.prices,
-                               stocks=stocks,
-                               trading_cost_model=self.trading_cost_model,
-                               initial_cash=self.initial_cash)
+        return EquityPortfolio(
+            prices=self.prices,
+            stocks=stocks,
+            trading_cost_model=self.trading_cost_model,
+            initial_cash=self.initial_cash,
+        )
```

### Comparing `cvxsimulator-0.4.0/cvx/simulator/trading_costs.py` & `cvxsimulator-0.4.1/cvx/simulator/trading_costs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import abc
 
 
 @dataclass(frozen=True)
 class TradingCostModel(abc.ABC):
     @abc.abstractmethod
     def eval(self, prices, trades, **kwargs):
-        """ Evaluates the cost of a trade given the prices and the trades """
+        """Evaluates the cost of a trade given the prices and the trades"""
 
 
 @dataclass(frozen=True)
 class LinearCostModel(TradingCostModel):
     factor: float = 0.0
     bias: float = 0.0
```

### Comparing `cvxsimulator-0.4.0/pyproject.toml` & `cvxsimulator-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxsimulator"
-version = "v0.4.0"
+version = "v0.4.1"
 description = "Simple simulator for investors"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/simulator"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cvxsimulator-0.4.0/PKG-INFO` & `cvxsimulator-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.4.0
+Version: 0.4.1
 Summary: Simple simulator for investors
 Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

