# Comparing `tmp/cgpmgr-1.3.tar.gz` & `tmp/cgpmgr-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgpmgr-1.3.tar", last modified: Sat Jun  3 09:46:41 2023, max compression
+gzip compressed data, was "cgpmgr-1.4.tar", last modified: Sat Jun 17 13:13:45 2023, max compression
```

## Comparing `cgpmgr-1.3.tar` & `cgpmgr-1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-03 09:46:41.556194 cgpmgr-1.3/
--rw-r--r--   0 pi        (1000) pi        (1000)    11342 2021-09-04 14:18:09.000000 cgpmgr-1.3/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)      307 2023-06-03 09:46:41.546194 cgpmgr-1.3/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     3085 2021-11-01 12:43:53.000000 cgpmgr-1.3/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-03 09:46:41.516194 cgpmgr-1.3/cgpmgr/
--rwxr-xr-x   0 pi        (1000) pi        (1000)       19 2021-09-05 05:17:17.000000 cgpmgr-1.3/cgpmgr/__init__.py
--rwxr-xr-x   0 pi        (1000) pi        (1000)    30353 2023-06-03 09:42:53.000000 cgpmgr-1.3/cgpmgr/cli.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-03 09:46:41.546194 cgpmgr-1.3/cgpmgr.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)      307 2023-06-03 09:46:41.000000 cgpmgr-1.3/cgpmgr.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      241 2023-06-03 09:46:41.000000 cgpmgr-1.3/cgpmgr.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-06-03 09:46:41.000000 cgpmgr-1.3/cgpmgr.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-06-03 09:46:41.000000 cgpmgr-1.3/cgpmgr.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       14 2023-06-03 09:46:41.000000 cgpmgr-1.3/cgpmgr.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        7 2023-06-03 09:46:41.000000 cgpmgr-1.3/cgpmgr.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-06-03 09:46:41.556194 cgpmgr-1.3/setup.cfg
--rwxr-xr-x   0 pi        (1000) pi        (1000)      478 2023-06-03 09:42:53.000000 cgpmgr-1.3/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-17 13:13:45.200005 cgpmgr-1.4/
+-rw-r--r--   0 pi        (1000) pi        (1000)    11342 2021-09-04 14:18:09.000000 cgpmgr-1.4/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)      307 2023-06-17 13:13:45.200005 cgpmgr-1.4/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     2812 2023-06-05 04:58:21.000000 cgpmgr-1.4/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-17 13:13:45.170005 cgpmgr-1.4/cgpmgr/
+-rwxr-xr-x   0 pi        (1000) pi        (1000)       19 2021-09-05 05:17:17.000000 cgpmgr-1.4/cgpmgr/__init__.py
+-rwxr-xr-x   0 pi        (1000) pi        (1000)    30617 2023-06-17 13:11:23.000000 cgpmgr-1.4/cgpmgr/cli.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-17 13:13:45.190005 cgpmgr-1.4/cgpmgr.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)      307 2023-06-17 13:13:45.000000 cgpmgr-1.4/cgpmgr.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      241 2023-06-17 13:13:45.000000 cgpmgr-1.4/cgpmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-06-17 13:13:45.000000 cgpmgr-1.4/cgpmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-06-17 13:13:45.000000 cgpmgr-1.4/cgpmgr.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       14 2023-06-17 13:13:45.000000 cgpmgr-1.4/cgpmgr.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        7 2023-06-17 13:13:45.000000 cgpmgr-1.4/cgpmgr.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-06-17 13:13:45.200005 cgpmgr-1.4/setup.cfg
+-rwxr-xr-x   0 pi        (1000) pi        (1000)      478 2023-06-17 13:11:15.000000 cgpmgr-1.4/setup.py
```

### Comparing `cgpmgr-1.3/LICENSE` & `cgpmgr-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cgpmgr-1.3/README.md` & `cgpmgr-1.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 ## 概要
-Raspberry Pi用電源管理、制御基板「[RPZ-PowerMGR](https://www.indoorcorgielec.com/products/rpz-powermgr/)」コントロールツールです。本ソフトウェアをインストール後にcgpmgrコマンドが使用できるようになり、以下のことが可能になります。
+Raspberry Pi / Jetson Nano用電源管理、制御基板「[RPZ-PowerMGR](https://www.indoorcorgielec.com/products/rpz-powermgr/)」コントロールツールです。本ソフトウェアをインストール後にcgpmgrコマンドが使用できるようになり、以下のことが可能になります。
 
 - RPZ-PowerMGR基板の設定の変更
 - 電源ON/OFFするスケジュール日時の追加、削除、インポート、エクスポート
-- Raspberry Pi本体の消費電流の測定、エクスポート
+- Raspberry Pi / Jetson本体の消費電流の測定、エクスポート
 - RPZ-PowerMGR基板のファームウェア更新
 
-Raspberry Piは大変便利な小型コンピューターです。しかし、電源まわりには課題もあります。Raspberry Piを使っていて、次のような悩みを持ったことはありませんか？
+Raspberry PiやJetson Nanoは便利なシングルボードコンピュータですが、次のような悩みを持ったことはありませんか？
 
 - USBケーブルを抜き差ししないと電源をON、OFFできない
 - ネットワークや遠隔から電源をOFFできない
 - インターネットに繋がっていないと時刻がずれる
 - 決まった時間だけ起動して消費電力を抑えたい
 - モバイルバッテリーで長時間運用したい
 - どれくらい電力を消費しているか知りたい
 
 電源管理、省電力運用に必要な機能を網羅している「[RPZ-PowerMGR](https://www.indoorcorgielec.com/products/rpz-powermgr/)」拡張基板を使えばこれらの問題を全て解決できます。
 
 ## 必要環境
-ハードウェア: 40ピン端子を持つRaspberry Piシリーズ \
-OS: Raspberry Pi OS
+### ハードウェア
+
+- 40ピン端子を持つRaspberry Piシリーズ
+- Jetson Nano
+
+### OS
+- Raspberry Pi OS
+- JetPack4.6
 
 ## 動作確認済モデル
 - Raspberry Pi 4 Model B
 - Raspberry Pi 3 Model B/B+
 - Raspberry Pi Zero W/WH
 - Raspberry Pi Zero
+- Jetson Nano Developer Kit B01
+- Jetson Nano 2GB Developer Kit
 
 ## インストール
 
-以下のコマンドでコントロールツールをインストール/アップグレードできます。具体的なセットアップ手順は[セットアップ(ハードウェア)](https://www.indoorcorgielec.com/products/rpz-powermgr/#%E3%82%BB%E3%83%83%E3%83%88%E3%82%A2%E3%83%83%E3%83%97%E3%83%8F%E3%83%BC%E3%83%89%E3%82%A6%E3%82%A7%E3%82%A2)、[セットアップ(ソフトウェア)](https://www.indoorcorgielec.com/products/rpz-powermgr/#%E3%82%BB%E3%83%83%E3%83%88%E3%82%A2%E3%83%83%E3%83%97%E3%82%BD%E3%83%95%E3%83%88%E3%82%A6%E3%82%A7%E3%82%A2)を参照して下さい。
+以下のコマンドでコントロールツールをインストール/アップグレードできます。取り付けやOSのセットアップ手順は[製品ページ](https://www.indoorcorgielec.com/products/rpz-powermgr/)を参照してください. 
 
 `sudo python3 -m pip install -U cgpmgr`
 
 ## 使い方
 コマンドラインから`cgpmgr -h`を実行することでオプションの解説が表示されます。シチュエーション別の使い方は、以下の解説記事をご参照下さい。
 
 - [スイッチでRaspberry Piの電源ON/OFF](https://www.indoorcorgielec.com/resources/raspberry-pi/rpz-powermgr-switch/)
```

### Comparing `cgpmgr-1.3/cgpmgr/cli.py` & `cgpmgr-1.4/cgpmgr/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Raspberry Pi/Jetson Nano電源管理 拡張基板 RPZ-PowerMGR用コントロールツール
 Indoor Corgi, https://www.indoorcorgielec.com
 GitHub: https://github.com/IndoorCorgi/cgpmgr
-Version 1.3
+Version 1.4
 
 必要環境:
 1) Raspberry Pi OS / Jetson Linux, Python3
 2) I2Cインターフェース
   Raspberry PiでI2Cを有効にする方法
   https://www.indoorcorgielec.com/resources/raspberry-pi/raspberry-pi-i2c/
 3) 電源管理 拡張基板 RPZ-PowerMGR
@@ -43,15 +43,16 @@
              省略するとRepeat(繰り返し). 
   -D <date>  登録するスケジュールの月/日を指定. *か**で全てに一致. 
              日はSun, Mon, Tue, Wed, Thu, Fri, Satで曜日も指定可能. 例)5/10, , 9/Sun, */15. 
   <time>     登録するスケジュールの時:分を指定. *か**で全てに一致. 
              分は*指定不可. 例)21:30, *:45
   on         電源をONするスケジュールを登録する. 
   off        電源をOFFするスケジュールを登録する. 
-  -l <min>   現在からmin分後にスケジュールを登録. 秒は切り上げになる. 1-999の範囲で指定. 
+  -l <min>   現在からmin分後にスケジュールを登録. 秒は切り上げになる. 0-999の範囲で指定. 
+             0を指定すると1分単位で可能な限り早いスケジュールになる. 
              このオプションで登録するとOneTime(1回のみ)になる. 
   -R <num>   指定すると登録済みスケジュールから指定番号のものを削除. 255を指定すると全て削除. 
   -i         スケジュールをcsvファイルから読み出して追加する. 
              省略すると登録済みスケジュールをcsvファイルに保存する.
 
   me         Raspberry Pi/Jetson Nanoの消費電流測定, 結果ログを行うサブコマンド. 
              オプションを指定しないと直近の電流測定値を表示. 
@@ -301,18 +302,22 @@
     if args['off']:
       sch[0] |= 0x40
 
     if args['-o']:
       sch[0] |= 0x80
 
     if args['-l'] != None:
-      if not check_digit('-l', args['-l'], 1, 999):
+      if not check_digit('-l', args['-l'], 0, 999):
         return
       dtrtc = read_rtc()
-      dt = dtrtc + datetime.timedelta(minutes=1 + int(args['-l']))
+      delay = int(args['-l'])
+      if delay == 0:
+        dt = dtrtc + datetime.timedelta(seconds=75)  # 通信, 計算マージン15秒 + 桁繰り上げ用60秒
+      else:
+        dt = dtrtc + datetime.timedelta(minutes=1 + delay)
       sch[0] |= dt.minute | 0x80
       sch[1] = dt.hour
       sch[2] = dt.day
       sch[3] = dt.month
 
     if args['on'] or args['off']:
       sch_count = i2c_read(0x30, 1)[0]  # 登録済みスケジュールの数
```

