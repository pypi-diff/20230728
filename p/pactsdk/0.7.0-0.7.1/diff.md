# Comparing `tmp/pactsdk-0.7.0.tar.gz` & `tmp/pactsdk-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pactsdk-0.7.0.tar", max compression
+gzip compressed data, was "pactsdk-0.7.1.tar", max compression
```

## Comparing `pactsdk-0.7.0.tar` & `pactsdk-0.7.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1063 2022-07-14 08:55:23.297528 pactsdk-0.7.0/LICENSE
--rw-r--r--   0        0        0     5482 2023-03-30 10:07:17.918258 pactsdk-0.7.0/README.md
--rw-r--r--   0        0        0      680 2023-06-12 13:14:44.907642 pactsdk-0.7.0/pactsdk/__init__.py
--rw-r--r--   0        0        0     4504 2023-01-03 15:45:49.490178 pactsdk-0.7.0/pactsdk/add_liquidity.py
--rw-r--r--   0        0        0     2174 2022-07-14 08:55:23.297528 pactsdk-0.7.0/pactsdk/api.py
--rw-r--r--   0        0        0     8096 2023-03-30 09:06:45.857841 pactsdk-0.7.0/pactsdk/asset.py
--rw-r--r--   0        0        0     6971 2023-06-12 13:14:34.580973 pactsdk-0.7.0/pactsdk/client.py
--rw-r--r--   0        0        0     2085 2023-06-12 13:14:34.580973 pactsdk-0.7.0/pactsdk/config.py
--rw-r--r--   0        0        0     2353 2023-06-05 09:02:08.789645 pactsdk-0.7.0/pactsdk/constant_product_calculator.py
--rw-r--r--   0        0        0      962 2023-06-12 13:14:34.580973 pactsdk-0.7.0/pactsdk/encoding.py
--rw-r--r--   0        0        0      143 2022-07-14 08:55:23.297528 pactsdk-0.7.0/pactsdk/exceptions.py
--rw-r--r--   0        0        0      191 2023-03-30 09:06:45.871175 pactsdk-0.7.0/pactsdk/factories/__init__.py
--rw-r--r--   0        0        0     6986 2023-03-30 09:06:45.874508 pactsdk-0.7.0/pactsdk/factories/base_factory.py
--rw-r--r--   0        0        0     1950 2023-03-30 09:06:45.874508 pactsdk-0.7.0/pactsdk/factories/constant_product.py
--rw-r--r--   0        0        0     1000 2023-03-30 09:06:45.874508 pactsdk-0.7.0/pactsdk/factories/get_pool_factory.py
--rw-r--r--   0        0        0     4637 2023-03-30 09:06:45.847841 pactsdk-0.7.0/pactsdk/farming/README.md
--rw-r--r--   0        0        0      565 2023-03-30 09:06:45.847841 pactsdk-0.7.0/pactsdk/farming/__init__.py
--rw-r--r--   0        0        0     7907 2023-04-11 09:21:34.039780 pactsdk-0.7.0/pactsdk/farming/escrow.py
--rw-r--r--   0        0        0    16770 2023-04-11 09:21:34.039780 pactsdk-0.7.0/pactsdk/farming/farm.py
--rw-r--r--   0        0        0     5785 2023-03-30 09:06:45.851175 pactsdk-0.7.0/pactsdk/farming/farm_state.py
--rw-r--r--   0        0        0      786 2023-03-30 09:06:45.861175 pactsdk-0.7.0/pactsdk/farming/farming_client.py
--rw-r--r--   0        0        0    20492 2023-06-12 13:14:34.580973 pactsdk-0.7.0/pactsdk/folks_lending_pool.py
--rw-r--r--   0        0        0     1484 2023-03-30 09:06:45.854508 pactsdk-0.7.0/pactsdk/gas_station.py
--rw-r--r--   0        0        0    24155 2023-03-30 10:07:05.564919 pactsdk-0.7.0/pactsdk/pool.py
--rw-r--r--   0        0        0    11887 2023-03-30 09:06:45.871175 pactsdk-0.7.0/pactsdk/pool_calculator.py
--rw-r--r--   0        0        0     2863 2023-03-30 09:06:45.871175 pactsdk-0.7.0/pactsdk/pool_state.py
--rw-r--r--   0        0        0    12291 2023-01-03 15:45:34.790183 pactsdk-0.7.0/pactsdk/stableswap_calculator.py
--rw-r--r--   0        0        0     5592 2022-07-14 08:55:23.300861 pactsdk-0.7.0/pactsdk/swap.py
--rw-r--r--   0        0        0     1905 2023-03-30 09:06:45.854508 pactsdk-0.7.0/pactsdk/transaction_group.py
--rw-r--r--   0        0        0     2166 2023-06-01 12:21:01.694131 pactsdk-0.7.0/pactsdk/utils.py
--rw-r--r--   0        0        0     5535 2022-08-18 13:32:35.849222 pactsdk-0.7.0/pactsdk/zap.py
--rw-r--r--   0        0        0     1064 2023-06-12 13:14:49.660976 pactsdk-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     6214 1970-01-01 00:00:00.000000 pactsdk-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2022-07-14 08:55:23.297528 pactsdk-0.7.1/LICENSE
+-rw-r--r--   0        0        0     5478 2023-07-25 08:24:33.039267 pactsdk-0.7.1/README.md
+-rw-r--r--   0        0        0      680 2023-07-28 09:37:58.285459 pactsdk-0.7.1/pactsdk/__init__.py
+-rw-r--r--   0        0        0     6055 2023-07-25 08:24:33.039267 pactsdk-0.7.1/pactsdk/add_liquidity.py
+-rw-r--r--   0        0        0     2195 2023-07-28 09:38:15.568433 pactsdk-0.7.1/pactsdk/api.py
+-rw-r--r--   0        0        0     8096 2023-03-30 09:06:45.857841 pactsdk-0.7.1/pactsdk/asset.py
+-rw-r--r--   0        0        0     6971 2023-06-12 13:14:34.580973 pactsdk-0.7.1/pactsdk/client.py
+-rw-r--r--   0        0        0     2085 2023-06-12 13:14:34.580973 pactsdk-0.7.1/pactsdk/config.py
+-rw-r--r--   0        0        0     2353 2023-06-05 09:02:08.789645 pactsdk-0.7.1/pactsdk/constant_product_calculator.py
+-rw-r--r--   0        0        0      962 2023-06-12 13:14:34.580973 pactsdk-0.7.1/pactsdk/encoding.py
+-rw-r--r--   0        0        0      143 2022-07-14 08:55:23.297528 pactsdk-0.7.1/pactsdk/exceptions.py
+-rw-r--r--   0        0        0      191 2023-03-30 09:06:45.871175 pactsdk-0.7.1/pactsdk/factories/__init__.py
+-rw-r--r--   0        0        0     6986 2023-03-30 09:06:45.874508 pactsdk-0.7.1/pactsdk/factories/base_factory.py
+-rw-r--r--   0        0        0     1950 2023-03-30 09:06:45.874508 pactsdk-0.7.1/pactsdk/factories/constant_product.py
+-rw-r--r--   0        0        0     1000 2023-03-30 09:06:45.874508 pactsdk-0.7.1/pactsdk/factories/get_pool_factory.py
+-rw-r--r--   0        0        0     4637 2023-03-30 09:06:45.847841 pactsdk-0.7.1/pactsdk/farming/README.md
+-rw-r--r--   0        0        0      565 2023-03-30 09:06:45.847841 pactsdk-0.7.1/pactsdk/farming/__init__.py
+-rw-r--r--   0        0        0     7907 2023-04-11 09:21:34.039780 pactsdk-0.7.1/pactsdk/farming/escrow.py
+-rw-r--r--   0        0        0    16770 2023-04-11 09:21:34.039780 pactsdk-0.7.1/pactsdk/farming/farm.py
+-rw-r--r--   0        0        0     5785 2023-03-30 09:06:45.851175 pactsdk-0.7.1/pactsdk/farming/farm_state.py
+-rw-r--r--   0        0        0      786 2023-03-30 09:06:45.861175 pactsdk-0.7.1/pactsdk/farming/farming_client.py
+-rw-r--r--   0        0        0    20711 2023-07-25 08:24:33.039267 pactsdk-0.7.1/pactsdk/folks_lending_pool.py
+-rw-r--r--   0        0        0     1484 2023-03-30 09:06:45.854508 pactsdk-0.7.1/pactsdk/gas_station.py
+-rw-r--r--   0        0        0    22903 2023-07-28 09:38:15.568433 pactsdk-0.7.1/pactsdk/pool.py
+-rw-r--r--   0        0        0    11887 2023-03-30 09:06:45.871175 pactsdk-0.7.1/pactsdk/pool_calculator.py
+-rw-r--r--   0        0        0     2863 2023-03-30 09:06:45.871175 pactsdk-0.7.1/pactsdk/pool_state.py
+-rw-r--r--   0        0        0    12291 2023-01-03 15:45:34.790183 pactsdk-0.7.1/pactsdk/stableswap_calculator.py
+-rw-r--r--   0        0        0     5592 2022-07-14 08:55:23.300861 pactsdk-0.7.1/pactsdk/swap.py
+-rw-r--r--   0        0        0     1905 2023-03-30 09:06:45.854508 pactsdk-0.7.1/pactsdk/transaction_group.py
+-rw-r--r--   0        0        0     2166 2023-06-01 12:21:01.694131 pactsdk-0.7.1/pactsdk/utils.py
+-rw-r--r--   0        0        0     5579 2023-07-25 08:24:33.039267 pactsdk-0.7.1/pactsdk/zap.py
+-rw-r--r--   0        0        0     1064 2023-07-28 09:37:52.855575 pactsdk-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     6210 1970-01-01 00:00:00.000000 pactsdk-0.7.1/PKG-INFO
```

### Comparing `pactsdk-0.7.0/LICENSE` & `pactsdk-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pactsdk-0.7.0/README.md` & `pactsdk-0.7.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 #     secondary_asset_price_after_swap=1.6442824791774173,
 #     primary_asset_price_change_pct=-31.549580645715963,
 #     secondary_asset_price_change_pct=46.091142966447585,
 # )
 
 # Let's submit the swap.
 swap_tx_group = swap.prepare_tx_group(address)
-signed_tx_group = swap_tx_group.sign_txn(private_key)
+signed_tx_group = swap_tx_group.sign(private_key)
 algod.send_transactions(signed_tx_group)
 ```
 
 ## Composability of transactions.
 
 The SDK has two sets of methods for creating transactions:
```

### Comparing `pactsdk-0.7.0/pactsdk/__init__.py` & `pactsdk-0.7.1/pactsdk/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 
 from .add_liquidity import LiquidityAddition  # noqa
 from .asset import Asset, fetch_asset_by_index  # noqa
 from .client import PactClient  # noqa
 from .exceptions import PactSdkError  # noqa
 from .factories import *  # noqa
 from .farming import *  # noqa
```

### Comparing `pactsdk-0.7.0/pactsdk/add_liquidity.py` & `pactsdk-0.7.1/pactsdk/add_liquidity.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Set of utility classes for adding liquidity to the pool.
 """
 
-
+import math
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, cast
 
 from pactsdk.exceptions import PactSdkError
 from pactsdk.stableswap_calculator import (
     StableswapCalculator,
     StableswapParams,
@@ -16,21 +16,28 @@
 from .constant_product_calculator import get_constant_product_minted_liquidity_tokens
 from .transaction_group import TransactionGroup
 
 if TYPE_CHECKING:
     from .pool import Pool
 
 
+# The amount of liquidity tokens that will be locked in a contract forever when adding the first liquidity.
+MIN_LT_AMOUNT = 1000
+
+
 @dataclass
 class AddLiquidityEffect:
     """The effect of adding liquidity to the pool."""
 
     minted_liquidity_tokens: int
     """Amount of new liquidity tokens minted when adding the liquidity. All the minted tokens will be received by the liquidity provider."""
 
+    minimum_minted_liquidity_tokens: int
+    """Amount of minimum liquidity tokens received. The transaction will fail if the real value will be lower than this."""
+
     amplifier: float
     """Current stableswap amplifier. Zero for constant product pools."""
 
     bonus_pct: float
     """
     Only for stableswaps. Zero for constant product pools.
 
@@ -57,18 +64,22 @@
 
     primary_asset_amount: int
     """Amount of primary asset the will be added to the pool."""
 
     secondary_asset_amount: int
     """Amount of secondary asset the will be added to the pool."""
 
+    slippage_pct: float
+    """The maximum amount of slippage allowed in performing the add liquidity."""
+
     effect: AddLiquidityEffect = field(init=False)
     """The effect of adding the liquidity computed at the time of construction."""
 
     def __post_init__(self):
+        self._validate_liquidity_addition()
         self.effect = self.build_effect()
 
     def prepare_tx_group(self, address: str) -> TransactionGroup:
         """Creates the transactions needed to perform adding liquidity and returns them as a transaction group ready to be signed and committed.
 
         Args:
             address: The account that will be performing adding liquidity.
@@ -77,14 +88,25 @@
             A transaction group that when executed will add the liquidity to the pool.
         """
         return self.pool.prepare_add_liquidity_tx_group(
             address=address,
             liquidity_addition=self,
         )
 
+    def _validate_liquidity_addition(self):
+        if self.pool.state.total_liquidity == 0:
+            # First liquidity addition, the following condition must be met: sqrt(asset1 * asset2) - 1000 > 0
+            minted_lt = math.isqrt(
+                self.primary_asset_amount * self.secondary_asset_amount
+            )
+            if minted_lt <= MIN_LT_AMOUNT:
+                raise ValueError("Provided amounts of tokens are too low.")
+        if self.slippage_pct < 0 or self.slippage_pct > 100:
+            raise ValueError("Splippage must be between 0 and 100")
+
     def build_effect(self) -> AddLiquidityEffect:
         amplifier = 0.0
         bonus_pct = 0.0
         tx_fee = 3000
 
         swap_calc = self.pool.calculator.swap_calculator
         state = self.pool.state
@@ -118,13 +140,24 @@
                 state.total_liquidity,
             )
             if minted_liquidity_tokens <= 0:
                 raise PactSdkError(
                     "Amount of minted liquidity tokens must be greater then 0.",
                 )
 
+        minimum_minted_liquidity_tokens = round(
+            minted_liquidity_tokens
+            - (minted_liquidity_tokens * self.slippage_pct) / 100
+        )
+        minimum_minted_liquidity_tokens = max(0, minimum_minted_liquidity_tokens)
+
+        # If this is the first liquidity addition, 1000 tokens will be locked in the contract.
+        if self.pool.state.total_liquidity == 0:
+            minimum_minted_liquidity_tokens -= 1000
+
         return AddLiquidityEffect(
             minted_liquidity_tokens=minted_liquidity_tokens,
+            minimum_minted_liquidity_tokens=minimum_minted_liquidity_tokens,
             amplifier=amplifier,
             bonus_pct=bonus_pct,
             tx_fee=tx_fee,
         )
```

### Comparing `pactsdk-0.7.0/pactsdk/api.py` & `pactsdk-0.7.1/pactsdk/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,26 @@
     All keys are optional and can be omitted.
     """
 
     offset: int
     limit: int
     is_verified: str
     creator: str
-    primary_asset__algoid: int
-    secondary_asset__algoid: int
+    primary_asset__on_chain_id: int
+    secondary_asset__on_chain_id: int
     primary_asset__unit_name: str
     secondary_asset__unit_name: str
     primary_asset__name: str
     secondary_asset__name: str
 
 
 class ApiAsset(TypedDict):
     """Details about the liquidity pool assets returned from the asset pool."""
 
-    algoid: str
+    on_chain_id: str
     decimals: int
     id: int
     is_liquidity_token: bool
     is_verified: bool
     name: str
     total_amount: str
     tvl_usd: str
@@ -40,15 +40,15 @@
     volume_24h: str
 
 
 class ApiPool(TypedDict):
     """The individual pool information returned from :py:func:`pactsdk.pool.list_pools`, this contains the basic pool information."""
 
     address: str
-    appid: str
+    on_chain_id: str
     confirmed_round: int
     creator: str
     fee_amount_7d: str
     fee_amount_24h: str
     fee_usd_7d: str
     fee_usd_24h: str
     tvl_usd: str
```

### Comparing `pactsdk-0.7.0/pactsdk/asset.py` & `pactsdk-0.7.1/pactsdk/asset.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.7.0/pactsdk/client.py` & `pactsdk-0.7.1/pactsdk/client.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.7.0/pactsdk/config.py` & `pactsdk-0.7.1/pactsdk/config.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.7.0/pactsdk/constant_product_calculator.py` & `pactsdk-0.7.1/pactsdk/constant_product_calculator.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.7.0/pactsdk/encoding.py` & `pactsdk-0.7.1/pactsdk/encoding.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.7.0/pactsdk/factories/base_factory.py` & `pactsdk-0.7.1/pactsdk/factories/base_factory.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.7.0/pactsdk/factories/constant_product.py` & `pactsdk-0.7.1/pactsdk/factories/constant_product.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.7.0/pactsdk/factories/get_pool_factory.py` & `pactsdk-0.7.1/pactsdk/factories/get_pool_factory.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.7.0/pactsdk/farming/README.md` & `pactsdk-0.7.1/pactsdk/farming/README.md`

 * *Files identical despite different names*

### Comparing `pactsdk-0.7.0/pactsdk/farming/__init__.py` & `pactsdk-0.7.1/pactsdk/farming/__init__.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.7.0/pactsdk/farming/escrow.py` & `pactsdk-0.7.1/pactsdk/farming/escrow.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.7.0/pactsdk/farming/farm.py` & `pactsdk-0.7.1/pactsdk/farming/farm.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.7.0/pactsdk/farming/farm_state.py` & `pactsdk-0.7.1/pactsdk/farming/farm_state.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.7.0/pactsdk/farming/farming_client.py` & `pactsdk-0.7.1/pactsdk/farming/farming_client.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.7.0/pactsdk/folks_lending_pool.py` & `pactsdk-0.7.1/pactsdk/folks_lending_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,26 +172,30 @@
 
     primary_asset_amount: int
     """Amount of original primary asset deposited."""
 
     secondary_asset_amount: int
     """Amount of original secondary asset deposited."""
 
+    slippage_pct: float
+    """The maximum amount of slippage allowed in performing the add liquidity."""
+
     liquidity_addition: LiquidityAddition = dataclasses.field(init=False)
     """Information about actual add liquidity operation on the Pact pool."""
 
     def __post_init__(self):
         self.liquidity_addition = LiquidityAddition(
             pool=self.lending_pool_adapter.pact_pool,
             primary_asset_amount=self.lending_pool_adapter.primary_lending_pool.convert_deposit(
                 self.primary_asset_amount
             ),
             secondary_asset_amount=self.lending_pool_adapter.secondary_lending_pool.convert_deposit(
                 self.secondary_asset_amount
             ),
+            slippage_pct=self.slippage_pct,
         )
         self.liquidity_addition.effect.tx_fee = PRE_ADD_LIQ_FEE + ADD_LIQ_FEE
 
 
 @dataclasses.dataclass
 class LendingSwap:
     """A wrapper around Swap object that adds some lending specific information."""
@@ -259,19 +263,21 @@
         }
         return assets_map[f_asset]
 
     def prepare_add_liquidity(
         self,
         primary_asset_amount: int,
         secondary_asset_amount: int,
+        slippage_pct: float,
     ) -> LendingLiquidityAddition:
         return LendingLiquidityAddition(
             lending_pool_adapter=self,
             primary_asset_amount=primary_asset_amount,
             secondary_asset_amount=secondary_asset_amount,
+            slippage_pct=slippage_pct,
         )
 
     def prepare_add_liquidity_tx_group(
         self,
         address: str,
         liquidity_addition: LendingLiquidityAddition,
     ) -> TransactionGroup:
```

### Comparing `pactsdk-0.7.0/pactsdk/gas_station.py` & `pactsdk-0.7.1/pactsdk/gas_station.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.7.0/pactsdk/pool.py` & `pactsdk-0.7.1/pactsdk/pool.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,19 +124,19 @@
         primary_asset_index: The asset id for the primary asset of the pool.
         secondary_asset_index: The asset id for the secondary asset of the pool.
 
     Returns:
         List of asset ids.
     """
     params: ListPoolsParams = {
-        "primary_asset__algoid": primary_asset_index,
-        "secondary_asset__algoid": secondary_asset_index,
+        "primary_asset__on_chain_id": primary_asset_index,
+        "secondary_asset__on_chain_id": secondary_asset_index,
     }
     data = list_pools(pact_api_url, params)
-    return [int(pool["appid"]) for pool in data["results"]]
+    return [int(pool["on_chain_id"]) for pool in data["results"]]
 
 
 @dataclass
 class Pool:
     """Pool represents a liquidity pool in the PACT AMM.
 
     Typically, users don't have to instantiate this class manually. Use :py:meth:`pactsdk.client.PactClient.fetch_pool_by_id` or :py:meth:`pactsdk.client.PactClient.fetch_pools_by_assets` instead.
@@ -250,28 +250,30 @@
         self.state = self.parse_internal_state(self.internal_state)
         return self.state
 
     def prepare_add_liquidity(
         self,
         primary_asset_amount: int,
         secondary_asset_amount: int,
+        slippage_pct: float,
     ) -> LiquidityAddition:
         """
         Creates a new LiquidityAddition instance.
 
         Args:
             options: Options for adding the liquidity.
 
         Returns:
             A new LiquidityAddition object.
         """
         return LiquidityAddition(
             pool=self,
             primary_asset_amount=primary_asset_amount,
             secondary_asset_amount=secondary_asset_amount,
+            slippage_pct=slippage_pct,
         )
 
     def prepare_add_liquidity_tx_group(
         self,
         address: str,
         liquidity_addition: LiquidityAddition,
     ) -> TransactionGroup:
@@ -301,16 +303,14 @@
 
         In typical circumstances 3 transactions are generated:
 
         - deposit of asset A
         - deposit of asset B
         - "ADDLIQ" application call to add liquidity with the above deposits
 
-        For constant product pools only - if the pool is empty and the product of both assets is larger or equal 2**64 than an additional set of 3 transactions is built.
-
         The initial liquidity must satisfy the expression `sqrt(a * b) - 1000 > 0`.
 
         Args:
             address: Account address that will deposit the primary and secondary assets and receive the LP token.
             primary_asset_amount: The amount of primary asset to deposit.
             secondary_asset_amount: The amount of secondary asset to deposit.
             suggested_params: Algorand suggested parameters for transactions.
@@ -321,57 +321,34 @@
 
         Returns:
             List of transactions to add the liquidity.
         """
         primary_asset_amount = liquidity_addition.primary_asset_amount
         secondary_asset_amount = liquidity_addition.secondary_asset_amount
 
-        initial_liq_txs: list[transaction.Transaction] = []
         if self.calculator.is_empty:
             assert (
                 math.isqrt(primary_asset_amount * secondary_asset_amount) - 1000 > 0
             ), "Initial liquidity must satisfy the expression `sqrt(a * b) - 1000 > 0`"
 
-            if self.pool_type == "CONSTANT_PRODUCT":
-                # Adding initial liquidity has a limitation that the product of 2 assets must be lower than 2**64. Let's check if we can fit below the limit.
-                max_product = 2**64
-                product = primary_asset_amount * secondary_asset_amount
-                if product >= max_product:
-                    # Need to split the liquidity into two chunks.
-                    divisor = int((product / max_product) ** 0.5 + 1)
-                    primary_small_amount = primary_asset_amount // divisor
-                    secondary_small_amount = secondary_asset_amount // divisor
-
-                    primary_asset_amount -= primary_small_amount
-                    secondary_asset_amount -= secondary_small_amount
-
-                    initial_liq_txs = self.build_raw_add_liquidity_txs(
-                        address=address,
-                        primary_asset_amount=primary_small_amount,
-                        secondary_asset_amount=secondary_small_amount,
-                        suggested_params=suggested_params,
-                        fee=liquidity_addition.effect.tx_fee,
-                        note=b"Pact initial add liquidity",
-                    )
-
-        txs = self.build_raw_add_liquidity_txs(
+        return self.build_raw_add_liquidity_txs(
             address=address,
             primary_asset_amount=primary_asset_amount,
             secondary_asset_amount=secondary_asset_amount,
+            minimum_minted_liquidity_tokens=liquidity_addition.effect.minimum_minted_liquidity_tokens,
             suggested_params=suggested_params,
             fee=liquidity_addition.effect.tx_fee,
         )
 
-        return [*initial_liq_txs, *txs]
-
     def build_raw_add_liquidity_txs(
         self,
         address: str,
         primary_asset_amount: int,
         secondary_asset_amount: int,
+        minimum_minted_liquidity_tokens: int,
         suggested_params: transaction.SuggestedParams,
         fee: int,
         note=b"",
     ):
         tx1 = self._make_deposit_tx(
             address=address,
             asset=self.primary_asset,
@@ -385,15 +362,15 @@
             amount=secondary_asset_amount,
             note=note or b"Pact add liquidity deposit",
             suggested_params=suggested_params,
         )
         tx3 = self._make_application_noop_tx(
             address=address,
             fee=fee,
-            args=["ADDLIQ", 0],
+            args=["ADDLIQ", minimum_minted_liquidity_tokens],
             extraAsset=self.liquidity_asset,
             suggested_params=suggested_params,
             note=note,
         )
 
         return [tx1, tx2, tx3]
```

### Comparing `pactsdk-0.7.0/pactsdk/pool_calculator.py` & `pactsdk-0.7.1/pactsdk/pool_calculator.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.7.0/pactsdk/pool_state.py` & `pactsdk-0.7.1/pactsdk/pool_state.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.7.0/pactsdk/stableswap_calculator.py` & `pactsdk-0.7.1/pactsdk/stableswap_calculator.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.7.0/pactsdk/swap.py` & `pactsdk-0.7.1/pactsdk/swap.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.7.0/pactsdk/transaction_group.py` & `pactsdk-0.7.1/pactsdk/transaction_group.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.7.0/pactsdk/utils.py` & `pactsdk-0.7.1/pactsdk/utils.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.7.0/pactsdk/zap.py` & `pactsdk-0.7.1/pactsdk/zap.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,8 +164,9 @@
 
         pool = copy.copy(self.pool)
         pool.state = updated_state
         return LiquidityAddition(
             pool=pool,
             primary_asset_amount=self.params.primary_add_liq,
             secondary_asset_amount=self.params.secondary_add_liq,
+            slippage_pct=self.slippage_pct,
         )
```

### Comparing `pactsdk-0.7.0/pyproject.toml` & `pactsdk-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pactsdk"
-version = "0.7.0"
+version = "0.7.1"
 description = "Python SDK for Pact smart contracts"
 authors = ["Mateusz Tomczyk <mateusz.tomczyk@ulam.io>"]
 homepage = "https://github.com/pactfi/pact-py-sdk"
 repository = "https://github.com/pactfi/pact-py-sdk"
 readme = "README.md"
 license = "MIT"
```

### Comparing `pactsdk-0.7.0/PKG-INFO` & `pactsdk-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pactsdk
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python SDK for Pact smart contracts
 Home-page: https://github.com/pactfi/pact-py-sdk
 License: MIT
 Author: Mateusz Tomczyk
 Author-email: mateusz.tomczyk@ulam.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -165,15 +165,15 @@
 #     secondary_asset_price_after_swap=1.6442824791774173,
 #     primary_asset_price_change_pct=-31.549580645715963,
 #     secondary_asset_price_change_pct=46.091142966447585,
 # )
 
 # Let's submit the swap.
 swap_tx_group = swap.prepare_tx_group(address)
-signed_tx_group = swap_tx_group.sign_txn(private_key)
+signed_tx_group = swap_tx_group.sign(private_key)
 algod.send_transactions(signed_tx_group)
 ```
 
 ## Composability of transactions.
 
 The SDK has two sets of methods for creating transactions:
```

