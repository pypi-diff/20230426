# Comparing `tmp/pgx-0.5.2.tar.gz` & `tmp/pgx-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgx-0.5.2.tar", last modified: Tue Apr 25 11:29:39 2023, max compression
+gzip compressed data, was "pgx-0.5.3.tar", last modified: Wed Apr 26 02:23:28 2023, max compression
```

## Comparing `pgx-0.5.2.tar` & `pgx-0.5.3.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.533492 pgx-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 11:29:27.000000 pgx-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-04-25 11:29:39.533492 pgx-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-04-25 11:29:27.000000 pgx-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.493492 pgx-0.5.2/pgx/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.497492 pgx-0.5.2/pgx/_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_mahjong/_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_mahjong/_hand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_mahjong/_meld.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_mahjong/_shanten.py
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_mahjong/_yaku.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.501492 pgx-0.5.2/pgx/_src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/api_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/chess_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.509492 pgx-0.5.2/pgx/_src/dwg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/animalshogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/hex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.513492 pgx-0.5.2/pgx/_src/dwg/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.521492 pgx-0.5.2/pgx/_src/dwg/images/chess/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/bBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/bKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/bKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/bPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/bQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/bRook.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/wBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/wKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/wKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/wPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/wQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/wRook.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.525492 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/1p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/2p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/3p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/4p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/5p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/6p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/7p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/8p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/9p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/b.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/gd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/oya.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/rd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/shogi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)    22783 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    18349 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)    37279 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29096 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/connect_four.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.525492 pgx-0.5.2/pgx/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/experimental/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/experimental/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/experimental/pettingzoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/experimental/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/experimental/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/experimental/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/leduc_holdem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.529492 pgx-0.5.2/pgx/minatar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/minatar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12583 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/minatar/asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/minatar/breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8476 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/minatar/freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    25972 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/minatar/seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9839 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/minatar/space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/minatar/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)    20421 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/tic_tac_toe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12491 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.493492 pgx-0.5.2/pgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-04-25 11:29:39.000000 pgx-0.5.2/pgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-25 11:29:39.000000 pgx-0.5.2/pgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:29:39.000000 pgx-0.5.2/pgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-25 11:29:39.000000 pgx-0.5.2/pgx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 11:29:39.000000 pgx-0.5.2/pgx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-25 11:29:28.000000 pgx-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 11:29:39.533492 pgx-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-25 11:29:28.000000 pgx-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.533492 pgx-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/minatar_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)    17462 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)    61896 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29755 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    39645 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_go.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22436 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_tic_tac_toe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.324855 pgx-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 02:23:18.000000 pgx-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-04-26 02:23:28.324855 pgx-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-04-26 02:23:18.000000 pgx-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.308855 pgx-0.5.3/pgx/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-26 02:23:18.000000 pgx-0.5.3/pgx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.312855 pgx-0.5.3/pgx/_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:18.000000 pgx-0.5.3/pgx/_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-26 02:23:18.000000 pgx-0.5.3/pgx/_mahjong/_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-26 02:23:18.000000 pgx-0.5.3/pgx/_mahjong/_hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-04-26 02:23:18.000000 pgx-0.5.3/pgx/_mahjong/_meld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-26 02:23:18.000000 pgx-0.5.3/pgx/_mahjong/_shanten.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-04-26 02:23:18.000000 pgx-0.5.3/pgx/_mahjong/_yaku.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.312855 pgx-0.5.3/pgx/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/api_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/chess_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.316855 pgx-0.5.3/pgx/_src/dwg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/animalshogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/hex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.316855 pgx-0.5.3/pgx/_src/dwg/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.316855 pgx-0.5.3/pgx/_src/dwg/images/chess/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/bBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/bKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/bKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/bPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/bQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/bRook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/wBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/wKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/wKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/wPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/wQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/chess/wRook.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.320855 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/1p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/2p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/3p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/4p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/5p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/6p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/7p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/8p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/9p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/gd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/oya.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/rd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/dwg/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/shogi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22783 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/_src/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18349 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37279 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29096 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/connect_four.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.320855 pgx-0.5.3/pgx/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/experimental/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/experimental/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/experimental/pettingzoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/experimental/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/experimental/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/experimental/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/leduc_holdem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.320855 pgx-0.5.3/pgx/minatar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/minatar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/minatar/asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/minatar/breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/minatar/freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26088 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/minatar/seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/minatar/space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/minatar/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20421 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/tic_tac_toe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12491 2023-04-26 02:23:19.000000 pgx-0.5.3/pgx/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.312855 pgx-0.5.3/pgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-04-26 02:23:28.000000 pgx-0.5.3/pgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-26 02:23:28.000000 pgx-0.5.3/pgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 02:23:28.000000 pgx-0.5.3/pgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-26 02:23:28.000000 pgx-0.5.3/pgx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 02:23:28.000000 pgx-0.5.3/pgx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-26 02:23:19.000000 pgx-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 02:23:28.324855 pgx-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-26 02:23:19.000000 pgx-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:28.324855 pgx-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/minatar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17462 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61896 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29755 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39645 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22436 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-04-26 02:23:19.000000 pgx-0.5.3/tests/test_tic_tac_toe.py
```

### Comparing `pgx-0.5.2/LICENSE` & `pgx-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/PKG-INFO` & `pgx-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgx
-Version: 0.5.2
+Version: 0.5.3
 Summary: GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)
 Home-page: https://github.com/sotetsuk/pgx
 Author: Sotetsu KOYAMADA
 Author-email: sotetsu.koyamada@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pgx Version: 0.5.2 Summary: GPU/TPU-accelerated
+Metadata-Version: 2.1 Name: pgx Version: 0.5.3 Summary: GPU/TPU-accelerated
 parallel game simulators for reinforcement learning (RL) Home-page: https://
 github.com/sotetsuk/pgx Author: Sotetsu KOYAMADA Author-email:
 sotetsu.koyamada@gmail.com Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown License-
 File: LICENSE [![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/
 badge.svg)](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
```

### Comparing `pgx-0.5.2/README.md` & `pgx-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_mahjong/_hand.py` & `pgx-0.5.3/pgx/_mahjong/_hand.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_mahjong/_meld.py` & `pgx-0.5.3/pgx/_mahjong/_meld.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_mahjong/_shanten.py` & `pgx-0.5.3/pgx/_mahjong/_shanten.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_mahjong/_yaku.py` & `pgx-0.5.3/pgx/_mahjong/_yaku.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/api_test.py` & `pgx-0.5.3/pgx/_src/api_test.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/chess_utils.py` & `pgx-0.5.3/pgx/_src/chess_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/animalshogi.py` & `pgx-0.5.3/pgx/_src/dwg/animalshogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/backgammon.py` & `pgx-0.5.3/pgx/_src/dwg/backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/bridge_bidding.py` & `pgx-0.5.3/pgx/_src/dwg/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/chess.py` & `pgx-0.5.3/pgx/_src/dwg/chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/connect_four.py` & `pgx-0.5.3/pgx/_src/dwg/connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/go.py` & `pgx-0.5.3/pgx/_src/dwg/go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/hex.py` & `pgx-0.5.3/pgx/_src/dwg/hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/chess/LICENSE` & `pgx-0.5.3/pgx/_src/dwg/images/chess/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/chess/bBishop.svg` & `pgx-0.5.3/pgx/_src/dwg/images/chess/bBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/chess/bKing.svg` & `pgx-0.5.3/pgx/_src/dwg/images/chess/bKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/chess/bKnight.svg` & `pgx-0.5.3/pgx/_src/dwg/images/chess/bKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/chess/bPawn.svg` & `pgx-0.5.3/pgx/_src/dwg/images/chess/bPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/chess/bQueen.svg` & `pgx-0.5.3/pgx/_src/dwg/images/chess/bQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/chess/bRook.svg` & `pgx-0.5.3/pgx/_src/dwg/images/chess/bRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/chess/wBishop.svg` & `pgx-0.5.3/pgx/_src/dwg/images/chess/wBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/chess/wKing.svg` & `pgx-0.5.3/pgx/_src/dwg/images/chess/wKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/chess/wKnight.svg` & `pgx-0.5.3/pgx/_src/dwg/images/chess/wKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/chess/wPawn.svg` & `pgx-0.5.3/pgx/_src/dwg/images/chess/wPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/chess/wQueen.svg` & `pgx-0.5.3/pgx/_src/dwg/images/chess/wQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/chess/wRook.svg` & `pgx-0.5.3/pgx/_src/dwg/images/chess/wRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/1p.svg` & `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/1p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg` & `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/2p.svg` & `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/2p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg` & `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/3p.svg` & `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/3p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg` & `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/4p.svg` & `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/4p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg` & `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/5p.svg` & `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/5p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg` & `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/6p.svg` & `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/6p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg` & `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/7p.svg` & `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/7p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg` & `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/8p.svg` & `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/8p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg` & `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/9p.svg` & `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/9p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg` & `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/b.svg` & `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/b.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/gd.svg` & `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/gd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/oya.svg` & `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/oya.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/rd.svg` & `pgx-0.5.3/pgx/_src/dwg/images/sparrow_mahjong/rd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/kuhn_poker.py` & `pgx-0.5.3/pgx/_src/dwg/kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/leduc_holdem.py` & `pgx-0.5.3/pgx/_src/dwg/leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/othello.py` & `pgx-0.5.3/pgx/_src/dwg/othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/play2048.py` & `pgx-0.5.3/pgx/_src/dwg/play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/shogi.py` & `pgx-0.5.3/pgx/_src/dwg/shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/sparrow_mahjong.py` & `pgx-0.5.3/pgx/_src/dwg/sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/dwg/tictactoe.py` & `pgx-0.5.3/pgx/_src/dwg/tictactoe.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/shogi_utils.py` & `pgx-0.5.3/pgx/_src/shogi_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/struct.py` & `pgx-0.5.3/pgx/_src/struct.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/_src/visualizer.py` & `pgx-0.5.3/pgx/_src/visualizer.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/animal_shogi.py` & `pgx-0.5.3/pgx/animal_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/backgammon.py` & `pgx-0.5.3/pgx/backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/bridge_bidding.py` & `pgx-0.5.3/pgx/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/chess.py` & `pgx-0.5.3/pgx/chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/connect_four.py` & `pgx-0.5.3/pgx/connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/experimental/bridge_bidding.py` & `pgx-0.5.3/pgx/experimental/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/experimental/gym.py` & `pgx-0.5.3/pgx/experimental/gym.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/experimental/pettingzoo.py` & `pgx-0.5.3/pgx/experimental/pettingzoo.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/experimental/visualize.py` & `pgx-0.5.3/pgx/experimental/visualize.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/experimental/wrappers.py` & `pgx-0.5.3/pgx/experimental/wrappers.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/go.py` & `pgx-0.5.3/pgx/go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/hex.py` & `pgx-0.5.3/pgx/hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/kuhn_poker.py` & `pgx-0.5.3/pgx/kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/leduc_holdem.py` & `pgx-0.5.3/pgx/leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/minatar/asterix.py` & `pgx-0.5.3/pgx/minatar/asterix.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((10, 10, 4), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
-    legal_action_mask: jnp.ndarray = jnp.ones(6, dtype=jnp.bool_)
+    legal_action_mask: jnp.ndarray = jnp.ones(5, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- MinAtar Asterix specific ---
     _player_x: jnp.ndarray = jnp.array(5, dtype=jnp.int32)
     _player_y: jnp.ndarray = jnp.array(5, dtype=jnp.int32)
     _entities: jnp.ndarray = jnp.ones((8, 4), dtype=jnp.int32) * INF
     _shot_timer: jnp.ndarray = jnp.ones(0, dtype=jnp.int32)
@@ -74,30 +74,41 @@
         visualize_minatar(self, filename)
 
 
 class MinAtarAsterix(v1.Env):
     def __init__(
         self,
         *,
-        minatar_version: Literal["v0", "v1"] = "v1",
+        use_minimal_action_set: bool = True,
         sticky_action_prob: float = 0.1,
     ):
         super().__init__()
-        self.minatar_version: Literal["v0", "v1"] = minatar_version
+        self.use_minimal_action_set = use_minimal_action_set
         self.sticky_action_prob: float = sticky_action_prob
+        self.minimal_action_set = jnp.int32([0, 1, 2, 3, 4])
+        self.legal_action_mask = jnp.ones(6, dtype=jnp.bool_)
+        if self.use_minimal_action_set:
+            self.legal_action_mask = jnp.ones(
+                self.minimal_action_set.shape[0], dtype=jnp.bool_
+            )
 
     def _init(self, key: jax.random.KeyArray) -> State:
-        return State(_rng_key=key)  # type: ignore
+        state = State()
+        state = state.replace(legal_action_mask=self.legal_action_mask)  # type: ignore
+        return state  # type: ignore
 
     def _step(self, state: v1.State, action) -> State:
         assert isinstance(state, State)
-        state = _step(
-            state, action, sticky_action_prob=self.sticky_action_prob
+        state = state.replace(legal_action_mask=self.legal_action_mask)  # type: ignore
+        action = jax.lax.select(
+            self.use_minimal_action_set,
+            self.minimal_action_set[action],
+            action,
         )
-        return state.replace(terminated=state._terminal)  # type: ignore
+        return _step(state, action, sticky_action_prob=self.sticky_action_prob)  # type: ignore
 
     def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state)
 
     @property
     def id(self) -> v1.EnvId:
@@ -160,28 +171,14 @@
 def _step_det(
     state: State,
     action: jnp.ndarray,
     lr,
     is_gold,
     slot,
 ):
-    return jax.lax.cond(
-        state._terminal,
-        lambda: state.replace(_last_action=action, reward=jnp.zeros_like(state.reward)),  # type: ignore
-        lambda: _step_det_at_non_terminal(state, action, lr, is_gold, slot),
-    )
-
-
-def _step_det_at_non_terminal(
-    state: State,
-    action: jnp.ndarray,
-    lr: bool,
-    is_gold: bool,
-    slot: int,
-):
     ramping: bool = True
     r = jnp.float32(0)
 
     # Spawn enemy if timer is up
     entities, spawn_timer = jax.lax.cond(
         state._spawn_timer == 0,
         lambda: (
@@ -270,16 +267,18 @@
             state._ramp_timer,
             state._ramp_index,
         ),
     )
     state = state.replace(_spawn_speed=spawn_speed, _move_speed=move_speed, _ramp_timer=ramp_timer, _ramp_index=ramp_index)  # type: ignore
 
     state = state.replace(  # type: ignore
-        reward=r[jnp.newaxis], _last_action=action  # 1-d array
-    )  # type: ignore
+        reward=r[jnp.newaxis],
+        _last_action=action,  # 1-d array
+        terminated=terminal,
+    )
     return state
 
 
 # Spawn a new enemy or treasure at a random location with random direction (if all rows are filled do nothing)
 def _spawn_entity(entities, lr, is_gold, slot):
     x = jax.lax.cond(lr == 1, lambda: 0, lambda: 9)
     new_entities = entities
```

### Comparing `pgx-0.5.2/pgx/minatar/breakout.py` & `pgx-0.5.3/pgx/minatar/breakout.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((10, 10, 4), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
-    legal_action_mask: jnp.ndarray = jnp.ones(6, dtype=jnp.bool_)
+    legal_action_mask: jnp.ndarray = jnp.ones(3, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- MinAtar Breakout specific ---
     _ball_y: jnp.ndarray = THREE
     _ball_x: jnp.ndarray = ZERO
     _ball_dir: jnp.ndarray = TWO
     _pos: jnp.ndarray = FOUR
@@ -75,30 +75,41 @@
         visualize_minatar(self, filename)
 
 
 class MinAtarBreakout(v1.Env):
     def __init__(
         self,
         *,
-        minatar_version: Literal["v0", "v1"] = "v1",
+        use_minimal_action_set: bool = True,
         sticky_action_prob: float = 0.1,
     ):
         super().__init__()
-        self.minatar_version: Literal["v0", "v1"] = minatar_version
+        self.use_minimal_action_set = use_minimal_action_set
         self.sticky_action_prob: float = sticky_action_prob
+        self.minimal_action_set = jnp.int32([0, 1, 3])
+        self.legal_action_mask = jnp.ones(6, dtype=jnp.bool_)
+        if self.use_minimal_action_set:
+            self.legal_action_mask = jnp.ones(
+                self.minimal_action_set.shape[0], dtype=jnp.bool_
+            )
 
     def _init(self, key: jax.random.KeyArray) -> State:
-        return _init(key)  # type: ignore
+        state = _init(rng=key)  # type: ignore
+        state = state.replace(legal_action_mask=self.legal_action_mask)  # type: ignore
+        return state  # type: ignore
 
     def _step(self, state: v1.State, action) -> State:
         assert isinstance(state, State)
-        state = _step(
-            state, action, sticky_action_prob=self.sticky_action_prob
+        state = state.replace(legal_action_mask=self.legal_action_mask)  # type: ignore
+        action = jax.lax.select(
+            self.use_minimal_action_set,
+            self.minimal_action_set[action],
+            action,
         )
-        return state.replace(terminated=state._terminal)  # type: ignore
+        return _step(state, action, sticky_action_prob=self.sticky_action_prob)  # type: ignore
 
     def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state)
 
     @property
     def id(self) -> v1.EnvId:
@@ -131,22 +142,14 @@
 
 def _init(rng: jnp.ndarray) -> State:
     ball_start = jax.random.choice(rng, 2)
     return _init_det(ball_start=ball_start)
 
 
 def _step_det(state: State, action: jnp.ndarray):
-    return jax.lax.cond(
-        state._terminal,
-        lambda: state.replace(_last_action=action, reward=jnp.zeros_like(state.reward)),  # type: ignore
-        lambda: _step_det_at_non_terminal(state, action),
-    )
-
-
-def _step_det_at_non_terminal(state: State, action: jnp.ndarray):
     ball_y = state._ball_y
     ball_x = state._ball_x
     ball_dir = state._ball_dir
     pos = state._pos
     brick_map = state._brick_map
     strike = state._strike
     terminal = state._terminal
@@ -202,14 +205,15 @@
         _brick_map=brick_map,
         _strike=strike,
         _last_x=last_x,
         _last_y=last_y,
         _terminal=terminal,
         _last_action=action,
         reward=r[jnp.newaxis],
+        terminated=terminal,
     )
     return state
 
 
 def _apply_action(pos, action):
     pos = jax.lax.cond(
         action == 1, lambda: jax.lax.max(ZERO, pos - ONE), lambda: pos
```

### Comparing `pgx-0.5.2/pgx/minatar/freeway.py` & `pgx-0.5.3/pgx/minatar/freeway.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((10, 10, 7), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
-    legal_action_mask: jnp.ndarray = jnp.ones(6, dtype=jnp.bool_)
+    legal_action_mask: jnp.ndarray = jnp.ones(3, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- MinAtar Freeway specific ---
     _cars: jnp.ndarray = jnp.zeros((8, 4), dtype=jnp.int32)
     _pos: jnp.ndarray = jnp.array(9, dtype=jnp.int32)
     _move_timer: jnp.ndarray = jnp.array(player_speed, dtype=jnp.int32)
     _terminate_timer: jnp.ndarray = jnp.array(time_limit, dtype=jnp.int32)
@@ -65,30 +65,41 @@
         visualize_minatar(self, filename)
 
 
 class MinAtarFreeway(v1.Env):
     def __init__(
         self,
         *,
-        minatar_version: Literal["v0", "v1"] = "v1",
+        use_minimal_action_set: bool = True,
         sticky_action_prob: float = 0.1,
     ):
         super().__init__()
-        self.minatar_version: Literal["v0", "v1"] = minatar_version
+        self.use_minimal_action_set = use_minimal_action_set
         self.sticky_action_prob: float = sticky_action_prob
+        self.minimal_action_set = jnp.int32([0, 2, 4])
+        self.legal_action_mask = jnp.ones(6, dtype=jnp.bool_)
+        if self.use_minimal_action_set:
+            self.legal_action_mask = jnp.ones(
+                self.minimal_action_set.shape[0], dtype=jnp.bool_
+            )
 
     def _init(self, key: jax.random.KeyArray) -> State:
-        return _init(key)  # type: ignore
+        state = _init(rng=key)  # type: ignore
+        state = state.replace(legal_action_mask=self.legal_action_mask)  # type: ignore
+        return state  # type: ignore
 
     def _step(self, state: v1.State, action) -> State:
         assert isinstance(state, State)
-        state = _step(
-            state, action, sticky_action_prob=self.sticky_action_prob
+        state = state.replace(legal_action_mask=self.legal_action_mask)  # type: ignore
+        action = jax.lax.select(
+            self.use_minimal_action_set,
+            self.minimal_action_set[action],
+            action,
         )
-        return state.replace(terminated=state._terminal)  # type: ignore
+        return _step(state, action, sticky_action_prob=self.sticky_action_prob)  # type: ignore
 
     def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state)
 
     @property
     def id(self) -> v1.EnvId:
@@ -127,28 +138,14 @@
 
 def _step_det(
     state: State,
     action: jnp.ndarray,
     speeds: jnp.ndarray,
     directions: jnp.ndarray,
 ):
-    return jax.lax.cond(
-        state._terminal,
-        lambda: state.replace(_last_action=action, reward=jnp.zeros_like(state.reward)),  # type: ignore
-        lambda: _step_det_at_non_terminal(state, action, speeds, directions),
-    )
-
-
-def _step_det_at_non_terminal(
-    state: State,
-    action: jnp.ndarray,
-    speeds: jnp.ndarray,
-    directions: jnp.ndarray,
-):
-
     cars = state._cars
     pos = state._pos
     move_timer = state._move_timer
     terminate_timer = state._terminate_timer
     terminal = state._terminal
     last_action = action
 
@@ -189,14 +186,15 @@
         _cars=cars,
         _pos=pos,
         _move_timer=move_timer,
         _terminate_timer=terminate_timer,
         _terminal=terminal,
         _last_action=last_action,
         reward=r[jnp.newaxis],
+        terminated=terminal,
     )
 
     return next_state
 
 
 def _update_cars(pos, cars):
     def _update_stopped_car(pos, car):
```

### Comparing `pgx-0.5.2/pgx/minatar/seaquest.py` & `pgx-0.5.3/pgx/minatar/seaquest.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,30 +86,41 @@
         visualize_minatar(self, filename)
 
 
 class MinAtarSeaquest(v1.Env):
     def __init__(
         self,
         *,
-        minatar_version: Literal["v0", "v1"] = "v1",
+        use_minimal_action_set: bool = True,
         sticky_action_prob: float = 0.1,
     ):
         super().__init__()
-        self.minatar_version: Literal["v0", "v1"] = minatar_version
+        self.use_minimal_action_set = use_minimal_action_set
         self.sticky_action_prob: float = sticky_action_prob
+        self.minimal_action_set = jnp.int32([0, 1, 2, 3, 4, 5])
+        self.legal_action_mask = jnp.ones(6, dtype=jnp.bool_)
+        if self.use_minimal_action_set:
+            self.legal_action_mask = jnp.ones(
+                self.minimal_action_set.shape[0], dtype=jnp.bool_
+            )
 
     def _init(self, key: jax.random.KeyArray) -> State:
-        return _init_det()
+        state = State()
+        state = state.replace(legal_action_mask=self.legal_action_mask)  # type: ignore
+        return state
 
     def _step(self, state: v1.State, action) -> State:
         assert isinstance(state, State)
-        state = _step(
-            state, action, sticky_action_prob=self.sticky_action_prob
+        state = state.replace(legal_action_mask=self.legal_action_mask)  # type: ignore
+        action = jax.lax.select(
+            self.use_minimal_action_set,
+            self.minimal_action_set[action],
+            action,
         )
-        return state.replace(terminated=state._terminal)  # type: ignore
+        return _step(state, action, sticky_action_prob=self.sticky_action_prob)  # type: ignore
 
     def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state)
 
     @property
     def id(self) -> v1.EnvId:
@@ -156,32 +167,14 @@
     action: jnp.ndarray,
     enemy_lr,
     is_sub,
     enemy_y,
     diver_lr,
     diver_y,
 ):
-    return lax.cond(
-        state._terminal,
-        lambda: state.replace(_last_action=action, reward=jnp.zeros_like(state.reward)),  # type: ignore
-        lambda: _step_det_at_non_terminal(
-            state, action, enemy_lr, is_sub, enemy_y, diver_lr, diver_y
-        ),
-    )
-
-
-def _step_det_at_non_terminal(
-    state: State,
-    action: jnp.ndarray,
-    enemy_lr,
-    is_sub,
-    enemy_y,
-    diver_lr,
-    diver_y,
-):
     ramping = TRUE
 
     oxygen = state._oxygen
     diver_count = state._diver_count
     sub_x = state._sub_x
     sub_y = state._sub_y
     sub_or = state._sub_or
@@ -301,14 +294,15 @@
         _move_speed=move_speed,
         _ramp_index=ramp_index,
         _shot_timer=shot_timer,
         _surface=surface,
         _terminal=terminal,
         _last_action=action,
         reward=r[jnp.newaxis],
+        terminated=terminal,
     )
     return state
 
 
 def find_ix(arr):
     ix = lax.while_loop(lambda i: arr[i][0] != -1, lambda i: i + 1, 0)
     return ix
@@ -356,24 +350,24 @@
         lambda: (_f_bullets, e, FALSE),
     )
     return _f_bullets, e, removed
 
 
 def _update_friendly_bullets(f_bullets, e_subs, e_fish, r):
     def _remove(j, _f_bullets, _e_subs, _e_fish, _r):
-        _f_bullets, _e_fish, removed = _update_by_f_bullets_hit(
+        _f_bullets, _e_fish, fish_removed = _update_by_f_bullets_hit(
             j, _f_bullets, _e_fish
         )
-        _r += removed
-        _f_bullets, _e_subs, removed = lax.cond(
-            removed,
-            lambda: (_f_bullets, _e_subs, removed),
+        _r += fish_removed
+        _f_bullets, _e_subs, sub_removed = lax.cond(
+            fish_removed,
+            lambda: (_f_bullets, _e_subs, FALSE),
             lambda: _update_by_f_bullets_hit(j, _f_bullets, _e_subs),
         )
-        _r += removed
+        _r += sub_removed
         return _f_bullets, _e_subs, _e_fish, _r
 
     def _update_each(i, x):
         _f_bullets, _e_subs, _e_fish, _r = x
         j = 5 - i - 1
         is_filled = _is_filled(_f_bullets[j])
         _f_bullets = lax.cond(
@@ -846,11 +840,7 @@
             lambda: set_divers(_obs, state._divers[i]),
             lambda: _obs,
         ),
         obs,
     )
 
     return obs
-
-
-def _init_det() -> State:
-    return State()
```

### Comparing `pgx-0.5.2/pgx/minatar/space_invaders.py` & `pgx-0.5.3/pgx/minatar/space_invaders.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((10, 10, 6), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
-    legal_action_mask: jnp.ndarray = jnp.ones(6, dtype=jnp.bool_)
+    legal_action_mask: jnp.ndarray = jnp.ones(4, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- MinAtar SpaceInvaders specific ---
     _pos: jnp.ndarray = jnp.int32(5)
     _f_bullet_map: jnp.ndarray = jnp.zeros((10, 10), dtype=jnp.bool_)
     _e_bullet_map: jnp.ndarray = jnp.zeros((10, 10), dtype=jnp.bool_)
     _alien_map: jnp.ndarray = (
@@ -75,30 +75,41 @@
         visualize_minatar(self, filename)
 
 
 class MinAtarSpaceInvaders(v1.Env):
     def __init__(
         self,
         *,
-        minatar_version: Literal["v0", "v1"] = "v1",
+        use_minimal_action_set: bool = True,
         sticky_action_prob: float = 0.1,
     ):
         super().__init__()
-        self.minatar_version: Literal["v0", "v1"] = minatar_version
+        self.use_minimal_action_set = use_minimal_action_set
         self.sticky_action_prob: float = sticky_action_prob
+        self.minimal_action_set = jnp.int32([0, 1, 3, 5])
+        self.legal_action_mask = jnp.ones(6, dtype=jnp.bool_)
+        if self.use_minimal_action_set:
+            self.legal_action_mask = jnp.ones(
+                self.minimal_action_set.shape[0], dtype=jnp.bool_
+            )
 
     def _init(self, key: jax.random.KeyArray) -> State:
-        return _init_det()
+        state = State()
+        state = state.replace(legal_action_mask=self.legal_action_mask)  # type: ignore
+        return state  # type: ignore
 
     def _step(self, state: v1.State, action) -> State:
         assert isinstance(state, State)
-        state = _step(
-            state, action, sticky_action_prob=self.sticky_action_prob
+        state = state.replace(legal_action_mask=self.legal_action_mask)  # type: ignore
+        action = jax.lax.select(
+            self.use_minimal_action_set,
+            self.minimal_action_set[action],
+            action,
         )
-        return state.replace(terminated=state._terminal)  # type: ignore
+        return _step(state, action, sticky_action_prob=self.sticky_action_prob)  # type: ignore
 
     def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state)
 
     @property
     def id(self) -> v1.EnvId:
@@ -152,25 +163,14 @@
     return obs
 
 
 def _step_det(
     state: State,
     action: jnp.ndarray,
 ):
-    return lax.cond(
-        state._terminal,
-        lambda: state.replace(_last_action=action, reward=jnp.zeros_like(state.reward)),  # type: ignore
-        lambda: _step_det_at_non_terminal(state, action),
-    )
-
-
-def _step_det_at_non_terminal(
-    state: State,
-    action: jnp.ndarray,
-):
     r = jnp.float32(0)
 
     pos = state._pos
     f_bullet_map = state._f_bullet_map
     e_bullet_map = state._e_bullet_map
     alien_map = state._alien_map
     alien_dir = state._alien_dir
@@ -253,14 +253,15 @@
         _alien_move_timer=alien_move_timer,
         _alien_shot_timer=alien_shot_timer,
         _ramp_index=ramp_index,
         _shot_timer=shot_timer,
         _terminal=terminal,
         _last_action=action,
         reward=r[jnp.newaxis],
+        terminated=terminal,
     )
 
 
 def _resole_action(pos, f_bullet_map, shot_timer, action):
     f_bullet_map = lax.cond(
         (action == 5) & (shot_timer == 0),
         lambda: f_bullet_map.at[9, pos].set(TRUE),
@@ -312,11 +313,7 @@
         lambda: jnp.roll(alien_map, 1, axis=0),
         lambda: jnp.roll(alien_map, alien_dir, axis=1),
     )
     terminal = lax.cond(
         alien_map[9, pos], lambda: jnp.bool_(True), lambda: terminal
     )
     return alien_move_timer, alien_map, alien_dir, terminal
-
-
-def _init_det() -> State:
-    return State()
```

### Comparing `pgx-0.5.2/pgx/minatar/utils.py` & `pgx-0.5.3/pgx/minatar/utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/othello.py` & `pgx-0.5.3/pgx/othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/play2048.py` & `pgx-0.5.3/pgx/play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/shogi.py` & `pgx-0.5.3/pgx/shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/sparrow_mahjong.py` & `pgx-0.5.3/pgx/sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/tic_tac_toe.py` & `pgx-0.5.3/pgx/tic_tac_toe.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx/v1.py` & `pgx-0.5.3/pgx/v1.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/pgx.egg-info/PKG-INFO` & `pgx-0.5.3/pgx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgx
-Version: 0.5.2
+Version: 0.5.3
 Summary: GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)
 Home-page: https://github.com/sotetsuk/pgx
 Author: Sotetsu KOYAMADA
 Author-email: sotetsu.koyamada@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pgx Version: 0.5.2 Summary: GPU/TPU-accelerated
+Metadata-Version: 2.1 Name: pgx Version: 0.5.3 Summary: GPU/TPU-accelerated
 parallel game simulators for reinforcement learning (RL) Home-page: https://
 github.com/sotetsuk/pgx Author: Sotetsu KOYAMADA Author-email:
 sotetsu.koyamada@gmail.com Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown License-
 File: LICENSE [![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/
 badge.svg)](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
```

### Comparing `pgx-0.5.2/pgx.egg-info/SOURCES.txt` & `pgx-0.5.3/pgx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/setup.py` & `pgx-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="pgx",
-    version="0.5.2",
+    version="0.5.3",
     description="GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/sotetsuk/pgx",
     author="Sotetsu KOYAMADA",
     author_email="sotetsu.koyamada@gmail.com",
     keywords="",
```

### Comparing `pgx-0.5.2/tests/minatar_utils.py` & `pgx-0.5.3/tests/minatar_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/tests/test_animal_shogi.py` & `pgx-0.5.3/tests/test_animal_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/tests/test_asterix.py` & `pgx-0.5.3/tests/test_asterix.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,25 +58,16 @@
                 minatar2pgx(s, asterix.State),
                 a,
                 lr,
                 is_gold,
                 slot,
             )
             assert_states(s_next, pgx2minatar(s_next_pgx, state_keys))
-
-        # check terminal state
-        s = extract_state(env, state_keys)
-        a = random.randrange(num_actions)
-        r, done = env.act(a)
-        lr, is_gold, slot = env.env.lr, env.env.is_gold, env.env.slot
-        s_next = extract_state(env, state_keys)
-        s_next_pgx = _step_det(
-            minatar2pgx(s, asterix.State), a, lr, is_gold, slot
-        )
-        assert_states(s_next, pgx2minatar(s_next_pgx, state_keys))
+            assert r == s_next_pgx.reward[0]
+            assert done == s_next_pgx.terminated
 
 
 def test_observe():
     env = Environment("asterix", sticky_action_prob=0.0)
     num_actions = env.num_actions()
 
     N = 10
@@ -100,11 +91,21 @@
         obs_pgx = _observe(s_pgx)
         assert jnp.allclose(
             env.state(),
             obs_pgx,
         )
 
 
+def test_minimal_action_set():
+    import pgx
+    env = pgx.make("minatar/asterix")
+    assert env.num_actions == 5
+    state = jax.jit(env.init)(jax.random.PRNGKey(0))
+    assert state.legal_action_mask.shape == (5,)
+    state = jax.jit(env.step)(state, 0)
+    assert state.legal_action_mask.shape == (5,)
+
+
 def test_api():
     import pgx
     env = pgx.make("minatar/asterix")
     pgx.api_test(env, 10)
```

### Comparing `pgx-0.5.2/tests/test_backgammon.py` & `pgx-0.5.3/tests/test_backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/tests/test_breakout.py` & `pgx-0.5.3/tests/test_breakout.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,37 +23,29 @@
 _init_det = jax.jit(breakout._init_det)
 observe = jax.jit(breakout._observe)
 
 def test_step_det():
     env = Environment("breakout", sticky_action_prob=0.0)
     num_actions = env.num_actions()
 
-    N = 100
-    for _ in range(N):
+    N = 1000
+    for n in range(N):
         env.reset()
         done = False
         while not done:
             s = extract_state(env, state_keys)
             a = random.randrange(num_actions)
             r, done = env.act(a)
             s_next = extract_state(env, state_keys)
             s_next_pgx = _step_det(
                 minatar2pgx(s, breakout.State), a
             )
             assert_states(s_next, pgx2minatar(s_next_pgx, state_keys))
-
-        # check terminal state
-        s = extract_state(env, state_keys)
-        a = random.randrange(num_actions)
-        r, done = env.act(a)
-        s_next = extract_state(env, state_keys)
-        s_next_pgx = _step_det(
-            minatar2pgx(s, breakout.State), a
-        )
-        assert_states(s_next, pgx2minatar(s_next_pgx, state_keys))
+            assert r == s_next_pgx.reward[0]
+            assert done == s_next_pgx.terminated
 
 
 def test_init_det():
     env = Environment("breakout", sticky_action_prob=0.0)
     N = 1
     for _ in range(N):
         env.reset()
@@ -88,11 +80,21 @@
         obs_pgx = observe(s_pgx)
         assert jnp.allclose(
             env.state(),
             obs_pgx,
         )
 
 
+def test_minimal_action_set():
+    import pgx
+    env = pgx.make("minatar/breakout")
+    assert env.num_actions == 3
+    state = jax.jit(env.init)(jax.random.PRNGKey(0))
+    assert state.legal_action_mask.shape == (3,)
+    state = jax.jit(env.step)(state, 0)
+    assert state.legal_action_mask.shape == (3,)
+
+
 def test_api():
     import pgx
     env = pgx.make("minatar/breakout")
     pgx.api_test(env, 10)
```

### Comparing `pgx-0.5.2/tests/test_bridge_bidding.py` & `pgx-0.5.3/tests/test_bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/tests/test_chess.py` & `pgx-0.5.3/tests/test_chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/tests/test_connect_four.py` & `pgx-0.5.3/tests/test_connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/tests/test_freeway.py` & `pgx-0.5.3/tests/test_freeway.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,28 +40,16 @@
             s_next_pgx = _step_det(
                 minatar2pgx(s, freeway.State),
                 a,
                 speeds,
                 directions,
             )
             assert_states(s_next, pgx2minatar(s_next_pgx, state_keys))
-
-        # check terminal state
-        s = extract_state(env, state_keys)
-        a = random.randrange(num_actions)
-        r, done = env.act(a)
-        # extract random variables
-        speeds, directions = jnp.array(env.env.speeds), jnp.array(
-            env.env.directions
-        )
-        s_next = extract_state(env, state_keys)
-        s_next_pgx = _step_det(
-            minatar2pgx(s, freeway.State), a, speeds, directions
-        )
-        assert_states(s_next, pgx2minatar(s_next_pgx, state_keys))
+            assert r == s_next_pgx.reward[0]
+            assert done == s_next_pgx.terminated
 
 
 def test_init_det():
     env = Environment("freeway", sticky_action_prob=0.0)
     N = 10
     for _ in range(N):
         env.reset()
@@ -98,11 +86,21 @@
         obs_pgx = _to_obs(s_pgx)
         assert jnp.allclose(
             env.state(),
             obs_pgx,
         )
 
 
+def test_minimal_action_set():
+    import pgx
+    env = pgx.make("minatar/freeway")
+    assert env.num_actions == 3
+    state = jax.jit(env.init)(jax.random.PRNGKey(0))
+    assert state.legal_action_mask.shape == (3,)
+    state = jax.jit(env.step)(state, 0)
+    assert state.legal_action_mask.shape == (3,)
+
+
 def test_api():
     import pgx
     env = pgx.make("minatar/freeway")
     pgx.api_test(env, 10)
```

### Comparing `pgx-0.5.2/tests/test_go.py` & `pgx-0.5.3/tests/test_go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/tests/test_hex.py` & `pgx-0.5.3/tests/test_hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/tests/test_kuhn_poker.py` & `pgx-0.5.3/tests/test_kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/tests/test_leduc_holdem.py` & `pgx-0.5.3/tests/test_leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/tests/test_mahjong.py` & `pgx-0.5.3/tests/test_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/tests/test_othello.py` & `pgx-0.5.3/tests/test_othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/tests/test_play2048.py` & `pgx-0.5.3/tests/test_play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/tests/test_seaquest.py` & `pgx-0.5.3/tests/test_seaquest.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     "shot_timer",
     "surface",
     "terminal",
     "last_action",
 }
 
 _step_det = jax.jit(seaquest._step_det)
-_init_det = jax.jit(seaquest._init_det)
 observe = jax.jit(seaquest._observe)
 
 
 def test_step_det():
     env = Environment("seaquest", sticky_action_prob=0.0)
     num_actions = env.num_actions()
 
@@ -61,45 +60,25 @@
                 env.state(),
                 observe(s_next_pgx),
             )
             # if not jnp.allclose(env.state(), observe(s_next_pgx)):
             #     for field in fields(s_next_pgx):
             #         print(str(field.name) + "\n" + str(getattr(s_next_pgx, field.name)) + "\n"  + str(getattr(minatar2pgx(extract_state(env, state_keys), seaquest.MinAtarSeaquestState), field.name)))
             #     assert False
-
-        # check terminal state
-        s = extract_state(env, state_keys)
-        a = random.randrange(num_actions)
-        r, done = env.act(a)
-        enemy_lr, is_sub, enemy_y, diver_lr, diver_y = env.env.enemy_lr, env.env.is_sub, env.env.enemy_y, env.env.diver_lr, env.env.diver_y
-        s_next_pgx = _step_det(
-            minatar2pgx(s, seaquest.State), a,
-            enemy_lr,
-            is_sub,
-            enemy_y,
-            diver_lr,
-            diver_y
-        )
-        assert jnp.allclose(
-            env.state(),
-            observe(s_next_pgx),
-        )
-        # if not jnp.allclose(env.state(), observe(s_next_pgx)):
-        #     for field in fields(s_next_pgx):
-        #         print(str(field.name) + "\n" + str(getattr(s_next_pgx, field.name)) + "\n"  + str(getattr(minatar2pgx(extract_state(env, state_keys), seaquest.MinAtarSeaquestState), field.name)))
-        #     assert False
+            assert r == s_next_pgx.reward[0]
+            assert done == s_next_pgx.terminated
 
 
 def test_init_det():
     env = Environment("seaquest", sticky_action_prob=0.0)
     N = 100
     for _ in range(N):
         env.reset()
         s = extract_state(env, state_keys)
-        s_pgx = _init_det()
+        s_pgx = seaquest.State()
         s_pgx2 = minatar2pgx(s, seaquest.State)
         for field in fields(s_pgx):
             assert jnp.allclose(getattr(s_pgx, field.name), getattr(s_pgx2, field.name))
 
 
 def test_observe():
     env = Environment("seaquest", sticky_action_prob=0.0)
@@ -194,11 +173,21 @@
     # print(state.e_fish)
     print("e_subs")
     print(state._e_subs)
     assert (state._e_bullets[0] == jnp.int32([-1, -1, -1])).all()
     assert (state._e_subs[0] == jnp.int32([6, 6, 0, 2, 0])).all()
 
 
+def test_minimal_action_set():
+    import pgx
+    env = pgx.make("minatar/seaquest")
+    assert env.num_actions == 6
+    state = jax.jit(env.init)(jax.random.PRNGKey(0))
+    assert state.legal_action_mask.shape == (6,)
+    state = jax.jit(env.step)(state, 0)
+    assert state.legal_action_mask.shape == (6,)
+
+
 def test_api():
     import pgx
     env = pgx.make("minatar/seaquest")
     pgx.api_test(env, 10)
```

### Comparing `pgx-0.5.2/tests/test_shogi.py` & `pgx-0.5.3/tests/test_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/tests/test_space_invaders.py` & `pgx-0.5.3/tests/test_space_invaders.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     "shot_timer",
     "terminal",
     "last_action",
 ]
 
 _step_det = jax.jit(space_invaders._step_det)
 _nearest_alien = jax.jit(space_invaders._nearest_alien)
-_init_det = jax.jit(space_invaders._init_det)
 observe = jax.jit(space_invaders._observe)
 
 
 def test_neareset_alien():
     pos: jnp.ndarray = jnp.int32(3)
     alien_map: jnp.ndarray = (
         jnp.zeros((10, 10), dtype=jnp.bool_).at[0:4, 2:8].set(True)
@@ -50,33 +49,25 @@
             r, done = env.act(a)
             s_next = extract_state(env, state_keys)
             s_next_pgx = _step_det(
                 minatar2pgx(s, space_invaders.State),
                 a,
             )
             assert_states(s_next, pgx2minatar(s_next_pgx, state_keys))
-
-        # check terminal state
-        s = extract_state(env, state_keys)
-        a = random.randrange(num_actions)
-        r, done = env.act(a)
-        s_next = extract_state(env, state_keys)
-        s_next_pgx = _step_det(
-            minatar2pgx(s, space_invaders.State), a
-        )
-        assert_states(s_next, pgx2minatar(s_next_pgx, state_keys))
+            assert r == s_next_pgx.reward[0]
+            assert done == s_next_pgx.terminated
 
 
 def test_init_det():
     env = Environment("space_invaders", sticky_action_prob=0.0)
     N = 10
     for _ in range(N):
         env.reset()
         s = extract_state(env, state_keys)
-        s_pgx = _init_det()
+        s_pgx = space_invaders.State()
         assert_states(s, pgx2minatar(s_pgx, state_keys))
 
 
 def test_observe():
     env = Environment("space_invaders", sticky_action_prob=0.0)
     num_actions = env.num_actions()
 
@@ -100,11 +91,20 @@
         s_pgx = minatar2pgx(s, space_invaders.State)
         obs_pgx = observe(s_pgx)
         assert jnp.allclose(
             env.state(),
             obs_pgx,
         )
 
+def test_minimal_action_set():
+    import pgx
+    env = pgx.make("minatar/space_invaders")
+    assert env.num_actions == 4
+    state = jax.jit(env.init)(jax.random.PRNGKey(0))
+    assert state.legal_action_mask.shape == (4,)
+    state = jax.jit(env.step)(state, 0)
+    assert state.legal_action_mask.shape == (4,)
+
 def test_api():
     import pgx
     env = pgx.make("minatar/space_invaders")
     pgx.api_test(env, 10)
```

### Comparing `pgx-0.5.2/tests/test_sparrow_mahjong.py` & `pgx-0.5.3/tests/test_sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.2/tests/test_tic_tac_toe.py` & `pgx-0.5.3/tests/test_tic_tac_toe.py`

 * *Files identical despite different names*

