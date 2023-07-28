# Comparing `tmp/degiroasync-0.20.0.tar.gz` & `tmp/degiroasync-0.21.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "degiroasync-0.20.0.tar", last modified: Sat Jul 22 08:29:25 2023, max compression
+gzip compressed data, was "degiroasync-0.21.0.tar", last modified: Fri Jul 28 21:41:34 2023, max compression
```

## Comparing `degiroasync-0.20.0.tar` & `degiroasync-0.21.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-22 08:29:25.126965 degiroasync-0.20.0/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1075 2022-01-20 21:38:48.000000 degiroasync-0.20.0/LICENSE
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     5039 2023-07-22 08:29:25.126965 degiroasync-0.20.0/PKG-INFO
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     4347 2023-07-08 15:05:00.000000 degiroasync-0.20.0/README.md
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-22 08:29:25.118965 degiroasync-0.20.0/degiroasync/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      692 2022-04-13 19:10:04.000000 degiroasync-0.20.0/degiroasync/__init__.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-22 08:29:25.122965 degiroasync-0.20.0/degiroasync/api/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     4382 2023-07-21 19:06:29.000000 degiroasync-0.20.0/degiroasync/api/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     8334 2022-05-12 19:40:07.000000 degiroasync-0.20.0/degiroasync/api/orders.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    36107 2023-07-21 21:54:58.000000 degiroasync-0.20.0/degiroasync/api/product.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    14340 2023-07-21 19:48:47.000000 degiroasync-0.20.0/degiroasync/api/session.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-22 08:29:25.122965 degiroasync-0.20.0/degiroasync/core/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1551 2023-03-13 17:53:33.000000 degiroasync-0.20.0/degiroasync/core/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     6629 2023-07-21 18:43:03.000000 degiroasync-0.20.0/degiroasync/core/constants.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    14341 2023-07-10 07:20:34.000000 degiroasync-0.20.0/degiroasync/core/core.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      547 2023-03-13 16:44:13.000000 degiroasync-0.20.0/degiroasync/core/exceptions.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    16450 2023-07-09 14:06:23.000000 degiroasync-0.20.0/degiroasync/core/helpers.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-22 08:29:25.126965 degiroasync-0.20.0/degiroasync/webapi/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1925 2023-07-08 14:01:46.000000 degiroasync-0.20.0/degiroasync/webapi/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    17277 2023-07-21 14:22:18.000000 degiroasync-0.20.0/degiroasync/webapi/login.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    12060 2023-07-02 17:18:26.000000 degiroasync-0.20.0/degiroasync/webapi/orders.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    29667 2023-07-22 08:23:55.000000 degiroasync-0.20.0/degiroasync/webapi/product.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-22 08:29:25.118965 degiroasync-0.20.0/degiroasync.egg-info/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     5039 2023-07-22 08:29:25.000000 degiroasync-0.20.0/degiroasync.egg-info/PKG-INFO
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      743 2023-07-22 08:29:25.000000 degiroasync-0.20.0/degiroasync.egg-info/SOURCES.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)        1 2023-07-22 08:29:25.000000 degiroasync-0.20.0/degiroasync.egg-info/dependency_links.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      270 2023-07-22 08:29:25.000000 degiroasync-0.20.0/degiroasync.egg-info/requires.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)       18 2023-07-22 08:29:25.000000 degiroasync-0.20.0/degiroasync.egg-info/top_level.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      108 2022-02-26 15:27:30.000000 degiroasync-0.20.0/pyproject.toml
--rw-rw-r--   0 laumas    (1000) laumas    (1000)       38 2023-07-22 08:29:25.130965 degiroasync-0.20.0/setup.cfg
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     2167 2023-07-21 21:56:37.000000 degiroasync-0.20.0/setup.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-22 08:29:25.126965 degiroasync-0.20.0/tests/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)        0 2023-07-02 12:58:48.000000 degiroasync-0.20.0/tests/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1504 2023-07-02 16:37:29.000000 degiroasync-0.20.0/tests/integration_login.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     4826 2023-07-08 08:25:07.000000 degiroasync-0.20.0/tests/test_core.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    45164 2023-07-21 21:56:03.000000 degiroasync-0.20.0/tests/test_degiroapi.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    19746 2023-07-22 08:24:06.000000 degiroasync-0.20.0/tests/test_degirowebapi.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      153 2022-01-27 15:50:02.000000 degiroasync-0.20.0/tests/test_setup.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-28 21:41:34.679663 degiroasync-0.21.0/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1075 2022-01-20 21:38:48.000000 degiroasync-0.21.0/LICENSE
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     5062 2023-07-28 21:41:34.679663 degiroasync-0.21.0/PKG-INFO
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     4347 2023-07-08 15:05:00.000000 degiroasync-0.21.0/README.md
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-28 21:41:34.671663 degiroasync-0.21.0/degiroasync/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      692 2022-04-13 19:10:04.000000 degiroasync-0.21.0/degiroasync/__init__.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-28 21:41:34.675663 degiroasync-0.21.0/degiroasync/api/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     4403 2023-07-22 11:04:11.000000 degiroasync-0.21.0/degiroasync/api/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     8394 2023-07-22 10:59:38.000000 degiroasync-0.21.0/degiroasync/api/orders.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    36794 2023-07-23 09:25:48.000000 degiroasync-0.21.0/degiroasync/api/product.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    14321 2023-07-22 10:47:14.000000 degiroasync-0.21.0/degiroasync/api/session.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-28 21:41:34.675663 degiroasync-0.21.0/degiroasync/core/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1551 2023-03-13 17:53:33.000000 degiroasync-0.21.0/degiroasync/core/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     6629 2023-07-21 18:43:03.000000 degiroasync-0.21.0/degiroasync/core/constants.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    14341 2023-07-10 07:20:34.000000 degiroasync-0.21.0/degiroasync/core/core.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      547 2023-03-13 16:44:13.000000 degiroasync-0.21.0/degiroasync/core/exceptions.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    16472 2023-07-22 11:00:22.000000 degiroasync-0.21.0/degiroasync/core/helpers.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-28 21:41:34.679663 degiroasync-0.21.0/degiroasync/webapi/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1925 2023-07-08 14:01:46.000000 degiroasync-0.21.0/degiroasync/webapi/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    17352 2023-07-22 10:54:38.000000 degiroasync-0.21.0/degiroasync/webapi/login.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    12111 2023-07-22 10:57:57.000000 degiroasync-0.21.0/degiroasync/webapi/orders.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    29660 2023-07-22 10:58:15.000000 degiroasync-0.21.0/degiroasync/webapi/product.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-28 21:41:34.675663 degiroasync-0.21.0/degiroasync.egg-info/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     5062 2023-07-28 21:41:34.000000 degiroasync-0.21.0/degiroasync.egg-info/PKG-INFO
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      743 2023-07-28 21:41:34.000000 degiroasync-0.21.0/degiroasync.egg-info/SOURCES.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)        1 2023-07-28 21:41:34.000000 degiroasync-0.21.0/degiroasync.egg-info/dependency_links.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      270 2023-07-28 21:41:34.000000 degiroasync-0.21.0/degiroasync.egg-info/requires.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)       18 2023-07-28 21:41:34.000000 degiroasync-0.21.0/degiroasync.egg-info/top_level.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      108 2022-02-26 15:27:30.000000 degiroasync-0.21.0/pyproject.toml
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)       38 2023-07-28 21:41:34.683663 degiroasync-0.21.0/setup.cfg
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     2200 2023-07-22 10:46:29.000000 degiroasync-0.21.0/setup.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-28 21:41:34.679663 degiroasync-0.21.0/tests/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)        0 2023-07-02 12:58:48.000000 degiroasync-0.21.0/tests/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1504 2023-07-02 16:37:29.000000 degiroasync-0.21.0/tests/integration_login.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     4826 2023-07-08 08:25:07.000000 degiroasync-0.21.0/tests/test_core.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    45794 2023-07-22 10:27:33.000000 degiroasync-0.21.0/tests/test_degiroapi.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    19746 2023-07-22 08:24:06.000000 degiroasync-0.21.0/tests/test_degirowebapi.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      153 2022-01-27 15:50:02.000000 degiroasync-0.21.0/tests/test_setup.py
```

### Comparing `degiroasync-0.20.0/LICENSE` & `degiroasync-0.21.0/LICENSE`

 * *Files identical despite different names*

### Comparing `degiroasync-0.20.0/PKG-INFO` & `degiroasync-0.21.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: degiroasync
-Version: 0.20.0
+Version: 0.21.0
 Summary: A Python asynchronous library for Degiro trading service.
 Home-page: https://github.com/OhMajesticLama/degiroasync
 Author-email: ohmajesticlama@gmail.com
 Project-URL: Documentation, https://ohmajesticlama.github.io/degiroasync/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # DegiroAsync
 
 ## Documentation
```

### Comparing `degiroasync-0.20.0/README.md` & `degiroasync-0.21.0/README.md`

 * *Files identical despite different names*

### Comparing `degiroasync-0.20.0/degiroasync/__init__.py` & `degiroasync-0.21.0/degiroasync/__init__.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.20.0/degiroasync/api/__init__.py` & `degiroasync-0.21.0/degiroasync/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,12 +125,13 @@
             check_order,
             get_orders,
             get_transactions,
             Order,
             Transaction,
 
             # Constants
-            #PRODUCT,
-            #ORDER,
-            #PRICE,
-            #POSITION
-)]
+            # PRODUCT,
+            # ORDER,
+            # PRICE,
+            # POSITION
+        )
+        ]
```

### Comparing `degiroasync-0.20.0/degiroasync/api/orders.py` & `degiroasync-0.21.0/degiroasync/api/orders.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from .product import ProductFactory
 from .. import webapi
 from ..core import SessionCore
 from ..core import ORDER
 from ..core import TRANSACTION
 from ..core import LOGGER_NAME
 from ..core import camelcase_dict_to_snake
-from ..core.helpers import dict_from_attr_list
 
 
 LOGGER = logging.getLogger(LOGGER_NAME)
 
 
 @JSONclass(annotations=True, annotations_type=True)
 class Order:
@@ -40,15 +39,32 @@
     # 'CREATE' or ... ?
     type: Optional[str] = None
     is_active: bool
 
     #: Not always available for "Outstanding" orders
     status: Optional[ORDER.STATUS] = None
 
-# {'id': 182722888, 'productId': 65153, 'date': '2020-02-07T09:00:10+01:00', 'buysell': 'B', 'price': 36.07, 'quantity': 20, 'total': -721.4, 'orderTypeId': 0, 'counterParty': 'MK', 'transfered': False, 'fxRate': 0, 'totalInBaseCurrency': -721.4, 'feeInBaseCurrency': -0.29, 'totalPlusFeeInBaseCurrency': -721.69, 'transactionTypeId': 0, 'tradingVenue': 'XPAR'})
+    # {
+    # 'id': 182722888,
+    # 'productId': 65153,
+    # 'date': '2020-02-07T09:00:10+01:00',
+    # 'buysell': 'B',
+    # 'price': 36.07,
+    # 'quantity': 20,
+    # 'total': -721.4,
+    # 'orderTypeId': 0,
+    # 'counterParty': 'MK',
+    # 'transfered': False,
+    # 'fxRate': 0,
+    # 'totalInBaseCurrency': -721.4,
+    # 'feeInBaseCurrency': -0.29,
+    # 'totalPlusFeeInBaseCurrency': -721.69,
+    # 'transactionTypeId': 0,
+    # 'tradingVenue': 'XPAR'
+    # }
 
 
 @JSONclass(annotations=True, annotations_type=True)
 class Transaction:
     id: str
     product: ProductBase
     date: datetime.datetime
```

### Comparing `degiroasync-0.20.0/degiroasync/api/product.py` & `degiroasync-0.21.0/degiroasync/api/product.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
                 f'[{self.info.name} | {self.info.symbol}]>')
 
 
 class ProductFactory:
     @classmethod
     async def init_batch(
             cls,
-            session: SessionCore,
+            session: Session,
             attributes_iter: Iterable[Dict[str, Any]],
             size=50
     ) -> AsyncGenerator[ProductBase, None]:
         """
         Bulk init Product instances.
 
         This is useful to do batch requests to populate additional attributes
@@ -112,15 +112,15 @@
             All attributes provided will be set to the Product.base
             oject.
 
         Returns an iterable of Product instances
 
         .. code-block:: python
 
-            import asyncio
+            ...  # This code should be inside an async callable
             products_attrs = (
                         {'id': 1, 'product_type_id': PRODUCT.TYPEID.STOCK},
                         {'id': 2, 'product_type_id': PRODUCT.TYPEID.STOCK},
                         {'id': 3, 'product_type_id': PRODUCT.TYPEID.STOCK},
                 )
             products_gen = ProductFactory.init_batch(session, products_attrs)
             # At this stage, we have an awaitable for each product.
@@ -247,15 +247,14 @@
                     product_type_id,
                     ProductGeneric
                 )
                 LOGGER.debug(
                         "api.ProductFactory.init_product| type_id %s class %s",
                         product_type_id, inst_cls)
                 product_info = camelcase_dict_to_snake(product_info)
-                #if inst_cls is Stock:
                 if (
                         product_info.get('exchange_id')
                         and issubclass(inst_cls, Stock)
                         ):
                     # WARNING: There could be exchange_id key, but empty value,
                     # We don't want to set it here if that's the case
                     product_info['exchange'] = (
@@ -374,15 +373,30 @@
     realized_fx_pl: Union[float, int]
     today_realized_fx_pl: Union[float, int]
     pl_base: Dict[str, float]
     today_pl_base: Dict[str, float]
     portfolio_value_correction: Union[float, int]
 
     # Example camel case JSON:
-# {'id': '8217023', 'position_type': 'PRODUCT', 'size': 70, 'price': 55.39, 'value': 3877.3, 'pl_base': {'EUR': -4796.53}, 'today_pl_base': {'EUR': -3877.3}, 'portfolio_value_correction': 0, 'break_even_price': 68.36, 'average_fx_rate': 1, 'realized_product_pl': -11.33, 'realized_fx_pl': 0, 'today_realized_product_pl': 0.0, 'today_realized_fx_pl': 0}
+    # {
+    # 'id': '8217023',
+    # 'position_type': 'PRODUCT',
+    # 'size': 70,
+    # 'price': 55.39,
+    # 'value': 3877.3,
+    # 'pl_base': {'EUR': -4796.53},
+    # 'today_pl_base': {'EUR': -3877.3},
+    # 'portfolio_value_correction': 0,
+    # 'break_even_price': 68.36,
+    # 'average_fx_rate': 1,
+    # 'realized_product_pl': -11.33,
+    # 'realized_fx_pl': 0,
+    # 'today_realized_product_pl': 0.0,
+    # 'today_realized_fx_pl': 0
+    # }
 
 
 async def get_portfolio(
         session: SessionCore
 ) -> Sequence[Position]:
     """
     Returns Products in portfolio. Refer to  `Products` classes for minimum
@@ -580,15 +594,16 @@
             yield ('close', [x[1] for x in data])
         else:
             raise NotImplementedError(f"Price type {self.type} not supported.")
 
     def iterrows(self) -> Iterable[Dict[str, Union[datetime.datetime, float]]]:
         """
         Provide data by columns, can be fed directly to instantiate a
-        `pandas.DataFrame <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html>`
+        `pandas.DataFrame
+        <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html>`_
 
         With `pandas.DataFrame`:
 
             >>> pricedata = PriceData(
                     start=datetime.datetime(2023, 6, 29),
                     end=datetime.datetime(2023, 7, 5),
                     resolution=PRICE.RESOLUTION.OHLC
@@ -629,25 +644,25 @@
                         'close': row[4],
                         }
         else:
             raise NotImplementedError(f"Price type {self.type} not supported.")
 
     @property
     def date(self):
-        #print(
+        # print(
         #        "degiroasync.PriceSeries.date is deprecated and will be "
         #        "removed in a future version. "
         #        "Please use PriceSeries.items() or PriceSeries.iterrows().",
         #        file=sys.stderr
         #        )
         return [d.isoformat() for d in self._get_dates_it()]
 
     @property
     def price(self) -> Sequence[Union[float, Sequence[float]]]:
-        #print(
+        # print(
         #        "degiroasync.PriceSeries.price is deprecated and will be "
         #        "removed in a future version. "
         #        "Please use PriceSeries.items() or PriceSeries.iterrows()",
         #        file=sys.stderr
         #        )
         if self.type == PRICE.TYPE.OHLC:
             return [row[1:] for row in self.__series['data']]
@@ -803,14 +818,18 @@
                           (by_isin, 'isin'),
                           (by_symbol, 'symbol'),
                           (exchange_id, 'exchangeId'),
                           ):
             if attr is not None and p_json.get(key) != attr:
                 return False
         return True
+    if exchange_id is not None:
+        exchange = session.dictionary.exchange_by(id=exchange_id)
+        country = session.dictionary.country_by(name=exchange.country_name)
+        country_id = country.id
 
     resp_json = await webapi.search_product(
         session,
         by_text,
         product_type_id=product_type_id,
         country_id=country_id,
         index_id=index_id,
@@ -835,14 +854,17 @@
         # This could be optimized later on with a generator class to be
         # able to yield data as soon as we receive it while still not
         # blocking further calls to be launched, should it be needed.
         LOGGER.debug("api.search_product (batch len, symbol)| (%s, %s)",
                      len(products), by_symbol)
         return products, n_unfiltered, total
 
+    elif total <= offset:
+        # It's expected to be empty here. Return.
+        return [], 0, total
     else:
         LOGGER.debug("No 'products' key in response. Stop.")
         raise ResponseError(f"No 'products' key in response {resp_json} ")
 
 
 async def search_product(
         session: Session,
@@ -918,14 +940,16 @@
             by_text = by_symbol
         elif by_isin is not None:
             by_text = by_isin
         elif by_country is not None:
             pass  # Could also be set without text deal with it after
         elif by_index is not None:
             pass  # Manage below
+        elif by_exchange is not None:
+            pass  # Manage below
         else:
             raise AssertionError(
                     "by_text is None and no search parameters was set or "
                     "found. Have you set a search parameters to "
                     "search_product?"
                     "\n If yes, this shouldn't be happening, please open a bug"
                     " report."
@@ -994,14 +1018,17 @@
             } for offset in range(n_unfiltered, total, limit)
             )
         # The use of _search_one and gather improves performance over
         # sequential queries in a while loop as before.
         # 20230713 FR symbols query, throttling at 10 queries per 1 second:
         #   - With gather+_search_one: 3.6s
         #   - With legacy sequential calls: 6.9s
+        # Waiting times could be further reduced by making a queue and an async
+        # generator for the consumer instead of using a gather here.
+        # However, consumption is less straightforward.
         answers = await asyncio.gather(
                     *[_search_one(**kwa) for kwa in args])
         for prods, _, _ in answers:
             products += prods
 
     return list(unique_everseen(products, lambda p: p.info.id))
```

### Comparing `degiroasync-0.20.0/degiroasync/api/session.py` & `degiroasync-0.21.0/degiroasync/api/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Union, List, Dict, Any
 from typing import Set
 import sys
 from typing import Optional
 import functools
 import logging
 import pprint
-import dataclasses
 import copy
 
 from jsonloader import JSONclass
 
 from ..core import LOGGER_NAME
 from ..core import SessionCore
 from ..core import Config
```

### Comparing `degiroasync-0.20.0/degiroasync/core/__init__.py` & `degiroasync-0.21.0/degiroasync/core/__init__.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.20.0/degiroasync/core/constants.py` & `degiroasync-0.21.0/degiroasync/core/constants.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.20.0/degiroasync/core/core.py` & `degiroasync-0.21.0/degiroasync/core/core.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.20.0/degiroasync/core/exceptions.py` & `degiroasync-0.21.0/degiroasync/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.20.0/degiroasync/core/helpers.py` & `degiroasync-0.21.0/degiroasync/core/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from typing import List, Dict, Any, Iterable, Callable, Union, Coroutine
+from typing import List, Dict, Any, Iterable, Callable, Coroutine
 from typing import Optional
 import logging
 import sys
 import functools
 import asyncio
 import time
 
@@ -277,15 +277,16 @@
             ]
     ```
 
     """
     dict_out = {}
     for attr in attributes_list:
         if 'name' not in attr or 'value' not in attr:
-            message = f"A provided params does not have a 'name' or 'value': {attr}"
+            message = (f"A provided params does not have a 'name' or 'value': "
+                       f"{attr}")
             LOGGER.info(message)
             if not ignore_error:
                 raise ValueError(message)
             else:
                 continue
         name, value = attr['name'], attr['value']
         if not hasattr(name, int.__hash__.__name__):
```

### Comparing `degiroasync-0.20.0/degiroasync/webapi/__init__.py` & `degiroasync-0.21.0/degiroasync/webapi/__init__.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.20.0/degiroasync/webapi/login.py` & `degiroasync-0.21.0/degiroasync/webapi/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from typing import Union, Dict, Any, Optional
+from typing import Dict, Any, Optional
 import logging
 import json
 import base64
 import struct
 import hmac
 import hashlib
 import time
 
 from ..core.constants import LOGGER_NAME
 from ..core.constants import LOGIN
-from ..core.constants import TIMEOUT
 from ..core import Credentials, SessionCore, URLs, Config, PAClient
 from ..core import check_session_config
 from ..core.helpers import check_response
 from ..core.helpers import camelcase_dict_to_snake
 from ..core.helpers import ThrottlingClient
 
 LOGGER = logging.getLogger(LOGGER_NAME)
@@ -280,15 +279,18 @@
          'investmentFundSortColumns': [{'id': 'exchangeHiqAbbr'},
                                        {'id': 'name'},
                                        {'id': 'exchangeName'}],
          'leveragedAggregateTypes': [{'id': 'shortLong', 'name': 'shortLong'},
                                      {'id': 'underlyingProductId',
                                       'name': 'underlyingProductId'},
                                      {'id': 'exchange', 'name': 'exchange'},
-                                     {'id': 'underlying', 'name': 'underlying'},
+                                     {
+                                        'id': 'underlying',
+                                        'name': 'underlying'
+                                     },
                                      {'id': 'issuer', 'name': 'issuer'},
                                      {'id': 'expirationDateRange',
                                       'name': 'expirationDateRange'}],
          'leveragedSortColumns': [{'id': 'leverage'},
                                   {'id': 'financingLevel'},
                                   {'id': 'stoploss'},
                                   {'id': 'exchangeHiqAbbr'},
```

### Comparing `degiroasync-0.20.0/degiroasync/webapi/orders.py` & `degiroasync-0.21.0/degiroasync/webapi/orders.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import logging
 from typing import Union, Dict, Any
 import datetime
 
-import httpx
-
 from .product import get_trading_update
 from ..core import SessionCore
 from ..core import URLs
 from ..core import constants
 from ..core import ORDER
-from ..core.constants import TIMEOUT
 from ..core import join_url
 from ..core import check_session_client
 from ..core import check_session_config
 from ..core.helpers import check_response
 from ..core.helpers import dict_from_attr_list
 
 
@@ -51,31 +48,38 @@
 
     time_type:
         Specify if we want a DAY or PERMANENT order.
 
     Check `degiroasync.core.ORDER` for details.
 
     Example data with request:
-    ```
-    {
-        "buySell": "BUY",
-        "orderType": 0,
-        "price": 10,
-        "productId": "96008",
-        "size": 1,
-        "timeType": 1
-    }
-    ```
+
+    .. code-block:: python
+        {
+            "buySell": "BUY",
+            "orderType": 0,
+            "price": 10,
+            "productId": "96008",
+            "size": 1,
+            "timeType": 1
+        }
 
     Example JSON response:
-    ```
-    # TODO: Next time we place an order
-    {'data': {'confirmationId': 'a8e49a7e-4d79-4f21-961b-988dc0806d09', 'freeSpaceNew': 55395, 'transactionFee': 0.5, 'showExAnteReportLink': True}}
 
-    ```
+    .. code-block:: python
+
+        {
+            'data': {
+            'confirmationId': 'a8e49a7e-4d79-4f21-961b-988dc0806d09',
+            'freeSpaceNew': 55395,
+            'transactionFee': 0.5,
+            'showExAnteReportLink': True
+            }
+        }
+
     """
     # This call will not have integration tests to prevent misplaced orders
     # All changes must be manually verified to work as intended.
     _order_calls_check(session,
                        product_id=product_id,
                        buy_sell=buy_sell,
                        time_type=time_type,
@@ -277,15 +281,15 @@
     # TODO: assess if historicalOrders is relevant here
     # or if it should be removed and we should only rely on get_orders_history
     orders = await get_trading_update(
         session,
         params={
             'orders': 0,
             }
-            #'historicalOrders': 0}
+        # 'historicalOrders': 0}
     )
     LOGGER.debug("webapi.get_orders| orders %s", orders)
     orders = {
             'orders': [
                 dict_from_attr_list(order['value'])
                 for order in orders['orders']['value']
                 if order['name'] == 'order'
```

### Comparing `degiroasync-0.20.0/degiroasync/webapi/product.py` & `degiroasync-0.21.0/degiroasync/webapi/product.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Union, Any, List, Dict
+from typing import Any, List, Dict
 from typing import Optional
 
 from ..core import SessionCore, URLs
 from ..core import join_url
 from ..core import check_session_config
 from ..core import check_session_client
 from ..core.constants import LOGGER_NAME
```

### Comparing `degiroasync-0.20.0/degiroasync.egg-info/PKG-INFO` & `degiroasync-0.21.0/degiroasync.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: degiroasync
-Version: 0.20.0
+Version: 0.21.0
 Summary: A Python asynchronous library for Degiro trading service.
 Home-page: https://github.com/OhMajesticLama/degiroasync
 Author-email: ohmajesticlama@gmail.com
 Project-URL: Documentation, https://ohmajesticlama.github.io/degiroasync/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # DegiroAsync
 
 ## Documentation
```

### Comparing `degiroasync-0.20.0/degiroasync.egg-info/SOURCES.txt` & `degiroasync-0.21.0/degiroasync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `degiroasync-0.20.0/setup.py` & `degiroasync-0.21.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,26 @@
     description = "A Python asynchronous library for Degiro trading service."
     readme_path = os.path.join(os.path.dirname(__file__), 'README.md')
     with open(readme_path, "r") as fh:
         long_description = fh.read()
 
     setuptools.setup(
         name="degiroasync",
-        version="0.20.0",
+        version="0.21.0",
         author_email="ohmajesticlama@gmail.com",
         description=description,
         long_description=long_description,
         long_description_content_type='text/markdown',
         url="https://github.com/OhMajesticLama/degiroasync",
         project_urls={
             'Documentation':
                 'https://ohmajesticlama.github.io/degiroasync/index.html'
             },
         packages=setuptools.find_packages(),
+        python_requires=">=3.8",
         install_requires=[
             'httpx >= 0.21.3, < 1.0',
             'jsonloader >= 0.8.1, < 1.0',
             'asyncstdlib >= 3.10.3, < 4.0',
             'more_itertools >= 8.12.0, < 9'
             ],
         extras_require={
```

### Comparing `degiroasync-0.20.0/tests/integration_login.py` & `degiroasync-0.21.0/tests/integration_login.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.20.0/tests/test_core.py` & `degiroasync-0.21.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.20.0/tests/test_degiroapi.py` & `degiroasync-0.21.0/tests/test_degiroapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -973,14 +973,29 @@
             # is to target one specific product. Raise an error if it doesn't
             # work.
             self.assertEqual(len(products), 1)
             for product in products:
                 # We should only have airbus products here
                 self.assertTrue('airbus' in product.info.name.lower())
 
+        async def test_search_product_exchange(self):
+            session = await _IntegrationLogin._login()
+            exchange_hiq = 'EPA'
+            products = await degiroasync.api.search_product(
+                    session,
+                    by_exchange=exchange_hiq)
+            self.assertGreater(len(products), 40)
+            # Let's see if we can find airbus
+            found = False
+            for product in products:
+                # We should only have airbus products here
+                if 'airbus' in product.info.name.lower():
+                    found = True
+            self.assertEqual(found, True)
+
         async def test_search_product_country(self):
             session = await _IntegrationLogin._login()
             products = await degiroasync.api.search_product(
                     session,
                     by_country='FR',
                     max_iter=1,  # We don't need every product for this test.
                     )
```

### Comparing `degiroasync-0.20.0/tests/test_degirowebapi.py` & `degiroasync-0.21.0/tests/test_degirowebapi.py`

 * *Files identical despite different names*

