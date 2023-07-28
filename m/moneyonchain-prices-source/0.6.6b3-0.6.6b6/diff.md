# Comparing `tmp/moneyonchain_prices_source-0.6.6b3.tar.gz` & `tmp/moneyonchain_prices_source-0.6.6b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneyonchain_prices_source-0.6.6b3.tar", last modified: Wed Jul 19 18:39:45 2023, max compression
+gzip compressed data, was "moneyonchain_prices_source-0.6.6b6.tar", last modified: Fri Jul 28 17:11:13 2023, max compression
```

## Comparing `moneyonchain_prices_source-0.6.6b3.tar` & `moneyonchain_prices_source-0.6.6b6.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-19 18:39:45.917329 moneyonchain_prices_source-0.6.6b3/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    14035 2023-07-19 18:39:45.917329 moneyonchain_prices_source-0.6.6b3/PKG-INFO
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    10484 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b3/README.md
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-19 18:39:45.845330 moneyonchain_prices_source-0.6.6b3/moc_prices_source/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6610 2023-07-18 22:30:26.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/__init__.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      486 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/cli.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4577 2023-07-12 17:16:52.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/cli_check.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      625 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/coins.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2847 2023-07-19 18:33:35.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/computed_pairs.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3892 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/conf.py
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-19 18:39:45.861330 moneyonchain_prices_source-0.6.6b3/moc_prices_source/data/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      174 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/data/database_default.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       17 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/data/redis_default.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2312 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/data/weighing.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5715 2023-07-10 20:39:21.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/database.py
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-19 18:39:45.905329 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2521 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/__init__.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      766 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/bnb_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      720 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_ars_argenbtc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      791 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_ars_belo_app.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_ars_bitso.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      762 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_ars_buenbit.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_ars_cryptomkt.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      836 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_ars_decrypto.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      805 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_ars_ripio.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      677 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_ars_ripio_exch.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      643 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_ars_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_ars_satoshitango.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usd_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      693 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usd_bitgo.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usd_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usd_bittrex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      503 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usd_blockchain.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      518 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usd_cex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      526 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usd_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usd_gemini.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      513 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usd_itbit.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      582 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usd_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      559 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usd_kucoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      524 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usd_okcoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2023-07-11 20:25:45.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      525 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usdt_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usdt_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      581 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usdt_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4887 2023-07-18 22:12:42.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/coins.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    13823 2023-07-12 15:36:26.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/engine_base.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-07-10 19:46:36.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/eth_btc_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/eth_btc_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/eth_btc_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/eth_btc_gemini.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      580 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/eth_btc_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1616 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/gas_btc_rsk.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2023-07-12 15:32:05.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/moc_btc_sovryn.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-05-12 17:54:43.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/rif_btc_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2023-07-12 15:32:05.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/rif_btc_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-07-12 15:32:05.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/rif_btc_bithumbpro.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      666 2023-07-12 15:32:05.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/rif_btc_coinbene.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-07-12 15:32:05.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/rif_btc_coingecko.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      639 2023-07-12 15:32:05.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/rif_btc_kucoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-07-12 15:32:05.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/rif_btc_mexc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-07-12 15:32:05.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/rif_btc_mxc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2023-07-12 15:32:05.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/rif_btc_sovryn.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2023-07-11 14:34:01.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/rif_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      822 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ambito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      950 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccb_emdx.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      651 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccb_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      829 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccl_ambito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      640 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      615 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccl_criptoya.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1321 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccl_cronista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1299 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      866 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccl_dolarito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccl_dolarsi.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1177 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccl_infobae.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1358 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccl_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      858 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccl_lanacion.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      653 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccl_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      982 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_clarin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      632 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      612 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_criptoya.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1305 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_cronista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1281 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_dolarhoy.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      867 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_dolarito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1108 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_dolarsi.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1164 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_infobae.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1331 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      855 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_lanacion.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      921 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_mxn_bitso.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1069 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_mxn_citibanamex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1224 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_mxn_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1181 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_mxn_currencymeuk.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1193 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_mxn_eldolar_info.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1155 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_mxn_eleconomista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1344 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_mxn_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1078 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_mxn_intercam.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_mxn_themoneyconverter.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      806 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_mxn_wise.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1223 2023-07-19 18:32:55.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_mxn_xrates.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-11 21:09:00.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usdt_usd_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-11 20:50:33.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usdt_usd_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2023-07-11 21:05:01.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usdt_usd_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/my_logging.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6008 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/to_db.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        7 2023-07-19 18:38:09.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/version.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5014 2023-07-18 22:35:17.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source/weighing.py
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      118 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source_check
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      128 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b3/moc_prices_source_to_db
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-19 18:39:45.905329 moneyonchain_prices_source-0.6.6b3/moneyonchain_prices_source.egg-info/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    14035 2023-07-19 18:39:44.000000 moneyonchain_prices_source-0.6.6b3/moneyonchain_prices_source.egg-info/PKG-INFO
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4666 2023-07-19 18:39:45.000000 moneyonchain_prices_source-0.6.6b3/moneyonchain_prices_source.egg-info/SOURCES.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        1 2023-07-19 18:39:44.000000 moneyonchain_prices_source-0.6.6b3/moneyonchain_prices_source.egg-info/dependency_links.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      100 2023-07-19 18:39:44.000000 moneyonchain_prices_source-0.6.6b3/moneyonchain_prices_source.egg-info/requires.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       18 2023-07-19 18:39:44.000000 moneyonchain_prices_source-0.6.6b3/moneyonchain_prices_source.egg-info/top_level.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       38 2023-07-19 18:39:45.917329 moneyonchain_prices_source-0.6.6b3/setup.cfg
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)     1565 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b3/setup.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-28 17:11:13.917979 moneyonchain_prices_source-0.6.6b6/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4787 2023-07-28 17:11:13.917979 moneyonchain_prices_source-0.6.6b6/PKG-INFO
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2942 2023-07-28 16:02:42.000000 moneyonchain_prices_source-0.6.6b6/README.md
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-28 17:11:13.897980 moneyonchain_prices_source-0.6.6b6/moc_prices_source/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6610 2023-07-26 17:12:40.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/__init__.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      486 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/cli.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    10644 2023-07-28 15:37:53.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/cli_check.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      625 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/coins.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3101 2023-07-27 12:10:08.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/computed_pairs.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3892 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/conf.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-28 17:11:13.897980 moneyonchain_prices_source-0.6.6b6/moc_prices_source/data/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      174 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/data/database_default.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       17 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/data/redis_default.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2312 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/data/weighing.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5715 2023-07-10 20:39:21.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/database.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-28 17:11:13.913979 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2521 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/__init__.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      766 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/bnb_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      720 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_argenbtc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      791 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_belo_app.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_bitso.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      762 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_buenbit.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_cryptomkt.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      836 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_decrypto.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      805 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_ripio.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      677 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_ripio_exch.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      643 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_satoshitango.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      693 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_bitgo.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_bittrex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      503 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_blockchain.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      518 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_cex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      526 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_gemini.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      513 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_itbit.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      582 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      559 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_kucoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      524 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_okcoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      525 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usdt_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usdt_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      581 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usdt_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5000 2023-07-26 17:37:06.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/coins.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    13823 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/engine_base.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/eth_btc_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/eth_btc_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/eth_btc_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/eth_btc_gemini.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      580 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/eth_btc_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1616 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/gas_btc_rsk.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/moc_btc_sovryn.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-05-12 17:54:43.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_bithumbpro.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      666 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_coinbene.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_coingecko.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      639 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_kucoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_mexc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_mxc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_sovryn.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      822 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ambito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      950 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccb_emdx.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      651 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccb_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      829 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_ambito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      640 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      615 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_criptoya.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1321 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_cronista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1299 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      866 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_dolarito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_dolarsi.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1177 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_infobae.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1358 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      858 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_lanacion.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      653 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      982 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_clarin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      632 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      612 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_criptoya.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1305 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_cronista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1281 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_dolarhoy.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      867 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_dolarito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1108 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_dolarsi.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1164 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_infobae.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1331 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      855 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_lanacion.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      921 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_bitso.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1069 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_citibanamex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1224 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1181 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_currencymeuk.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1193 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_eldolar_info.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1155 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_eleconomista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1344 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1078 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_intercam.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_themoneyconverter.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      806 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_wise.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1223 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_xrates.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usdt_usd_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usdt_usd_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usdt_usd_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/my_logging.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6008 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/to_db.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        7 2023-07-28 17:10:06.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/version.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5014 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/weighing.py
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      118 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source_check
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      128 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source_to_db
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-28 17:11:13.917979 moneyonchain_prices_source-0.6.6b6/moneyonchain_prices_source.egg-info/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4787 2023-07-28 17:11:13.000000 moneyonchain_prices_source-0.6.6b6/moneyonchain_prices_source.egg-info/PKG-INFO
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4666 2023-07-28 17:11:13.000000 moneyonchain_prices_source-0.6.6b6/moneyonchain_prices_source.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        1 2023-07-28 17:11:13.000000 moneyonchain_prices_source-0.6.6b6/moneyonchain_prices_source.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      100 2023-07-28 17:11:13.000000 moneyonchain_prices_source-0.6.6b6/moneyonchain_prices_source.egg-info/requires.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       18 2023-07-28 17:11:13.000000 moneyonchain_prices_source-0.6.6b6/moneyonchain_prices_source.egg-info/top_level.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       38 2023-07-28 17:11:13.917979 moneyonchain_prices_source-0.6.6b6/setup.cfg
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)     1868 2023-07-28 17:07:59.000000 moneyonchain_prices_source-0.6.6b6/setup.py
```

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/__init__.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/__init__.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/coins.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/coins.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/computed_pairs.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/computed_pairs.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,16 +4,20 @@
 from types   import LambdaType
 
 base_dir = dirname(abspath(__file__))
 
 bkpath   = sys.path[:]
 sys.path.insert(0, dirname(base_dir), )
 
-from moc_prices_source.engines.coins import RIF_USDT, BTC_USD, MOC_BTC, RIF_BTC, ETH_BTC, MOC_USD, RIF_USD, RIF_USD_B, RIF_USD_T, ETH_USD, USDT_USD_B, USDT_USD, BTC_USDT, BNB_USD, BNB_USDT, USD_ARS_CCB_MOC, BTC_ARS, RIF_USD_TB, RIF_USD_WMTB
+from moc_prices_source.engines.coins import \
+    RIF_USDT, BTC_USD, MOC_BTC, RIF_BTC, ETH_BTC, MOC_USD, RIF_USD, RIF_USD_B, \
+    RIF_USD_T, ETH_USD, USDT_USD_B, USDT_USD, BTC_USDT, BNB_USD, BNB_USDT, \
+    USD_ARS_CCB_MOC, BTC_ARS, RIF_USD_TB, RIF_USD_WMTB
 from moc_prices_source.weighing import weighted_median
+from moc_prices_source.cli import tabulate
 
 sys.path = bkpath
 
 
 
 computed_pairs = {
     MOC_USD: {
@@ -56,28 +60,32 @@
     },
     USD_ARS_CCB_MOC: {
         'requirements': [BTC_ARS, BTC_USD],
         'formula': lambda btc_ars, btc_usd: btc_ars / btc_usd
     },
 }
 
+for pair, data in computed_pairs.items():
+    formula = data['formula']
+    if isinstance(formula, LambdaType):
+        formula_desc = ':'.join(getsource(formula).split('lambda')[-1].strip(
+            ).split(':')[1:]).strip()
+    else:
+        formula_desc = repr(formula)
+    data['formula_desc'] = '\n'.join(map(str.strip, formula_desc.split('\n')))
 
 
 def show_computed_pairs_fromula():
     print()
     print("Computed pairs formula")
     print("-------- ----- -------")
     print("")
-    for pair, data in computed_pairs.items():
-        formula = data['formula']
-        if isinstance(formula, LambdaType):
-            formula = ':'.join(getsource(formula).split('lambda')[-1].strip().split(':')[1:]).strip()
-        else:
-            formula = repr(formula)
-        print(f"{pair} = {formula}")
+    table = [[str(pair), '=', data['formula_desc']] for pair,
+             data in computed_pairs.items()]
+    print(tabulate(table, tablefmt='plain'))
     print("")
 
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     show_computed_pairs_fromula()
```

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/conf.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/conf.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/data/weighing.json` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/data/weighing.json`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/database.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/database.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/__init__.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/bnb_usdt_binance.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/bnb_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_ars_argenbtc.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_argenbtc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_ars_belo_app.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_belo_app.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_ars_bitso.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_bitso.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_ars_buenbit.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_buenbit.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_ars_cryptomkt.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_cryptomkt.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_ars_decrypto.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_decrypto.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_ars_ripio.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_ripio.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_ars_ripio_exch.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_ripio_exch.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_ars_rofex.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_ars_satoshitango.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_satoshitango.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usd_bitfinex.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usd_bitgo.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_bitgo.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usd_bitstamp.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_bitstamp.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usd_bittrex.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_bittrex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usd_cex.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_cex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usd_coinbase.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usd_itbit.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_itbit.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usd_kraken.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usd_kucoin.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_kucoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usd_okcoin.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_okcoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usdt_binance.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usdt_bitfinex.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usdt_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usdt_coinbase.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usdt_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/btc_usdt_kraken.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usdt_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/coins.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/coins.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,18 @@
         return self._from
 
     @property
     def to_(self):
         return self._to
 
     @property
+    def long_name(self):
+        return f"{self} (from {self.from_.name} to {self.to_.name})"
+    
+    @property
     def as_dict(self):
         return {
             'from':    self.from_,
             'to':      self.to_,
             'variant': self.variant
         }
```

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/engine_base.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/engine_base.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/eth_btc_binance.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/eth_btc_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/eth_btc_bitfinex.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/eth_btc_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/eth_btc_bitstamp.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/eth_btc_bitstamp.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/eth_btc_kraken.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/eth_btc_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/gas_btc_rsk.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/gas_btc_rsk.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/moc_btc_sovryn.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/moc_btc_sovryn.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/rif_btc_binance.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/rif_btc_bitfinex.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/rif_btc_bithumbpro.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_bithumbpro.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/rif_btc_coinbene.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_coinbene.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/rif_btc_coingecko.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_coingecko.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/rif_btc_kucoin.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_kucoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/rif_btc_mexc.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_mexc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/rif_btc_mxc.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_mxc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/rif_btc_sovryn.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_sovryn.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/rif_usdt_binance.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ambito.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ambito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccb_emdx.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccb_emdx.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccb_rofex.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccb_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccl_ambito.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_ambito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccl_criptoya.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_criptoya.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccl_cronista.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_cronista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccl_dolarito.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_dolarito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccl_dolarsi.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_dolarsi.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccl_infobae.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_infobae.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccl_infodolar.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccl_lanacion.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_lanacion.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_ccl_rofex.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_clarin.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_clarin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_coinmonitor.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_criptoya.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_criptoya.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_cronista.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_cronista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_dolarhoy.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_dolarhoy.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_dolarito.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_dolarito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_dolarsi.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_dolarsi.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_infobae.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_infobae.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_infodolar.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_ars_lanacion.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_lanacion.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_mxn_bitso.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_bitso.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_mxn_citibanamex.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_citibanamex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_mxn_coinmonitor.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_mxn_currencymeuk.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_currencymeuk.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_mxn_eldolar_info.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_eldolar_info.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_mxn_eleconomista.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_eleconomista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_mxn_infodolar.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_mxn_intercam.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_intercam.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_mxn_themoneyconverter.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_themoneyconverter.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_mxn_wise.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_wise.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usd_mxn_xrates.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_xrates.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usdt_usd_bitstamp.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usdt_usd_bitstamp.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usdt_usd_coinbase.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usdt_usd_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/engines/usdt_usd_kraken.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usdt_usd_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/my_logging.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/my_logging.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/to_db.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/to_db.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moc_prices_source/weighing.py` & `moneyonchain_prices_source-0.6.6b6/moc_prices_source/weighing.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/moneyonchain_prices_source.egg-info/SOURCES.txt` & `moneyonchain_prices_source-0.6.6b6/moneyonchain_prices_source.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b3/setup.py` & `moneyonchain_prices_source-0.6.6b6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,31 @@
 from setuptools import setup, find_packages
 from os.path    import dirname, abspath
 
 base_dir = dirname(abspath(__file__))
 
+with open(base_dir + "/moc_prices_source/version.txt", "r") as file_:
+    version = file_.read().split()[0]
+
 with open(base_dir + "/README.md", "r") as file_:
     long_description = file_.read()
 
-with open(base_dir + "/moc_prices_source/version.txt", "r") as file_:
-    version = file_.read().split()[0]
+# Fix some links
+
+url = "https://github.com/money-on-chain/moc_prices_source"
+
+long_description = long_description.replace(
+    "](" + url + ")",
+    "](" + url + "/tree/v" + version + ")"
+)
+
+long_description = long_description.replace(
+    "](docs/",
+    "](" + url + "/blob/v" + version + "/docs/"
+)
 
 requirements = []
 requires_files = ["/requirements.txt",
                   "/moneyonchain_prices_source.egg-info/requires.txt"]
 for file_path in requires_files:
     try:
         with open(base_dir + file_path, "r") as file_:
```

