# Comparing `tmp/pams-0.0.9.tar.gz` & `tmp/pams-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pams-0.0.9.tar", max compression
+gzip compressed data, was "pams-0.1.0.tar", max compression
```

## Comparing `pams-0.0.9.tar` & `pams-0.1.0.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0     1072 2023-01-07 11:10:00.324881 pams-0.0.9/LICENSE
--rw-r--r--   0        0        0     1903 2023-01-07 11:10:00.324881 pams-0.0.9/README.md
--rw-r--r--   0        0        0      520 2023-01-07 11:10:00.328881 pams-0.0.9/pams/__init__.py
--rw-r--r--   0        0        0      187 2023-01-07 11:10:00.328881 pams-0.0.9/pams/agents/__init__.py
--rw-r--r--   0        0        0     5561 2023-01-07 11:10:00.328881 pams-0.0.9/pams/agents/arbitrage_agent.py
--rw-r--r--   0        0        0     8376 2023-01-07 11:10:00.328881 pams-0.0.9/pams/agents/base.py
--rw-r--r--   0        0        0     9238 2023-01-07 11:10:00.328881 pams-0.0.9/pams/agents/fcn_agent.py
--rw-r--r--   0        0        0      332 2023-01-07 11:10:00.328881 pams-0.0.9/pams/agents/high_frequency_agent.py
--rw-r--r--   0        0        0     2323 2023-01-07 11:10:00.328881 pams-0.0.9/pams/agents/test_agent.py
--rw-r--r--   0        0        0      114 2023-01-07 11:10:00.328881 pams-0.0.9/pams/events/__init__.py
--rw-r--r--   0        0        0     8592 2023-01-07 11:10:00.328881 pams-0.0.9/pams/events/base.py
--rw-r--r--   0        0        0     3030 2023-01-07 11:10:00.328881 pams-0.0.9/pams/events/fundamental_price_shock.py
--rw-r--r--   0        0        0     7006 2023-01-07 11:10:00.328881 pams-0.0.9/pams/fundamentals.py
--rw-r--r--   0        0        0     2838 2023-01-07 11:10:00.328881 pams-0.0.9/pams/index_market.py
--rw-r--r--   0        0        0      447 2023-01-07 11:10:00.328881 pams-0.0.9/pams/logs/__init__.py
--rw-r--r--   0        0        0    13513 2023-01-07 11:10:00.328881 pams-0.0.9/pams/logs/base.py
--rw-r--r--   0        0        0     1397 2023-01-07 11:10:00.328881 pams-0.0.9/pams/logs/market_step_loggers.py
--rw-r--r--   0        0        0    23106 2023-01-07 11:10:00.328881 pams-0.0.9/pams/market.py
--rw-r--r--   0        0        0     5458 2023-01-07 11:10:00.328881 pams-0.0.9/pams/order.py
--rw-r--r--   0        0        0     3587 2023-01-07 11:10:00.328881 pams-0.0.9/pams/order_book.py
--rw-r--r--   0        0        0       66 2023-01-07 11:10:00.328881 pams-0.0.9/pams/runners/__init__.py
--rw-r--r--   0        0        0     3174 2023-01-07 11:10:00.328881 pams-0.0.9/pams/runners/base.py
--rw-r--r--   0        0        0    23621 2023-01-07 11:10:00.328881 pams-0.0.9/pams/runners/sequential.py
--rw-r--r--   0        0        0     2730 2023-01-07 11:10:00.328881 pams-0.0.9/pams/session.py
--rw-r--r--   0        0        0    13751 2023-01-07 11:10:00.328881 pams-0.0.9/pams/simulator.py
--rw-r--r--   0        0        0      147 2023-01-07 11:10:00.328881 pams-0.0.9/pams/utils/__init__.py
--rw-r--r--   0        0        0      909 2023-01-07 11:10:00.328881 pams-0.0.9/pams/utils/class_finder.py
--rw-r--r--   0        0        0     1141 2023-01-07 11:10:00.328881 pams-0.0.9/pams/utils/json_extends.py
--rw-r--r--   0        0        0     3094 2023-01-07 11:10:00.328881 pams-0.0.9/pams/utils/json_random.py
--rw-r--r--   0        0        0       22 2023-01-07 11:10:00.328881 pams-0.0.9/pams/version.py
--rw-r--r--   0        0        0     1048 2023-01-07 11:10:00.328881 pams-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 pams-0.0.9/setup.py
--rw-r--r--   0        0        0     2912 1970-01-01 00:00:00.000000 pams-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-26 12:59:39.332702 pams-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1903 2023-04-26 12:59:39.336701 pams-0.1.0/README.md
+-rw-r--r--   0        0        0      594 2023-04-26 12:59:39.336701 pams-0.1.0/pams/__init__.py
+-rw-r--r--   0        0        0      187 2023-04-26 12:59:39.336701 pams-0.1.0/pams/agents/__init__.py
+-rw-r--r--   0        0        0     6689 2023-04-26 12:59:39.336701 pams-0.1.0/pams/agents/arbitrage_agent.py
+-rw-r--r--   0        0        0     8620 2023-04-26 12:59:39.336701 pams-0.1.0/pams/agents/base.py
+-rw-r--r--   0        0        0     9663 2023-04-26 12:59:39.336701 pams-0.1.0/pams/agents/fcn_agent.py
+-rw-r--r--   0        0        0      363 2023-04-26 12:59:39.336701 pams-0.1.0/pams/agents/high_frequency_agent.py
+-rw-r--r--   0        0        0     2323 2023-04-26 12:59:39.336701 pams-0.1.0/pams/agents/test_agent.py
+-rw-r--r--   0        0        0      114 2023-04-26 12:59:39.336701 pams-0.1.0/pams/events/__init__.py
+-rw-r--r--   0        0        0     9916 2023-04-26 12:59:39.336701 pams-0.1.0/pams/events/base.py
+-rw-r--r--   0        0        0     3832 2023-04-26 12:59:39.336701 pams-0.1.0/pams/events/fundamental_price_shock.py
+-rw-r--r--   0        0        0    10298 2023-04-26 12:59:39.336701 pams-0.1.0/pams/fundamentals.py
+-rw-r--r--   0        0        0     6379 2023-04-26 12:59:39.336701 pams-0.1.0/pams/index_market.py
+-rw-r--r--   0        0        0      447 2023-04-26 12:59:39.336701 pams-0.1.0/pams/logs/__init__.py
+-rw-r--r--   0        0        0    13673 2023-04-26 12:59:39.336701 pams-0.1.0/pams/logs/base.py
+-rw-r--r--   0        0        0     1465 2023-04-26 12:59:39.336701 pams-0.1.0/pams/logs/market_step_loggers.py
+-rw-r--r--   0        0        0    33146 2023-04-26 12:59:39.336701 pams-0.1.0/pams/market.py
+-rw-r--r--   0        0        0    10140 2023-04-26 12:59:39.336701 pams-0.1.0/pams/order.py
+-rw-r--r--   0        0        0     6151 2023-04-26 12:59:39.336701 pams-0.1.0/pams/order_book.py
+-rw-r--r--   0        0        0       66 2023-04-26 12:59:39.336701 pams-0.1.0/pams/runners/__init__.py
+-rw-r--r--   0        0        0     3848 2023-04-26 12:59:39.336701 pams-0.1.0/pams/runners/base.py
+-rw-r--r--   0        0        0    27383 2023-04-26 12:59:39.336701 pams-0.1.0/pams/runners/sequential.py
+-rw-r--r--   0        0        0     6187 2023-04-26 12:59:39.336701 pams-0.1.0/pams/session.py
+-rw-r--r--   0        0        0    18332 2023-04-26 12:59:39.340702 pams-0.1.0/pams/simulator.py
+-rw-r--r--   0        0        0      147 2023-04-26 12:59:39.340702 pams-0.1.0/pams/utils/__init__.py
+-rw-r--r--   0        0        0     1353 2023-04-26 12:59:39.340702 pams-0.1.0/pams/utils/class_finder.py
+-rw-r--r--   0        0        0     2312 2023-04-26 12:59:39.340702 pams-0.1.0/pams/utils/json_extends.py
+-rw-r--r--   0        0        0     7435 2023-04-26 12:59:39.340702 pams-0.1.0/pams/utils/json_random.py
+-rw-r--r--   0        0        0       22 2023-04-26 12:59:39.340702 pams-0.1.0/pams/version.py
+-rw-r--r--   0        0        0     1271 2023-04-26 12:59:39.340702 pams-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2527 1970-01-01 00:00:00.000000 pams-0.1.0/PKG-INFO
```

### Comparing `pams-0.0.9/LICENSE` & `pams-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pams-0.0.9/README.md` & `pams-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pams-0.0.9/pams/__init__.py` & `pams-0.1.0/pams/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,10 +7,12 @@
 from pams.market import Market
 from pams.order import LIMIT_ORDER
 from pams.order import MARKET_ORDER
 from pams.order import Cancel
 from pams.order import Order
 from pams.order import OrderKind
 from pams.order_book import OrderBook
+from pams.runners import Runner
+from pams.runners import SequentialRunner
 from pams.session import Session
 from pams.simulator import Simulator
 from pams.version import __version__
```

### Comparing `pams-0.0.9/pams/agents/arbitrage_agent.py` & `pams-0.1.0/pams/agents/arbitrage_agent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import random
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 from ..index_market import IndexMarket
+from ..logs import Logger
 from ..market import Market
 from ..order import LIMIT_ORDER
 from ..order import Cancel
 from ..order import Order
 from .high_frequency_agent import HighFrequencyAgent
 
 
@@ -18,24 +20,36 @@
     This class inherits from the HighFrequencyAgent class.
     Arbitrage agent mainly aimed to take arbitrage chance between spot markets and its index market.
 
     Note:
         Currently, index markets must have the same weight for each constitutional stock.
     """
 
-    order_volume: int = 1
-    order_threshold_price: float = 1.0
-    order_time_length: int = 1
+    def __init__(
+        self,
+        agent_id: int,
+        prng: random.Random,
+        simulator: "Simulator",  # type: ignore  # NOQA
+        name: str,
+        logger: Optional[Logger] = None,
+    ) -> None:
+        super().__init__(
+            agent_id=agent_id, prng=prng, simulator=simulator, name=name, logger=logger
+        )
+
+        self.order_volume: int = 1
+        self.order_threshold_price: float = 1.0
+        self.order_time_length: int = 1
 
     def setup(  # type: ignore
         self,
         settings: Dict[str, Any],
         accessible_markets_ids: List[int],
         *args,
-        **kwargs
+        **kwargs,
     ) -> None:
         """agent setup. Usually be called from simulator/runner automatically.
 
         Args:
             settings (Dict[str, Any]): agent configuration. Usually, automatically set from json config of simulator.
                                        This must include the parameters "orderVolume", "orderThresholdPrice".
                                        This can include the parameter "orderTimeLength".
@@ -45,19 +59,23 @@
             None
         """
         super(ArbitrageAgent, self).setup(
             settings, accessible_markets_ids, *args, **kwargs
         )
         if "orderVolume" not in settings:
             raise ValueError("orderVolume is required for ArbitrageAgent")
+        if not isinstance(settings["orderVolume"], int):
+            raise ValueError("orderVolume have to be int")
         self.order_volume = settings["orderVolume"]
         if "orderThresholdPrice" not in settings:
             raise ValueError("orderThresholdPrice is required for ArbitrageAgent")
         self.order_threshold_price = settings["orderThresholdPrice"]
         if "orderTimeLength" in settings:
+            if not isinstance(settings["orderTimeLength"], int):
+                raise ValueError("orderTimeLength have to be int")
             self.order_time_length = settings["orderTimeLength"]
 
     def _submit_orders(self, market: Market) -> List[Union[Order, Cancel]]:
         """internal sub routine for submitting orders by market.
 
         Args:
             market (List[Market]): markets to order.
@@ -74,15 +92,15 @@
         spots: List[Market] = index.get_components()
         if not index.is_running or not index.is_all_markets_running():
             return orders
         market_index: float = index.get_index()
         market_price: float = index.get_market_price()
 
         if len(set(map(lambda x: x.outstanding_shares, spots))) > 1:
-            raise AssertionError(
+            raise NotImplementedError(
                 "currently, the components must have the same outstanding shares"
             )
 
         if (
             market_price < market_index
             and market_index - market_price > self.order_threshold_price
         ):
@@ -146,7 +164,19 @@
         .. seealso::
             - :func:`pams.agents.Agent.submit_orders`
         """
         orders: List[Union[Order, Cancel]] = []
         for market in markets:
             orders.extend(self._submit_orders(market=market))
         return orders
+
+    def __repr__(self) -> str:
+        """string representation of FCN agent class.
+
+        Returns:
+            str: string representation of this class.
+        """
+        return (
+            f"<{self.__class__.__module__}.{self.__class__.__name__} | id={self.agent_id}, rnd={self.prng}, "
+            f"order_volume={self.order_volume}, order_threshold_price={self.order_threshold_price}, "
+            f"order_time_length={self.order_time_length}>"
+        )
```

### Comparing `pams-0.0.9/pams/agents/base.py` & `pams-0.1.0/pams/agents/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         - :class:`pams.agents.FCNAgent`: FCNAgent
     """
 
     def __init__(
         self,
         agent_id: int,
         prng: random.Random,
-        simulator: "Simulator",  # type: ignore
+        simulator: "Simulator",  # type: ignore  # NOQA
         name: str,
         logger: Optional[Logger] = None,
     ) -> None:
         """agent initialization. Usually call from simulator automatically.
 
         Args:
             agent_id (int): agent id. This is also required to generate orders to identify who submit orders.
@@ -57,31 +57,39 @@
              It is because sometimes agent process runs one of parallelized threads.
         """
         self.agent_id: int = agent_id
         self.name: str = name
         self.asset_volumes: Dict[int, int] = {}
         self.cash_amount: float = 0
         self.prng: random.Random = prng
-        self.sim: "Simulator" = simulator  # type: ignore
+        self.simulator: "Simulator" = simulator  # type: ignore  # NOQA
         self.logger: Optional[Logger] = logger
 
+    def __repr__(self) -> str:
+        return (
+            f"<{self.__class__.__module__}.{self.__class__.__name__} | id={self.agent_id}, name={self.name}, "
+            f"logger={self.logger}>"
+        )
+
     def setup(self, settings: Dict[str, Any], accessible_markets_ids: List[int], *args, **kwargs) -> None:  # type: ignore
         """agent setup. Usually be called from simulator/runner automatically.
 
         Args:
             settings (Dict[str, Any]): agent configuration.  Usually, automatically set from json config of simulator.
                                        This must include the parameters "cashAmount" and "assetVolume".
             accessible_markets_ids (List[int]): list of market IDs.
 
         Returns:
             None
         """
         if "cashAmount" not in settings:
             raise ValueError("cashAmount is required property of agent settings")
-        self.cash_amount = settings["cashAmount"]
+        self.cash_amount = JsonRandom(prng=self.prng).random(
+            json_value=settings["cashAmount"]
+        )
         if "assetVolume" not in settings:
             raise ValueError("cashAmount is required property of agent settings")
 
         for market_id in accessible_markets_ids:
             self.set_market_accessible(market_id=market_id)
             volume = int(
                 JsonRandom(prng=self.prng).random(json_value=settings["assetVolume"])
@@ -94,15 +102,15 @@
         Args:
             market_id (int): market ID.
 
         Returns:
             int: asset volume for the specified market ID.
         """
         if not self.is_market_accessible(market_id=market_id):
-            raise AssertionError(f"market {market_id} is not accessible")
+            raise ValueError(f"market {market_id} is not accessible")
         return self.asset_volumes[market_id]
 
     def get_cash_amount(self) -> float:
         """getter of the cash amount held by the agent.
 
         Returns:
             float: cash amount held by this agent.
@@ -168,15 +176,17 @@
             market_id (int): market ID.
             volume (int): volume to be set for the market
 
         Returns:
             None
         """
         if not self.is_market_accessible(market_id=market_id):
-            raise AssertionError(f"market {market_id} is not accessible")
+            raise ValueError(f"market {market_id} is not accessible")
+        if not isinstance(volume, int):
+            raise ValueError("volume have to be int")
         self.asset_volumes[market_id] = volume
 
     def set_cash_amount(self, cash_amount: float) -> None:
         """setter of the cash amount held by agent.
 
         Args:
             cash_amount (float): cash amount held by this agent.
@@ -191,14 +201,16 @@
 
         Args:
             market_id (int): market ID.
 
         Returns:
             None
         """
+        if self.is_market_accessible(market_id=market_id):
+            raise ValueError(f"market {market_id} is already accessible")
         self.asset_volumes[market_id] = 0
 
     @abstractmethod
     def submit_orders(self, markets: List[Market]) -> List[Union[Order, Cancel]]:
         """submit orders (abstract method). This method automatically called from runners.
 
         This method is called only when this agent has a chance to submit orders.
@@ -222,35 +234,22 @@
             market_id (int): market ID.
             delta (int): amount of change in the asset volume.
 
         Returns:
             None
         """
         if not self.is_market_accessible(market_id=market_id):
-            raise AssertionError(f"market {market_id} is not accessible")
+            raise ValueError(f"market {market_id} is not accessible")
+        if not isinstance(delta, int):
+            raise ValueError("delta have to be int")
         self.asset_volumes[market_id] += delta
 
     def update_cash_amount(self, delta: float) -> None:
         """increasing or decreasing the cash amount.
 
         Args:
             delta (float): amount of change in the cash amount.
 
         Returns:
             None
         """
         self.cash_amount += delta
-
-    def __repr__(self) -> str:
-        """string representation of agent class.
-
-        Returns:
-            str: string representation of this class.
-        """
-        return (
-            self.__class__.__name__
-            + str(id)
-            + ","
-            + str(self.cash_amount)
-            + ","
-            + str(self.asset_volumes)
-        )
```

### Comparing `pams-0.0.9/pams/agents/fcn_agent.py` & `pams-0.1.0/pams/agents/fcn_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,35 +28,35 @@
 
     - "fixed" : :math:`p (1 ± k)` where :math:`0 \leq k \leq 1`
     - "normal" : :math:`p + N(0, k)` where :math:`k > 0`
 
     References:
         - Chiarella, C., & Iori, G. (2002). A simulation analysis of the microstructure of double auction markets.
           Quantitative Finance, 2(5), 346–353. https://doi.org/10.1088/1469-7688/2/5/303
-    """
+    """  # NOQA
 
     fundamental_weight: float
     chart_weight: float
-    is_chart_following: bool = True
     margin_type: int
     mean_reversion_time: int
     noise_scale: float
     noise_weight: float
     order_margin: float
     time_window_size: int
 
     def __init__(
         self,
         agent_id: int,
         prng: random.Random,
-        simulator: "Simulator",  # type: ignore
+        simulator: "Simulator",  # type: ignore  # NOQA
         name: str,
         logger: Optional[Logger] = None,
     ):
         super().__init__(agent_id, prng, simulator, name, logger)
+        self.is_chart_following = True
 
     def is_finite(self, x: float) -> bool:
         """determine if it is a valid value.
 
         Args:
             x (float): value.
 
@@ -93,16 +93,20 @@
         self.noise_scale = json_random.random(json_value=settings["noiseScale"])
         self.time_window_size = int(
             json_random.random(json_value=settings["timeWindowSize"])
         )
         self.order_margin = json_random.random(json_value=settings["orderMargin"])
         if settings.get("marginType") in [None, "fixed"]:
             self.margin_type = MARGIN_FIXED
-        else:
+        elif settings.get("marginType") == "normal":
             self.margin_type = MARGIN_NORMAL
+        else:
+            raise ValueError(
+                "marginType have to be normal or fixed (not specified is also allowed.)"
+            )
         if "meanReversionTime" in settings:
             self.mean_reversion_time = int(
                 json_random.random(json_value=settings["meanReversionTime"])
             )
         else:
             self.mean_reversion_time = self.time_window_size
 
@@ -231,19 +235,21 @@
                         volume=order_volume,
                         price=order_price,
                         ttl=self.time_window_size,
                     )
                 )
         return orders
 
-    def __str__(self) -> str:
+    def __repr__(self) -> str:
         """string representation of FCN agent class.
 
         Returns:
             str: string representation of this class.
         """
         return (
-            f"Agent:{self.agent_id}[rnd:{self.prng},cw:{self.chart_weight},fw:{self.fundamental_weight},"
-            + f"following:{self.is_chart_following},mtypr:{self.margin_type},mrt:{self.mean_reversion_time},"
-            + f"ns:{self.noise_scale},nw:{self.noise_weight},om:{self.order_margin},tws:{self.time_window_size},"
-            + f"cash:{self.cash_amount}]"
+            f"<{self.__class__.__module__}.{self.__class__.__name__} | id={self.agent_id}, rnd={self.prng}, "
+            f"chart_weight={self.chart_weight}, fundamental_weight={self.fundamental_weight}, "
+            f"noise_weight={self.noise_weight}, is_chart_following:{self.is_chart_following}, "
+            f"margin_type={self.margin_type}, mean_reversion_time:{self.mean_reversion_time}, "
+            f"noise_scale={self.noise_scale}, time_window_size={self.time_window_size}, "
+            f"order_margin={'MARGIN_FIXED' if self.order_margin == MARGIN_FIXED else 'MARGIN_NORMAL'}"
         )
```

### Comparing `pams-0.0.9/pams/agents/test_agent.py` & `pams-0.1.0/pams/agents/test_agent.py`

 * *Files identical despite different names*

### Comparing `pams-0.0.9/pams/events/base.py` & `pams-0.1.0/pams/events/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 from abc import ABC
 from abc import abstractmethod
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Type
+from typing import cast
+
+from pams.market import Market
 
 
 class EventHook:
     """Event Hook class.
 
     Event hook define when and what events are hooked from simulator.
     It means that Event ( :class:`Event` ) can be used for multiple time if you appropriately set the event hook using the evnet.
@@ -55,19 +58,39 @@
         self.is_before = is_before
         self.time = time
         if specific_class is not None or specific_instance is not None:
             if hook_type not in ["market"]:
                 raise ValueError(
                     "specific_class and specific_instance are not supported except for market"
                 )
-        self.specific_class: Optional[Type] = (
-            specific_class.__class__ if specific_class is not None else None
-        )
+            else:
+                if hook_type == "market":
+                    if specific_class is not None and not issubclass(
+                        specific_class, Market
+                    ):
+                        raise ValueError("specific_class and hook_type is incompatible")
+                    if specific_instance is not None and not isinstance(
+                        specific_instance, Market
+                    ):
+                        raise ValueError(
+                            "specific_instance and hook_type is incompatible"
+                        )
+                else:
+                    raise AssertionError
+        specific_class = cast(Optional[Type], specific_class)
+        self.specific_class: Optional[Type] = specific_class
         self.specific_instance: Optional[object] = specific_instance
 
+    def __repr__(self) -> str:
+        return (
+            f"<{self.__class__.__module__}.{self.__class__.__name__} | hook_type={self.hook_type}, "
+            f"is_before={self.is_before}, time={self.time}, specific_class={self.specific_class}, "
+            f"specific_instance={self.specific_instance}, event={self.event}>"
+        )
+
 
 class EventABC(ABC):
     """event base class (ABC class).
 
     It defines what the event is.
     All events should inherit this class.
 
@@ -75,16 +98,16 @@
         - :class:`pams.events.FundamentalPriceShock`
     """
 
     def __init__(
         self,
         event_id: int,
         prng: random.Random,
-        session: "Session",  # type: ignore
-        simulator: "Simulator",  # type: ignore
+        session: "Session",  # type: ignore  # NOQA
+        simulator: "Simulator",  # type: ignore  # NOQA
         name: str,
     ) -> None:
         """event initialization. Usually be called from simulator/runner automatically.
 
         Args:
             event_id (int): event ID.
             prng (random.Random): pseudo random number generator for this event.
@@ -97,14 +120,20 @@
         """
         self.event_id: int = event_id
         self.prng: random.Random = prng
         self.simulator = simulator
         self.name: str = name
         self.session = session
 
+    def __repr__(self) -> str:
+        return (
+            f"<{self.__class__.__module__}.{self.__class__.__name__} | id={self.event_id}, name={self.name}, "
+            f"session={self.session}>"
+        )
+
     def setup(self, settings: Dict[str, Any], *args, **kwargs) -> None:  # type: ignore
         """event setup. Usually be called from simulator/runner automatically.
 
         Args:
             settings (Dict[str, Any]): agent configuration. Usually, automatically set from json config of simulator.
 
         Returns:
@@ -119,114 +148,114 @@
         You must implement this.
 
         Returns:
             List[EventHook]: The list of event hook ( :class:`EventHook` )
         """
         pass
 
-    def hooked_before_order(self, simulator: "Simulator", order: "Order") -> None:  # type: ignore
+    def hooked_before_order(self, simulator: "Simulator", order: "Order") -> None:  # type: ignore  # NOQA
         """This method is hooked before order placements if you set the event hook.
         Please be careful that the order haven't yet been accepted by markets and it could be leakage of order information.
 
         .. seealso:
             - ToDo: simulation flow
 
         Args:
             simulator (Simulator): simulator for reference.
             order (Order): order accepting now.
         """
         pass
 
-    def hooked_after_order(self, simulator: "Simulator", order_log: "OrderLog") -> None:  # type: ignore
+    def hooked_after_order(self, simulator: "Simulator", order_log: "OrderLog") -> None:  # type: ignore  # NOQA
         """This method is hooked after order placements if you set the event hook.
         Please be careful that the order haven't yet been executed if it could be executed immediately.
 
         .. seealso:
             - ToDo: simulation flow
 
         Args:
             simulator (Simulator): simulator for reference.
             order_log (OrderLog): order accepted.
         """
         pass
 
-    def hooked_before_cancel(self, simulator: "Simulator", cancel: "Cancel") -> None:  # type: ignore
+    def hooked_before_cancel(self, simulator: "Simulator", cancel: "Cancel") -> None:  # type: ignore  # NOQA
         """This method is hooked before order cancellations if you set the event hook.
         Please be careful that the cancel order haven't yet been executed.
 
         .. seealso:
             - ToDo: simulation flow
 
         Args:
             simulator (Simulator): simulator for reference.
             cancel (Cancel): cancel order submitted.
         """
         pass
 
-    def hooked_after_cancel(self, simulator: "Simulator", cancel_log: "CancelLog") -> None:  # type: ignore
+    def hooked_after_cancel(self, simulator: "Simulator", cancel_log: "CancelLog") -> None:  # type: ignore  # NOQA
         """This method is hooked after order cancellations if you set the event hook.
 
         .. seealso:
             - ToDo: simulation flow
 
         Args:
             simulator (Simulator): simulator for reference.
             cancel_log (CancelLog): cancel order submitted.
         """
         pass
 
-    def hooked_after_execution(self, simulator: "Simulator", execution_log: "ExecutionLog") -> None:  # type: ignore
+    def hooked_after_execution(self, simulator: "Simulator", execution_log: "ExecutionLog") -> None:  # type: ignore  # NOQA
         """This method is hooked after order executions if you set the event hook.
 
         .. seealso:
             - ToDo: simulation flow
 
         Args:
             simulator (Simulator): simulator for reference.
             execution_log (ExecutionLog): execution log.
         """
         pass
 
-    def hooked_before_session(self, simulator: "Simulator", session: "Session") -> None:  # type: ignore
+    def hooked_before_session(self, simulator: "Simulator", session: "Session") -> None:  # type: ignore  # NOQA
         """This method is hooked before session beginnings if you set the event hook.
 
         .. seealso:
             - ToDo: simulation flow
 
         Args:
             simulator (Simulator): simulator for reference.
             session (Session): session to be started.
         """
         pass
 
-    def hooked_after_session(self, simulator: "Simulator", session: "Session") -> None:  # type: ignore
+    def hooked_after_session(self, simulator: "Simulator", session: "Session") -> None:  # type: ignore  # NOQA
         """This method is hooked after session ends if you set the event hook.
 
         .. seealso:
             - ToDo: simulation flow
 
         Args:
             simulator (Simulator): simulator for reference.
             session (Session): session to be ended.
         """
         pass
 
-    def hooked_before_step_for_market(self, simulator: "Simulator", market: "Market") -> None:  # type: ignore
+    def hooked_before_step_for_market(self, simulator: "Simulator", market: "Market") -> None:  # type: ignore  # NOQA
         """This method is hooked at each step before market processing if you set the event hook.
 
         .. seealso:
             - ToDo: simulation flow
 
         Args:
             simulator (Simulator): simulator for reference.
             market (Market): market to be processed.
         """
         pass
 
-    def hooked_after_step_for_market(self, simulator: "Simulator", market: "Market") -> None:  # type: ignore
+    def hooked_after_step_for_market(self, simulator: "Simulator", market: "Market") -> None:  # type: ignore  # NOQA
         """This method is hooked at each step after market processing if you set the event hook.
 
         .. seealso:
             - ToDo: simulation flow
 
         Args:
             simulator (Simulator): simulator for reference.
```

### Comparing `pams-0.0.9/pams/logs/base.py` & `pams-0.1.0/pams/logs/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
         self.time: int = time
         self.agent_id: int = agent_id
         self.is_buy: bool = is_buy
         self.kind: OrderKind = kind
         self.price: Optional[float] = price
         self.volume: int = volume
         self.ttl: Optional[int] = ttl
+        # TODO: Type validation
 
 
 class CancelLog(Log):
     """Cancel type log class.
 
     This log is usually generated when a cancel order is accepted by markets.
     """
@@ -112,14 +113,15 @@
         self.order_time: int = order_time
         self.agent_id: int = agent_id
         self.is_buy: bool = is_buy
         self.kind: OrderKind = kind
         self.price: Optional[float] = price
         self.volume: int = volume
         self.ttl: Optional[int] = ttl
+        # TODO: Type validation
 
 
 class ExecutionLog(Log):
     """Execution type log class.
 
     This log is usually generated when an order is executed on markets.
     """
@@ -151,72 +153,73 @@
         self.time: int = time
         self.buy_agent_id: int = buy_agent_id
         self.sell_agent_id: int = sell_agent_id
         self.buy_order_id: int = buy_order_id
         self.sell_order_id: int = sell_order_id
         self.price: float = price
         self.volume: int = volume
+        # TODO: Type validation
 
 
 class SimulationBeginLog(Log):
     """Simulation beginning log class."""
 
-    def __init__(self, simulator: "Simulator"):  # type: ignore
+    def __init__(self, simulator: "Simulator"):  # type: ignore  # NOQA
         """initialize.
 
         Args:
             simulator (:class:`pams.Simulator`): simulator.
         """
         self.simulator = simulator
 
 
 class SimulationEndLog(Log):
     """Simulation ending log class."""
 
-    def __init__(self, simulator: "Simulator"):  # type: ignore
+    def __init__(self, simulator: "Simulator"):  # type: ignore  # NOQA
         """initialize.
 
         Args:
             simulator (:class:`pams.Simulator`): simulator.
         """
         self.simulator = simulator
 
 
 class SessionBeginLog(Log):
     """Session beginning log class."""
 
-    def __init__(self, session: "Session", simulator: "Simulator"):  # type: ignore
+    def __init__(self, session: "Session", simulator: "Simulator"):  # type: ignore  # NOQA
         """initialize.
 
         Args:
             session (:class:`pams.Session`): session.
             simulator (:class:`pams.Simulator`): simulator.
         """
         self.simulator = simulator
         self.session = session
 
 
 class SessionEndLog(Log):
     """Session ending log class."""
 
-    def __init__(self, session: "Session", simulator: "Simulator"):  # type: ignore
+    def __init__(self, session: "Session", simulator: "Simulator"):  # type: ignore  # NOQA
         """initialize.
 
         Args:
             session (:class:`pams.Session`): session.
             simulator (:class:`pams.Simulator`): simulator.
         """
         self.simulator = simulator
         self.session = session
 
 
 class MarketStepBeginLog(Log):
     """Market step beginning log class."""
 
-    def __init__(self, session: "Session", market: "Market", simulator: "Simulator"):  # type: ignore
+    def __init__(self, session: "Session", market: "Market", simulator: "Simulator"):  # type: ignore  # NOQA
         """initialize.
 
         Args:
             session (:class:`pams.Session`): session.
             market (:class:`pams.Market`): market.
             simulator (:class:`pams.Simulator`): simulator.
         """
@@ -224,15 +227,15 @@
         self.market = market
         self.simulator = simulator
 
 
 class MarketStepEndLog(Log):
     """Market step ending log class."""
 
-    def __init__(self, session: "Session", market: "Market", simulator: "Simulator"):  # type: ignore
+    def __init__(self, session: "Session", market: "Market", simulator: "Simulator"):  # type: ignore  # NOQA
         """initialize.
 
         Args:
             session (:class:`pams.Session`): session.
             market (:class:`pams.Market`): market.
             simulator (:class:`pams.Simulator`): simulator.
         """
@@ -252,21 +255,21 @@
     Therefore, the logging sequence of market 1 and market 2 is not always the same.
     For handling this problem, logger should save the logs from those markets and the end of each step,
      the logs are processed and written.
     However, for some implementation, non-blocking log writing should be also supported.
     Therefore, this logger has 2 methods to handling logs -- :func:`write` and :func:`write_and_direct_process`
     """
 
-    simulator: "Simulator"  # type: ignore
+    simulator: "Simulator"  # type: ignore  # NOQA
 
     def __init__(self) -> None:
         """initialize logger."""
         self.pending_logs: List[Log] = []
 
-    def _set_simulator(self, simulator: "Simulator") -> None:  # type: ignore
+    def _set_simulator(self, simulator: "Simulator") -> None:  # type: ignore  # NOQA
         """set simulator.
 
         Args:
             simulator (:class:`pams.Simulator`): simulator.
 
         Returns:
             None
```

### Comparing `pams-0.0.9/pams/logs/market_step_loggers.py` & `pams-0.1.0/pams/logs/market_step_loggers.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,17 @@
             f"{log.session.session_id} {log.market.get_time()} {log.market.market_id} {log.market.name} {log.market.get_market_price()} {log.market.get_fundamental_price()}"
         )
 
 
 class MarketStepSaver(Logger):
     """Saver of the market step class."""
 
-    market_step_logs: List[Dict] = []
+    def __init__(self) -> None:
+        super().__init__()
+        self.market_step_logs: List[Dict] = []
 
     def process_market_step_end_log(self, log: MarketStepEndLog) -> None:
         """stack the market log.
 
         Args:
             log (:class:`pams.logs.MarketStepEndLog`): market log.
```

### Comparing `pams-0.0.9/pams/runners/base.py` & `pams-0.1.0/pams/runners/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,71 @@
 import json
 import os
 import random
 import time
 from abc import ABC
 from abc import abstractmethod
+from io import TextIOBase
 from io import TextIOWrapper
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import TextIO
 from typing import Type
 from typing import Union
 
+from ..agents import Agent
+from ..agents import HighFrequencyAgent
 from ..logs.base import Logger
 from ..simulator import Simulator
 
 
 class Runner(ABC):
     """Runner of the market simulator class (Abstract class).
 
     .. seealso::
         - :class:`pams.runners.SequentialRunner`
     """
 
     def __init__(
         self,
-        settings: Union[Dict, TextIOWrapper, os.PathLike, str],
+        settings: Union[Dict, TextIOBase, TextIO, TextIOWrapper, os.PathLike, str],
         prng: Optional[random.Random] = None,
         logger: Optional[Logger] = None,
         simulator_class: Type[Simulator] = Simulator,
     ):
         """initialize.
 
         Args:
-            settings (Union[Dict, TextIOWrapper, os.PathLike, str]): runner configuration.
+            settings (Union[Dict, TextIOBase, TextIO, TextIOWrapper, os.PathLike, str]): runner configuration.
                 You can set python dictionary, a file pointer, or a file path.
             prng (random.Random, Optional): pseudo random number generator for this runner.
             logger (Logger, Optional): logger instance.
             simulator_class (Type[Simulator]): type of simulator.
 
         Returns:
             None
         """
         self.settings: Dict
         if isinstance(settings, Dict):
             self.settings = settings
-        elif isinstance(settings, TextIOWrapper):
+        elif (
+            isinstance(settings, TextIOBase)
+            or isinstance(settings, TextIO)
+            or isinstance(settings, TextIOWrapper)
+        ):
             self.settings = json.load(fp=settings)
         else:
             self.settings = json.load(fp=open(settings, mode="r"))
         self._prng: random.Random = prng if prng is not None else random.Random()
         self.logger = logger
         self.simulator: Simulator = simulator_class(
             prng=random.Random(self._prng.randint(0, 2**31))
         )
-        self.registered_class: List[Type] = []
+        self.registered_classes: List[Type] = []
 
     def main(self) -> None:
         """main process. The process is executed while measuring time."""
         setup_start_time_ns = time.time_ns()
         self._setup()
         start_time_ns = time.time_ns()
         self._run()
@@ -75,21 +83,33 @@
 
         Args:
             cls (Type): class to register.
 
         Returns:
             None
         """
-        self.registered_class.append(cls)
+        self.registered_classes.append(cls)
 
     @abstractmethod
     def _setup(self) -> None:
         """internal usage class for setup. This method should be implemented in descendants."""
         pass
 
     @abstractmethod
     def _run(self) -> None:
         """internal usage class for simulation running. This method should be implemented in descendants.
 
         Usually the process in this methods should be control simulation flow and parallelization.
         """
         pass
+
+    @staticmethod
+    def judge_hft_or_not(agent: Agent) -> bool:
+        """determine if the agent is type of the :class:`pams.agents.HighFrequencyAgent`.
+
+        Args:
+            agent (Agent): agent instance.
+
+        Returns:
+            bool: whether the agent class is the :class:`pams.agents.HighFrequencyAgent` or not.
+        """
+        return isinstance(agent, HighFrequencyAgent)
```

### Comparing `pams-0.0.9/pams/runners/sequential.py` & `pams-0.1.0/pams/runners/sequential.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import os
 import random
-import time
 from io import TextIOWrapper
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Type
 from typing import Union
 
 from ..agents.base import Agent
-from ..agents.high_frequency_agent import HighFrequencyAgent
 from ..events import EventABC
 from ..events import EventHook
 from ..index_market import IndexMarket
 from ..logs.base import CancelLog
 from ..logs.base import ExecutionLog
 from ..logs.base import Log
 from ..logs.base import Logger
@@ -34,32 +32,58 @@
 from ..simulator import Simulator
 from ..utils.class_finder import find_class
 from ..utils.json_extends import json_extends
 from .base import Runner
 
 
 class SequentialRunner(Runner):
+    """Sequential runner class."""
+
     def __init__(
         self,
         settings: Union[Dict, TextIOWrapper, os.PathLike, str],
         prng: Optional[random.Random] = None,
         logger: Optional[Logger] = None,
         simulator_class: Type[Simulator] = Simulator,
     ):
+        """initialize.
+
+        Args:
+            settings (Union[Dict, TextIOWrapper, os.PathLike, str]): runner configuration.
+            prng (random.Random, Optional): pseudo random number generator for this runner.
+            logger (Logger, Optional): logger instance.
+            simulator_class (Type[Simulator]): type of simulator.
+
+        Returns:
+            None
+        """
         super().__init__(settings, prng, logger, simulator_class)
         self._pending_setups: List[Tuple[Callable, Dict]] = []
 
-    @staticmethod
-    def judge_hft_or_not(agent: Agent) -> bool:
-        return isinstance(agent, HighFrequencyAgent)
-
     def _generate_markets(self, market_type_names: List[str]) -> None:
+        """generate markets. (Internal method)
+
+        Args:
+            market_type_names (List[str]): name list of market type.
+
+        Returns:
+            None
+        """
         i_market = 0
         for name in market_type_names:
+            if name not in self.settings:
+                raise ValueError(f"{name} setting is missing in config")
             market_settings: Dict = self.settings[name]
+            market_settings = json_extends(
+                whole_json=self.settings,
+                parent_name=name,
+                target_json=market_settings,
+                excludes_fields=["from", "to"],
+            )
+            # TODO: warn "from" and "to" is included in parent setting and not set to this setting.
             n_markets = 1
             id_from = 0
             id_to = 0
             if "numMarkets" in market_settings:
                 n_markets = int(market_settings["numMarkets"])
                 id_to = n_markets - 1
             if "from" in market_settings or "to" in market_settings:
@@ -67,32 +91,34 @@
                     raise ValueError(
                         f"both {name}.from and {name}.to are required in json file if you use"
                     )
                 if "numMarkets" in market_settings:
                     raise ValueError(
                         f"{name}.numMarkets and ({name}.from or {name}.to) cannot be used at the same time"
                     )
-                n_markets = market_settings["to"] - market_settings["from"]
-                id_from = market_settings["from"]
-                id_to = market_settings["to"]
+                n_markets = int(market_settings["to"]) - int(market_settings["from"])
+                id_from = int(market_settings["from"])
+                id_to = int(market_settings["to"])
+            if "numMarkets" in market_settings:
+                del market_settings["numMarkets"]
+            if "from" in market_settings:
+                del market_settings["from"]
+            if "to" in market_settings:
+                del market_settings["to"]
             prefix: str
             if "prefix" in market_settings:
                 prefix = market_settings["prefix"]
+                del market_settings["prefix"]
             else:
                 prefix = name + ("-" if n_markets > 1 else "")
-            market_settings = json_extends(
-                whole_json=self.settings,
-                parent_name=name,
-                target_json=market_settings,
-                excludes_fields=["numMarkets", "from", "to", "prefix"],
-            )
             if "class" not in market_settings:
                 raise ValueError(f"class is not defined for {name}")
             market_class: Type[Market] = find_class(
-                name=market_settings["class"], optional_class_list=self.registered_class
+                name=market_settings["class"],
+                optional_class_list=self.registered_classes,
             )
             if not issubclass(market_class, Market):
                 raise ValueError(
                     f"market class for {name} does not inherit Market class"
                 )
             if "fundamentalPrice" in market_settings:
                 fundamental_price = float(market_settings["fundamentalPrice"])
@@ -127,17 +153,34 @@
                         volatility=fundamental_volatility,
                     )
                 self._pending_setups.append(
                     (market.setup, {"settings": market_settings})
                 )
 
     def _generate_agents(self, agent_type_names: List[str]) -> None:
+        """generate agents. (Internal method)
+
+        Args:
+            agent_type_names (List[str]): name list of agent type.
+
+        Returns:
+            None
+        """
         i_agent = 0
         for name in agent_type_names:
+            if name not in self.settings:
+                raise ValueError(f"{name} setting is missing in config")
             agent_settings: Dict = self.settings[name]
+            agent_settings = json_extends(
+                whole_json=self.settings,
+                parent_name=name,
+                target_json=agent_settings,
+                excludes_fields=["from", "to"],
+            )
+            # TODO: warn "from" and "to" is included in parent setting and not set to this setting.
             n_agents = 1
             id_from = 0
             id_to = 0
             if "numAgents" in agent_settings:
                 n_agents = int(agent_settings["numAgents"])
                 id_to = n_agents - 1
             if "from" in agent_settings or "to" in agent_settings:
@@ -145,37 +188,38 @@
                     raise ValueError(
                         f"both {name}.from and {name}.to are required in json file if you use"
                     )
                 if "numAgents" in agent_settings:
                     raise ValueError(
                         f"{name}.numMarkets and ({name}.from or {name}.to) cannot be used at the same time"
                     )
-                n_agents = agent_settings["to"] - agent_settings["from"]
-                id_from = agent_settings["from"]
-                id_to = agent_settings["to"]
+                n_agents = int(agent_settings["to"]) - int(agent_settings["from"])
+                id_from = int(agent_settings["from"])
+                id_to = int(agent_settings["to"])
+            if "numAgents" in agent_settings:
+                del agent_settings["numAgents"]
+            if "from" in agent_settings:
+                del agent_settings["from"]
+            if "to" in agent_settings:
+                del agent_settings["to"]
             prefix: str
             if "prefix" in agent_settings:
                 prefix = agent_settings["prefix"]
+                del agent_settings["prefix"]
             else:
                 prefix = name + ("-" if n_agents > 1 else "")
-            agent_settings = json_extends(
-                whole_json=self.settings,
-                parent_name=name,
-                target_json=agent_settings,
-                excludes_fields=["numAgents", "from", "to", "prefix"],
-            )
+
             if "class" not in agent_settings:
                 raise ValueError(f"class is not defined for {name}")
             agent_class: Type[Agent] = find_class(
-                name=agent_settings["class"], optional_class_list=self.registered_class
+                name=agent_settings["class"],
+                optional_class_list=self.registered_classes,
             )
             if not issubclass(agent_class, Agent):
-                raise ValueError(
-                    f"market class for {name} does not inherit Market class"
-                )
+                raise ValueError(f"agent class for {name} does not inherit Agent class")
             if "markets" not in agent_settings:
                 raise ValueError(f"markets is required in {name}")
             accessible_market_names: List[str] = agent_settings["markets"]
             accessible_market_ids: List[int] = sum(
                 [
                     list(
                         map(
@@ -204,39 +248,52 @@
                             "settings": agent_settings,
                             "accessible_markets_ids": accessible_market_ids,
                         },
                     )
                 )
 
     def _set_fundamental_correlation(self) -> None:
+        """set fundamental correlation. (Internal method)"""
         if "fundamentalCorrelations" in self.settings["simulation"]:
             corr_settings: Dict = self.settings["simulation"]["fundamentalCorrelations"]
             for key, value in corr_settings.items():
                 if key == "pairwise":
                     if (
                         not isinstance(value, list)
                         or sum([len(x) != 3 for x in value]) > 0
                     ):
                         raise ValueError(
                             "simulation.fundamentalCorrelations.pairwise has invalid format data"
                         )
                     for (market1_name, market2_name, corr) in value:
                         market1 = self.simulator.name2market[market1_name]
                         market2 = self.simulator.name2market[market2_name]
+                        for m in [market1, market2]:
+                            if (
+                                self.simulator.fundamentals.volatilities[m.market_id]
+                                == 0.0
+                            ):
+                                raise ValueError(
+                                    f"For applying fundamental correlation fo {m.name}, "
+                                    f"fundamentalVolatility for {m.name} is required"
+                                )
                         self.simulator.fundamentals.set_correlation(
                             market_id1=market1.market_id,
                             market_id2=market2.market_id,
                             corr=float(corr),
                         )
                 else:
                     raise NotImplementedError(
                         f"{key} for simulation.fundamentalCorrelations is not supported"
                     )
 
     def _generate_sessions(self) -> None:
+        """generate sessions. (Internal method)"""
+        if "sessions" not in self.settings["simulation"]:
+            raise ValueError("sessions is missing under 'simulation' config")
         session_settings: Dict = self.settings["simulation"]["sessions"]
         if not isinstance(session_settings, list):
             raise ValueError("simulation.sessions must be list[dict]")
         i_session = 0
         i_event = 0
         session_start_time: int = 0
         for session_setting in session_settings:
@@ -245,15 +302,15 @@
                     "for each element in simulation.sessions must have sessionName"
                 )
             session = Session(
                 session_id=i_session,
                 prng=random.Random(self._prng.randint(0, 2**31)),
                 session_start_time=session_start_time,
                 simulator=self.simulator,
-                name=session_setting["sessionName"],
+                name=str(session_setting["sessionName"]),
                 logger=self.logger,
             )
             i_session += 1
             if "iterationSteps" not in session_setting:
                 raise ValueError(
                     "iterationSteps is required in each element of simulation.sessions"
                 )
@@ -270,15 +327,16 @@
                         target_json=event_setting,
                         excludes_fields=["numMarkets", "from", "to", "prefix"],
                     )
                     if "class" not in event_setting:
                         raise ValueError(f"class is required in {event_name}")
                     event_class_name = event_setting["class"]
                     event_class: Type[EventABC] = find_class(
-                        name=event_class_name, optional_class_list=self.registered_class
+                        name=event_class_name,
+                        optional_class_list=self.registered_classes,
                     )
                     event = event_class(
                         event_id=i_event,
                         prng=random.Random(self._prng.randint(0, 2**31)),
                         session=session,
                         simulator=self.simulator,
                         name=event_name,
@@ -292,14 +350,15 @@
                         event_hooks: List[EventHook] = _event.hook_registration()
                         for event_hook in event_hooks:
                             self.simulator._add_event(event_hook)
 
                     self._pending_setups.append((event_hook_setup, {"_event": event}))
 
     def _setup(self) -> None:
+        """runner setup. (Internal method)"""
         if "simulation" not in self.settings:
             raise ValueError("simulation is required in json file")
 
         if "markets" not in self.settings["simulation"]:
             raise ValueError("simulation.markets is required in json file")
         market_type_names: List[str] = self.settings["simulation"]["markets"]
         if (
@@ -328,15 +387,26 @@
             or sum([not isinstance(m, dict) for m in session_settings]) > 0
         ):
             raise ValueError("simulation.sessions in json file have to be List[Dict]")
         self._generate_sessions()
 
         _ = [func(**kwargs) for func, kwargs in self._pending_setups]
 
-    def _collect_orders(self, session: Session) -> List[List[Union[Order, Cancel]]]:
+    def _collect_orders_from_normal_agents(
+        self, session: Session
+    ) -> List[List[Union[Order, Cancel]]]:
+        """collect orders from normal_agents. (Internal method)
+        orders are corrected until the total number of orders reaches max_normal_orders
+
+        Args:
+            session (Session): session.
+
+        Returns:
+            List[List[Union[Order, Cancel]]]: orders lists.
+        """
         agents = self.simulator.normal_frequency_agents
         agents = self._prng.sample(agents, len(agents))
         n_orders = 0
         all_orders: List[List[Union[Order, Cancel]]] = []
         for agent in agents:
             if n_orders >= session.max_normal_orders:
                 break
@@ -345,24 +415,34 @@
                 if not session.with_order_placement:
                     raise AssertionError("currently order is not accepted")
                 if sum([order.agent_id != agent.agent_id for order in orders]) > 0:
                     raise ValueError(
                         "spoofing order is not allowed. please check agent_id in order"
                     )
                 all_orders.append(orders)
+                # TODO: currently the original impl is used
+                # n_orders += len(orders)
                 n_orders += 1
         return all_orders
 
     def _handle_orders(
         self, session: Session, local_orders: List[List[Union[Order, Cancel]]]
     ) -> List[List[Union[Order, Cancel]]]:
-        agents = self.simulator.high_frequency_agents
-        agents = self._prng.sample(agents, len(agents))
+        """handle orders. (Internal method)
+        processing local orders and correct and process the orders from high frequency agents.
+
+        Args:
+            session (Session): session.
+            local_orders (List[List[Union[Order, Cancel]]]): local orders.
+
+        Returns:
+            List[List[Union[Order, Cancel]]]: order lists.
+        """
         sequential_orders = self._prng.sample(local_orders, len(local_orders))
-        all_orders: List[List[Union[Order, Cancel]]] = []
+        all_orders: List[List[Union[Order, Cancel]]] = [*sequential_orders]
         for orders in sequential_orders:
             for order in orders:
                 if not session.with_order_placement:
                     raise AssertionError("currently order is not accepted")
                 market: Market = self.simulator.id2market[order.market_id]
                 if isinstance(order, Order):
                     self.simulator._trigger_event_before_order(order=order)
@@ -371,15 +451,15 @@
                     agent.submitted_order(log=log)
                     self.simulator._trigger_event_after_order(order_log=log)
                 elif isinstance(order, Cancel):
                     self.simulator._trigger_event_before_cancel(cancel=order)
                     log_: CancelLog = market._cancel_order(cancel=order)
                     agent = self.simulator.id2agent[order.order.agent_id]
                     agent.canceled_order(log=log_)
-                    self.simulator._trigger_event_after_cancel(cancel_log=order)
+                    self.simulator._trigger_event_after_cancel(cancel_log=log_)
                 else:
                     raise NotImplementedError
                 if session.with_order_execution:
                     logs: List[ExecutionLog] = market._execution()
                     self.simulator._update_agents_for_execution(execution_logs=logs)
                     for execution_log in logs:
                         agent = self.simulator.id2agent[execution_log.buy_agent_id]
@@ -390,14 +470,16 @@
                             execution_log=execution_log
                         )
 
             if session.high_frequency_submission_rate < self._prng.random():
                 continue
 
             n_high_freq_orders = 0
+            agents = self.simulator.high_frequency_agents
+            agents = self._prng.sample(agents, len(agents))
             for agent in agents:
                 if n_high_freq_orders >= session.max_high_frequency_orders:
                     break
 
                 high_freq_orders: List[Union[Order, Cancel]] = agent.submit_orders(
                     markets=self.simulator.markets
                 )
@@ -413,47 +495,65 @@
                         )
                         > 0
                     ):
                         raise ValueError(
                             "spoofing order is not allowed. please check agent_id in order"
                         )
                     all_orders.append(high_freq_orders)
+                    # TODO: currently the original impl is used
                     n_high_freq_orders += 1
+                    # n_high_freq_orders += len(high_freq_orders)
                     for order in high_freq_orders:
                         market = self.simulator.id2market[order.market_id]
                         if isinstance(order, Order):
                             self.simulator._trigger_event_before_order(order=order)
                             log = market._add_order(order=order)
                             agent = self.simulator.id2agent[order.agent_id]
                             agent.submitted_order(log=log)
                             self.simulator._trigger_event_after_order(order_log=log)
                         elif isinstance(order, Cancel):
                             self.simulator._trigger_event_before_cancel(cancel=order)
                             log_ = market._cancel_order(cancel=order)
                             agent = self.simulator.id2agent[order.order.agent_id]
                             agent.canceled_order(log=log_)
-                            self.simulator._trigger_event_after_cancel(cancel_log=order)
+                            self.simulator._trigger_event_after_cancel(cancel_log=log_)
                         else:
                             raise NotImplementedError
                         if session.with_order_execution:
                             logs = market._execution()
                             for execution_log in logs:
                                 agent.executed_order(log=execution_log)
                                 self.simulator._trigger_event_after_execution(
                                     execution_log=execution_log
                                 )
         return all_orders
 
     def _update_markets(self, session: Session) -> None:
-        local_orders: List[List[Union[Order, Cancel]]] = self._collect_orders(
-            session=session
-        )
+        """update markets. (Internal method)
+
+        Args:
+            session (Session): session.
+
+        Returns:
+            None
+        """
+        local_orders: List[
+            List[Union[Order, Cancel]]
+        ] = self._collect_orders_from_normal_agents(session=session)
         self._handle_orders(session=session, local_orders=local_orders)
 
     def _iterate_market_updates(self, session: Session) -> None:
+        """iterate market updates. (Internal method)
+
+        Args:
+            session (Session): session.
+
+        Returns:
+            None
+        """
         markets: List[Market] = self.simulator.markets
         for market in markets:
             market._is_running = session.with_order_execution
 
         for _ in range(session.iteration_steps):
             for market in markets:
                 self.simulator._trigger_event_before_step_for_market(market=market)
@@ -470,14 +570,15 @@
                         session=session, market=market, simulator=self.simulator
                     )
                     log.read_and_write_with_direct_process(logger=self.logger)
                 self.simulator._trigger_event_after_step_for_market(market=market)
             self.simulator._update_times_on_markets(self.simulator.markets)  # t++
 
     def _run(self) -> None:
+        """main process. (Internal method)"""
         if self.logger is not None:
             log: Log = SimulationBeginLog(simulator=self.simulator)  # must be blocking
             log.read_and_write(logger=self.logger)
             self.logger._process()
         self.simulator._update_times_on_markets(self.simulator.markets)  # t: -1 -> 0
 
         for session in self.simulator.sessions:
```

### Comparing `pams-0.0.9/pams/utils/class_finder.py` & `pams-0.1.0/pams/utils/class_finder.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,30 @@
 from typing import List
 from typing import Optional
 from typing import Type
 
 
 def find_class(name: str, optional_class_list: Optional[List[Type]] = None) -> Type:
+    """find class from pams name spaces.
+
+    .. seealso::
+        If you want to use user-defined classes, please use :class:`pams.runners.class_register`.
+
+    Args:
+        name (str): class name.
+        optional_class_list (List[Type], Optional): optional class list.
+
+    Returns:
+        Type: class type.
+    """
     _1 = __import__("pams", globals(), locals())
     _2 = __import__("pams.agents", globals(), locals(), ["*"])
     _3 = __import__("pams.events", globals(), locals(), ["*"])
+    _4 = __import__("pams.logs", globals(), locals(), ["*"])
+    _5 = __import__("pams.utils", globals(), locals(), ["*"])
 
     candidates_spaces = [*globals().values(), *locals().values()]
 
     object_class_candidates = [
         getattr(m, name) for m in candidates_spaces if hasattr(m, name)
     ]
     if optional_class_list is not None:
```

### Comparing `pams-0.0.9/pyproject.toml` & `pams-0.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 [tool.poetry]
 name = "pams"
-version = "0.0.9"
+version = "0.1.0"
 description = "PAMS: Platform for Artificial Market Simulations"
 authors = ["Masanori HIRANO <masa.hirano.1996@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 tqdm = "^4.64.1"
-numpy = [
-    {version = "^1.23.4", python = ">=3.8,<4.0"},
-    {version = "^1.21.0", python = ">=3.7,<3.8"}
-]
-scipy = [
-    {version = "^1.9.2", python = ">=3.8,<4.0"},
-    {version = "^1.7.0", python = ">=3.7,<3.8"}
-]
+numpy = "^1.23.4"
+scipy = "^1.9.2"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
 isort = "^5.10.1"
 mypy = "^0.982"
 pytest = "^7.1.3"
@@ -28,21 +22,48 @@
 Sphinx = "^5.3.0"
 furo = "^2022.9.29"
 jupyter = "^1.0.0"
 matplotlib = "^3.4.2"
 sphinx-intl = "^2.0.1"
 sphinx-copybutton = "^0.5.0"
 sphinx-autodoc-typehints = "^1.19.5"
+flake8 = "^6.0.0"
+pyproject-flake8 = "^6.0.0.post1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 [tool.black]
 skip-magic-trailing-comma = true
 
 [tool.isort]
 profile = 'black'
 force_single_line = true
+skip = [
+    ".git",
+    "__pycache__",
+    "docs",
+    "build",
+    "dist",
+    "examples",
+    ".venv",
+    "tests/examples"
+]
 
 [tool.mypy]
 disallow_untyped_defs = true
 ignore_missing_imports = true
+
+[tool.flake8]
+ignore = "E203,E231,E501,W503"
+max-line-length = 88
+exclude = [
+    ".git",
+    "__pycache__",
+    "docs",
+    "build",
+    "dist",
+    "examples",
+    ".venv",
+    "__init__.py"
+    ]
+select = "B,B950,C,E,F,W"
```

### Comparing `pams-0.0.9/PKG-INFO` & `pams-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 Metadata-Version: 2.1
 Name: pams
-Version: 0.0.9
+Version: 0.1.0
 Summary: PAMS: Platform for Artificial Market Simulations
 License: MIT
 Author: Masanori HIRANO
 Author-email: masa.hirano.1996@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: numpy (>=1.21.0,<2.0.0) ; python_version >= "3.7" and python_version < "3.8"
-Requires-Dist: numpy (>=1.23.4,<2.0.0) ; python_version >= "3.8" and python_version < "4.0"
-Requires-Dist: scipy (>=1.7.0,<2.0.0) ; python_version >= "3.7" and python_version < "3.8"
-Requires-Dist: scipy (>=1.9.2,<2.0.0) ; python_version >= "3.8" and python_version < "4.0"
+Requires-Dist: numpy (>=1.23.4,<2.0.0)
+Requires-Dist: scipy (>=1.9.2,<2.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 # pams
 PAMS: Platform for Artificial Market Simulations
 
 [![python](https://img.shields.io/pypi/pyversions/pams.svg)](https://pypi.org/project/pams)
```

