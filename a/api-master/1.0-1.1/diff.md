# Comparing `tmp/api_master-1.0.tar.gz` & `tmp/api_master-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_master-1.0.tar", last modified: Fri Jun 16 23:14:06 2023, max compression
+gzip compressed data, was "api_master-1.1.tar", last modified: Fri Jun 16 23:25:16 2023, max compression
```

## Comparing `api_master-1.0.tar` & `api_master-1.1.tar`

### file list

```diff
@@ -1,299 +1,299 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.429265 api_master-1.0/
--rw-rw-rw-   0        0        0     2484 2023-06-16 23:14:06.428264 api_master-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1929 2023-06-16 23:10:25.000000 api_master-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.285811 api_master-1.0/api_master.egg-info/
--rw-rw-rw-   0        0        0     2484 2023-06-16 23:14:06.000000 api_master-1.0/api_master.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10676 2023-06-16 23:14:06.000000 api_master-1.0/api_master.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 23:14:06.000000 api_master-1.0/api_master.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-16 23:14:06.000000 api_master-1.0/api_master.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.288810 api_master-1.0/polygonsdk/
--rw-rw-rw-   0        0        0        0 2023-06-11 22:28:58.000000 api_master-1.0/polygonsdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.292941 api_master-1.0/polygonsdk/_discord/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/_discord/__init__.py
--rw-rw-rw-   0        0        0     7983 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/_discord/discord_stock_example.py
--rw-rw-rw-   0        0        0    44936 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/_discord/discord_stock_market.py
--rw-rw-rw-   0        0        0    16306 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/_discord/embeddings.py
--rw-rw-rw-   0        0        0      581 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/_discord/emojis.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.294941 api_master-1.0/polygonsdk/_discord/hooks/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/_discord/hooks/__init__.py
--rw-rw-rw-   0        0        0     1594 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/_discord/hooks/channel_webhooks.py
--rw-rw-rw-   0        0        0    10521 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/_discord/hooks/hook_dicts.py
--rw-rw-rw-   0        0        0     5462 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/_discord/hooks/send_webhook.py
--rw-rw-rw-   0        0        0    33594 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/_discord/live_discord.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.296940 api_master-1.0/polygonsdk/_discord/selectmenus/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/_discord/selectmenus/__init__.py
--rw-rw-rw-   0        0        0    33209 2023-06-11 22:20:44.000000 api_master-1.0/polygonsdk/_discord/selectmenus/mainselect.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.297941 api_master-1.0/polygonsdk/_discord/views/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/_discord/views/__init__.py
--rw-rw-rw-   0        0        0     1640 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/_discord/views/mainview.py
--rw-rw-rw-   0        0        0     3792 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/_discord/views/menus.py
--rw-rw-rw-   0        0        0     7502 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/_discord/webhook_creation.py
--rw-rw-rw-   0        0        0     7264 2023-06-16 23:04:23.000000 api_master-1.0/polygonsdk/app.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.300187 api_master-1.0/polygonsdk/bot/
--rw-rw-rw-   0        0        0       72 2023-06-16 22:29:19.000000 api_master-1.0/polygonsdk/bot/__init__.py
--rw-rw-rw-   0        0        0    13209 2023-06-11 22:18:58.000000 api_master-1.0/polygonsdk/bot/autocomp.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.304876 api_master-1.0/polygonsdk/bot/cogs/
--rw-rw-rw-   0        0        0      162 2023-06-16 22:30:15.000000 api_master-1.0/polygonsdk/bot/cogs/__init__.py
--rw-rw-rw-   0        0        0     4478 2023-06-16 03:42:45.000000 api_master-1.0/polygonsdk/bot/cogs/earnings.py
--rw-rw-rw-   0        0        0     1406 2023-06-16 02:49:27.000000 api_master-1.0/polygonsdk/bot/cogs/evaluate.py
--rw-rw-rw-   0        0        0    11853 2023-06-06 22:47:55.000000 api_master-1.0/polygonsdk/bot/cogs/jasmy.py
--rw-rw-rw-   0        0        0     2219 2023-06-15 04:47:31.000000 api_master-1.0/polygonsdk/bot/cogs/navigate.py
--rw-rw-rw-   0        0        0     1794 2023-06-06 22:53:29.000000 api_master-1.0/polygonsdk/bot/cogs/scan.py
--rw-rw-rw-   0        0        0    10785 2023-06-16 03:00:26.000000 api_master-1.0/polygonsdk/bot/cogs/stream.py
--rw-rw-rw-   0        0        0    32431 2023-06-16 03:44:06.000000 api_master-1.0/polygonsdk/bot/cogs/webull.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.311729 api_master-1.0/polygonsdk/bot/cogs2/
--rw-rw-rw-   0        0        0        0 2022-10-11 19:37:24.000000 api_master-1.0/polygonsdk/bot/cogs2/__init__.py
--rw-rw-rw-   0        0        0    13678 2023-06-06 22:33:16.000000 api_master-1.0/polygonsdk/bot/cogs2/analysis.py
--rw-rw-rw-   0        0        0     4580 2023-06-16 02:58:46.000000 api_master-1.0/polygonsdk/bot/cogs2/collect.py
--rw-rw-rw-   0        0        0    14094 2023-06-16 03:47:55.000000 api_master-1.0/polygonsdk/bot/cogs2/economy.py
--rw-rw-rw-   0        0        0    13966 2023-06-16 03:00:46.000000 api_master-1.0/polygonsdk/bot/cogs2/learn.py
--rw-rw-rw-   0        0        0     3830 2023-06-16 03:47:27.000000 api_master-1.0/polygonsdk/bot/cogs2/news.py
--rw-rw-rw-   0        0        0    75051 2023-04-11 14:56:18.000000 api_master-1.0/polygonsdk/bot/cogs2/occ.py
--rw-rw-rw-   0        0        0    19227 2023-06-16 03:43:01.000000 api_master-1.0/polygonsdk/bot/cogs2/options.py
--rw-rw-rw-   0        0        0     1823 2023-06-16 02:52:02.000000 api_master-1.0/polygonsdk/bot/cogs2/prices_and_technicals.py
--rw-rw-rw-   0        0        0    50520 2023-06-16 03:47:06.000000 api_master-1.0/polygonsdk/bot/cogs2/stock.py
--rw-rw-rw-   0        0        0    17675 2023-06-16 03:02:03.000000 api_master-1.0/polygonsdk/bot/cogs2/view.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.317727 api_master-1.0/polygonsdk/bot/cogs3/
--rw-rw-rw-   0        0        0        0 2022-10-18 03:53:56.000000 api_master-1.0/polygonsdk/bot/cogs3/__init__.py
--rw-rw-rw-   0        0        0     2420 2023-06-16 03:03:50.000000 api_master-1.0/polygonsdk/bot/cogs3/allinone.py
--rw-rw-rw-   0        0        0     4646 2023-06-16 03:07:36.000000 api_master-1.0/polygonsdk/bot/cogs3/cboe.py
--rw-rw-rw-   0        0        0    13259 2023-06-16 03:11:09.000000 api_master-1.0/polygonsdk/bot/cogs3/discord.py
--rw-rw-rw-   0        0        0    15308 2023-06-16 03:45:39.000000 api_master-1.0/polygonsdk/bot/cogs3/fed.py
--rw-rw-rw-   0        0        0     4049 2023-06-16 03:15:01.000000 api_master-1.0/polygonsdk/bot/cogs3/fudstop.py
--rw-rw-rw-   0        0        0    10534 2023-06-16 03:14:52.000000 api_master-1.0/polygonsdk/bot/cogs3/iv.py
--rw-rw-rw-   0        0        0     7484 2023-06-16 03:14:29.000000 api_master-1.0/polygonsdk/bot/cogs3/reddit.py
--rw-rw-rw-   0        0        0     2604 2023-06-16 03:13:44.000000 api_master-1.0/polygonsdk/bot/cogs3/school.py
--rw-rw-rw-   0        0        0     8852 2023-06-16 03:11:56.000000 api_master-1.0/polygonsdk/bot/cogs3/social.py
--rw-rw-rw-   0        0        0     9893 2023-06-16 03:41:40.000000 api_master-1.0/polygonsdk/bot/cogs3/strat.py
--rw-rw-rw-   0        0        0     6919 2023-06-11 22:19:59.000000 api_master-1.0/polygonsdk/bot/discord_emojis.py
--rw-rw-rw-   0        0        0     1440 2023-06-16 03:51:23.000000 api_master-1.0/polygonsdk/bot/main.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.320727 api_master-1.0/polygonsdk/bot/utils/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/bot/utils/__init__.py
--rw-rw-rw-   0        0        0     1368 2023-06-16 02:40:26.000000 api_master-1.0/polygonsdk/bot/utils/crypto_coins.py
--rw-rw-rw-   0        0        0      998 2023-06-16 02:35:33.000000 api_master-1.0/polygonsdk/bot/utils/date_times.py
--rw-rw-rw-   0        0        0   224003 2023-06-16 03:10:59.000000 api_master-1.0/polygonsdk/bot/utils/lists_and_dicts.py
--rw-rw-rw-   0        0        0   199781 2023-06-16 02:46:46.000000 api_master-1.0/polygonsdk/bot/utils/webull_tickers.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.321728 api_master-1.0/polygonsdk/bot/views/
--rw-rw-rw-   0        0        0       49 2023-06-16 22:29:34.000000 api_master-1.0/polygonsdk/bot/views/__init__.py
--rw-rw-rw-   0        0        0  1503928 2023-06-16 03:50:00.000000 api_master-1.0/polygonsdk/bot/views/learnviews.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.332727 api_master-1.0/polygonsdk/bot/views/uiviews/
--rw-rw-rw-   0        0        0   320159 2023-06-16 03:04:42.000000 api_master-1.0/polygonsdk/bot/views/uiviews/MarketAnalysis.py
--rw-rw-rw-   0        0        0     5109 2023-06-16 03:43:55.000000 api_master-1.0/polygonsdk/bot/views/uiviews/TickerAnalysis.py
--rw-rw-rw-   0        0        0        0 2022-10-25 14:28:50.000000 api_master-1.0/polygonsdk/bot/views/uiviews/__init__ copy.py
--rw-rw-rw-   0        0        0        0 2022-10-25 14:28:50.000000 api_master-1.0/polygonsdk/bot/views/uiviews/__init__.py
--rw-rw-rw-   0        0        0     5169 2023-06-16 03:04:01.000000 api_master-1.0/polygonsdk/bot/views/uiviews/capitalflow.py
--rw-rw-rw-   0        0        0   110984 2022-11-14 02:53:40.000000 api_master-1.0/polygonsdk/bot/views/uiviews/cmslist.py
--rw-rw-rw-   0        0        0   107414 2023-06-16 12:53:34.000000 api_master-1.0/polygonsdk/bot/views/uiviews/cmslist2.py
--rw-rw-rw-   0        0        0    18026 2023-06-16 03:04:21.000000 api_master-1.0/polygonsdk/bot/views/uiviews/directiondrop.py
--rw-rw-rw-   0        0        0     9311 2023-06-16 03:04:32.000000 api_master-1.0/polygonsdk/bot/views/uiviews/financialselects.py
--rw-rw-rw-   0        0        0    12480 2023-06-16 03:04:50.000000 api_master-1.0/polygonsdk/bot/views/uiviews/ftds.py
--rw-rw-rw-   0        0        0     4675 2023-06-16 03:04:58.000000 api_master-1.0/polygonsdk/bot/views/uiviews/leveragedropdown.py
--rw-rw-rw-   0        0        0     7693 2023-06-16 03:05:03.000000 api_master-1.0/polygonsdk/bot/views/uiviews/lowfloat.py
--rw-rw-rw-   0        0        0     4487 2023-06-16 03:51:49.000000 api_master-1.0/polygonsdk/bot/views/uiviews/masterview.py
--rw-rw-rw-   0        0        0     5619 2022-11-05 23:34:22.000000 api_master-1.0/polygonsdk/bot/views/uiviews/mostactive.py
--rw-rw-rw-   0        0        0     6579 2022-11-05 23:04:27.000000 api_master-1.0/polygonsdk/bot/views/uiviews/pressrelease.py
--rw-rw-rw-   0        0        0     3355 2023-06-16 03:17:25.000000 api_master-1.0/polygonsdk/bot/views/uiviews/quote.py
--rw-rw-rw-   0        0        0    13749 2023-06-16 03:04:42.000000 api_master-1.0/polygonsdk/bot/views/uiviews/shortinterest.py
--rw-rw-rw-   0        0        0     3551 2023-06-16 12:56:25.000000 api_master-1.0/polygonsdk/cfg.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.334727 api_master-1.0/polygonsdk/examples/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/__init__.py
--rw-rw-rw-   0        0        0     5940 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/all_attributes.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.335727 api_master-1.0/polygonsdk/examples/functions/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:36:14.000000 api_master-1.0/polygonsdk/examples/functions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.339727 api_master-1.0/polygonsdk/examples/functions/options/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:36:18.000000 api_master-1.0/polygonsdk/examples/functions/options/__init__.py
--rw-rw-rw-   0        0        0      706 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/functions/options/create_option_symbol.py
--rw-rw-rw-   0        0        0      910 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/functions/options/fetch_entire_chain.py
--rw-rw-rw-   0        0        0     1625 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/functions/options/option_quote.py
--rw-rw-rw-   0        0        0     2408 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/functions/options/option_trades.py
--rw-rw-rw-   0        0        0     1797 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/functions/options/plot_option_aggs.py
--rw-rw-rw-   0        0        0     5590 2023-06-14 15:27:10.000000 api_master-1.0/polygonsdk/examples/functions/options/scanner_example.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.343729 api_master-1.0/polygonsdk/examples/functions/stocks/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:36:22.000000 api_master-1.0/polygonsdk/examples/functions/stocks/__init__.py
--rw-rw-rw-   0        0        0     1796 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/functions/stocks/latest_news.py
--rw-rw-rw-   0        0        0     1408 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/functions/stocks/plot_aggs.py
--rw-rw-rw-   0        0        0     8185 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/functions/stocks/scan_candles.py
--rw-rw-rw-   0        0        0     2116 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/functions/stocks/stock_aggregates.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.353727 api_master-1.0/polygonsdk/examples/functions/technical_analysis/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:36:27.000000 api_master-1.0/polygonsdk/examples/functions/technical_analysis/__init__.py
--rw-rw-rw-   0        0        0      533 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/functions/technical_analysis/bollinger_bands.py
--rw-rw-rw-   0        0        0     4375 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/functions/technical_analysis/candle_patterns.py
--rw-rw-rw-   0        0        0     1376 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/functions/technical_analysis/ema.py
--rw-rw-rw-   0        0        0      693 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/functions/technical_analysis/find_gaps.py
--rw-rw-rw-   0        0        0     2399 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/functions/technical_analysis/get_ema.py
--rw-rw-rw-   0        0        0      644 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/functions/technical_analysis/get_logo.py
--rw-rw-rw-   0        0        0     3195 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/functions/technical_analysis/get_macd.py
--rw-rw-rw-   0        0        0      665 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/functions/technical_analysis/get_pivot_points.py
--rw-rw-rw-   0        0        0     2051 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/functions/technical_analysis/get_rsi.py
--rw-rw-rw-   0        0        0     1935 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/functions/technical_analysis/get_sma.py
--rw-rw-rw-   0        0        0      930 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/functions/technical_analysis/macd_sma_rsi.py
--rw-rw-rw-   0        0        0      487 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/functions/technical_analysis/rate_of_change.py
--rw-rw-rw-   0        0        0      627 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/functions/technical_analysis/rsi.py
--rw-rw-rw-   0        0        0     1189 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/functions/technical_analysis/support_resistance.py
--rw-rw-rw-   0        0        0      703 2023-06-14 15:26:12.000000 api_master-1.0/polygonsdk/examples/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.358729 api_master-1.0/polygonsdk/examples/realtime_markets/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/realtime_markets/__init__.py
--rw-rw-rw-   0        0        0     2479 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/realtime_markets/crypto_market.py
--rw-rw-rw-   0        0        0    44945 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/realtime_markets/discord_market.py
--rw-rw-rw-   0        0        0      922 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/realtime_markets/forex_market.py
--rw-rw-rw-   0        0        0      776 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/realtime_markets/indices_market.py
--rw-rw-rw-   0        0        0      989 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/realtime_markets/options_market.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.361730 api_master-1.0/polygonsdk/examples/simulated_markets/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/simulated_markets/__init__.py
--rw-rw-rw-   0        0        0      688 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/examples/simulated_markets/helpers.py
--rw-rw-rw-   0        0        0     5115 2023-06-11 22:19:16.000000 api_master-1.0/polygonsdk/examples/simulated_markets/mock_discord.py
--rw-rw-rw-   0        0        0     1951 2023-06-12 01:17:16.000000 api_master-1.0/polygonsdk/examples/simulated_markets/mock_market.py
--rw-rw-rw-   0        0        0     1551 2023-06-12 01:18:49.000000 api_master-1.0/polygonsdk/examples/simulated_markets/mock_options_market.py
--rw-rw-rw-   0        0        0    14776 2023-06-16 14:39:01.000000 api_master-1.0/polygonsdk/examples/webull_data.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.366732 api_master-1.0/polygonsdk/funcs/
--rw-rw-rw-   0        0        0        0 2023-06-11 22:29:36.000000 api_master-1.0/polygonsdk/funcs/__init__.py
--rw-rw-rw-   0        0        0    36181 2023-06-11 22:44:36.000000 api_master-1.0/polygonsdk/funcs/get_data.py
--rw-rw-rw-   0        0        0      619 2023-06-13 22:33:48.000000 api_master-1.0/polygonsdk/funcs/get_latest_crypto_data.py
--rw-rw-rw-   0        0        0      585 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/funcs/get_latest_forex_data.py
--rw-rw-rw-   0        0        0      446 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/funcs/get_latest_indices_data.py
--rw-rw-rw-   0        0        0      762 2023-06-11 21:54:23.000000 api_master-1.0/polygonsdk/funcs/get_latest_options_data.py
--rw-rw-rw-   0        0        0      598 2023-06-12 00:39:12.000000 api_master-1.0/polygonsdk/funcs/get_latest_ticker_data.py
--rw-rw-rw-   0        0        0      335 2023-06-16 14:21:39.000000 api_master-1.0/polygonsdk/funcs/get_webull_data.py
--rw-rw-rw-   0        0        0     1052 2023-06-12 01:22:03.000000 api_master-1.0/polygonsdk/funcs/sec_filings.py
--rw-rw-rw-   0        0        0     2264 2023-06-12 01:16:14.000000 api_master-1.0/polygonsdk/funcs/webull_examples.py
--rw-rw-rw-   0        0        0     1252 2023-06-16 14:28:50.000000 api_master-1.0/polygonsdk/myconfig.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.367732 api_master-1.0/polygonsdk/sdks/
--rw-rw-rw-   0        0        0       18 2023-06-14 15:23:50.000000 api_master-1.0/polygonsdk/sdks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.369732 api_master-1.0/polygonsdk/sdks/discord_sdk/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/discord_sdk/__init__.py
--rw-rw-rw-   0        0        0       53 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/discord_sdk/channel_ids.py
--rw-rw-rw-   0        0        0     4497 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/discord_sdk/discord_sdk.py
--rw-rw-rw-   0        0        0     2157 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/discord_sdk/searching.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.383747 api_master-1.0/polygonsdk/sdks/examples/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/__init__.py
--rw-rw-rw-   0        0        0     6184 2023-06-12 00:26:46.000000 api_master-1.0/polygonsdk/sdks/examples/all_attributes.py
--rw-rw-rw-   0        0        0      517 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/bollinger_bands.py
--rw-rw-rw-   0        0        0      706 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/create_option_symbol.py
--rw-rw-rw-   0        0        0     1664 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/ema.py
--rw-rw-rw-   0        0        0      910 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/fetch_entire_chain.py
--rw-rw-rw-   0        0        0      649 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/find_gaps.py
--rw-rw-rw-   0        0        0      823 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/get_all_options_data.py
--rw-rw-rw-   0        0        0     2399 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/get_ema.py
--rw-rw-rw-   0        0        0      600 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/get_latest_crypto_data.py
--rw-rw-rw-   0        0        0      585 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/get_latest_forex_data.py
--rw-rw-rw-   0        0        0      446 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/get_latest_indices_data.py
--rw-rw-rw-   0        0        0      644 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/get_latest_ticker_data.py
--rw-rw-rw-   0        0        0     3161 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/get_macd.py
--rw-rw-rw-   0        0        0      582 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/get_pivot_points.py
--rw-rw-rw-   0        0        0     2051 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/get_rsi.py
--rw-rw-rw-   0        0        0     2172 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/get_sma.py
--rw-rw-rw-   0        0        0     1796 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/latest_news.py
--rw-rw-rw-   0        0        0     1625 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/option_quote.py
--rw-rw-rw-   0        0        0     2408 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/option_trades.py
--rw-rw-rw-   0        0        0     1408 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/plot_aggs.py
--rw-rw-rw-   0        0        0      796 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/plot_macd.py
--rw-rw-rw-   0        0        0     1797 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/plot_option_aggs.py
--rw-rw-rw-   0        0        0      487 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/rate_of_change.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.385748 api_master-1.0/polygonsdk/sdks/examples/realtime_markets/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/realtime_markets/__init__.py
--rw-rw-rw-   0        0        0     2479 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/realtime_markets/crypto_market.py
--rw-rw-rw-   0        0        0      922 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/realtime_markets/forex_market.py
--rw-rw-rw-   0        0        0      776 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/realtime_markets/indices_market.py
--rw-rw-rw-   0        0        0      989 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/realtime_markets/options_market.py
--rw-rw-rw-   0        0        0     4837 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/scanner_example.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.387747 api_master-1.0/polygonsdk/sdks/examples/simulated_markets/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/simulated_markets/__init__.py
--rw-rw-rw-   0        0        0      688 2023-06-14 15:26:03.000000 api_master-1.0/polygonsdk/sdks/examples/simulated_markets/helpers.py
--rw-rw-rw-   0        0        0     2606 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/simulated_markets/mock_market.py
--rw-rw-rw-   0        0        0     1806 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/simulated_markets/mock_options_market.py
--rw-rw-rw-   0        0        0     2116 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/stock_aggregates.py
--rw-rw-rw-   0        0        0     1189 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/examples/support_resistance.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.389748 api_master-1.0/polygonsdk/sdks/fudstop_sdk/
--rw-rw-rw-   0        0        0        1 2023-06-12 00:06:40.000000 api_master-1.0/polygonsdk/sdks/fudstop_sdk/__init__.py
--rw-rw-rw-   0        0        0     2909 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/fudstop_sdk/fudstop_sdk.py
--rw-rw-rw-   0        0        0     1661 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/fudstop_sdk/gaps.py
--rw-rw-rw-   0        0        0      427 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/fudstop_sdk/option_vol_totals.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.391748 api_master-1.0/polygonsdk/sdks/helpers/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/helpers/__init__.py
--rw-rw-rw-   0        0        0     2001 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/helpers/conditions.py
--rw-rw-rw-   0        0        0        2 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/helpers/get_cik.py
--rw-rw-rw-   0        0        0     5442 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/helpers/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.393747 api_master-1.0/polygonsdk/sdks/models/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/models/__init__.py
--rw-rw-rw-   0        0        0      488 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/models/common.py
--rw-rw-rw-   0        0        0     5097 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/models/maps.py
--rw-rw-rw-   0        0        0    13078 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/models/test_events.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.407750 api_master-1.0/polygonsdk/sdks/polygon_sdk/
--rw-rw-rw-   0        0        0      543 2023-06-16 22:28:47.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/__init__.py
--rw-rw-rw-   0        0        0     1265 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/aggregates.py
--rw-rw-rw-   0        0        0    29379 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/async_options_sdk.py
--rw-rw-rw-   0        0        0    52775 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/async_polygon_sdk.py
--rw-rw-rw-   0        0        0     1135 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/company_info.py
--rw-rw-rw-   0        0        0      703 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/daily_open_close.py
--rw-rw-rw-   0        0        0    15043 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/financials.py
--rw-rw-rw-   0        0        0     6644 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/forex_crypto.py
--rw-rw-rw-   0        0        0     8957 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/get_all_options.py
--rw-rw-rw-   0        0        0     1131 2023-06-11 21:54:24.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/indices_snapshot.py
--rw-rw-rw-   0        0        0      823 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/logo.py
--rw-rw-rw-   0        0        0    27900 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/mapping_dicts.py
--rw-rw-rw-   0        0        0      782 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/models.py
--rw-rw-rw-   0        0        0      819 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/news.py
--rw-rw-rw-   0        0        0      820 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/option_aggs.py
--rw-rw-rw-   0        0        0     1493 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/option_quote.py
--rw-rw-rw-   0        0        0     3079 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/option_snapshot.py
--rw-rw-rw-   0        0        0      873 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/option_trades.py
--rw-rw-rw-   0        0        0      538 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/pivot_points.py
--rw-rw-rw-   0        0        0      690 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/quote.py
--rw-rw-rw-   0        0        0      151 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/sec.py
--rw-rw-rw-   0        0        0     4192 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/snapshot.py
--rw-rw-rw-   0        0        0     1313 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/technical_conditions.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.410747 api_master-1.0/polygonsdk/sdks/polygon_sdk/technicals/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/technicals/__init__.py
--rw-rw-rw-   0        0        0      248 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/technicals/ema.py
--rw-rw-rw-   0        0        0      229 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/technicals/macd.py
--rw-rw-rw-   0        0        0      233 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/technicals/rsi.py
--rw-rw-rw-   0        0        0      244 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/technicals/sma.py
--rw-rw-rw-   0        0        0     3361 2023-06-13 21:44:27.000000 api_master-1.0/polygonsdk/sdks/polygon_sdk/tickernews.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.411800 api_master-1.0/polygonsdk/sdks/stocksera_sdk/
--rw-rw-rw-   0        0        0      103 2023-06-16 22:27:26.000000 api_master-1.0/polygonsdk/sdks/stocksera_sdk/__init__.py
--rw-rw-rw-   0        0        0      757 2023-06-14 23:11:39.000000 api_master-1.0/polygonsdk/sdks/stocksera_sdk/borrowed.py
--rw-rw-rw-   0        0        0      956 2023-06-14 23:30:32.000000 api_master-1.0/polygonsdk/sdks/stocksera_sdk/earnings.py
--rw-rw-rw-   0        0        0     1309 2023-06-16 14:28:24.000000 api_master-1.0/polygonsdk/sdks/stocksera_sdk/stocksera_sdk.py
--rw-rw-rw-   0        0        0      580 2023-06-14 23:22:44.000000 api_master-1.0/polygonsdk/sdks/stocksera_sdk/treasury.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.411800 api_master-1.0/polygonsdk/sdks/terminals/
--rw-rw-rw-   0        0        0        0 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/terminals/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.411800 api_master-1.0/polygonsdk/sdks/terminals/crypto/
--rw-rw-rw-   0        0        0        0 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/terminals/crypto/__init__.py
--rw-rw-rw-   0        0        0     1672 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/terminals/crypto/menu.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.423259 api_master-1.0/polygonsdk/sdks/webull_sdk/
--rw-rw-rw-   0        0        0      440 2023-06-16 22:31:19.000000 api_master-1.0/polygonsdk/sdks/webull_sdk/__init__.py
--rw-rw-rw-   0        0        0      882 2023-06-11 22:15:21.000000 api_master-1.0/polygonsdk/sdks/webull_sdk/calendar.py
--rw-rw-rw-   0        0        0     9144 2023-06-16 14:33:32.000000 api_master-1.0/polygonsdk/sdks/webull_sdk/capitalflow.py
--rw-rw-rw-   0        0        0     1152 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/webull_sdk/cost_distribution.py
--rw-rw-rw-   0        0        0     2282 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/webull_sdk/derivative_query.py
--rw-rw-rw-   0        0        0     2426 2023-06-11 22:15:21.000000 api_master-1.0/polygonsdk/sdks/webull_sdk/etf_finder.py
--rw-rw-rw-   0        0        0      486 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/webull_sdk/etf_holdings.py
--rw-rw-rw-   0        0        0     1100 2023-06-16 14:24:58.000000 api_master-1.0/polygonsdk/sdks/webull_sdk/events.py
--rw-rw-rw-   0        0        0     7818 2023-06-11 22:15:21.000000 api_master-1.0/polygonsdk/sdks/webull_sdk/financial_statement.py
--rw-rw-rw-   0        0        0     3780 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/webull_sdk/forecast.py
--rw-rw-rw-   0        0        0     1033 2023-06-11 22:15:21.000000 api_master-1.0/polygonsdk/sdks/webull_sdk/institutional_holdings.py
--rw-rw-rw-   0        0        0     1235 2023-06-16 22:35:10.000000 api_master-1.0/polygonsdk/sdks/webull_sdk/manage.py
--rw-rw-rw-   0        0        0      617 2023-06-11 22:15:21.000000 api_master-1.0/polygonsdk/sdks/webull_sdk/news.py
--rw-rw-rw-   0        0        0      307 2023-06-11 22:15:21.000000 api_master-1.0/polygonsdk/sdks/webull_sdk/shortinterest.py
--rw-rw-rw-   0        0        0     2730 2023-06-11 21:54:25.000000 api_master-1.0/polygonsdk/sdks/webull_sdk/top_gainers.py
--rw-rw-rw-   0        0        0    16723 2023-06-11 22:15:21.000000 api_master-1.0/polygonsdk/sdks/webull_sdk/top_options.py
--rw-rw-rw-   0        0        0     5556 2023-06-11 22:15:21.000000 api_master-1.0/polygonsdk/sdks/webull_sdk/webull_data.py
--rw-rw-rw-   0        0        0    42510 2023-06-16 14:52:27.000000 api_master-1.0/polygonsdk/sdks/webull_sdk/webull_sdk.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.423259 api_master-1.0/polygonsdk/static/
--rw-rw-rw-   0        0        0      101 2023-06-14 14:26:46.000000 api_master-1.0/polygonsdk/static/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.424264 api_master-1.0/polygonsdk/static/css/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:37:24.000000 api_master-1.0/polygonsdk/static/css/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.425264 api_master-1.0/polygonsdk/static/images/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:37:29.000000 api_master-1.0/polygonsdk/static/images/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.425264 api_master-1.0/polygonsdk/static/js/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:37:34.000000 api_master-1.0/polygonsdk/static/js/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.427263 api_master-1.0/polygonsdk/static/py/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:37:38.000000 api_master-1.0/polygonsdk/static/py/__init__.py
--rw-rw-rw-   0        0        0      573 2023-06-15 22:05:01.000000 api_master-1.0/polygonsdk/static/py/commands.py
--rw-rw-rw-   0        0        0      796 2023-06-12 21:29:16.000000 api_master-1.0/polygonsdk/static/py/snippets.py
--rw-rw-rw-   0        0        0      312 2023-06-12 21:41:31.000000 api_master-1.0/polygonsdk/static/py/website_components.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:14:06.428264 api_master-1.0/polygonsdk/templates/
--rw-rw-rw-   0        0        0        0 2023-06-16 22:25:34.000000 api_master-1.0/polygonsdk/templates/__init__.py
--rw-rw-rw-   0        0        0     4315 2023-06-15 21:34:52.000000 api_master-1.0/polygonsdk/test.py
--rw-rw-rw-   0        0        0       42 2023-06-16 23:14:06.429265 api_master-1.0/setup.cfg
--rw-rw-rw-   0        0        0      755 2023-06-16 23:13:29.000000 api_master-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:16.060930 api_master-1.1/
+-rw-rw-rw-   0        0        0     2484 2023-06-16 23:25:16.060699 api_master-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1929 2023-06-16 23:10:25.000000 api_master-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.886058 api_master-1.1/api_master.egg-info/
+-rw-rw-rw-   0        0        0     2484 2023-06-16 23:25:15.000000 api_master-1.1/api_master.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10676 2023-06-16 23:25:15.000000 api_master-1.1/api_master.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 23:25:15.000000 api_master-1.1/api_master.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-16 23:25:15.000000 api_master-1.1/api_master.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.886058 api_master-1.1/polygonsdk/
+-rw-rw-rw-   0        0        0      189 2023-06-16 23:22:57.000000 api_master-1.1/polygonsdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.893565 api_master-1.1/polygonsdk/_discord/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/_discord/__init__.py
+-rw-rw-rw-   0        0        0     7983 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/_discord/discord_stock_example.py
+-rw-rw-rw-   0        0        0    44936 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/_discord/discord_stock_market.py
+-rw-rw-rw-   0        0        0    16306 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/_discord/embeddings.py
+-rw-rw-rw-   0        0        0      581 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/_discord/emojis.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.896307 api_master-1.1/polygonsdk/_discord/hooks/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/_discord/hooks/__init__.py
+-rw-rw-rw-   0        0        0     1594 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/_discord/hooks/channel_webhooks.py
+-rw-rw-rw-   0        0        0    10521 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/_discord/hooks/hook_dicts.py
+-rw-rw-rw-   0        0        0     5462 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/_discord/hooks/send_webhook.py
+-rw-rw-rw-   0        0        0    33594 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/_discord/live_discord.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.896816 api_master-1.1/polygonsdk/_discord/selectmenus/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/_discord/selectmenus/__init__.py
+-rw-rw-rw-   0        0        0    33209 2023-06-11 22:20:44.000000 api_master-1.1/polygonsdk/_discord/selectmenus/mainselect.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.898820 api_master-1.1/polygonsdk/_discord/views/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/_discord/views/__init__.py
+-rw-rw-rw-   0        0        0     1640 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/_discord/views/mainview.py
+-rw-rw-rw-   0        0        0     3792 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/_discord/views/menus.py
+-rw-rw-rw-   0        0        0     7502 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/_discord/webhook_creation.py
+-rw-rw-rw-   0        0        0     7264 2023-06-16 23:04:23.000000 api_master-1.1/polygonsdk/app.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.906823 api_master-1.1/polygonsdk/bot/
+-rw-rw-rw-   0        0        0       72 2023-06-16 22:29:19.000000 api_master-1.1/polygonsdk/bot/__init__.py
+-rw-rw-rw-   0        0        0    13384 2023-06-16 23:23:57.000000 api_master-1.1/polygonsdk/bot/autocomp.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.912335 api_master-1.1/polygonsdk/bot/cogs/
+-rw-rw-rw-   0        0        0      162 2023-06-16 22:30:15.000000 api_master-1.1/polygonsdk/bot/cogs/__init__.py
+-rw-rw-rw-   0        0        0     4478 2023-06-16 03:42:45.000000 api_master-1.1/polygonsdk/bot/cogs/earnings.py
+-rw-rw-rw-   0        0        0     1406 2023-06-16 02:49:27.000000 api_master-1.1/polygonsdk/bot/cogs/evaluate.py
+-rw-rw-rw-   0        0        0    11853 2023-06-06 22:47:55.000000 api_master-1.1/polygonsdk/bot/cogs/jasmy.py
+-rw-rw-rw-   0        0        0     2219 2023-06-15 04:47:31.000000 api_master-1.1/polygonsdk/bot/cogs/navigate.py
+-rw-rw-rw-   0        0        0     1794 2023-06-06 22:53:29.000000 api_master-1.1/polygonsdk/bot/cogs/scan.py
+-rw-rw-rw-   0        0        0    10785 2023-06-16 03:00:26.000000 api_master-1.1/polygonsdk/bot/cogs/stream.py
+-rw-rw-rw-   0        0        0    32431 2023-06-16 03:44:06.000000 api_master-1.1/polygonsdk/bot/cogs/webull.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.917838 api_master-1.1/polygonsdk/bot/cogs2/
+-rw-rw-rw-   0        0        0        0 2022-10-11 19:37:24.000000 api_master-1.1/polygonsdk/bot/cogs2/__init__.py
+-rw-rw-rw-   0        0        0    13678 2023-06-06 22:33:16.000000 api_master-1.1/polygonsdk/bot/cogs2/analysis.py
+-rw-rw-rw-   0        0        0     4580 2023-06-16 02:58:46.000000 api_master-1.1/polygonsdk/bot/cogs2/collect.py
+-rw-rw-rw-   0        0        0    14094 2023-06-16 03:47:55.000000 api_master-1.1/polygonsdk/bot/cogs2/economy.py
+-rw-rw-rw-   0        0        0    13966 2023-06-16 03:00:46.000000 api_master-1.1/polygonsdk/bot/cogs2/learn.py
+-rw-rw-rw-   0        0        0     3830 2023-06-16 03:47:27.000000 api_master-1.1/polygonsdk/bot/cogs2/news.py
+-rw-rw-rw-   0        0        0    75051 2023-04-11 14:56:18.000000 api_master-1.1/polygonsdk/bot/cogs2/occ.py
+-rw-rw-rw-   0        0        0    19227 2023-06-16 03:43:01.000000 api_master-1.1/polygonsdk/bot/cogs2/options.py
+-rw-rw-rw-   0        0        0     1823 2023-06-16 02:52:02.000000 api_master-1.1/polygonsdk/bot/cogs2/prices_and_technicals.py
+-rw-rw-rw-   0        0        0    50520 2023-06-16 03:47:06.000000 api_master-1.1/polygonsdk/bot/cogs2/stock.py
+-rw-rw-rw-   0        0        0    17675 2023-06-16 03:02:03.000000 api_master-1.1/polygonsdk/bot/cogs2/view.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.923844 api_master-1.1/polygonsdk/bot/cogs3/
+-rw-rw-rw-   0        0        0        0 2022-10-18 03:53:56.000000 api_master-1.1/polygonsdk/bot/cogs3/__init__.py
+-rw-rw-rw-   0        0        0     2420 2023-06-16 03:03:50.000000 api_master-1.1/polygonsdk/bot/cogs3/allinone.py
+-rw-rw-rw-   0        0        0     4646 2023-06-16 03:07:36.000000 api_master-1.1/polygonsdk/bot/cogs3/cboe.py
+-rw-rw-rw-   0        0        0    13259 2023-06-16 03:11:09.000000 api_master-1.1/polygonsdk/bot/cogs3/discord.py
+-rw-rw-rw-   0        0        0    15308 2023-06-16 03:45:39.000000 api_master-1.1/polygonsdk/bot/cogs3/fed.py
+-rw-rw-rw-   0        0        0     4049 2023-06-16 03:15:01.000000 api_master-1.1/polygonsdk/bot/cogs3/fudstop.py
+-rw-rw-rw-   0        0        0    10534 2023-06-16 03:14:52.000000 api_master-1.1/polygonsdk/bot/cogs3/iv.py
+-rw-rw-rw-   0        0        0     7484 2023-06-16 03:14:29.000000 api_master-1.1/polygonsdk/bot/cogs3/reddit.py
+-rw-rw-rw-   0        0        0     2604 2023-06-16 03:13:44.000000 api_master-1.1/polygonsdk/bot/cogs3/school.py
+-rw-rw-rw-   0        0        0     8852 2023-06-16 03:11:56.000000 api_master-1.1/polygonsdk/bot/cogs3/social.py
+-rw-rw-rw-   0        0        0     9893 2023-06-16 03:41:40.000000 api_master-1.1/polygonsdk/bot/cogs3/strat.py
+-rw-rw-rw-   0        0        0     6919 2023-06-11 22:19:59.000000 api_master-1.1/polygonsdk/bot/discord_emojis.py
+-rw-rw-rw-   0        0        0     1440 2023-06-16 03:51:23.000000 api_master-1.1/polygonsdk/bot/main.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.927776 api_master-1.1/polygonsdk/bot/utils/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/bot/utils/__init__.py
+-rw-rw-rw-   0        0        0     1368 2023-06-16 02:40:26.000000 api_master-1.1/polygonsdk/bot/utils/crypto_coins.py
+-rw-rw-rw-   0        0        0      998 2023-06-16 02:35:33.000000 api_master-1.1/polygonsdk/bot/utils/date_times.py
+-rw-rw-rw-   0        0        0   224003 2023-06-16 03:10:59.000000 api_master-1.1/polygonsdk/bot/utils/lists_and_dicts.py
+-rw-rw-rw-   0        0        0   199781 2023-06-16 02:46:46.000000 api_master-1.1/polygonsdk/bot/utils/webull_tickers.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.928367 api_master-1.1/polygonsdk/bot/views/
+-rw-rw-rw-   0        0        0       49 2023-06-16 22:29:34.000000 api_master-1.1/polygonsdk/bot/views/__init__.py
+-rw-rw-rw-   0        0        0  1503928 2023-06-16 03:50:00.000000 api_master-1.1/polygonsdk/bot/views/learnviews.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.938115 api_master-1.1/polygonsdk/bot/views/uiviews/
+-rw-rw-rw-   0        0        0   320159 2023-06-16 03:04:42.000000 api_master-1.1/polygonsdk/bot/views/uiviews/MarketAnalysis.py
+-rw-rw-rw-   0        0        0     5109 2023-06-16 03:43:55.000000 api_master-1.1/polygonsdk/bot/views/uiviews/TickerAnalysis.py
+-rw-rw-rw-   0        0        0        0 2022-10-25 14:28:50.000000 api_master-1.1/polygonsdk/bot/views/uiviews/__init__ copy.py
+-rw-rw-rw-   0        0        0        0 2022-10-25 14:28:50.000000 api_master-1.1/polygonsdk/bot/views/uiviews/__init__.py
+-rw-rw-rw-   0        0        0     5169 2023-06-16 03:04:01.000000 api_master-1.1/polygonsdk/bot/views/uiviews/capitalflow.py
+-rw-rw-rw-   0        0        0   110984 2022-11-14 02:53:40.000000 api_master-1.1/polygonsdk/bot/views/uiviews/cmslist.py
+-rw-rw-rw-   0        0        0   107414 2023-06-16 12:53:34.000000 api_master-1.1/polygonsdk/bot/views/uiviews/cmslist2.py
+-rw-rw-rw-   0        0        0    18026 2023-06-16 03:04:21.000000 api_master-1.1/polygonsdk/bot/views/uiviews/directiondrop.py
+-rw-rw-rw-   0        0        0     9311 2023-06-16 03:04:32.000000 api_master-1.1/polygonsdk/bot/views/uiviews/financialselects.py
+-rw-rw-rw-   0        0        0    12480 2023-06-16 03:04:50.000000 api_master-1.1/polygonsdk/bot/views/uiviews/ftds.py
+-rw-rw-rw-   0        0        0     4675 2023-06-16 03:04:58.000000 api_master-1.1/polygonsdk/bot/views/uiviews/leveragedropdown.py
+-rw-rw-rw-   0        0        0     7693 2023-06-16 03:05:03.000000 api_master-1.1/polygonsdk/bot/views/uiviews/lowfloat.py
+-rw-rw-rw-   0        0        0     4487 2023-06-16 03:51:49.000000 api_master-1.1/polygonsdk/bot/views/uiviews/masterview.py
+-rw-rw-rw-   0        0        0     5619 2022-11-05 23:34:22.000000 api_master-1.1/polygonsdk/bot/views/uiviews/mostactive.py
+-rw-rw-rw-   0        0        0     6579 2022-11-05 23:04:27.000000 api_master-1.1/polygonsdk/bot/views/uiviews/pressrelease.py
+-rw-rw-rw-   0        0        0     3355 2023-06-16 03:17:25.000000 api_master-1.1/polygonsdk/bot/views/uiviews/quote.py
+-rw-rw-rw-   0        0        0    13749 2023-06-16 03:04:42.000000 api_master-1.1/polygonsdk/bot/views/uiviews/shortinterest.py
+-rw-rw-rw-   0        0        0     3551 2023-06-16 12:56:25.000000 api_master-1.1/polygonsdk/cfg.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.938115 api_master-1.1/polygonsdk/examples/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/__init__.py
+-rw-rw-rw-   0        0        0     5940 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/all_attributes.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.943622 api_master-1.1/polygonsdk/examples/functions/
+-rw-rw-rw-   0        0        0        0 2023-06-13 22:36:14.000000 api_master-1.1/polygonsdk/examples/functions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.948288 api_master-1.1/polygonsdk/examples/functions/options/
+-rw-rw-rw-   0        0        0        0 2023-06-13 22:36:18.000000 api_master-1.1/polygonsdk/examples/functions/options/__init__.py
+-rw-rw-rw-   0        0        0      706 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/functions/options/create_option_symbol.py
+-rw-rw-rw-   0        0        0      910 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/functions/options/fetch_entire_chain.py
+-rw-rw-rw-   0        0        0     1625 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/functions/options/option_quote.py
+-rw-rw-rw-   0        0        0     2408 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/functions/options/option_trades.py
+-rw-rw-rw-   0        0        0     1797 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/functions/options/plot_option_aggs.py
+-rw-rw-rw-   0        0        0     5590 2023-06-14 15:27:10.000000 api_master-1.1/polygonsdk/examples/functions/options/scanner_example.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.950801 api_master-1.1/polygonsdk/examples/functions/stocks/
+-rw-rw-rw-   0        0        0        0 2023-06-13 22:36:22.000000 api_master-1.1/polygonsdk/examples/functions/stocks/__init__.py
+-rw-rw-rw-   0        0        0     1796 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/functions/stocks/latest_news.py
+-rw-rw-rw-   0        0        0     1408 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/functions/stocks/plot_aggs.py
+-rw-rw-rw-   0        0        0     8185 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/functions/stocks/scan_candles.py
+-rw-rw-rw-   0        0        0     2116 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/functions/stocks/stock_aggregates.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.959531 api_master-1.1/polygonsdk/examples/functions/technical_analysis/
+-rw-rw-rw-   0        0        0        0 2023-06-13 22:36:27.000000 api_master-1.1/polygonsdk/examples/functions/technical_analysis/__init__.py
+-rw-rw-rw-   0        0        0      533 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/functions/technical_analysis/bollinger_bands.py
+-rw-rw-rw-   0        0        0     4375 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/functions/technical_analysis/candle_patterns.py
+-rw-rw-rw-   0        0        0     1376 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/functions/technical_analysis/ema.py
+-rw-rw-rw-   0        0        0      693 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/functions/technical_analysis/find_gaps.py
+-rw-rw-rw-   0        0        0     2399 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/functions/technical_analysis/get_ema.py
+-rw-rw-rw-   0        0        0      644 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/functions/technical_analysis/get_logo.py
+-rw-rw-rw-   0        0        0     3195 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/functions/technical_analysis/get_macd.py
+-rw-rw-rw-   0        0        0      665 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/functions/technical_analysis/get_pivot_points.py
+-rw-rw-rw-   0        0        0     2051 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/functions/technical_analysis/get_rsi.py
+-rw-rw-rw-   0        0        0     1935 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/functions/technical_analysis/get_sma.py
+-rw-rw-rw-   0        0        0      930 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/functions/technical_analysis/macd_sma_rsi.py
+-rw-rw-rw-   0        0        0      487 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/functions/technical_analysis/rate_of_change.py
+-rw-rw-rw-   0        0        0      627 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/functions/technical_analysis/rsi.py
+-rw-rw-rw-   0        0        0     1189 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/functions/technical_analysis/support_resistance.py
+-rw-rw-rw-   0        0        0      703 2023-06-14 15:26:12.000000 api_master-1.1/polygonsdk/examples/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.963531 api_master-1.1/polygonsdk/examples/realtime_markets/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/realtime_markets/__init__.py
+-rw-rw-rw-   0        0        0     2479 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/realtime_markets/crypto_market.py
+-rw-rw-rw-   0        0        0    44945 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/realtime_markets/discord_market.py
+-rw-rw-rw-   0        0        0      922 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/realtime_markets/forex_market.py
+-rw-rw-rw-   0        0        0      776 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/realtime_markets/indices_market.py
+-rw-rw-rw-   0        0        0      989 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/realtime_markets/options_market.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.966531 api_master-1.1/polygonsdk/examples/simulated_markets/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/simulated_markets/__init__.py
+-rw-rw-rw-   0        0        0      688 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/examples/simulated_markets/helpers.py
+-rw-rw-rw-   0        0        0     5115 2023-06-11 22:19:16.000000 api_master-1.1/polygonsdk/examples/simulated_markets/mock_discord.py
+-rw-rw-rw-   0        0        0     1951 2023-06-12 01:17:16.000000 api_master-1.1/polygonsdk/examples/simulated_markets/mock_market.py
+-rw-rw-rw-   0        0        0     1551 2023-06-12 01:18:49.000000 api_master-1.1/polygonsdk/examples/simulated_markets/mock_options_market.py
+-rw-rw-rw-   0        0        0    14776 2023-06-16 14:39:01.000000 api_master-1.1/polygonsdk/examples/webull_data.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.972421 api_master-1.1/polygonsdk/funcs/
+-rw-rw-rw-   0        0        0        0 2023-06-11 22:29:36.000000 api_master-1.1/polygonsdk/funcs/__init__.py
+-rw-rw-rw-   0        0        0    36181 2023-06-11 22:44:36.000000 api_master-1.1/polygonsdk/funcs/get_data.py
+-rw-rw-rw-   0        0        0      619 2023-06-13 22:33:48.000000 api_master-1.1/polygonsdk/funcs/get_latest_crypto_data.py
+-rw-rw-rw-   0        0        0      585 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/funcs/get_latest_forex_data.py
+-rw-rw-rw-   0        0        0      446 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/funcs/get_latest_indices_data.py
+-rw-rw-rw-   0        0        0      762 2023-06-11 21:54:23.000000 api_master-1.1/polygonsdk/funcs/get_latest_options_data.py
+-rw-rw-rw-   0        0        0      598 2023-06-12 00:39:12.000000 api_master-1.1/polygonsdk/funcs/get_latest_ticker_data.py
+-rw-rw-rw-   0        0        0      335 2023-06-16 14:21:39.000000 api_master-1.1/polygonsdk/funcs/get_webull_data.py
+-rw-rw-rw-   0        0        0     1052 2023-06-12 01:22:03.000000 api_master-1.1/polygonsdk/funcs/sec_filings.py
+-rw-rw-rw-   0        0        0     2264 2023-06-12 01:16:14.000000 api_master-1.1/polygonsdk/funcs/webull_examples.py
+-rw-rw-rw-   0        0        0     1252 2023-06-16 14:28:50.000000 api_master-1.1/polygonsdk/myconfig.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.972421 api_master-1.1/polygonsdk/sdks/
+-rw-rw-rw-   0        0        0        0 2023-06-16 23:22:30.000000 api_master-1.1/polygonsdk/sdks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.974427 api_master-1.1/polygonsdk/sdks/discord_sdk/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/discord_sdk/__init__.py
+-rw-rw-rw-   0        0        0       53 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/discord_sdk/channel_ids.py
+-rw-rw-rw-   0        0        0     4497 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/discord_sdk/discord_sdk.py
+-rw-rw-rw-   0        0        0     2157 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/discord_sdk/searching.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.989964 api_master-1.1/polygonsdk/sdks/examples/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/__init__.py
+-rw-rw-rw-   0        0        0     6184 2023-06-12 00:26:46.000000 api_master-1.1/polygonsdk/sdks/examples/all_attributes.py
+-rw-rw-rw-   0        0        0      517 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/bollinger_bands.py
+-rw-rw-rw-   0        0        0      706 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/create_option_symbol.py
+-rw-rw-rw-   0        0        0     1664 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/ema.py
+-rw-rw-rw-   0        0        0      910 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/fetch_entire_chain.py
+-rw-rw-rw-   0        0        0      649 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/find_gaps.py
+-rw-rw-rw-   0        0        0      823 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/get_all_options_data.py
+-rw-rw-rw-   0        0        0     2399 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/get_ema.py
+-rw-rw-rw-   0        0        0      600 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/get_latest_crypto_data.py
+-rw-rw-rw-   0        0        0      585 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/get_latest_forex_data.py
+-rw-rw-rw-   0        0        0      446 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/get_latest_indices_data.py
+-rw-rw-rw-   0        0        0      644 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/get_latest_ticker_data.py
+-rw-rw-rw-   0        0        0     3161 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/get_macd.py
+-rw-rw-rw-   0        0        0      582 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/get_pivot_points.py
+-rw-rw-rw-   0        0        0     2051 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/get_rsi.py
+-rw-rw-rw-   0        0        0     2172 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/get_sma.py
+-rw-rw-rw-   0        0        0     1796 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/latest_news.py
+-rw-rw-rw-   0        0        0     1625 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/option_quote.py
+-rw-rw-rw-   0        0        0     2408 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/option_trades.py
+-rw-rw-rw-   0        0        0     1408 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/plot_aggs.py
+-rw-rw-rw-   0        0        0      796 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/plot_macd.py
+-rw-rw-rw-   0        0        0     1797 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/plot_option_aggs.py
+-rw-rw-rw-   0        0        0      487 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/rate_of_change.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.993467 api_master-1.1/polygonsdk/sdks/examples/realtime_markets/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/realtime_markets/__init__.py
+-rw-rw-rw-   0        0        0     2479 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/realtime_markets/crypto_market.py
+-rw-rw-rw-   0        0        0      922 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/realtime_markets/forex_market.py
+-rw-rw-rw-   0        0        0      776 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/realtime_markets/indices_market.py
+-rw-rw-rw-   0        0        0      989 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/realtime_markets/options_market.py
+-rw-rw-rw-   0        0        0     4837 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/scanner_example.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:15.996272 api_master-1.1/polygonsdk/sdks/examples/simulated_markets/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/simulated_markets/__init__.py
+-rw-rw-rw-   0        0        0      688 2023-06-14 15:26:03.000000 api_master-1.1/polygonsdk/sdks/examples/simulated_markets/helpers.py
+-rw-rw-rw-   0        0        0     2606 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/simulated_markets/mock_market.py
+-rw-rw-rw-   0        0        0     1806 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/simulated_markets/mock_options_market.py
+-rw-rw-rw-   0        0        0     2116 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/stock_aggregates.py
+-rw-rw-rw-   0        0        0     1189 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/examples/support_resistance.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:16.013578 api_master-1.1/polygonsdk/sdks/fudstop_sdk/
+-rw-rw-rw-   0        0        0        1 2023-06-12 00:06:40.000000 api_master-1.1/polygonsdk/sdks/fudstop_sdk/__init__.py
+-rw-rw-rw-   0        0        0     3095 2023-06-16 23:24:04.000000 api_master-1.1/polygonsdk/sdks/fudstop_sdk/fudstop_sdk.py
+-rw-rw-rw-   0        0        0     1847 2023-06-16 23:24:08.000000 api_master-1.1/polygonsdk/sdks/fudstop_sdk/gaps.py
+-rw-rw-rw-   0        0        0      613 2023-06-16 23:24:13.000000 api_master-1.1/polygonsdk/sdks/fudstop_sdk/option_vol_totals.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:16.015583 api_master-1.1/polygonsdk/sdks/helpers/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/helpers/__init__.py
+-rw-rw-rw-   0        0        0     2001 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/helpers/conditions.py
+-rw-rw-rw-   0        0        0        2 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/helpers/get_cik.py
+-rw-rw-rw-   0        0        0     5442 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/helpers/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:16.017583 api_master-1.1/polygonsdk/sdks/models/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/models/__init__.py
+-rw-rw-rw-   0        0        0      488 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/models/common.py
+-rw-rw-rw-   0        0        0     5097 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/models/maps.py
+-rw-rw-rw-   0        0        0    13078 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/models/test_events.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:16.032328 api_master-1.1/polygonsdk/sdks/polygon_sdk/
+-rw-rw-rw-   0        0        0      543 2023-06-16 22:28:47.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/__init__.py
+-rw-rw-rw-   0        0        0     1265 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/aggregates.py
+-rw-rw-rw-   0        0        0    29379 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/async_options_sdk.py
+-rw-rw-rw-   0        0        0    52775 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/async_polygon_sdk.py
+-rw-rw-rw-   0        0        0     1135 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/company_info.py
+-rw-rw-rw-   0        0        0      703 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/daily_open_close.py
+-rw-rw-rw-   0        0        0    15043 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/financials.py
+-rw-rw-rw-   0        0        0     6644 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/forex_crypto.py
+-rw-rw-rw-   0        0        0     8957 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/get_all_options.py
+-rw-rw-rw-   0        0        0     1131 2023-06-11 21:54:24.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/indices_snapshot.py
+-rw-rw-rw-   0        0        0      823 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/logo.py
+-rw-rw-rw-   0        0        0    27900 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/mapping_dicts.py
+-rw-rw-rw-   0        0        0      782 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/models.py
+-rw-rw-rw-   0        0        0      819 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/news.py
+-rw-rw-rw-   0        0        0      820 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/option_aggs.py
+-rw-rw-rw-   0        0        0     1493 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/option_quote.py
+-rw-rw-rw-   0        0        0     3079 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/option_snapshot.py
+-rw-rw-rw-   0        0        0      873 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/option_trades.py
+-rw-rw-rw-   0        0        0      538 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/pivot_points.py
+-rw-rw-rw-   0        0        0      690 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/quote.py
+-rw-rw-rw-   0        0        0      151 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/sec.py
+-rw-rw-rw-   0        0        0     4192 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/snapshot.py
+-rw-rw-rw-   0        0        0     1313 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/technical_conditions.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:16.035328 api_master-1.1/polygonsdk/sdks/polygon_sdk/technicals/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/technicals/__init__.py
+-rw-rw-rw-   0        0        0      248 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/technicals/ema.py
+-rw-rw-rw-   0        0        0      229 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/technicals/macd.py
+-rw-rw-rw-   0        0        0      233 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/technicals/rsi.py
+-rw-rw-rw-   0        0        0      244 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/technicals/sma.py
+-rw-rw-rw-   0        0        0     3361 2023-06-13 21:44:27.000000 api_master-1.1/polygonsdk/sdks/polygon_sdk/tickernews.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:16.038328 api_master-1.1/polygonsdk/sdks/stocksera_sdk/
+-rw-rw-rw-   0        0        0      103 2023-06-16 22:27:26.000000 api_master-1.1/polygonsdk/sdks/stocksera_sdk/__init__.py
+-rw-rw-rw-   0        0        0      757 2023-06-14 23:11:39.000000 api_master-1.1/polygonsdk/sdks/stocksera_sdk/borrowed.py
+-rw-rw-rw-   0        0        0      956 2023-06-14 23:30:32.000000 api_master-1.1/polygonsdk/sdks/stocksera_sdk/earnings.py
+-rw-rw-rw-   0        0        0     1309 2023-06-16 14:28:24.000000 api_master-1.1/polygonsdk/sdks/stocksera_sdk/stocksera_sdk.py
+-rw-rw-rw-   0        0        0      580 2023-06-14 23:22:44.000000 api_master-1.1/polygonsdk/sdks/stocksera_sdk/treasury.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:16.038328 api_master-1.1/polygonsdk/sdks/terminals/
+-rw-rw-rw-   0        0        0        0 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/terminals/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:16.039328 api_master-1.1/polygonsdk/sdks/terminals/crypto/
+-rw-rw-rw-   0        0        0        0 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/terminals/crypto/__init__.py
+-rw-rw-rw-   0        0        0     1672 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/terminals/crypto/menu.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:16.052196 api_master-1.1/polygonsdk/sdks/webull_sdk/
+-rw-rw-rw-   0        0        0      440 2023-06-16 22:31:19.000000 api_master-1.1/polygonsdk/sdks/webull_sdk/__init__.py
+-rw-rw-rw-   0        0        0      882 2023-06-11 22:15:21.000000 api_master-1.1/polygonsdk/sdks/webull_sdk/calendar.py
+-rw-rw-rw-   0        0        0     9144 2023-06-16 14:33:32.000000 api_master-1.1/polygonsdk/sdks/webull_sdk/capitalflow.py
+-rw-rw-rw-   0        0        0     1152 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/webull_sdk/cost_distribution.py
+-rw-rw-rw-   0        0        0     2282 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/webull_sdk/derivative_query.py
+-rw-rw-rw-   0        0        0     2426 2023-06-11 22:15:21.000000 api_master-1.1/polygonsdk/sdks/webull_sdk/etf_finder.py
+-rw-rw-rw-   0        0        0      486 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/webull_sdk/etf_holdings.py
+-rw-rw-rw-   0        0        0     1100 2023-06-16 14:24:58.000000 api_master-1.1/polygonsdk/sdks/webull_sdk/events.py
+-rw-rw-rw-   0        0        0     7818 2023-06-11 22:15:21.000000 api_master-1.1/polygonsdk/sdks/webull_sdk/financial_statement.py
+-rw-rw-rw-   0        0        0     3780 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/webull_sdk/forecast.py
+-rw-rw-rw-   0        0        0     1033 2023-06-11 22:15:21.000000 api_master-1.1/polygonsdk/sdks/webull_sdk/institutional_holdings.py
+-rw-rw-rw-   0        0        0     1235 2023-06-16 22:35:10.000000 api_master-1.1/polygonsdk/sdks/webull_sdk/manage.py
+-rw-rw-rw-   0        0        0      617 2023-06-11 22:15:21.000000 api_master-1.1/polygonsdk/sdks/webull_sdk/news.py
+-rw-rw-rw-   0        0        0      307 2023-06-11 22:15:21.000000 api_master-1.1/polygonsdk/sdks/webull_sdk/shortinterest.py
+-rw-rw-rw-   0        0        0     2730 2023-06-11 21:54:25.000000 api_master-1.1/polygonsdk/sdks/webull_sdk/top_gainers.py
+-rw-rw-rw-   0        0        0    16723 2023-06-11 22:15:21.000000 api_master-1.1/polygonsdk/sdks/webull_sdk/top_options.py
+-rw-rw-rw-   0        0        0     5556 2023-06-11 22:15:21.000000 api_master-1.1/polygonsdk/sdks/webull_sdk/webull_data.py
+-rw-rw-rw-   0        0        0    42510 2023-06-16 23:24:24.000000 api_master-1.1/polygonsdk/sdks/webull_sdk/webull_sdk.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:16.052196 api_master-1.1/polygonsdk/static/
+-rw-rw-rw-   0        0        0      101 2023-06-14 14:26:46.000000 api_master-1.1/polygonsdk/static/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:16.052196 api_master-1.1/polygonsdk/static/css/
+-rw-rw-rw-   0        0        0        0 2023-06-13 22:37:24.000000 api_master-1.1/polygonsdk/static/css/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:16.052196 api_master-1.1/polygonsdk/static/images/
+-rw-rw-rw-   0        0        0        0 2023-06-13 22:37:29.000000 api_master-1.1/polygonsdk/static/images/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:16.052196 api_master-1.1/polygonsdk/static/js/
+-rw-rw-rw-   0        0        0        0 2023-06-13 22:37:34.000000 api_master-1.1/polygonsdk/static/js/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:16.052196 api_master-1.1/polygonsdk/static/py/
+-rw-rw-rw-   0        0        0        0 2023-06-13 22:37:38.000000 api_master-1.1/polygonsdk/static/py/__init__.py
+-rw-rw-rw-   0        0        0      573 2023-06-15 22:05:01.000000 api_master-1.1/polygonsdk/static/py/commands.py
+-rw-rw-rw-   0        0        0      796 2023-06-12 21:29:16.000000 api_master-1.1/polygonsdk/static/py/snippets.py
+-rw-rw-rw-   0        0        0      312 2023-06-12 21:41:31.000000 api_master-1.1/polygonsdk/static/py/website_components.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:25:16.052196 api_master-1.1/polygonsdk/templates/
+-rw-rw-rw-   0        0        0        0 2023-06-16 22:25:34.000000 api_master-1.1/polygonsdk/templates/__init__.py
+-rw-rw-rw-   0        0        0     4315 2023-06-15 21:34:52.000000 api_master-1.1/polygonsdk/test.py
+-rw-rw-rw-   0        0        0       42 2023-06-16 23:25:16.060930 api_master-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      755 2023-06-16 23:25:00.000000 api_master-1.1/setup.py
```

### Comparing `api_master-1.0/PKG-INFO` & `api_master-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api_master
-Version: 1.0
+Version: 1.1
 Summary: Utilize several market-data APIs in production-ready format for real-time and simulated market analysis.
 Home-page: https://github.com/your-username/your-package-repo
 Author: Chuck Dustin
 Author-email: chuckdustin12@gmail.com
 Keywords: trading,stocks,options,crypto,forex,indices,discord
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `api_master-1.0/README.md` & `api_master-1.1/README.md`

 * *Files identical despite different names*

### Comparing `api_master-1.0/api_master.egg-info/PKG-INFO` & `api_master-1.1/api_master.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-master
-Version: 1.0
+Version: 1.1
 Summary: Utilize several market-data APIs in production-ready format for real-time and simulated market analysis.
 Home-page: https://github.com/your-username/your-package-repo
 Author: Chuck Dustin
 Author-email: chuckdustin12@gmail.com
 Keywords: trading,stocks,options,crypto,forex,indices,discord
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `api_master-1.0/api_master.egg-info/SOURCES.txt` & `api_master-1.1/api_master.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/_discord/discord_stock_example.py` & `api_master-1.1/polygonsdk/_discord/discord_stock_example.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/_discord/discord_stock_market.py` & `api_master-1.1/polygonsdk/_discord/discord_stock_market.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/_discord/embeddings.py` & `api_master-1.1/polygonsdk/_discord/embeddings.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/_discord/emojis.py` & `api_master-1.1/polygonsdk/_discord/emojis.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/_discord/hooks/channel_webhooks.py` & `api_master-1.1/polygonsdk/_discord/hooks/channel_webhooks.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/_discord/hooks/hook_dicts.py` & `api_master-1.1/polygonsdk/_discord/hooks/hook_dicts.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/_discord/hooks/send_webhook.py` & `api_master-1.1/polygonsdk/_discord/hooks/send_webhook.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/_discord/live_discord.py` & `api_master-1.1/polygonsdk/_discord/live_discord.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/_discord/selectmenus/mainselect.py` & `api_master-1.1/polygonsdk/_discord/selectmenus/mainselect.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/_discord/views/mainview.py` & `api_master-1.1/polygonsdk/_discord/views/mainview.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/_discord/views/menus.py` & `api_master-1.1/polygonsdk/_discord/views/menus.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/_discord/webhook_creation.py` & `api_master-1.1/polygonsdk/_discord/webhook_creation.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/app.py` & `api_master-1.1/polygonsdk/app.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/autocomp.py` & `api_master-1.1/polygonsdk/bot/autocomp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,14 @@
-
+import sys
 import os
+
+# Get the directory path of the polygonsdkmaster package
+package_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
+sys.path.append(package_dir)
+
 import disnake
 from disnake.ext import commands
 import json
 import typing
 from typing import List, Dict
 from typing import List
 import pandas as pd
```

### Comparing `api_master-1.0/polygonsdk/bot/cogs/earnings.py` & `api_master-1.1/polygonsdk/bot/cogs/earnings.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs/evaluate.py` & `api_master-1.1/polygonsdk/bot/cogs/evaluate.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs/jasmy.py` & `api_master-1.1/polygonsdk/bot/cogs/jasmy.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs/navigate.py` & `api_master-1.1/polygonsdk/bot/cogs/navigate.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs/scan.py` & `api_master-1.1/polygonsdk/bot/cogs/scan.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs/stream.py` & `api_master-1.1/polygonsdk/bot/cogs/stream.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs/webull.py` & `api_master-1.1/polygonsdk/bot/cogs/webull.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs2/analysis.py` & `api_master-1.1/polygonsdk/bot/cogs2/analysis.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs2/collect.py` & `api_master-1.1/polygonsdk/bot/cogs2/collect.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs2/economy.py` & `api_master-1.1/polygonsdk/bot/cogs2/economy.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs2/learn.py` & `api_master-1.1/polygonsdk/bot/cogs2/learn.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs2/news.py` & `api_master-1.1/polygonsdk/bot/cogs2/news.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs2/occ.py` & `api_master-1.1/polygonsdk/bot/cogs2/occ.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs2/options.py` & `api_master-1.1/polygonsdk/bot/cogs2/options.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs2/prices_and_technicals.py` & `api_master-1.1/polygonsdk/bot/cogs2/prices_and_technicals.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs2/stock.py` & `api_master-1.1/polygonsdk/bot/cogs2/stock.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs2/view.py` & `api_master-1.1/polygonsdk/bot/cogs2/view.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs3/allinone.py` & `api_master-1.1/polygonsdk/bot/cogs3/allinone.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs3/cboe.py` & `api_master-1.1/polygonsdk/bot/cogs3/cboe.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs3/discord.py` & `api_master-1.1/polygonsdk/bot/cogs3/discord.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs3/fed.py` & `api_master-1.1/polygonsdk/bot/cogs3/fed.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs3/fudstop.py` & `api_master-1.1/polygonsdk/bot/cogs3/fudstop.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs3/iv.py` & `api_master-1.1/polygonsdk/bot/cogs3/iv.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs3/reddit.py` & `api_master-1.1/polygonsdk/bot/cogs3/reddit.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs3/school.py` & `api_master-1.1/polygonsdk/bot/cogs3/school.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs3/social.py` & `api_master-1.1/polygonsdk/bot/cogs3/social.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/cogs3/strat.py` & `api_master-1.1/polygonsdk/bot/cogs3/strat.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/discord_emojis.py` & `api_master-1.1/polygonsdk/bot/discord_emojis.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/main.py` & `api_master-1.1/polygonsdk/bot/main.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/utils/crypto_coins.py` & `api_master-1.1/polygonsdk/bot/utils/crypto_coins.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/utils/date_times.py` & `api_master-1.1/polygonsdk/bot/utils/date_times.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/utils/lists_and_dicts.py` & `api_master-1.1/polygonsdk/bot/utils/lists_and_dicts.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/utils/webull_tickers.py` & `api_master-1.1/polygonsdk/bot/utils/webull_tickers.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/views/learnviews.py` & `api_master-1.1/polygonsdk/bot/views/learnviews.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/views/uiviews/MarketAnalysis.py` & `api_master-1.1/polygonsdk/bot/views/uiviews/MarketAnalysis.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/views/uiviews/TickerAnalysis.py` & `api_master-1.1/polygonsdk/bot/views/uiviews/TickerAnalysis.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/views/uiviews/capitalflow.py` & `api_master-1.1/polygonsdk/bot/views/uiviews/capitalflow.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/views/uiviews/cmslist.py` & `api_master-1.1/polygonsdk/bot/views/uiviews/cmslist.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/views/uiviews/cmslist2.py` & `api_master-1.1/polygonsdk/bot/views/uiviews/cmslist2.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/views/uiviews/directiondrop.py` & `api_master-1.1/polygonsdk/bot/views/uiviews/directiondrop.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/views/uiviews/financialselects.py` & `api_master-1.1/polygonsdk/bot/views/uiviews/financialselects.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/views/uiviews/ftds.py` & `api_master-1.1/polygonsdk/bot/views/uiviews/ftds.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/views/uiviews/leveragedropdown.py` & `api_master-1.1/polygonsdk/bot/views/uiviews/leveragedropdown.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/views/uiviews/lowfloat.py` & `api_master-1.1/polygonsdk/bot/views/uiviews/lowfloat.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/views/uiviews/masterview.py` & `api_master-1.1/polygonsdk/bot/views/uiviews/masterview.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/views/uiviews/mostactive.py` & `api_master-1.1/polygonsdk/bot/views/uiviews/mostactive.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/views/uiviews/pressrelease.py` & `api_master-1.1/polygonsdk/bot/views/uiviews/pressrelease.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/views/uiviews/quote.py` & `api_master-1.1/polygonsdk/bot/views/uiviews/quote.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/bot/views/uiviews/shortinterest.py` & `api_master-1.1/polygonsdk/bot/views/uiviews/shortinterest.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/cfg.py` & `api_master-1.1/polygonsdk/cfg.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/all_attributes.py` & `api_master-1.1/polygonsdk/examples/all_attributes.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/functions/options/create_option_symbol.py` & `api_master-1.1/polygonsdk/examples/functions/options/create_option_symbol.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/functions/options/fetch_entire_chain.py` & `api_master-1.1/polygonsdk/examples/functions/options/fetch_entire_chain.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/functions/options/option_quote.py` & `api_master-1.1/polygonsdk/examples/functions/options/option_quote.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/functions/options/option_trades.py` & `api_master-1.1/polygonsdk/examples/functions/options/option_trades.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/functions/options/plot_option_aggs.py` & `api_master-1.1/polygonsdk/examples/functions/options/plot_option_aggs.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/functions/options/scanner_example.py` & `api_master-1.1/polygonsdk/examples/functions/options/scanner_example.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/functions/stocks/latest_news.py` & `api_master-1.1/polygonsdk/examples/functions/stocks/latest_news.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/functions/stocks/plot_aggs.py` & `api_master-1.1/polygonsdk/examples/functions/stocks/plot_aggs.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/functions/stocks/scan_candles.py` & `api_master-1.1/polygonsdk/examples/functions/stocks/scan_candles.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/functions/stocks/stock_aggregates.py` & `api_master-1.1/polygonsdk/examples/functions/stocks/stock_aggregates.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/functions/technical_analysis/bollinger_bands.py` & `api_master-1.1/polygonsdk/examples/functions/technical_analysis/bollinger_bands.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/functions/technical_analysis/candle_patterns.py` & `api_master-1.1/polygonsdk/examples/functions/technical_analysis/candle_patterns.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/functions/technical_analysis/ema.py` & `api_master-1.1/polygonsdk/examples/functions/technical_analysis/ema.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/functions/technical_analysis/find_gaps.py` & `api_master-1.1/polygonsdk/examples/functions/technical_analysis/find_gaps.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/functions/technical_analysis/get_ema.py` & `api_master-1.1/polygonsdk/examples/functions/technical_analysis/get_ema.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/functions/technical_analysis/get_logo.py` & `api_master-1.1/polygonsdk/examples/functions/technical_analysis/get_logo.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/functions/technical_analysis/get_macd.py` & `api_master-1.1/polygonsdk/examples/functions/technical_analysis/get_macd.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/functions/technical_analysis/get_pivot_points.py` & `api_master-1.1/polygonsdk/examples/functions/technical_analysis/get_pivot_points.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/functions/technical_analysis/get_rsi.py` & `api_master-1.1/polygonsdk/examples/functions/technical_analysis/get_rsi.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/functions/technical_analysis/get_sma.py` & `api_master-1.1/polygonsdk/examples/functions/technical_analysis/get_sma.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/functions/technical_analysis/macd_sma_rsi.py` & `api_master-1.1/polygonsdk/examples/functions/technical_analysis/macd_sma_rsi.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/functions/technical_analysis/rsi.py` & `api_master-1.1/polygonsdk/examples/functions/technical_analysis/rsi.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/functions/technical_analysis/support_resistance.py` & `api_master-1.1/polygonsdk/examples/functions/technical_analysis/support_resistance.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/helpers.py` & `api_master-1.1/polygonsdk/examples/helpers.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/realtime_markets/crypto_market.py` & `api_master-1.1/polygonsdk/examples/realtime_markets/crypto_market.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/realtime_markets/discord_market.py` & `api_master-1.1/polygonsdk/examples/realtime_markets/discord_market.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/realtime_markets/forex_market.py` & `api_master-1.1/polygonsdk/examples/realtime_markets/forex_market.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/realtime_markets/indices_market.py` & `api_master-1.1/polygonsdk/examples/realtime_markets/indices_market.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/realtime_markets/options_market.py` & `api_master-1.1/polygonsdk/examples/realtime_markets/options_market.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/simulated_markets/helpers.py` & `api_master-1.1/polygonsdk/examples/simulated_markets/helpers.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/simulated_markets/mock_discord.py` & `api_master-1.1/polygonsdk/examples/simulated_markets/mock_discord.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/simulated_markets/mock_market.py` & `api_master-1.1/polygonsdk/examples/simulated_markets/mock_market.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/simulated_markets/mock_options_market.py` & `api_master-1.1/polygonsdk/examples/simulated_markets/mock_options_market.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/examples/webull_data.py` & `api_master-1.1/polygonsdk/examples/webull_data.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/funcs/get_data.py` & `api_master-1.1/polygonsdk/funcs/get_data.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/funcs/get_latest_crypto_data.py` & `api_master-1.1/polygonsdk/funcs/get_latest_crypto_data.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/funcs/get_latest_forex_data.py` & `api_master-1.1/polygonsdk/funcs/get_latest_forex_data.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/funcs/get_latest_options_data.py` & `api_master-1.1/polygonsdk/funcs/get_latest_options_data.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/funcs/get_latest_ticker_data.py` & `api_master-1.1/polygonsdk/funcs/get_latest_ticker_data.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/funcs/sec_filings.py` & `api_master-1.1/polygonsdk/funcs/sec_filings.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/funcs/webull_examples.py` & `api_master-1.1/polygonsdk/funcs/webull_examples.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/myconfig.py` & `api_master-1.1/polygonsdk/myconfig.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/discord_sdk/discord_sdk.py` & `api_master-1.1/polygonsdk/sdks/discord_sdk/discord_sdk.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/discord_sdk/searching.py` & `api_master-1.1/polygonsdk/sdks/discord_sdk/searching.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/all_attributes.py` & `api_master-1.1/polygonsdk/sdks/examples/all_attributes.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/bollinger_bands.py` & `api_master-1.1/polygonsdk/sdks/examples/bollinger_bands.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/create_option_symbol.py` & `api_master-1.1/polygonsdk/sdks/examples/create_option_symbol.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/ema.py` & `api_master-1.1/polygonsdk/sdks/examples/ema.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/fetch_entire_chain.py` & `api_master-1.1/polygonsdk/sdks/examples/fetch_entire_chain.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/find_gaps.py` & `api_master-1.1/polygonsdk/sdks/examples/find_gaps.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/get_all_options_data.py` & `api_master-1.1/polygonsdk/sdks/examples/get_all_options_data.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/get_ema.py` & `api_master-1.1/polygonsdk/sdks/examples/get_ema.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/get_latest_crypto_data.py` & `api_master-1.1/polygonsdk/sdks/examples/get_latest_crypto_data.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/get_latest_forex_data.py` & `api_master-1.1/polygonsdk/sdks/examples/get_latest_forex_data.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/get_latest_ticker_data.py` & `api_master-1.1/polygonsdk/sdks/examples/get_latest_ticker_data.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/get_macd.py` & `api_master-1.1/polygonsdk/sdks/examples/get_macd.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/get_pivot_points.py` & `api_master-1.1/polygonsdk/sdks/examples/get_pivot_points.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/get_rsi.py` & `api_master-1.1/polygonsdk/sdks/examples/get_rsi.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/get_sma.py` & `api_master-1.1/polygonsdk/sdks/examples/get_sma.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/latest_news.py` & `api_master-1.1/polygonsdk/sdks/examples/latest_news.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/option_quote.py` & `api_master-1.1/polygonsdk/sdks/examples/option_quote.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/option_trades.py` & `api_master-1.1/polygonsdk/sdks/examples/option_trades.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/plot_aggs.py` & `api_master-1.1/polygonsdk/sdks/examples/plot_aggs.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/plot_macd.py` & `api_master-1.1/polygonsdk/sdks/examples/plot_macd.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/plot_option_aggs.py` & `api_master-1.1/polygonsdk/sdks/examples/plot_option_aggs.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/realtime_markets/crypto_market.py` & `api_master-1.1/polygonsdk/sdks/examples/realtime_markets/crypto_market.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/realtime_markets/forex_market.py` & `api_master-1.1/polygonsdk/sdks/examples/realtime_markets/forex_market.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/realtime_markets/indices_market.py` & `api_master-1.1/polygonsdk/sdks/examples/realtime_markets/indices_market.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/realtime_markets/options_market.py` & `api_master-1.1/polygonsdk/sdks/examples/realtime_markets/options_market.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/scanner_example.py` & `api_master-1.1/polygonsdk/sdks/examples/scanner_example.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/simulated_markets/helpers.py` & `api_master-1.1/polygonsdk/sdks/examples/simulated_markets/helpers.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/simulated_markets/mock_market.py` & `api_master-1.1/polygonsdk/sdks/examples/simulated_markets/mock_market.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/simulated_markets/mock_options_market.py` & `api_master-1.1/polygonsdk/sdks/examples/simulated_markets/mock_options_market.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/stock_aggregates.py` & `api_master-1.1/polygonsdk/sdks/examples/stock_aggregates.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/examples/support_resistance.py` & `api_master-1.1/polygonsdk/sdks/examples/support_resistance.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/fudstop_sdk/fudstop_sdk.py` & `api_master-1.1/polygonsdk/sdks/fudstop_sdk/fudstop_sdk.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+import sys
+import os
+
+# Get the directory path of the polygonsdkmaster package
+package_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
+sys.path.append(package_dir)
+
 from datetime import datetime
 import asyncio
 from .option_vol_totals import OptionVolumeTotals
 import pandas as pd
 import aiohttp
 from cfg import YOUR_NASDAQ_KEY
 from io import StringIO
```

### Comparing `api_master-1.0/polygonsdk/sdks/fudstop_sdk/gaps.py` & `api_master-1.1/polygonsdk/sdks/fudstop_sdk/gaps.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+import sys
+import os
+
+# Get the directory path of the polygonsdkmaster package
+package_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
+sys.path.append(package_dir)
+
 def find_gaps(o, h, l, c, t):
     gap_ups = []
     gap_downs = []
 
     for i in range(1, len(o)):
         if o[i] > c[i-1]:  # Check if the opening price is greater than the previous high price
             gap_ups.append(i)
```

### Comparing `api_master-1.0/polygonsdk/sdks/helpers/conditions.py` & `api_master-1.1/polygonsdk/sdks/helpers/conditions.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/helpers/helpers.py` & `api_master-1.1/polygonsdk/sdks/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/models/maps.py` & `api_master-1.1/polygonsdk/sdks/models/maps.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/models/test_events.py` & `api_master-1.1/polygonsdk/sdks/models/test_events.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/polygon_sdk/__init__.py` & `api_master-1.1/polygonsdk/sdks/polygon_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/polygon_sdk/aggregates.py` & `api_master-1.1/polygonsdk/sdks/polygon_sdk/aggregates.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/polygon_sdk/async_options_sdk.py` & `api_master-1.1/polygonsdk/sdks/polygon_sdk/async_options_sdk.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/polygon_sdk/async_polygon_sdk.py` & `api_master-1.1/polygonsdk/sdks/polygon_sdk/async_polygon_sdk.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/polygon_sdk/company_info.py` & `api_master-1.1/polygonsdk/sdks/polygon_sdk/company_info.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/polygon_sdk/daily_open_close.py` & `api_master-1.1/polygonsdk/sdks/polygon_sdk/daily_open_close.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/polygon_sdk/financials.py` & `api_master-1.1/polygonsdk/sdks/polygon_sdk/financials.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/polygon_sdk/forex_crypto.py` & `api_master-1.1/polygonsdk/sdks/polygon_sdk/forex_crypto.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/polygon_sdk/get_all_options.py` & `api_master-1.1/polygonsdk/sdks/polygon_sdk/get_all_options.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/polygon_sdk/indices_snapshot.py` & `api_master-1.1/polygonsdk/sdks/polygon_sdk/indices_snapshot.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/polygon_sdk/logo.py` & `api_master-1.1/polygonsdk/sdks/polygon_sdk/logo.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/polygon_sdk/mapping_dicts.py` & `api_master-1.1/polygonsdk/sdks/polygon_sdk/mapping_dicts.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/polygon_sdk/models.py` & `api_master-1.1/polygonsdk/sdks/polygon_sdk/models.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/polygon_sdk/news.py` & `api_master-1.1/polygonsdk/sdks/polygon_sdk/news.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/polygon_sdk/option_aggs.py` & `api_master-1.1/polygonsdk/sdks/polygon_sdk/option_aggs.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/polygon_sdk/option_quote.py` & `api_master-1.1/polygonsdk/sdks/polygon_sdk/option_quote.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/polygon_sdk/option_snapshot.py` & `api_master-1.1/polygonsdk/sdks/polygon_sdk/option_snapshot.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/polygon_sdk/option_trades.py` & `api_master-1.1/polygonsdk/sdks/polygon_sdk/option_trades.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/polygon_sdk/pivot_points.py` & `api_master-1.1/polygonsdk/sdks/polygon_sdk/pivot_points.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/polygon_sdk/quote.py` & `api_master-1.1/polygonsdk/sdks/polygon_sdk/quote.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/polygon_sdk/snapshot.py` & `api_master-1.1/polygonsdk/sdks/polygon_sdk/snapshot.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/polygon_sdk/technical_conditions.py` & `api_master-1.1/polygonsdk/sdks/polygon_sdk/technical_conditions.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/polygon_sdk/tickernews.py` & `api_master-1.1/polygonsdk/sdks/polygon_sdk/tickernews.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/stocksera_sdk/borrowed.py` & `api_master-1.1/polygonsdk/sdks/stocksera_sdk/borrowed.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/stocksera_sdk/earnings.py` & `api_master-1.1/polygonsdk/sdks/stocksera_sdk/earnings.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/stocksera_sdk/stocksera_sdk.py` & `api_master-1.1/polygonsdk/sdks/stocksera_sdk/stocksera_sdk.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/stocksera_sdk/treasury.py` & `api_master-1.1/polygonsdk/sdks/stocksera_sdk/treasury.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/terminals/crypto/menu.py` & `api_master-1.1/polygonsdk/sdks/terminals/crypto/menu.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/webull_sdk/calendar.py` & `api_master-1.1/polygonsdk/sdks/webull_sdk/calendar.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/webull_sdk/capitalflow.py` & `api_master-1.1/polygonsdk/sdks/webull_sdk/capitalflow.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/webull_sdk/cost_distribution.py` & `api_master-1.1/polygonsdk/sdks/webull_sdk/cost_distribution.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/webull_sdk/derivative_query.py` & `api_master-1.1/polygonsdk/sdks/webull_sdk/derivative_query.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/webull_sdk/etf_finder.py` & `api_master-1.1/polygonsdk/sdks/webull_sdk/etf_finder.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/webull_sdk/events.py` & `api_master-1.1/polygonsdk/sdks/webull_sdk/events.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/webull_sdk/financial_statement.py` & `api_master-1.1/polygonsdk/sdks/webull_sdk/financial_statement.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/webull_sdk/forecast.py` & `api_master-1.1/polygonsdk/sdks/webull_sdk/forecast.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/webull_sdk/institutional_holdings.py` & `api_master-1.1/polygonsdk/sdks/webull_sdk/institutional_holdings.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/webull_sdk/manage.py` & `api_master-1.1/polygonsdk/sdks/webull_sdk/manage.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/webull_sdk/news.py` & `api_master-1.1/polygonsdk/sdks/webull_sdk/news.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/webull_sdk/top_gainers.py` & `api_master-1.1/polygonsdk/sdks/webull_sdk/top_gainers.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/webull_sdk/top_options.py` & `api_master-1.1/polygonsdk/sdks/webull_sdk/top_options.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/webull_sdk/webull_data.py` & `api_master-1.1/polygonsdk/sdks/webull_sdk/webull_data.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/sdks/webull_sdk/webull_sdk.py` & `api_master-1.1/polygonsdk/sdks/webull_sdk/webull_sdk.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/static/py/commands.py` & `api_master-1.1/polygonsdk/static/py/commands.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/static/py/snippets.py` & `api_master-1.1/polygonsdk/static/py/snippets.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/polygonsdk/test.py` & `api_master-1.1/polygonsdk/test.py`

 * *Files identical despite different names*

### Comparing `api_master-1.0/setup.py` & `api_master-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='api_master',
-    version='1.0',
+    version='1.1',
     author='Chuck Dustin',
     author_email='chuckdustin12@gmail.com',
     description='Utilize several market-data APIs in production-ready format for real-time and simulated market analysis.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/your-username/your-package-repo',
     packages=find_packages(),
```

