# Comparing `tmp/ELiDE-0.14.1.tar.gz` & `tmp/ELiDE-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ELiDE-0.14.1.tar", last modified: Wed Apr 26 21:02:38 2023, max compression
+gzip compressed data, was "dist/ELiDE-0.9.1.tar", last modified: Tue Oct 30 13:40:40 2018, max compression
```

## Comparing `ELiDE-0.14.1.tar` & `ELiDE-0.9.1.tar`

### file list

```diff
@@ -1,124 +1,103 @@
-drwxrwxr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2023-04-26 21:02:38.519867 ELiDE-0.14.1/
-drwxrwxr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2023-04-26 21:02:38.499866 ELiDE-0.14.1/ELiDE/
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      939 2022-09-07 08:44:17.000000 ELiDE-0.14.1/ELiDE/__init__.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      855 2022-09-07 08:44:17.000000 ELiDE-0.14.1/ELiDE/__main__.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    15158 2023-04-15 04:28:39.000000 ELiDE-0.14.1/ELiDE/app.py
-drwxrwxr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2023-04-26 21:02:38.503866 ELiDE-0.14.1/ELiDE/assets/
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)  2119496 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/Symbola.ttf
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    14901 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/polygons-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      320 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/polygons.atlas
-drwxrwxr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2023-04-26 21:02:38.515867 ELiDE-0.14.1/ELiDE/assets/rltiles/
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    21484 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/amulet-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     1347 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/amulet.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     2904 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/arm-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      714 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/arm.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    84744 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/armor-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     5464 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/armor.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    23680 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/base-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     2274 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/base.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     1746 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/beard-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      313 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/beard.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    38209 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/body-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     4282 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/body.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    21662 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/book-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     1463 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/book.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     2782 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/boot-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      593 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/boot.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     2473 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/cloak-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      301 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/cloak.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)   185627 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/dc-mon-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     9587 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/dc-mon.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    38794 2023-04-26 20:55:29.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/dungeon-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    38794 2023-04-16 07:45:29.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/dungeon-0.png~
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     2651 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/dungeon.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     6398 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/floor-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      253 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/floor.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    21295 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/food-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     1571 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/food.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     5147 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/gem-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      434 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/gem.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     3182 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/hair-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      777 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/hair.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    25141 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/hand1-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     5713 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/hand1.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    11800 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/hand2-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     2207 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/hand2.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     8894 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/head-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     2565 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/head.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     5376 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/leg-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      935 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/leg.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    29868 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/misc-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     2196 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/misc.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    10402 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/potion-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      878 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/potion.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     9495 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/ring-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     1355 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/ring.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     4925 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/scroll-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      931 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/scroll.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    14102 2023-04-26 20:55:29.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/wand-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     1472 2023-04-26 20:55:29.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/wand.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    41884 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/weapon-0.png
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     4343 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/rltiles/weapon.atlas
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)  2313664 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/assets/wallpape.jpg
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     1497 2023-01-10 07:38:50.000000 ELiDE-0.14.1/ELiDE/boardscatter.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     1684 2022-09-07 08:44:17.000000 ELiDE-0.14.1/ELiDE/boardview.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    14153 2023-04-26 20:55:29.000000 ELiDE-0.14.1/ELiDE/calendar.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    34176 2023-03-25 06:04:13.000000 ELiDE-0.14.1/ELiDE/card.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     9214 2023-04-08 01:18:43.000000 ELiDE-0.14.1/ELiDE/charmenu.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     4175 2023-04-21 09:37:00.000000 ELiDE-0.14.1/ELiDE/charsview.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     4346 2023-04-26 20:55:29.000000 ELiDE-0.14.1/ELiDE/collide.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     9845 2023-04-26 20:55:29.000000 ELiDE-0.14.1/ELiDE/dialog.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     3094 2022-09-07 08:44:17.000000 ELiDE-0.14.1/ELiDE/dummy.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     8832 2023-04-26 20:55:29.000000 ELiDE-0.14.1/ELiDE/game.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     2268 2022-09-07 08:44:17.000000 ELiDE-0.14.1/ELiDE/gen.py
-drwxrwxr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2023-04-26 21:02:38.515867 ELiDE-0.14.1/ELiDE/graph/
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      869 2023-01-10 07:38:50.000000 ELiDE-0.14.1/ELiDE/graph/__init__.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    21110 2023-03-31 15:40:56.000000 ELiDE-0.14.1/ELiDE/graph/arrow.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    34262 2023-04-26 20:55:29.000000 ELiDE-0.14.1/ELiDE/graph/board.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     1830 2023-01-10 07:38:50.000000 ELiDE-0.14.1/ELiDE/graph/pawn.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     5030 2023-01-10 07:38:50.000000 ELiDE-0.14.1/ELiDE/graph/spot.py
-drwxrwxr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2023-04-26 21:02:38.515867 ELiDE-0.14.1/ELiDE/grid/
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)        0 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/grid/__init__.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     8699 2023-04-26 20:55:29.000000 ELiDE-0.14.1/ELiDE/grid/board.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     3400 2022-09-07 08:44:17.000000 ELiDE-0.14.1/ELiDE/imagestackproxy.py
-drwxrwxr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2023-04-26 21:02:38.515867 ELiDE-0.14.1/ELiDE/kivygarden/
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)        0 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/kivygarden/__init__.py
-drwxrwxr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2023-04-26 21:02:38.515867 ELiDE-0.14.1/ELiDE/kivygarden/texturestack/
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    10503 2022-11-29 14:42:22.000000 ELiDE-0.14.1/ELiDE/kivygarden/texturestack/__init__.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     1128 2022-09-07 08:44:17.000000 ELiDE-0.14.1/ELiDE/kwlist.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     5573 2023-03-29 12:53:26.000000 ELiDE-0.14.1/ELiDE/menu.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     5781 2022-09-07 08:44:17.000000 ELiDE-0.14.1/ELiDE/pallet.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     3890 2022-09-07 08:44:17.000000 ELiDE-0.14.1/ELiDE/pawn.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    24301 2023-04-26 20:55:29.000000 ELiDE-0.14.1/ELiDE/pawnspot.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    16181 2023-04-22 13:43:38.000000 ELiDE-0.14.1/ELiDE/rulesview.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    23546 2023-04-08 01:10:03.000000 ELiDE-0.14.1/ELiDE/screen.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     6240 2022-09-07 08:44:17.000000 ELiDE-0.14.1/ELiDE/spritebuilder.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     8450 2022-09-07 08:44:17.000000 ELiDE-0.14.1/ELiDE/statcfg.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     4953 2023-04-08 01:08:46.000000 ELiDE-0.14.1/ELiDE/statlist.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     4395 2023-04-08 01:10:03.000000 ELiDE-0.14.1/ELiDE/stepper.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    20685 2023-04-08 01:10:03.000000 ELiDE-0.14.1/ELiDE/stores.py
-drwxrwxr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2023-04-26 21:02:38.519867 ELiDE-0.14.1/ELiDE/tests/
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)        0 2021-07-09 20:18:57.000000 ELiDE-0.14.1/ELiDE/tests/__init__.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     2639 2022-09-07 08:44:17.000000 ELiDE-0.14.1/ELiDE/tests/test_character_switcher.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     7787 2023-04-26 20:55:29.000000 ELiDE-0.14.1/ELiDE/tests/test_graphboard.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     2941 2023-02-05 02:49:42.000000 ELiDE-0.14.1/ELiDE/tests/test_gridboard.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     1825 2023-04-05 01:47:09.000000 ELiDE-0.14.1/ELiDE/tests/test_python_editor.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     9828 2023-03-20 00:54:21.000000 ELiDE-0.14.1/ELiDE/tests/test_rule_builder.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     6511 2023-03-12 00:22:48.000000 ELiDE-0.14.1/ELiDE/tests/test_screen.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     1725 2022-09-07 08:44:17.000000 ELiDE-0.14.1/ELiDE/tests/test_sprite_builder.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     2070 2022-09-07 08:44:17.000000 ELiDE-0.14.1/ELiDE/tests/test_strings_editor.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     3415 2023-04-05 01:43:33.000000 ELiDE-0.14.1/ELiDE/tests/util.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    10381 2022-09-07 08:44:17.000000 ELiDE-0.14.1/ELiDE/timestream.py
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     3614 2022-09-07 08:44:17.000000 ELiDE-0.14.1/ELiDE/util.py
-drwxrwxr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2023-04-26 21:02:38.499866 ELiDE-0.14.1/ELiDE.egg-info/
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    56420 2023-04-26 21:02:38.000000 ELiDE-0.14.1/ELiDE.egg-info/PKG-INFO
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)     2988 2023-04-26 21:02:38.000000 ELiDE-0.14.1/ELiDE.egg-info/SOURCES.txt
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)        1 2023-04-26 21:02:38.000000 ELiDE-0.14.1/ELiDE.egg-info/dependency_links.txt
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)       59 2023-04-26 21:02:38.000000 ELiDE-0.14.1/ELiDE.egg-info/requires.txt
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)        6 2023-04-26 21:02:38.000000 ELiDE-0.14.1/ELiDE.egg-info/top_level.txt
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    34523 2023-02-01 14:04:01.000000 ELiDE-0.14.1/LICENSE
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      141 2022-09-07 08:44:17.000000 ELiDE-0.14.1/MANIFEST.in
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    56420 2023-04-26 21:02:38.519867 ELiDE-0.14.1/PKG-INFO
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    15976 2023-04-26 20:55:29.000000 ELiDE-0.14.1/README.md
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      951 2023-04-26 20:57:35.000000 ELiDE-0.14.1/pyproject.toml
--rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)       38 2023-04-26 21:02:38.519867 ELiDE-0.14.1/setup.cfg
+drwxr-xr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2018-10-30 13:40:40.000000 ELiDE-0.9.1/
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     1613 2018-10-30 13:39:29.000000 ELiDE-0.9.1/setup.py
+drwxr-xr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2018-10-30 13:40:40.000000 ELiDE-0.9.1/ELiDE/
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    21518 2018-10-30 02:15:25.000000 ELiDE-0.9.1/ELiDE/stores.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     5254 2018-10-19 11:50:10.000000 ELiDE-0.9.1/ELiDE/collide.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    11161 2018-10-19 11:50:10.000000 ELiDE-0.9.1/ELiDE/dialog.py
+drwxr-xr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2018-10-30 13:40:40.000000 ELiDE-0.9.1/ELiDE/assets/
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)  2313664 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/wallpape.jpg
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     6392 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/marsh_davies_island_fg-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)  2119496 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/Symbola.ttf
+-rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      493 2018-05-04 18:39:38.000000 ELiDE-0.9.1/ELiDE/assets/orb.png
+-rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)      320 2018-05-27 12:15:22.000000 ELiDE-0.9.1/ELiDE/assets/polygons.atlas
+drwxr-xr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2018-10-30 13:40:40.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     1347 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/amulet.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     2274 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/base.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     8894 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/head-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     3182 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/hair-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     2904 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/arm-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)      301 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/cloak.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     4343 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/weapon.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)      593 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/boot.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    11800 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/hand2-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)      777 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/hair.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)   185627 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/dc-mon-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)      931 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/scroll.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     1571 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/food.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     1355 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/ring.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     1472 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/wand.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     5147 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/gem-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    38794 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/dungeon-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     2207 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/hand2.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     1746 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/beard-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     2196 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/misc.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    84744 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/armor-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     4925 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/scroll-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     4282 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/body.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     2565 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/head.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)      313 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/beard.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    14102 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/wand-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     5713 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/hand1.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     2782 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/boot-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     9587 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/dc-mon.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     5376 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/leg-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)      434 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/gem.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    25141 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/hand1-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    21484 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/amulet-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)      935 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/leg.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     1463 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/book.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     9495 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/ring-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    10402 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/potion-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)      878 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/potion.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    29868 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/misc-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    21662 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/book-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     5464 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/armor.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)      714 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/arm.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    38209 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/body-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    41884 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/weapon-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    23680 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/base-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     2473 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/cloak-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     2651 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/dungeon.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    21295 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/rltiles/food-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)      271 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/marsh_davies_island_fg.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     1896 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/marsh_davies_island_bg.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    11241 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/marsh_davies_crypt-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    52980 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/marsh_davies_island_bg-0.png
+-rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    14901 2018-05-27 12:15:22.000000 ELiDE-0.9.1/ELiDE/assets/polygons-0.png
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     1062 2017-06-17 19:48:16.000000 ELiDE-0.9.1/ELiDE/assets/marsh_davies_crypt.atlas
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     3502 2018-10-19 11:50:10.000000 ELiDE-0.9.1/ELiDE/dummy.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     4284 2018-10-19 11:50:10.000000 ELiDE-0.9.1/ELiDE/charsview.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    17137 2018-10-19 12:06:53.000000 ELiDE-0.9.1/ELiDE/screen.py
+drwxr-xr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2018-10-30 13:40:40.000000 ELiDE-0.9.1/ELiDE/kivygarden/
+drwxr-xr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2018-10-30 13:40:40.000000 ELiDE-0.9.1/ELiDE/kivygarden/texturestack/
+-rw-rw-r--   0 sanotehu  (1000) sanotehu  (1000)    12136 2018-09-19 23:12:29.000000 ELiDE-0.9.1/ELiDE/kivygarden/texturestack/__init__.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)      929 2018-10-19 11:50:10.000000 ELiDE-0.9.1/ELiDE/__main__.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    15523 2018-10-19 12:06:53.000000 ELiDE-0.9.1/ELiDE/statlist.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     5679 2018-10-19 11:50:10.000000 ELiDE-0.9.1/ELiDE/pallet.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    10072 2018-10-19 11:50:10.000000 ELiDE-0.9.1/ELiDE/game.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     1269 2018-10-19 11:50:10.000000 ELiDE-0.9.1/ELiDE/kwlist.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    18214 2018-10-19 12:06:53.000000 ELiDE-0.9.1/ELiDE/rulesview.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     8876 2018-10-19 12:06:53.000000 ELiDE-0.9.1/ELiDE/charmenu.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     4237 2018-10-19 11:50:10.000000 ELiDE-0.9.1/ELiDE/util.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     2139 2018-10-19 11:50:10.000000 ELiDE-0.9.1/ELiDE/menu.py
+drwxr-xr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2018-10-30 13:40:40.000000 ELiDE-0.9.1/ELiDE/board/
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    22017 2018-10-19 11:50:10.000000 ELiDE-0.9.1/ELiDE/board/arrow.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     3454 2018-10-19 11:50:10.000000 ELiDE-0.9.1/ELiDE/board/spot.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    37781 2018-10-19 12:06:53.000000 ELiDE-0.9.1/ELiDE/board/board.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     5054 2018-10-19 12:06:53.000000 ELiDE-0.9.1/ELiDE/board/pawn.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)      946 2018-10-19 11:50:10.000000 ELiDE-0.9.1/ELiDE/board/__init__.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    10730 2018-10-19 11:50:10.000000 ELiDE-0.9.1/ELiDE/board/pawnspot.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)      962 2018-10-19 11:50:10.000000 ELiDE-0.9.1/ELiDE/__init__.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    13778 2018-10-19 11:50:10.000000 ELiDE-0.9.1/ELiDE/app.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     6844 2018-10-19 11:50:10.000000 ELiDE-0.9.1/ELiDE/spritebuilder.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    10105 2018-10-19 11:50:10.000000 ELiDE-0.9.1/ELiDE/statcfg.py
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)    41610 2018-10-19 11:50:10.000000 ELiDE-0.9.1/ELiDE/card.py
+drwxr-xr-x   0 sanotehu  (1000) sanotehu  (1000)        0 2018-10-30 13:40:40.000000 ELiDE-0.9.1/ELiDE.egg-info/
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)       40 2018-10-30 13:40:40.000000 ELiDE-0.9.1/ELiDE.egg-info/requires.txt
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)        6 2018-10-30 13:40:40.000000 ELiDE-0.9.1/ELiDE.egg-info/top_level.txt
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)     2621 2018-10-30 13:40:40.000000 ELiDE-0.9.1/ELiDE.egg-info/SOURCES.txt
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)        1 2018-10-30 02:15:45.000000 ELiDE-0.9.1/ELiDE.egg-info/not-zip-safe
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)      178 2018-10-30 13:40:40.000000 ELiDE-0.9.1/ELiDE.egg-info/PKG-INFO
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)        1 2018-10-30 13:40:40.000000 ELiDE-0.9.1/ELiDE.egg-info/dependency_links.txt
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)      178 2018-10-30 13:40:40.000000 ELiDE-0.9.1/PKG-INFO
+-rw-r--r--   0 sanotehu  (1000) sanotehu  (1000)       38 2018-10-30 13:40:40.000000 ELiDE-0.9.1/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ELiDE-0.14.1/ELiDE/__init__.py` & `ELiDE-0.9.1/ELiDE/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 # This file is part of ELiDE, frontend to LiSE, a framework for life simulation games.
 # Copyright (c) Zachary Spector, public@zacharyspector.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, version 3.
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from kivy.resources import resource_add_path
-from . import calendar
-
 resource_add_path(__path__[0] + '/assets')
 
-__all__ = [
-	'graph', 'app', 'card', 'dialog', 'game', 'spritebuilder', 'calendar'
-]
+__all__ = ['board', 'app', 'card', 'dialog', 'game', 'spritebuilder']
```

### Comparing `ELiDE-0.14.1/ELiDE/__main__.py` & `ELiDE-0.9.1/ELiDE/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # This file is part of ELiDE, frontend to LiSE, a framework for life simulation games.
 # Copyright (c) Zachary Spector, public@zacharyspector.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, version 3.
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
 def elide():
-	from ELiDE.app import ELiDEApp
-	app = ELiDEApp()
-	app.run()
-
+    from ELiDE.app import ELiDEApp
+    app = ELiDEApp()
+    app.run()
 
 if __name__ == '__main__':
-	elide()
+    elide()
```

### Comparing `ELiDE-0.14.1/ELiDE/assets/Symbola.ttf` & `ELiDE-0.9.1/ELiDE/assets/Symbola.ttf`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/polygons-0.png` & `ELiDE-0.9.1/ELiDE/assets/polygons-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/amulet-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/amulet-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/amulet.atlas` & `ELiDE-0.9.1/ELiDE/assets/rltiles/amulet.atlas`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/arm-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/arm-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/arm.atlas` & `ELiDE-0.9.1/ELiDE/assets/rltiles/arm.atlas`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/armor-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/armor-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/armor.atlas` & `ELiDE-0.9.1/ELiDE/assets/rltiles/armor.atlas`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/base-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/base-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/base.atlas` & `ELiDE-0.9.1/ELiDE/assets/rltiles/base.atlas`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/beard-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/beard-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/body-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/body-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/body.atlas` & `ELiDE-0.9.1/ELiDE/assets/rltiles/body.atlas`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/book-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/book-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/book.atlas` & `ELiDE-0.9.1/ELiDE/assets/rltiles/book.atlas`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/boot-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/boot-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/boot.atlas` & `ELiDE-0.9.1/ELiDE/assets/rltiles/boot.atlas`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/cloak-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/cloak-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/dc-mon-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/dc-mon-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/dc-mon.atlas` & `ELiDE-0.9.1/ELiDE/assets/rltiles/dc-mon.atlas`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/dungeon-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/dungeon-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/dungeon.atlas` & `ELiDE-0.9.1/ELiDE/assets/rltiles/dungeon.atlas`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/food-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/food-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/food.atlas` & `ELiDE-0.9.1/ELiDE/assets/rltiles/food.atlas`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/gem-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/gem-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/hair-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/hair-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/hair.atlas` & `ELiDE-0.9.1/ELiDE/assets/rltiles/hair.atlas`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/hand1-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/hand1-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/hand1.atlas` & `ELiDE-0.9.1/ELiDE/assets/rltiles/hand1.atlas`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/hand2-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/hand2-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/hand2.atlas` & `ELiDE-0.9.1/ELiDE/assets/rltiles/hand2.atlas`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/head-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/head-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/head.atlas` & `ELiDE-0.9.1/ELiDE/assets/rltiles/head.atlas`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/leg-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/leg-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/leg.atlas` & `ELiDE-0.9.1/ELiDE/assets/rltiles/leg.atlas`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/misc-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/misc-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/misc.atlas` & `ELiDE-0.9.1/ELiDE/assets/rltiles/misc.atlas`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/potion-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/potion-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/potion.atlas` & `ELiDE-0.9.1/ELiDE/assets/rltiles/potion.atlas`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/ring-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/ring-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/ring.atlas` & `ELiDE-0.9.1/ELiDE/assets/rltiles/ring.atlas`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/scroll-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/scroll-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/scroll.atlas` & `ELiDE-0.9.1/ELiDE/assets/rltiles/scroll.atlas`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/wand-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/wand-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/wand.atlas` & `ELiDE-0.9.1/ELiDE/assets/rltiles/wand.atlas`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/weapon-0.png` & `ELiDE-0.9.1/ELiDE/assets/rltiles/weapon-0.png`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/rltiles/weapon.atlas` & `ELiDE-0.9.1/ELiDE/assets/rltiles/weapon.atlas`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/assets/wallpape.jpg` & `ELiDE-0.9.1/ELiDE/assets/wallpape.jpg`

 * *Files identical despite different names*

### Comparing `ELiDE-0.14.1/ELiDE/charsview.py` & `ELiDE-0.9.1/ELiDE/charsview.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,143 +1,131 @@
 # This file is part of ELiDE, frontend to LiSE, a framework for life simulation games.
 # Copyright (c) Zachary Spector, public@zacharyspector.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, version 3.
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from functools import partial
 
-from kivy.app import App
 from kivy.clock import Clock
 from kivy.lang import Builder
 from kivy.uix.screenmanager import Screen
 from kivy.uix.recycleview import RecycleView
-from kivy.properties import ListProperty, ObjectProperty, StringProperty, \
- NumericProperty
+from kivy.properties import ListProperty, ObjectProperty, StringProperty
 
-from .stores import RecycleToggleButton
 from .util import SelectableRecycleBoxLayout
 
+
 # TODO: Visual preview
 # TODO: Background image chooser
 
-
 class CharactersRecycleBoxLayout(SelectableRecycleBoxLayout):
-	character_name = StringProperty()
+    character_name = StringProperty()
 
-	def apply_selection(self, index, view, is_selected):
-		super().apply_selection(index, view, is_selected)
-		if is_selected:
-			self.character_name = view.text
+    def apply_selection(self, index, view, is_selected):
+        super().apply_selection(index, view, is_selected)
+        if is_selected:
+            self.character_name = view.text
 
 
 class CharactersView(RecycleView):
-	character_name = StringProperty()
+    character_name = StringProperty()
 
-	def __init__(self, **kwargs):
-		self.i2name = {}
-		self.name2i = {}
-		super().__init__(**kwargs)
+    def __init__(self, **kwargs):
+        self.i2name = {}
+        self.name2i = {}
+        super().__init__(**kwargs)
 
 
 class CharactersScreen(Screen):
-	toggle = ObjectProperty()
-	charsview = ObjectProperty()
-	character_name = StringProperty()
-	wallpaper_path = StringProperty()
-	names = ListProperty()
-	new_board = ObjectProperty()
-	push_character_name = ObjectProperty()
-
-	@property
-	def engine(self):
-		return App.get_running_app().engine
-
-	def new_character(self, name, *args):
-		self.engine.add_character(name)
-		self.ids.newname.text = ''
-		i = len(self.charsview.data)
-		self.charsview.i2name[i] = name
-		self.charsview.name2i[name] = i
-		self.charsview.data.append({'index': i, 'text': name})
-		self.names.append(name)
-		self.new_board(name)
-		self.push_character_name(name)
-
-	def _trigger_new_character(self, name):
-		part = partial(self.new_character, name)
-		if hasattr(self, '_scheduled_new_character'):
-			Clock.unschedule(self._scheduled_new_character)
-		self._scheduled_new_character = Clock.schedule_once(part)
-
-	def _munge_names(self, names):
-		for i, name in enumerate(names):
-			self.charsview.i2name[i] = name
-			self.charsview.name2i[name] = i
-			yield {'index': i, 'text': name}
-
-	def on_names(self, *args):
-		app = App.get_running_app()
-		if not app.character or not self.charsview:
-			Clock.schedule_once(self.on_names, 0)
-			return
-		self.charsview.data = list(self._munge_names(self.names))
-		charname = app.character.name
-		for i, name in enumerate(self.names):
-			if name == charname:
-				self.charsview.children[0].select_node(i)
-				return
-
-	def on_charsview(self, *args):
-		if not self.push_character_name:
-			Clock.schedule_once(self.on_charsview, 0)
-			return
-		self.charsview.bind(character_name=self.setter('character_name'))
-		self.bind(character_name=self.push_character_name)
+    toggle = ObjectProperty()
+    charsview = ObjectProperty()
+    engine = ObjectProperty()
+    character_name = StringProperty()
+    wallpaper_path = StringProperty()
+    names = ListProperty()
+    new_board = ObjectProperty()
+    push_character_name = ObjectProperty()
+
+    def new_character(self, name, *args):
+        self.engine.add_character(name)
+        self.ids.newname.text = ''
+        i = len(self.charsview.data)
+        self.charsview.i2name[i] = name
+        self.charsview.name2i[name] = i
+        self.charsview.data.append({'index': i, 'text': name})
+        self.names.append(name)
+        self.new_board(name)
+        self.push_character_name(name)
+
+    def _trigger_new_character(self, name):
+        part = partial(self.new_character, name)
+        Clock.unschedule(part)
+        Clock.schedule_once(part)
+
+    def _munge_names(self, names):
+        for i, name in enumerate(names):
+            self.charsview.i2name[i] = name
+            self.charsview.name2i[name] = i
+            yield {'index': i, 'text': name}
+
+    def on_names(self, *args):
+        if not self.charsview:
+            Clock.schedule_once(self.on_names, 0)
+            return
+        self.charsview.data = list(self._munge_names(self.names))
+
+    def on_charsview(self, *args):
+        if not self.push_character_name:
+            Clock.schedule_once(self.on_charsview, 0)
+            return
+        self.charsview.bind(character_name=self.setter('character_name'))
+        self.bind(character_name=self.push_character_name)
 
 
 Builder.load_string("""
 #: import resource_find kivy.resources.resource_find
 <CharactersView>:
-	viewclass: 'RecycleToggleButton'
-	character_name: boxl.character_name
-	CharactersRecycleBoxLayout:
-		id: boxl
-		multiselect: False
-		default_size: None, dp(56)
-		default_size_hint: 1, None
-		size_hint_y: None
-		height: self.minimum_height
-		orientation: 'vertical'
+    viewclass: 'RecycleToggleButton'
+    character_name: boxl.character_name
+    CharactersRecycleBoxLayout:
+        id: boxl
+        multiselect: False
+        default_size: None, dp(56)
+        default_size_hint: 1, None
+        size_hint_y: None
+        height: self.minimum_height
+        orientation: 'vertical'
 <CharactersScreen>:
-	name: 'chars'
-	charsview: charsview
-	BoxLayout:
-		id: chars
-		orientation: 'vertical'
-		CharactersView:
-			id: charsview
-			size_hint_y: 0.8
-			character_name: root.character_name
-		TextInput:
-			id: newname
-			size_hint_y: 0.1
-			hint_text: 'New character name'
-			write_tab: False
-			multiline: False
-		Button:
-			text: '+'
-			on_release: root._trigger_new_character(newname.text)
-			size_hint_y: 0.05
-		Button:
-			text: 'Close'
-			on_release: root.toggle()
-			size_hint_y: 0.05
+    name: 'chars'
+    charsview: charsview
+    BoxLayout:
+        id: chars
+        orientation: 'vertical'
+        CharactersView:
+            id: charsview
+            size_hint_y: 0.8
+            character_name: root.character_name
+        TextInput:
+            id: newname
+            size_hint_y: 0.1
+            hint_text: 'New character name'
+            write_tab: False
+            multiline: False
+        Button:
+            text: '+'
+            on_release: root._trigger_new_character(newname.text)
+            size_hint_y: 0.05
+        Button:
+            text: 'Close'
+            on_release: root.toggle()
+            size_hint_y: 0.05
 """)
```

### Comparing `ELiDE-0.14.1/ELiDE/dummy.py` & `ELiDE-0.9.1/ELiDE/dummy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,96 +1,107 @@
 # This file is part of ELiDE, frontend to LiSE, a framework for life simulation games.
 # Copyright (c) Zachary Spector, public@zacharyspector.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, version 3.
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
-from kivy.properties import (NumericProperty, ObjectProperty,
-								ReferenceListProperty, StringProperty)
+from kivy.properties import (
+    NumericProperty,
+    ObjectProperty,
+    ReferenceListProperty,
+    StringProperty
+)
 from kivy.lang import Builder
 from kivy.logger import Logger
 
 from .kivygarden.texturestack import ImageStack
 
 from . import menu  # for kv
 
 
 class Dummy(ImageStack):
-	"""A widget that looks like the ones on the graph, which, when dragged
-	onto the graph, creates one of them.
+    """A widget that looks like the ones on the board, which, when dragged
+    onto the board, creates one of them.
 
-	"""
-	_touch = ObjectProperty(None, allownone=True)
-	name = StringProperty()
-	prefix = StringProperty()
-	num = NumericProperty()
-	x_start = NumericProperty(0)
-	y_start = NumericProperty(0)
-	pos_start = ReferenceListProperty(x_start, y_start)
-	x_down = NumericProperty(0)
-	y_down = NumericProperty(0)
-	pos_down = ReferenceListProperty(x_down, y_down)
-	x_up = NumericProperty(0)
-	y_up = NumericProperty(0)
-	pos_up = ReferenceListProperty(x_up, y_up)
-	x_center_up = NumericProperty(0)
-	y_center_up = NumericProperty(0)
-	center_up = ReferenceListProperty(x_center_up, y_center_up)
-	right_up = NumericProperty(0)
-	top_up = NumericProperty(0)
-
-	def on_paths(self, *args, **kwargs):
-		super().on_paths(*args, **kwargs)
-		Logger.debug("Dummy: {} got paths {}".format(self.name, self.paths))
-
-	def on_touch_down(self, touch):
-		"""If hit, record my starting position, that I may return to it in
-		``on_touch_up`` after creating a real :class:`graph.Spot` or
-		:class:`graph.Pawn` instance.
-
-		"""
-		if not self.collide_point(*touch.pos):
-			return False
-		self.pos_start = self.pos
-		self.pos_down = (self.x - touch.x, self.y - touch.y)
-		touch.grab(self)
-		self._touch = touch
-		return True
-
-	def on_touch_move(self, touch):
-		"""Follow the touch"""
-		if touch is not self._touch:
-			return False
-		self.pos = (touch.x + self.x_down, touch.y + self.y_down)
-		return True
-
-	def on_touch_up(self, touch):
-		"""Return to ``pos_start``, but first, save my current ``pos`` into
-		``pos_up``, so that the layout knows where to put the real
-		:class:`graph.Spot` or :class:`graph.Pawn` instance.
-
-		"""
-		if touch is not self._touch:
-			return False
-		self.pos_up = self.pos
-		self.pos = self.pos_start
-		self._touch = None
-		return True
+    """
+    _touch = ObjectProperty(None, allownone=True)
+    name = StringProperty()
+    prefix = StringProperty()
+    num = NumericProperty()
+    x_start = NumericProperty(0)
+    y_start = NumericProperty(0)
+    pos_start = ReferenceListProperty(x_start, y_start)
+    x_down = NumericProperty(0)
+    y_down = NumericProperty(0)
+    pos_down = ReferenceListProperty(x_down, y_down)
+    x_up = NumericProperty(0)
+    y_up = NumericProperty(0)
+    pos_up = ReferenceListProperty(x_up, y_up)
+    x_center_up = NumericProperty(0)
+    y_center_up = NumericProperty(0)
+    center_up = ReferenceListProperty(x_center_up, y_center_up)
+    right_up = NumericProperty(0)
+    top_up = NumericProperty(0)
+
+    def on_paths(self, *args, **kwargs):
+        super().on_paths(*args, **kwargs)
+        Logger.debug("Dummy: {} got paths {}".format(self.name, self.paths))
+
+    def on_touch_down(self, touch):
+        """If hit, record my starting position, that I may return to it in
+        ``on_touch_up`` after creating a real :class:`board.Spot` or
+        :class:`board.Pawn` instance.
+
+        """
+        if not self.collide_point(*touch.pos):
+            return False
+        self.pos_start = self.pos
+        self.pos_down = (
+            self.x - touch.x,
+            self.y - touch.y
+        )
+        touch.grab(self)
+        self._touch = touch
+        return True
+
+    def on_touch_move(self, touch):
+        """Follow the touch"""
+        if touch is not self._touch:
+            return False
+        self.pos = (
+            touch.x + self.x_down,
+            touch.y + self.y_down
+        )
+        return True
+
+    def on_touch_up(self, touch):
+        """Return to ``pos_start``, but first, save my current ``pos`` into
+        ``pos_up``, so that the layout knows where to put the real
+        :class:`board.Spot` or :class:`board.Pawn` instance.
+
+        """
+        if touch is not self._touch:
+            return False
+        self.pos_up = self.pos
+        self.pos = self.pos_start
+        self._touch = None
+        return True
 
 
 kv = """
 <Dummy>:
-	name: "".join((self.prefix, str(self.num)))
-	x_center_up: self.x_up + self.width / 2
-	y_center_up: self.y_up + self.height / 2
-	right_up: self.x_up + self.width
-	top_up: self.y_up + self.height
+    name: "".join((self.prefix, str(self.num)))
+    x_center_up: self.x_up + self.width / 2
+    y_center_up: self.y_up + self.height / 2
+    right_up: self.x_up + self.width
+    top_up: self.y_up + self.height
 """
 Builder.load_string(kv)
```

### Comparing `ELiDE-0.14.1/ELiDE/graph/__init__.py` & `ELiDE-0.9.1/ELiDE/board/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # This file is part of ELiDE, frontend to LiSE, a framework for life simulation games.
 # Copyright (c) Zachary Spector, public@zacharyspector.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, version 3.
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
-from .board import GraphBoard
+from .arrow import Arrow
+from .board import Board
 from .pawn import Pawn
-from .spot import GraphSpot
+from .spot import Spot
 
-__all__ = ['GraphBoard', 'Pawn', 'GraphSpot']
+__all__ = ['Arrow', 'Board', 'Pawn', 'Spot']
```

### Comparing `ELiDE-0.14.1/ELiDE/kwlist.py` & `ELiDE-0.9.1/ELiDE/kwlist.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # This file is part of ELiDE, frontend to LiSE, a framework for life simulation games.
 # Copyright (c) Zachary Spector, public@zacharyspector.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, version 3.
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from kivy.lang import Builder
 from kivy.uix.modalview import ModalView
 from kivy.properties import ListProperty
 
 
 class KeywordListModal(ModalView):
-	data = ListProperty([])
+    data = ListProperty([])
 
 
 Builder.load_string("""
 <KeywordListModal>:
-	size_hint_x: 0.6
-	BoxLayout:
-		orientation: 'vertical'
-		StatListView:
-			data: root.data
-		BoxLayout:
-			Button:
-				text: 'Cancel'
-			Button:
-				text: 'Done'
+    size_hint_x: 0.6
+    BoxLayout:
+        orientation: 'vertical'
+        StatListView:
+            data: root.data
+        BoxLayout:
+            Button:
+                text: 'Cancel'
+            Button:
+                text: 'Done'
 """)
```

### Comparing `ELiDE-0.14.1/ELiDE.egg-info/SOURCES.txt` & `ELiDE-0.9.1/ELiDE.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,42 @@
-LICENSE
-MANIFEST.in
-README.md
-pyproject.toml
+setup.py
 ELiDE/__init__.py
 ELiDE/__main__.py
 ELiDE/app.py
-ELiDE/boardscatter.py
-ELiDE/boardview.py
-ELiDE/calendar.py
 ELiDE/card.py
 ELiDE/charmenu.py
 ELiDE/charsview.py
 ELiDE/collide.py
 ELiDE/dialog.py
 ELiDE/dummy.py
 ELiDE/game.py
-ELiDE/gen.py
-ELiDE/imagestackproxy.py
 ELiDE/kwlist.py
 ELiDE/menu.py
 ELiDE/pallet.py
-ELiDE/pawn.py
-ELiDE/pawnspot.py
 ELiDE/rulesview.py
 ELiDE/screen.py
 ELiDE/spritebuilder.py
 ELiDE/statcfg.py
 ELiDE/statlist.py
-ELiDE/stepper.py
 ELiDE/stores.py
-ELiDE/timestream.py
 ELiDE/util.py
 ELiDE.egg-info/PKG-INFO
 ELiDE.egg-info/SOURCES.txt
 ELiDE.egg-info/dependency_links.txt
+ELiDE.egg-info/not-zip-safe
 ELiDE.egg-info/requires.txt
 ELiDE.egg-info/top_level.txt
 ELiDE/assets/Symbola.ttf
+ELiDE/assets/marsh_davies_crypt-0.png
+ELiDE/assets/marsh_davies_crypt.atlas
+ELiDE/assets/marsh_davies_island_bg-0.png
+ELiDE/assets/marsh_davies_island_bg.atlas
+ELiDE/assets/marsh_davies_island_fg-0.png
+ELiDE/assets/marsh_davies_island_fg.atlas
+ELiDE/assets/orb.png
 ELiDE/assets/polygons-0.png
 ELiDE/assets/polygons.atlas
 ELiDE/assets/wallpape.jpg
 ELiDE/assets/rltiles/amulet-0.png
 ELiDE/assets/rltiles/amulet.atlas
 ELiDE/assets/rltiles/arm-0.png
 ELiDE/assets/rltiles/arm.atlas
@@ -57,18 +53,15 @@
 ELiDE/assets/rltiles/boot-0.png
 ELiDE/assets/rltiles/boot.atlas
 ELiDE/assets/rltiles/cloak-0.png
 ELiDE/assets/rltiles/cloak.atlas
 ELiDE/assets/rltiles/dc-mon-0.png
 ELiDE/assets/rltiles/dc-mon.atlas
 ELiDE/assets/rltiles/dungeon-0.png
-ELiDE/assets/rltiles/dungeon-0.png~
 ELiDE/assets/rltiles/dungeon.atlas
-ELiDE/assets/rltiles/floor-0.png
-ELiDE/assets/rltiles/floor.atlas
 ELiDE/assets/rltiles/food-0.png
 ELiDE/assets/rltiles/food.atlas
 ELiDE/assets/rltiles/gem-0.png
 ELiDE/assets/rltiles/gem.atlas
 ELiDE/assets/rltiles/hair-0.png
 ELiDE/assets/rltiles/hair.atlas
 ELiDE/assets/rltiles/hand1-0.png
@@ -87,26 +80,14 @@
 ELiDE/assets/rltiles/ring.atlas
 ELiDE/assets/rltiles/scroll-0.png
 ELiDE/assets/rltiles/scroll.atlas
 ELiDE/assets/rltiles/wand-0.png
 ELiDE/assets/rltiles/wand.atlas
 ELiDE/assets/rltiles/weapon-0.png
 ELiDE/assets/rltiles/weapon.atlas
-ELiDE/graph/__init__.py
-ELiDE/graph/arrow.py
-ELiDE/graph/board.py
-ELiDE/graph/pawn.py
-ELiDE/graph/spot.py
-ELiDE/grid/__init__.py
-ELiDE/grid/board.py
-ELiDE/kivygarden/__init__.py
-ELiDE/kivygarden/texturestack/__init__.py
-ELiDE/tests/__init__.py
-ELiDE/tests/test_character_switcher.py
-ELiDE/tests/test_graphboard.py
-ELiDE/tests/test_gridboard.py
-ELiDE/tests/test_python_editor.py
-ELiDE/tests/test_rule_builder.py
-ELiDE/tests/test_screen.py
-ELiDE/tests/test_sprite_builder.py
-ELiDE/tests/test_strings_editor.py
-ELiDE/tests/util.py
+ELiDE/board/__init__.py
+ELiDE/board/arrow.py
+ELiDE/board/board.py
+ELiDE/board/pawn.py
+ELiDE/board/pawnspot.py
+ELiDE/board/spot.py
+ELiDE/kivygarden/texturestack/__init__.py
```

