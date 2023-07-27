# Comparing `tmp/cvxsimulator-0.6.3.tar.gz` & `tmp/cvxsimulator-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.6.3.tar", max compression
+gzip compressed data, was "cvxsimulator-0.7.0.tar", max compression
```

## Comparing `cvxsimulator-0.6.3.tar` & `cvxsimulator-0.7.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0    10790 2023-07-27 03:11:23.671758 cvxsimulator-0.6.3/LICENSE
--rw-r--r--   0        0        0     5741 2023-07-27 03:11:23.671758 cvxsimulator-0.6.3/README.md
--rw-r--r--   0        0        0        0 2023-07-27 03:11:23.747761 cvxsimulator-0.6.3/cvx/simulator/__init__.py
--rw-r--r--   0        0        0    15121 2023-07-27 03:11:23.747761 cvxsimulator-0.6.3/cvx/simulator/builder.py
--rw-r--r--   0        0        0     1613 2023-07-27 03:11:23.747761 cvxsimulator-0.6.3/cvx/simulator/grid.py
--rw-r--r--   0        0        0     1559 2023-07-27 03:11:23.747761 cvxsimulator-0.6.3/cvx/simulator/month.py
--rw-r--r--   0        0        0    23615 2023-07-27 03:11:23.751763 cvxsimulator-0.6.3/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      795 2023-07-27 03:11:23.751763 cvxsimulator-0.6.3/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0     1114 2023-07-27 03:11:59.242169 cvxsimulator-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     6388 1970-01-01 00:00:00.000000 cvxsimulator-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0    10790 2023-07-27 23:00:04.962563 cvxsimulator-0.7.0/LICENSE
+-rw-r--r--   0        0        0     5741 2023-07-27 23:00:04.962563 cvxsimulator-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 23:00:05.026564 cvxsimulator-0.7.0/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0    15915 2023-07-27 23:00:05.026564 cvxsimulator-0.7.0/cvx/simulator/builder.py
+-rw-r--r--   0        0        0     1924 2023-07-27 23:00:05.026564 cvxsimulator-0.7.0/cvx/simulator/grid.py
+-rw-r--r--   0        0        0     1570 2023-07-27 23:00:05.026564 cvxsimulator-0.7.0/cvx/simulator/month.py
+-rw-r--r--   0        0        0    24512 2023-07-27 23:00:05.026564 cvxsimulator-0.7.0/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      965 2023-07-27 23:00:05.026564 cvxsimulator-0.7.0/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      474 2023-07-27 23:00:05.026564 cvxsimulator-0.7.0/cvx/simulator/types.py
+-rw-r--r--   0        0        0     1114 2023-07-27 23:00:37.311171 cvxsimulator-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6388 1970-01-01 00:00:00.000000 cvxsimulator-0.7.0/PKG-INFO
```

### Comparing `cvxsimulator-0.6.3/LICENSE` & `cvxsimulator-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.6.3/README.md` & `cvxsimulator-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.6.3/cvx/simulator/builder.py` & `cvxsimulator-0.7.0/cvx/simulator/builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Optional
+from datetime import datetime
+from typing import Any, Generator, Optional, Tuple
 
 import pandas as pd
 
 from cvx.simulator.portfolio import EquityPortfolio
 from cvx.simulator.trading_costs import TradingCostModel
 
 
@@ -29,38 +30,38 @@
     """
 
     prices: pd.Series = None
     position: pd.Series = None
     cash: float = 1e6
 
     @property
-    def value(self):
+    def value(self) -> float:
         """
         The value property computes the value of the portfolio at the current
         time taking into account the current holdings and current stock prices.
         If the value cannot be computed due to missing positions
         (they might be still None), zero is returned instead.
         """
         try:
-            return (self.prices * self.position).sum()
+            return float((self.prices * self.position).sum())
         except TypeError:
             return 0.0
 
     @property
-    def nav(self):
+    def nav(self) -> float:
         """
         The nav property computes the net asset value (NAV) of the portfolio,
         which is the sum of the current value of the
         portfolio as determined by the value property,
         and the current amount of cash available in the portfolio.
         """
         return self.value + self.cash
 
     @property
-    def weights(self):
+    def weights(self) -> pd.Series:
         """
         The weights property computes the weighting of each asset in the current
         portfolio as a fraction of the total portfolio value (nav).
 
         Returns:
 
         a pandas series object containing the weighting of each asset as a
@@ -69,33 +70,38 @@
         """
         try:
             return (self.prices * self.position) / self.nav
         except TypeError:
             return 0 * self.prices
 
     @property
-    def leverage(self):
+    def leverage(self) -> float:
         """
         The `leverage` property computes the leverage of the portfolio,
         which is the sum of the absolute values of the portfolio weights.
         """
-        return self.weights.abs().sum()
+        return float(self.weights.abs().sum())
 
     @property
-    def position_robust(self):
+    def position_robust(self) -> pd.Series:
         """
         The position_robust property returns the current position of the
         portfolio or a series of zeroes if the position is still missing.
         """
         if self.position is None:
             self.position = 0.0 * self.prices
 
         return self.position
 
-    def update(self, position, model=None, **kwargs):
+    def update(
+        self,
+        position: pd.Series,
+        model: Optional[TradingCostModel] = None,
+        **kwargs: Any,
+    ) -> _State:
         """
         The update method updates the current state of the portfolio with the
         new input position. It calculates the trades made based on the new
         and the previous position, updates the internal position and
         cash attributes, and applies any trading costs according to a model parameter.
 
         The method takes three input parameters:
@@ -130,25 +136,25 @@
             self.cash -= model.eval(self.prices, trades=trades, **kwargs).sum()
 
         # builder is frozen, so we can't construct a new state
         return self
 
 
 def builder(
-    prices,
-    weights=None,
-    market_cap=None,
-    trade_volume=None,
-    initial_cash=1e6,
-    trading_cost_model=None,
-    max_cap_fraction=None,
-    min_cap_fraction=None,
-    max_trade_fraction=None,
-    min_trade_fraction=None,
-):
+    prices: pd.DataFrame,
+    weights: Optional[pd.DataFrame] = None,
+    market_cap: Optional[pd.DataFrame] = None,
+    trade_volume: Optional[pd.DataFrame] = None,
+    initial_cash: float = 1e6,
+    trading_cost_model: Optional[TradingCostModel] = None,
+    max_cap_fraction: Optional[float] = None,
+    min_cap_fraction: Optional[float] = None,
+    max_trade_fraction: Optional[float] = None,
+    min_trade_fraction: Optional[float] = None,
+) -> _Builder:
     """The builder function creates an instance of the _Builder class, which
     is used to construct a portfolio of assets. The function takes in a pandas
     DataFrame of historical prices for the assets in the portfolio, optional
     weights for each asset, an initial cash value, and a trading cost model.
     The function first asserts that the prices DataFrame has a monotonic
     increasing and unique index. It then creates a DataFrame of zeros to hold
     the number of shares of each asset owned at each time step. The function
@@ -186,25 +192,25 @@
     return builder
 
 
 @dataclass(frozen=True)
 class _Builder:
     prices: pd.DataFrame
     stocks: pd.DataFrame
-    trading_cost_model: TradingCostModel
+    trading_cost_model: Optional[TradingCostModel] = None
     initial_cash: float = 1e6
     _state: _State = field(default_factory=_State)
     market_cap: pd.DataFrame = None
     trade_volume: pd.DataFrame = None
     max_cap_fraction: Optional[float] = None
     min_cap_fraction: Optional[float] = None
     max_trade_fraction: Optional[float] = None
     min_trade_fraction: Optional[float] = None
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         """
         The __post_init__ method is a special method of initialized instances
         of the _Builder class and is called after initialization.
         It sets the initial amount of cash in the portfolio to be equal to the input initial_cash parameter.
 
         The method takes no input parameter. It initializes the cash attribute in the internal
         _State object with the initial amount of cash in the portfolio, self.initial_cash.
@@ -212,86 +218,88 @@
         Note that this method is often used in Python classes for additional initialization routines
         that can only be performed after the object is fully initialized. __post_init__
         is called automatically after the object initialization.
         """
         self._state.cash = self.initial_cash
 
     @property
-    def index(self):
+    def index(self) -> pd.DatetimeIndex:
         """A property that returns the index of the portfolio,
         which is the time period for which the portfolio data is available.
 
         Returns: pd.Index: A pandas index representing the
         time period for which the portfolio data is available.
 
         Notes: The function extracts the index of the prices dataframe,
         which represents the time periods for which data is available for the portfolio.
         The resulting index will be a pandas index object
         with the same length as the number of rows in the prices dataframe."""
 
-        return self.prices.index
+        return pd.DatetimeIndex(self.prices.index)
 
     @property
-    def assets(self):
+    def assets(self) -> pd.Index:
         """A property that returns a list of the assets held by the portfolio.
 
         Returns: list: A list of the assets held by the portfolio.
 
         Notes: The function extracts the column names of the prices dataframe,
         which correspond to the assets held by the portfolio.
         The resulting list will contain the names of all assets
         held by the portfolio, without any duplicates."""
         return self.prices.columns
 
     @property
-    def returns(self):
+    def returns(self) -> pd.DataFrame:
         return self.prices.pct_change().dropna(axis=0, how="all")
 
-    def cov(self, **kwargs):
+    def cov(
+        self, **kwargs: Any
+    ) -> Generator[Tuple[datetime, pd.DataFrame], None, None]:
         # You can do much better using volatility adjusted returns rather than returns
         cov = self.returns.ewm(**kwargs).cov()
         cov = cov.dropna(how="all", axis=0)
         for t in cov.index.get_level_values(level=0).unique():
             yield t, cov.loc[t, :, :]
 
         # {t: cov.loc[t, :, :] for t in cov.index.get_level_values('date').unique()}
 
-    def set_weights(self, time, weights: pd.Series):
+    def set_weights(self, time: datetime, weights: pd.Series) -> None:
         """
         Set the position via weights (e.g. fractions of the nav)
 
         :param time: time
         :param weights: series of weights
         """
         assert isinstance(weights, pd.Series), "weights must be a pandas Series"
         self[time] = (self._state.nav * weights) / self._state.prices
 
-    def set_cashposition(self, time, cashposition: pd.Series):
+    def set_cashposition(self, time: datetime, cashposition: pd.Series) -> None:
         """
         Set the position via cash positions (e.g. USD invested per asset)
 
         :param time: time
         :param cashposition: series of cash positions
         """
         assert isinstance(
             cashposition, pd.Series
         ), "cashposition must be a pandas Series"
         self[time] = cashposition / self._state.prices
 
-    def set_position(self, time, position):
+    def set_position(self, time: datetime, position: pd.Series) -> None:
         """
         Set the position via number of assets (e.g. number of stocks)
 
         :param time: time
         :param position: series of number of stocks
         """
         assert isinstance(position, pd.Series), "position must be a pandas Series"
         self[time] = position
 
-    def __iter__(self):
+    def __iter__(self) -> Generator[Tuple[pd.DatetimeIndex, _State], None, None]:
         """
         The __iter__ method allows the object to be iterated over in a for loop,
         yielding time and the current state of the portfolio.
         The method yields a list of dates seen so far
         (excluding the first date) and returns a tuple
         containing the list of dates and the current portfolio state.
 
@@ -303,15 +311,15 @@
         taking into account the stock prices at each interval.
         """
         for t in self.index:
             # valuation of the current position
             self._state.prices = self.prices.loc[t]
             yield self.index[self.index <= t], self._state
 
-    def __setitem__(self, time, position):
+    def __setitem__(self, time: datetime, position: pd.Series) -> None:
         """
         The method __setitem__ updates the stock data in the dataframe for a specific time index
         with the input position. It first checks that position is a valid input,
         meaning it is a pandas Series object and has its index within the assets of the dataframe.
         The method takes two input parameters:
 
         time: time index for which to update the stock data
@@ -363,26 +371,26 @@
             trade = trade / self._state.prices
             # compute position
             position = self._state.position_robust + trade
 
         self.stocks.loc[time, position.index] = position
         self._state.update(position, model=self.trading_cost_model)
 
-    def __getitem__(self, time):
+    def __getitem__(self, time: datetime) -> pd.Series:
         """The __getitem__ method retrieves the stock data for a specific time in the dataframe.
         It returns the stock data for that time. The method takes one input parameter:
 
         time: the time index for which to retrieve the stock data
         Returns: stock data for the input time
 
         Note that the input time must be in the index of the dataframe, otherwise a KeyError will be raised.
         """
         return self.stocks.loc[time]
 
-    def build(self):
+    def build(self) -> EquityPortfolio:
         """A function that creates a new instance of the EquityPortfolio
         class based on the internal state of the Portfolio builder object.
 
         Returns: EquityPortfolio: A new instance of the EquityPortfolio class
         with the attributes (prices, stocks, initial_cash, trading_cost_model) as specified in the Portfolio builder.
 
         Notes: The function simply creates a new instance of the EquityPortfolio
```

### Comparing `cvxsimulator-0.6.3/cvx/simulator/grid.py` & `cvxsimulator-0.7.0/cvx/simulator/grid.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,58 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
+from typing import Any
+
 import numpy as np
 import pandas as pd
 
 
-def iron_frame(frame, rule):
+def iron_frame(frame: pd.DataFrame, rule: Any) -> pd.DataFrame:
     """
     The iron_frame function takes a pandas DataFrame
     and keeps it constant on a coarser grid.
 
     :param frame: The frame to be ironed
     :param rule: The rule to be used for the construction of the grid
     :return: the ironed frame
     """
-    s_index = resample_index(frame.index, rule)
+    # frame = pd.DataFrame(frame)
+    # frame.index = pd.DatetimeIndex(frame.index)
+
+    s_index = resample_index(pd.DatetimeIndex(frame.index), rule)
     return _project_frame_to_grid(frame, s_index)
 
 
-def resample_index(index, rule):
+def resample_index(index: pd.DatetimeIndex, rule: Any) -> pd.DatetimeIndex:
     """
     The resample_index function resamples a pandas DatetimeIndex object
     to a lower frequency using a specified rule.
 
 
     Note that the function does not modify the input index object,
     but rather returns a pandas DatetimeIndex
     """
     series = pd.Series(index=index, data=index)
     a = series.resample(rule=rule).first()
     return pd.DatetimeIndex(a.values)
 
 
-def _project_frame_to_grid(frame, grid):
+def _project_frame_to_grid(frame: pd.DataFrame, grid: pd.DatetimeIndex) -> pd.DataFrame:
     """
     The project_frame_to_grid function projects a pandas DataFrame
     to a coarser grid while still sharing the same index.
     It does that by taking over values of the frame from the coarser
     grid that are then forward filled.
     An application would be monthly rebalancing of a portfolio.
     E.g. on days in a particular grid we adjust the position and keep
     it constant for the rest of the month.
 
     :param frame: the frame (existing on a finer grid)
     :param grid: the coarse grid
     :return: a frame changing only values on days in the grid
     """
     sample = np.NaN * frame
-    sample.loc[grid] = frame.loc[grid]
+    for t in grid:
+        sample.loc[t] = frame.loc[t]
+    # sample.loc[grid] = frame.loc[grid]
     return sample.ffill()
```

### Comparing `cvxsimulator-0.6.3/cvx/simulator/month.py` & `cvxsimulator-0.7.0/cvx/simulator/month.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # -*- coding: utf-8 -*-
 """
 Popular year vs month performance table.
 """
 from __future__ import annotations
 
 import calendar
-from datetime import datetime
-from typing import Dict
 
 import numpy as np
 import pandas as pd
 
+from cvx.simulator.types import TIMESERIES
 
-def _compound(rets):
+
+def _compound(rets) -> float:  # type: ignore
     """
     Helper function for compounded return calculation.
     """
-    return (1.0 + rets).prod() - 1.0
+    return float((1.0 + rets).prod() - 1.0)
 
 
-def monthlytable(returns: Dict[datetime, float]) -> pd.DataFrame:
+def monthlytable(returns: TIMESERIES) -> pd.DataFrame:
     """
     Get a table of monthly returns.
 
     Args:
         returns: Series of individual returns.
 
     Returns:
```

### Comparing `cvxsimulator-0.6.3/cvx/simulator/portfolio.py` & `cvxsimulator-0.7.0/cvx/simulator/portfolio.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 from dataclasses import dataclass
+from datetime import datetime
 from enum import Enum
-from typing import Optional
+from typing import Any, Optional, Tuple
 
 import pandas as pd
 import quantstats as qs
 
 from cvx.simulator.grid import iron_frame
 from cvx.simulator.trading_costs import TradingCostModel
 
@@ -32,20 +33,25 @@
     ROLLING_VOLATILITY = 14
     YEARLY_RETURNS = 15
 
     #
     # def __call__(self, returns, **kwargs):
     #     return self._func(returns=returns, **kwargs)
 
-    def plot(self, returns, **kwargs):
+    def plot(self, returns: pd.DataFrame, **kwargs: Any) -> Any:
         func = getattr(qs.plots, self.name.lower())
         return func(returns=returns, **kwargs)
 
 
-def diff(portfolio1, portfolio2, initial_cash=1e6, trading_cost_model=None):
+def diff(
+    portfolio1: EquityPortfolio,
+    portfolio2: EquityPortfolio,
+    initial_cash: float = 1e6,
+    trading_cost_model: Optional[TradingCostModel] = None,
+) -> EquityPortfolio:
     # check both portfolios are on the same price grid
     pd.testing.assert_frame_equal(portfolio1.prices, portfolio2.prices)
 
     stocks = portfolio1.stocks - portfolio2.stocks
 
     return EquityPortfolio(
         prices=portfolio1.prices,
@@ -82,15 +88,15 @@
     will be set to a default value of 1,000,000."""
 
     prices: pd.DataFrame
     stocks: pd.DataFrame
     trading_cost_model: Optional[TradingCostModel] = None
     initial_cash: float = 1e6
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         """A class method that performs input validation after object initialization.
         Notes: The post_init method is called after an instance of the EquityPortfolio class has been initialized,
         and performs a series of input validation checks to ensure that the prices
         and stocks dataframes are in the expected format
         with no duplicates or missing data,
         and that the stocks dataframe represents valid equity positions
         for the assets held in the portfolio.
@@ -105,41 +111,41 @@
         assert self.stocks.index.is_monotonic_increasing
         assert self.stocks.index.is_unique
 
         assert set(self.stocks.index).issubset(set(self.prices.index))
         assert set(self.stocks.columns).issubset(set(self.prices.columns))
 
     @property
-    def index(self):
+    def index(self) -> pd.DatetimeIndex:
         """A property that returns the index of the EquityPortfolio instance,
         which is the time period for which the portfolio data is available.
 
         Returns: pd.Index: A pandas index representing the time period for which the
         portfolio data is available.
 
         Notes: The function extracts the index of the prices dataframe,
         which represents the time periods for which data is available for the portfolio.
         The resulting index will be a pandas index object with the same length
         as the number of rows in the prices dataframe."""
-        return self.prices.index
+        return pd.DatetimeIndex(self.prices.index)
 
     @property
-    def assets(self):
+    def assets(self) -> pd.Index:
         """A property that returns a list of the assets held by the EquityPortfolio object.
 
         Returns: list: A list of the assets held by the EquityPortfolio object.
 
         Notes: The function extracts the column names of the prices dataframe,
         which correspond to the assets held by the EquityPortfolio object.
         The resulting list will contain the names of all assets held by the portfolio, without any duplicates.
         """
         return self.prices.columns
 
     @property
-    def weights(self):
+    def weights(self) -> pd.DataFrame:
         """A property that returns a pandas dataframe representing
         the weights of various assets in the portfolio.
 
         Returns: pd.DataFrame: A pandas dataframe representing the weights
         of various assets in the portfolio.
 
         Notes: The function calculates the weights of various assets
@@ -147,30 +153,30 @@
         for each asset (as represented in the equity dataframe)
         by the total portfolio value (as represented in the nav dataframe).
         Both dataframes are assumed to have the same dimensions.
         The resulting dataframe will show the relative weight
         of each asset in the portfolio at each point in time."""
         return self.equity.apply(lambda x: x / self.nav)
 
-    def __getitem__(self, time):
+    def __getitem__(self, time: datetime) -> pd.Series:
         """The `__getitem__` method retrieves the stock data for a specific time in the dataframe.
         It returns the stock data for that time.
 
         The method takes one input parameter:
         - `time`: the time index for which to retrieve the stock data
 
         Returns:
         - stock data for the input time
 
         Note that the input time must be in the index of the dataframe,
         otherwise a KeyError will be raised."""
         return self.stocks.loc[time]
 
     @property
-    def trading_costs(self):
+    def trading_costs(self) -> pd.DataFrame:
         """A property that returns a pandas dataframe
         representing the trading costs incurred by the portfolio due to trades made.
 
         Returns: pd.DataFrame: A pandas dataframe representing the trading
         costs incurred by the portfolio due to trades made.
 
         Notes: The function calculates the trading costs using the specified
@@ -316,15 +322,15 @@
         Notes: The function calculates the ratio of the portfolio's current value
         vs. its current high-water-mark and then subtracting the result from 1.
         A positive drawdown means the portfolio is currently worth
         less than its high-water mark. A drawdown of 0.1 implies that the nav is currently 0.9 times the high-water mark
         """
         return 1.0 - self.nav / self.highwater
 
-    def __mul__(self, scalar):
+    def __mul__(self, scalar: float) -> "EquityPortfolio":
         """A method that allows multiplication of the EquityPortfolio object with a scalar constant.
 
         Args: scalar: A scalar constant that multiplies the number of shares
         of each asset held in the EquityPortfolio object.
 
         Returns: EquityPortfolio: A new EquityPortfolio object multiplied by the scalar constant.
 
@@ -342,26 +348,26 @@
         return EquityPortfolio(
             prices=self.prices,
             stocks=self.stocks * scalar,
             initial_cash=self.initial_cash * scalar,
             trading_cost_model=self.trading_cost_model,
         )
 
-    def __rmul__(self, scalar):
+    def __rmul__(self, scalar: float) -> EquityPortfolio:
         """A method that allows multiplication of the EquityPortfolio object with a scalar constant in a reversed order.
 
         Args: scalar: A scalar constant that multiplies the EquityPortfolio object in a reversed order.
 
         Returns: EquityPortfolio: A new EquityPortfolio object multiplied by the scalar constant.
 
         Notes: The rmul method allows multiplication of a scalar
         constant with an EquityPortfolio object in a reversed order"""
         return self.__mul__(scalar)
 
-    def __add__(self, port_new):
+    def __add__(self, port_new: EquityPortfolio) -> EquityPortfolio:
         """
         A method that allows addition of two EquityPortfolio objects.
         """
         # check if the other object is an EquityPortfolio object
         assert isinstance(port_new, EquityPortfolio)
 
         # make sure the prices are aligned for overlapping points
@@ -383,15 +389,15 @@
         return EquityPortfolio(
             prices=prices_right,
             stocks=positions,
             initial_cash=self.initial_cash + port_new.initial_cash,
             trading_cost_model=self.trading_cost_model,
         )
 
-    def reset_prices(self, prices):
+    def reset_prices(self, prices: pd.DataFrame) -> EquityPortfolio:
         """
         A method that constructs an EquityPortfolio object using finer prices.
         """
         # extract the relevant columns from prices
         p = prices[self.assets]
 
         # the prices need to contain the original index
@@ -412,15 +418,17 @@
         return EquityPortfolio(
             prices=p,
             stocks=stocks,
             initial_cash=self.initial_cash,
             trading_cost_model=self.trading_cost_model,
         )
 
-    def truncate(self, before=None, after=None):
+    def truncate(
+        self, before: Optional[datetime] = None, after: Optional[datetime] = None
+    ) -> EquityPortfolio:
         """
         The truncate method truncates the prices DataFrame, stocks DataFrame
         and the cash series of an EquityPortfolio object.
         The method also optionally accepts a before and/or after argument
         to specify a date range for truncation.
 
         The method returns a new EquityPortfolio object which is a truncated version
@@ -445,15 +453,15 @@
         )
 
     # @property
     # def start(self):
     #     """first index with a profit that is not zero"""
     #     return self.profit.ne(0).idxmax()
 
-    def resample(self, rule):
+    def resample(self, rule: Any) -> EquityPortfolio:
         """The resample method resamples an EquityPortfolio object to a new frequency
         specified by the rule argument.
         A new EquityPortfolio object is created with the original prices
         DataFrame and the resampled stocks DataFrame. The objects trading cost model and initial cash value
         are also copied into the new object.
 
         Note that the resample method does not modify the original EquityPortfolio object,
@@ -467,25 +475,25 @@
             stocks=stocks,
             trading_cost_model=self.trading_cost_model,
             initial_cash=self.initial_cash,
         )
 
     def metrics(
         self,
-        benchmark=None,
-        rf=0.0,
-        display=True,
-        mode="basic",
-        sep=False,
-        compound=True,
-        periods_per_year=252,
-        prepare_returns=True,
-        match_dates=True,
-        **kwargs,
-    ):
+        benchmark: Any = None,
+        rf: float = 0.0,
+        display: bool = True,
+        mode: str = "basic",
+        sep: bool = False,
+        compound: bool = True,
+        periods_per_year: int = 252,
+        prepare_returns: bool = True,
+        match_dates: bool = True,
+        **kwargs: Any,
+    ) -> pd.DataFrame:
         """
         The metrics method calculates the performance metrics of an EquityPortfolio object.
 
         :param kwargs:
         :return:
         """
         return qs.reports.metrics(
@@ -500,55 +508,55 @@
             prepare_returns=prepare_returns,
             match_dates=match_dates,
             **kwargs,
         )
 
     def plots(
         self,
-        benchmark=None,
-        grayscale=False,
-        figsize=(8, 5),
-        mode="basic",
-        compounded=True,
-        periods_per_year=252,
-        prepare_returns=True,
-        match_dates=True,
-        **kwargs,
-    ):
+        benchmark: Any = None,
+        grayscale: bool = False,
+        figsize: Tuple[int, int] = (8, 5),
+        mode: str = "basic",
+        compounded: bool = True,
+        periods_per_year: int = 252,
+        prepare_returns: bool = True,
+        match_dates: bool = True,
+        **kwargs: Any,
+    ) -> Any:
         return qs.reports.plots(
             returns=self.nav.pct_change().dropna(),
             benchmark=benchmark,
             grayscale=grayscale,
             figsize=figsize,
             mode=mode,
             compounded=compounded,
             periods_per_year=periods_per_year,
             prepare_returns=prepare_returns,
             match_dates=match_dates,
             **kwargs,
         )
 
-    def plot(self, kind: Plot, **kwargs):
+    def plot(self, kind: Plot, **kwargs: Any) -> Any:
         return kind.plot(returns=self.nav.pct_change().dropna(), **kwargs)
 
     def html(
         self,
-        benchmark=None,
-        rf=0.0,
-        grayscale=False,
-        title="Strategy Tearsheet",
-        output=None,
-        compounded=True,
-        periods_per_year=252,
-        download_filename="quantstats-tearsheet.html",
-        figfmt="svg",
-        template_path=None,
-        match_dates=True,
-        **kwargs,
-    ):
+        benchmark: Any = None,
+        rf: float = 0.0,
+        grayscale: bool = False,
+        title: str = "Strategy Tearsheet",
+        output: Any = None,
+        compounded: bool = True,
+        periods_per_year: int = 252,
+        download_filename: str = "quantstats-tearsheet.html",
+        figfmt: str = "svg",
+        template_path: Any = None,
+        match_dates: bool = True,
+        **kwargs: Any,
+    ) -> Any:
         return qs.reports.html(
             returns=self.nav.pct_change().dropna(),
             benchmark=benchmark,
             rf=rf,
             grayscale=grayscale,
             title=title,
             output=output,
@@ -559,26 +567,26 @@
             template_path=template_path,
             match_dates=match_dates,
             **kwargs,
         )
 
     def snapshot(
         self,
-        grayscale=False,
-        figsize=(10, 8),
-        title="Portfolio Summary",
-        fontname="Arial",
-        lw=1.5,
-        mode="comp",
-        subtitle=True,
-        savefig=None,
-        show=True,
-        log_scale=False,
-        **kwargs,
-    ):
+        grayscale: bool = False,
+        figsize: Tuple[int, int] = (10, 8),
+        title: str = "Portfolio Summary",
+        fontname: str = "Arial",
+        lw: float = 1.5,
+        mode: str = "comp",
+        subtitle: bool = True,
+        savefig: Any = None,
+        show: bool = True,
+        log_scale: bool = False,
+        **kwargs: Any,
+    ) -> Any:
         """
         The snapshot method creates a snapshot of the performance of an EquityPortfolio object.
 
         :param grayscale:
         :param figsize:
         :param title:
         :param fontname:
```

### Comparing `cvxsimulator-0.6.3/cvx/simulator/trading_costs.py` & `cvxsimulator-0.7.0/cvx/simulator/trading_costs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import abc
 from dataclasses import dataclass
+from typing import Any
+
+import pandas as pd
 
 
 @dataclass(frozen=True)
 class TradingCostModel(abc.ABC):
     @abc.abstractmethod
-    def eval(self, prices, trades, **kwargs):
+    def eval(
+        self, prices: pd.DataFrame, trades: pd.DataFrame, **kwargs: Any
+    ) -> pd.DataFrame:
         """Evaluates the cost of a trade given the prices and the trades
 
         Arguments
             prices: the price per asset
             trades: the trade per asset, e.g. number of stocks traded
             **kwargs: additional arguments, e.g. volatility, liquidity, spread, etc.
         """
 
 
 @dataclass(frozen=True)
 class LinearCostModel(TradingCostModel):
     factor: float = 0.0
     bias: float = 0.0
 
-    def eval(self, prices, trades, **kwargs):
+    def eval(
+        self, prices: pd.DataFrame, trades: pd.DataFrame, **kwargs: Any
+    ) -> pd.DataFrame:
         volume = prices * trades
         return self.factor * volume.abs() + self.bias * trades.abs()
```

### Comparing `cvxsimulator-0.6.3/pyproject.toml` & `cvxsimulator-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxsimulator"
-version = "v0.6.3"
+version = "v0.7.0"
 description = "Simple simulator for investors"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/simulator"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cvxsimulator-0.6.3/PKG-INFO` & `cvxsimulator-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.6.3
+Version: 0.7.0
 Summary: Simple simulator for investors
 Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

