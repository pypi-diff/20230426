# Comparing `tmp/inewave-0.0.94.tar.gz` & `tmp/inewave-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inewave-0.0.94.tar", last modified: Mon Apr 10 20:32:55 2023, max compression
+gzip compressed data, was "inewave-0.0.95.tar", last modified: Tue Apr 25 14:39:48 2023, max compression
```

## Comparing `inewave-0.0.94.tar` & `inewave-0.0.95.tar`

### file list

```diff
@@ -1,637 +1,652 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:32:55.320457 inewave-0.0.94/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-10 20:29:16.000000 inewave-0.0.94/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-10 20:32:55.316457 inewave-0.0.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-10 20:29:16.000000 inewave-0.0.94/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:32:55.192455 inewave-0.0.94/inewave/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:32:55.192455 inewave-0.0.94/inewave/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/_utils/leituracsv.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:32:55.200455 inewave-0.0.94/inewave/newave/
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/abertura.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/adterm.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/agrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    16024 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/arquivos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/bid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/cadic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/caso.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/clasgas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/clast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/confhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/conft.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/cortes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12456 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/cortesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/curva.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    73214 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/dger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/eafpast.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/elnino.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/enavazb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/enavazf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/energiab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/energiaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/energias.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/ensoaux.py
--rw-r--r--   0 runner    (1001) docker     (123)    14777 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/eolicacadastro.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/eolicaconfiguracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/eolicafte.py
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/eolicageracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/eolicahistorico.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/eolicaposto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/eolicasubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/exph.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/expt.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/forward.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/forwardh.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/gee.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/ghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/gtminpat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11512 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/itaipu.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/manutt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:32:55.208455 inewave-0.0.94/inewave/newave/modelos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/abertura.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/adterm.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/agrint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/arquivos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:32:55.212455 inewave-0.0.94/inewave/newave/modelos/arquivoscsv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/arquivoscsv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/arquivoscsv/arquivocsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/bid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:32:55.212455 inewave-0.0.94/inewave/newave/modelos/blocos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/blocos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/blocos/tabelacsv.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/blocos/versaomodelo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/cadic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/caso.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/clasgas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/clast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/confhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/conft.py
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/cortesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/curva.py
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)   133284 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/dger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/eafpast.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/elnino.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/enavazb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/enavazf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/energiab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/energiaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/energias.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/ensoaux.py
--rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/eolicacadastro.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/eolicaconfiguracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/eolicafte.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/eolicageracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/eolicahistorico.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/eolicaposto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/eolicasubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/exph.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/expt.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/gee.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/ghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/gtminpat.py
--rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/itaipu.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/manutt.py
--rw-r--r--   0 runner    (1001) docker     (123)    16085 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/modif.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/newavetim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)    30568 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/parp.py
--rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/parpeol.py
--rw-r--r--   0 runner    (1001) docker     (123)    23387 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)    17460 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/patamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/penalid.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/perda.py
--rw-r--r--   0 runner    (1001) docker     (123)    23967 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/pmo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/re.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/ree.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/sar.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/shist.py
--rw-r--r--   0 runner    (1001) docker     (123)    20502 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/sistema.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/tecno.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/term.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/vazaob.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/vazaof.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/vazaos.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/vazoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modelos/vazpast.py
--rw-r--r--   0 runner    (1001) docker     (123)    15254 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/modif.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/newavetim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)    18834 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/parp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12901 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/parpeol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15582 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/patamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/penalid.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/perda.py
--rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/pmo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/re.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/ree.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/sar.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/shist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/sistema.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/tecno.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/term.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/vazaob.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/vazaof.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/vazaos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/vazoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/newave/vazpast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:32:55.212455 inewave-0.0.94/inewave/nwlistcf/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistcf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistcf/estados.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:32:55.212455 inewave-0.0.94/inewave/nwlistcf/modelos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistcf/modelos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistcf/modelos/estados.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistcf/modelos/nwlistcf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistcf/nwlistcf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:32:55.220455 inewave-0.0.94/inewave/nwlistop/
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/cdef.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/cmarg.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/coper.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/corteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/cterm.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/deficit.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/defsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/depminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/dlppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/dlpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/eaf.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/eafb.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/eafbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/eafm.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/earmf.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/earmfm.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/earmfp.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/evert.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/evertm.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/evertsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/exces.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/excessin.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/fteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/geol.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/geolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/geolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/ghmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/ghtot.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/gttot.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/intercambio.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/invade.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/invadem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/mediasmerc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/mediassin.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/mercl.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/merclsin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:32:55.232455 inewave-0.0.94/inewave/nwlistop/modelos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:32:55.232455 inewave-0.0.94/inewave/nwlistop/modelos/arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/arquivos/arquivoree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/arquivos/arquivosin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/arquivos/arquivousina.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:32:55.232455 inewave-0.0.94/inewave/nwlistop/modelos/blocos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/blocos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/blocos/parsubmercados.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/blocos/ree.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/blocos/submercado.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/blocos/usina.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/blocos/valoresserie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/cdef.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/cmarg.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/coper.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/corteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/cterm.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/def.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/defsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/depminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/dflppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/dflpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/eaf.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/eafb.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/eafbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/eafm.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/earmf.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/earmfm.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/earmfp.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/evert.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/evertm.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/evertsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/exces.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/excessin.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/fteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/geol.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/geolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/geolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/ghmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/ghtot.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/gttot.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/intercambio.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/invade.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/invadem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/mediasmerc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/mediassin.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/mercl.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/merclsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/perdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/perdfm.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/qafluh.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/qincruh.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/vagua.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/varmuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/vento.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/vertuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/verturb.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/verturbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/vevmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/vevminm.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/vghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/vghminm.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/modelos/vturuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/perdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/perdfm.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/qafluh.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/qincruh.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/vagua.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/varmuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/vento.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/vertuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/verturb.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/verturbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/vevmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/vevminm.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/vghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/vghminm.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/nwlistop/vturuh.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/inewave/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:32:55.192455 inewave-0.0.94/inewave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-10 20:32:55.000000 inewave-0.0.94/inewave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19440 2023-04-10 20:32:55.000000 inewave-0.0.94/inewave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:32:55.000000 inewave-0.0.94/inewave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-10 20:32:55.000000 inewave-0.0.94/inewave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-10 20:32:55.000000 inewave-0.0.94/inewave.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 20:32:55.320457 inewave-0.0.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-10 20:29:16.000000 inewave-0.0.94/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:32:55.232455 inewave-0.0.94/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:32:55.236455 inewave-0.0.94/tests/_arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/_arquivos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:32:55.236455 inewave-0.0.94/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:32:55.300456 inewave-0.0.94/tests/mocks/arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/adterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/arquivos.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (123)    46951 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/cadic.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/caso.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/cdef.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (123)    30063 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/clast.py
--rw-r--r--   0 runner    (1001) docker     (123)   847210 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/cmarg.py
--rw-r--r--   0 runner    (1001) docker     (123)   295249 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/confhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/conft.py
--rw-r--r--   0 runner    (1001) docker     (123)   295245 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/coper.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105146 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/corteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)   295190 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/cterm.py
--rw-r--r--   0 runner    (1001) docker     (123)   295196 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/curva.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/deficit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/defsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/depminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)   847164 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/dger.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105161 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105169 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/dlppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105154 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105161 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105169 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/dlpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105154 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)   120243 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (123)   267099 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/eaf.py
--rw-r--r--   0 runner    (1001) docker     (123)   267152 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/eafb.py
--rw-r--r--   0 runner    (1001) docker     (123)   267153 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/eafbm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267155 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/eafm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/eafpast.py
--rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/earmf.py
--rw-r--r--   0 runner    (1001) docker     (123)   267144 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/earmfm.py
--rw-r--r--   0 runner    (1001) docker     (123)   291239 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/earmfp.py
--rw-r--r--   0 runner    (1001) docker     (123)   291240 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (123)    14002 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   267156 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/eolicacadastro.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/eolicaconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/eolicafte.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/eolicageracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/eolicahistorico.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/eolicaposto.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/eolicasubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)    56476 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/estados.py
--rw-r--r--   0 runner    (1001) docker     (123)   267137 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/evert.py
--rw-r--r--   0 runner    (1001) docker     (123)   267138 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/evertm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267139 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/evertsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1104654 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/exces.py
--rw-r--r--   0 runner    (1001) docker     (123)  1104652 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/excessin.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/exph.py
--rw-r--r--   0 runner    (1001) docker     (123)  1104650 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/fteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1104652 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105178 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/geol.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105179 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/geolm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105181 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/geolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   847144 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105136 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/ghmax.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105138 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105139 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105138 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105141 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105140 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105189 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/ghtot.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105190 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (123)    49768 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105188 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/gttot.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105191 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1087195 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/intercambio.py
--rw-r--r--   0 runner    (1001) docker     (123)   267122 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/invade.py
--rw-r--r--   0 runner    (1001) docker     (123)   267130 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/invadem.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/mercl.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/merclsin.py
--rw-r--r--   0 runner    (1001) docker     (123)    56692 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/modif.py
--rw-r--r--   0 runner    (1001) docker     (123)    45543 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/newavetim.py
--rw-r--r--   0 runner    (1001) docker     (123)    76518 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/nwlistcf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10775 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)   378349 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/parp.py
--rw-r--r--   0 runner    (1001) docker     (123)    50087 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/parpeol.py
--rw-r--r--   0 runner    (1001) docker     (123)    38585 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/patamar.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/penalid.py
--rw-r--r--   0 runner    (1001) docker     (123)   267136 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/perdf.py
--rw-r--r--   0 runner    (1001) docker     (123)   267137 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/perdfm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267139 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   380918 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/pmo.py
--rw-r--r--   0 runner    (1001) docker     (123)   283145 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/qafluh.py
--rw-r--r--   0 runner    (1001) docker     (123)   283145 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/qincruh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/re.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/ree.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105160 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105160 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (123)    20855 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/sistema.py
--rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/term.py
--rw-r--r--   0 runner    (1001) docker     (123)   271157 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/vagua.py
--rw-r--r--   0 runner    (1001) docker     (123)   283139 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (123)   283209 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/varmuh.py
--rw-r--r--   0 runner    (1001) docker     (123)    32259 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/vazpast.py
--rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/vento.py
--rw-r--r--   0 runner    (1001) docker     (123)   847200 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/vertuh.py
--rw-r--r--   0 runner    (1001) docker     (123)   267155 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/verturb.py
--rw-r--r--   0 runner    (1001) docker     (123)   267156 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/verturbm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267158 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   267122 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/vevmin.py
--rw-r--r--   0 runner    (1001) docker     (123)   267130 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/vevminm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267117 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105173 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/vghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105174 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/vghminm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105176 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   847195 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)   847135 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/arquivos/vturuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/mocks/mock_open.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:32:55.308457 inewave-0.0.94/tests/newave/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_adterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_arquivos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_cadic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_caso.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_clast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_confhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_conft.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_curva.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    48797 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_dger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_eafpast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_enavazb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_enavazf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_energiab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_energiaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_energias.py
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_eolicacadastro.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_eolicaconfiguracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_eolicafte.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_eolicageracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_eolicahistorico.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_eolicaposto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_eolicasubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_exph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_modif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_newavetim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_parp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_parpeol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_patamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_penalid.py
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_pmo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_re.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_ree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_sistema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_term.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_vazaob.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_vazaof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_vazaos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_vazoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/newave/test_vazpast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:32:55.308457 inewave-0.0.94/tests/nwlistcf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistcf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistcf/test_estados.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistcf/test_nwlistcf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:32:55.316457 inewave-0.0.94/tests/nwlistop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_cdef.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_cmarg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_coper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_corteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_cterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_deficit.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_defsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_depminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_dlppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_dlpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_eaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_eafb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_eafbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_eafm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_earmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_earmfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_earmfp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_evert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_evertm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_evertsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_exces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_excessin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_fteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_geol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_geolm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_geolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_ghmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_ghtot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_gttot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_intercambio.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_invade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_invadem.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_mediasmerc.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_mediassin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_mercl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_merclsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_perdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_perdfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_qafluh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_qincruh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_vagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_varmuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_vento.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_vertuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_verturb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_verturbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_vevmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_vevminm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_vghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_vghminm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-10 20:29:16.000000 inewave-0.0.94/tests/nwlistop/test_vturuh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.284622 inewave-0.0.95/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-25 14:36:08.000000 inewave-0.0.95/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-25 14:39:48.284622 inewave-0.0.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-25 14:36:08.000000 inewave-0.0.95/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.136619 inewave-0.0.95/inewave/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.140619 inewave-0.0.95/inewave/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/_utils/leituracsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.148619 inewave-0.0.95/inewave/newave/
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/abertura.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/adterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/agrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16024 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/bid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/cadic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/clasgas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/clast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/confhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/conft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/cortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12456 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/cortesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/curva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73214 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/dger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/elnino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/enavazb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/enavazf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/energiab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/energiaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/energias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/engnat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/ensoaux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14777 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/eolicacadastro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/eolicaconfiguracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/eolicafte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/eolicageracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/eolicahistorico.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/eolicaposto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/eolicasubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/exph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/expt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/forwardh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/gee.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/gtminpat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11512 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/itaipu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/manutt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.160619 inewave-0.0.95/inewave/newave/modelos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/abertura.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/adterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/agrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/arquivos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.160619 inewave-0.0.95/inewave/newave/modelos/arquivoscsv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/arquivoscsv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/arquivoscsv/arquivocsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/bid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.160619 inewave-0.0.95/inewave/newave/modelos/blocos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/blocos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/blocos/tabelacsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/blocos/versaomodelo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/cadic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/clasgas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/clast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/confhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/conft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/cortesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/curva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133284 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/dger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/elnino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/enavazb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/enavazf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/energiab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/energiaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/energias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/engnat.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/ensoaux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/eolicacadastro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/eolicaconfiguracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/eolicafte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/eolicageracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/eolicahistorico.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/eolicaposto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/eolicasubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/exph.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/expt.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/gee.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/gtminpat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/itaipu.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/manutt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16085 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/modif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30568 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/parp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23387 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17460 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/patamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/penalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/perda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24454 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/pmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/restricaoeletrica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/restricaoenergia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/restricaovazao.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/sar.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/shist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20502 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/sistema.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/tecno.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/vazaob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/vazaof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/vazaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/vazoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/vazpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15254 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18834 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/parp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12901 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15582 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/patamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/penalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/perda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/pmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/restricaoeletrica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/restricaoenergia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/restricaovazao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/sar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/shist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/sistema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/tecno.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/vazaob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/vazaof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/vazaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/vazoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/vazpast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.160619 inewave-0.0.95/inewave/nwlistcf/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistcf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistcf/estados.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.160619 inewave-0.0.95/inewave/nwlistcf/modelos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistcf/modelos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistcf/modelos/estados.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistcf/modelos/nwlistcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistcf/nwlistcf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.172619 inewave-0.0.95/inewave/nwlistop/
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/cdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/coper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/cterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/deficit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/defsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/dlppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/dlpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/eaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/eafb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/eafm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/earmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/evert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/evertm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/exces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/excessin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/geol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/geolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/gttot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/invade.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/invadem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/mediasmerc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/mediassin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/mercl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/merclsin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.184620 inewave-0.0.95/inewave/nwlistop/modelos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.184620 inewave-0.0.95/inewave/nwlistop/modelos/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivoree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivosin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivousina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.184620 inewave-0.0.95/inewave/nwlistop/modelos/blocos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/blocos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/blocos/parsubmercados.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/blocos/ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/blocos/submercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/blocos/usina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/blocos/valoresserie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/cdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/coper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/cterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/def.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/defsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/dflppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/dflpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/eaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/eafb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/eafm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/earmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/evert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/evertm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/exces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/excessin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/geol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/geolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/gttot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/invade.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/invadem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/mediasmerc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/mediassin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/mercl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/merclsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/perdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/vagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/vento.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/verturb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/vturuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/perdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/vagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/vento.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/verturb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/vturuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.140619 inewave-0.0.95/inewave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-25 14:39:48.000000 inewave-0.0.95/inewave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19993 2023-04-25 14:39:48.000000 inewave-0.0.95/inewave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:39:48.000000 inewave-0.0.95/inewave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-25 14:39:48.000000 inewave-0.0.95/inewave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 14:39:48.000000 inewave-0.0.95/inewave.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:39:48.284622 inewave-0.0.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-25 14:36:08.000000 inewave-0.0.95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.184620 inewave-0.0.95/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.184620 inewave-0.0.95/tests/_arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/_arquivos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.184620 inewave-0.0.95/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.256621 inewave-0.0.95/tests/mocks/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/adterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46951 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/cadic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/cdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30063 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/clast.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847210 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)   295249 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/confhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/conft.py
+-rw-r--r--   0 runner    (1001) docker     (123)   295245 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/coper.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105146 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   295190 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/cterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   295196 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/curva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/deficit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/defsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847164 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dger.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105161 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105169 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dlppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105154 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105161 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105169 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dlpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105154 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120243 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267099 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267152 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eafb.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267153 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267155 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eafm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/earmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267144 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   291239 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   291240 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14002 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267156 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eolicacadastro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eolicaconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eolicafte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eolicageracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eolicahistorico.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eolicaposto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eolicasubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56476 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/estados.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267137 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/evert.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267138 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/evertm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267139 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1104654 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/exces.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1104652 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/excessin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/exph.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1104650 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1104652 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105178 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/geol.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105179 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/geolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105181 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847144 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105136 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105138 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105139 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105138 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105141 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105140 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105189 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105190 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49768 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105188 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/gttot.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105191 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1087195 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267122 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/invade.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267130 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/invadem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/mercl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/merclsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56692 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/modif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45543 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76518 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/nwlistcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10775 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)   378349 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/parp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50087 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38585 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/patamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/penalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267136 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/perdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267137 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267139 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   380918 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/pmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283145 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283145 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/restricaoeletrica.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/restricaoenergia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/restricaovazao.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105160 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105160 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20855 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/sistema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/term.py
+-rw-r--r--   0 runner    (1001) docker     (123)   271157 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283139 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283209 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32259 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vazpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vento.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847200 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267155 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/verturb.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267156 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267158 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267122 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267130 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267117 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105173 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105174 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105176 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847195 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847135 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vturuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/mock_open.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.268622 inewave-0.0.95/tests/newave/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_adterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_cadic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_clast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_confhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_conft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_curva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48797 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_dger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_enavazb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_enavazf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_energiab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_energiaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_energias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_engnat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_eolicacadastro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_eolicaconfiguracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_eolicafte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_eolicageracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_eolicahistorico.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_eolicaposto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_eolicasubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_exph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_modif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_parp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_patamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_penalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_pmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_restricaoeletrica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_restricaoenergia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_restricaovazao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_sistema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_vazaob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_vazaof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_vazaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_vazoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_vazpast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.268622 inewave-0.0.95/tests/nwlistcf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistcf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistcf/test_estados.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistcf/test_nwlistcf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.284622 inewave-0.0.95/tests/nwlistop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_cdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_coper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_cterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_deficit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_defsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_dlppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_dlpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_eaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_eafb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_eafm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_earmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_evert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_evertm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_exces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_excessin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_geol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_geolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_gttot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_invade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_invadem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_mediasmerc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_mediassin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_mercl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_merclsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_perdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_vagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_vento.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_verturb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_vturuh.py
```

### Comparing `inewave-0.0.94/LICENSE.md` & `inewave-0.0.95/LICENSE.md`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/PKG-INFO` & `inewave-0.0.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inewave
-Version: 0.0.94
+Version: 0.0.95
 Summary: Interface para arquivos do NEWAVE
 Home-page: https://github.com/rjmalves/inewave
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `inewave-0.0.94/README.md` & `inewave-0.0.95/README.md`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/_utils/leituracsv.py` & `inewave-0.0.95/inewave/_utils/leituracsv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/config.py` & `inewave-0.0.95/inewave/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 MAX_SERIES_SINTETICAS = 2000
 MAX_PATAMARES = 5
 NUM_CENARIOS = 2000
 MAX_ANOS_ESTUDO = 30
-MAX_ANOS_HISTORICO = 120
+MAX_ANOS_HISTORICO = 100
 MAX_CONFIGURACOES = 360
 MAX_SUBMERCADOS = 15
 MAX_ITERS = 100
 MAX_FORWARDS = 300
 MAX_CORTES = MAX_ITERS * MAX_FORWARDS
 MAX_UHES = 330
 MAX_CONJUNTOS_MAQUINAS = 5
```

### Comparing `inewave-0.0.94/inewave/newave/__init__.py` & `inewave-0.0.95/inewave/newave/__init__.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/abertura.py` & `inewave-0.0.95/inewave/newave/abertura.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/adterm.py` & `inewave-0.0.95/inewave/newave/adterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/agrint.py` & `inewave-0.0.95/inewave/newave/agrint.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/arquivos.py` & `inewave-0.0.95/inewave/newave/arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/avl_cortesfpha_nwv.py` & `inewave-0.0.95/inewave/newave/avl_cortesfpha_nwv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/avl_desvfpha_s.py` & `inewave-0.0.95/inewave/newave/avl_desvfpha_s.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/avl_desvfpha_v_q.py` & `inewave-0.0.95/inewave/newave/avl_desvfpha_v_q.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/bid.py` & `inewave-0.0.95/inewave/newave/bid.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/cadic.py` & `inewave-0.0.95/inewave/newave/cadic.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/caso.py` & `inewave-0.0.95/inewave/newave/caso.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/clasgas.py` & `inewave-0.0.95/inewave/newave/clasgas.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/clast.py` & `inewave-0.0.95/inewave/newave/clast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/confhd.py` & `inewave-0.0.95/inewave/newave/confhd.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/conft.py` & `inewave-0.0.95/inewave/newave/conft.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/cortesh.py` & `inewave-0.0.95/inewave/newave/cortesh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/curva.py` & `inewave-0.0.95/inewave/newave/curva.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/cvar.py` & `inewave-0.0.95/inewave/newave/cvar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/dger.py` & `inewave-0.0.95/inewave/newave/dger.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/dsvagua.py` & `inewave-0.0.95/inewave/newave/dsvagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/eafpast.py` & `inewave-0.0.95/inewave/newave/eafpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/elnino.py` & `inewave-0.0.95/inewave/newave/elnino.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/enavazb.py` & `inewave-0.0.95/inewave/newave/enavazb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/enavazf.py` & `inewave-0.0.95/inewave/newave/enavazf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/energiab.py` & `inewave-0.0.95/inewave/newave/energiab.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/energiaf.py` & `inewave-0.0.95/inewave/newave/energiaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/energias.py` & `inewave-0.0.95/inewave/newave/energias.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/ensoaux.py` & `inewave-0.0.95/inewave/newave/ensoaux.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/eolicacadastro.py` & `inewave-0.0.95/inewave/newave/eolicacadastro.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/eolicaconfiguracao.py` & `inewave-0.0.95/inewave/newave/eolicaconfiguracao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/eolicafte.py` & `inewave-0.0.95/inewave/newave/eolicafte.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/eolicageracao.py` & `inewave-0.0.95/inewave/newave/eolicageracao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/eolicahistorico.py` & `inewave-0.0.95/inewave/newave/eolicahistorico.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/eolicaposto.py` & `inewave-0.0.95/inewave/newave/eolicaposto.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/eolicasubmercado.py` & `inewave-0.0.95/inewave/newave/eolicasubmercado.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/exph.py` & `inewave-0.0.95/inewave/newave/exph.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/expt.py` & `inewave-0.0.95/inewave/newave/expt.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/gee.py` & `inewave-0.0.95/inewave/newave/gee.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/ghmin.py` & `inewave-0.0.95/inewave/newave/ghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/gtminpat.py` & `inewave-0.0.95/inewave/newave/gtminpat.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/hidr.py` & `inewave-0.0.95/inewave/newave/hidr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/itaipu.py` & `inewave-0.0.95/inewave/newave/itaipu.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/manutt.py` & `inewave-0.0.95/inewave/newave/manutt.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/adterm.py` & `inewave-0.0.95/inewave/newave/modelos/adterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/arquivos.py` & `inewave-0.0.95/inewave/newave/modelos/arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/arquivoscsv/arquivocsv.py` & `inewave-0.0.95/inewave/newave/modelos/arquivoscsv/arquivocsv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/avl_cortesfpha_nwv.py` & `inewave-0.0.95/inewave/newave/modelos/avl_cortesfpha_nwv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/avl_desvfpha_s.py` & `inewave-0.0.95/inewave/newave/modelos/avl_desvfpha_s.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/avl_desvfpha_v_q.py` & `inewave-0.0.95/inewave/newave/modelos/avl_desvfpha_v_q.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/blocos/tabelacsv.py` & `inewave-0.0.95/inewave/newave/modelos/blocos/tabelacsv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/blocos/versaomodelo.py` & `inewave-0.0.95/inewave/newave/modelos/blocos/versaomodelo.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/cadic.py` & `inewave-0.0.95/inewave/newave/modelos/cadic.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/caso.py` & `inewave-0.0.95/inewave/newave/modelos/caso.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/clast.py` & `inewave-0.0.95/inewave/newave/modelos/clast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/confhd.py` & `inewave-0.0.95/inewave/newave/modelos/confhd.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/conft.py` & `inewave-0.0.95/inewave/newave/modelos/conft.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/cortesh.py` & `inewave-0.0.95/inewave/newave/modelos/cortesh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/curva.py` & `inewave-0.0.95/inewave/newave/modelos/curva.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/cvar.py` & `inewave-0.0.95/inewave/newave/modelos/cvar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/dger.py` & `inewave-0.0.95/inewave/newave/modelos/dger.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/dsvagua.py` & `inewave-0.0.95/inewave/newave/modelos/dsvagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/eafpast.py` & `inewave-0.0.95/inewave/newave/modelos/eafpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/enavazb.py` & `inewave-0.0.95/inewave/newave/modelos/enavazb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/enavazf.py` & `inewave-0.0.95/inewave/newave/modelos/enavazf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/energiab.py` & `inewave-0.0.95/inewave/newave/modelos/energiab.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/energiaf.py` & `inewave-0.0.95/inewave/newave/modelos/energiaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/energias.py` & `inewave-0.0.95/inewave/newave/modelos/energias.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/eolicacadastro.py` & `inewave-0.0.95/inewave/newave/modelos/eolicacadastro.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/eolicaconfiguracao.py` & `inewave-0.0.95/inewave/newave/modelos/eolicaconfiguracao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/eolicafte.py` & `inewave-0.0.95/inewave/newave/modelos/eolicafte.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/eolicageracao.py` & `inewave-0.0.95/inewave/newave/modelos/eolicageracao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/eolicahistorico.py` & `inewave-0.0.95/inewave/newave/modelos/eolicahistorico.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/eolicaposto.py` & `inewave-0.0.95/inewave/newave/modelos/eolicaposto.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/eolicasubmercado.py` & `inewave-0.0.95/inewave/newave/modelos/eolicasubmercado.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/exph.py` & `inewave-0.0.95/inewave/newave/modelos/exph.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/hidr.py` & `inewave-0.0.95/inewave/newave/modelos/hidr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/modif.py` & `inewave-0.0.95/inewave/newave/modelos/modif.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/newavetim.py` & `inewave-0.0.95/inewave/newave/modelos/newavetim.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/nwv_avl_evap.py` & `inewave-0.0.95/inewave/newave/modelos/nwv_avl_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/nwv_cortes_evap.py` & `inewave-0.0.95/inewave/newave/modelos/nwv_cortes_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/nwv_eco_evap.py` & `inewave-0.0.95/inewave/newave/modelos/nwv_eco_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/parp.py` & `inewave-0.0.95/inewave/newave/modelos/parp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/parpeol.py` & `inewave-0.0.95/inewave/newave/modelos/parpeol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/parpvaz.py` & `inewave-0.0.95/inewave/newave/modelos/parpvaz.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/patamar.py` & `inewave-0.0.95/inewave/newave/modelos/patamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/penalid.py` & `inewave-0.0.95/inewave/newave/modelos/penalid.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/pmo.py` & `inewave-0.0.95/inewave/newave/modelos/pmo.py`

 * *Files 5% similar despite different names*

```diff
@@ -624,64 +624,89 @@
             "produtibilidade_acumulada_calculo_altura_65",
             "produtibilidade_acumulada_calculo_altura_maxima",
             "produtibilidade_acumulada_calculo_evaporacao_altura_minima",
             "produtibilidade_acumulada_calculo_evaporacao_altura_65",
             "produtibilidade_acumulada_calculo_evaporacao_altura_maxima",
         ]
 
+    def __fecha_configuracao(
+        self,
+        df_usinas: pd.DataFrame,
+        df_reservatorios: pd.DataFrame,
+        df_acumuladas: pd.DataFrame,
+        cfg_atual: int,
+        df_atual: pd.DataFrame,
+    ) -> pd.DataFrame:
+        todas_usinas = list(
+            set(
+                df_usinas.index.tolist()
+                + df_reservatorios.index.tolist()
+                + df_acumuladas.index.tolist()
+            )
+        )
+        todas_usinas.sort()
+        df_agregado = pd.DataFrame(index=todas_usinas)
+        df_agregado.loc[
+            df_usinas.index,
+            "produtibilidade_equivalente_volmin_volmax",
+        ] = df_usinas["produtibilidade_equivalente_volmin_volmax"]
+        for col in self.__colunas_produtibilidades_reservatorios():
+            df_agregado.loc[
+                df_reservatorios.index,
+                col,
+            ] = df_reservatorios[col]
+        for col in self.__colunas_produtibilidades_acumuladas():
+            df_agregado.loc[
+                df_acumuladas.index,
+                col,
+            ] = df_acumuladas[col]
+        df_agregado["configuracao"] = cfg_atual
+        df_atual = pd.concat(
+            [df_atual, df_agregado.reset_index()],
+            ignore_index=True,
+        )
+        return df_atual
+
     # Override
     def read(self, file: IO, *args, **kwargs):
         cfg_atual = 0
         df_atual = pd.DataFrame()
         df_usinas = pd.DataFrame()
         df_reservatorios = pd.DataFrame()
         df_acumuladas = pd.DataFrame()
         while True:
             linha = file.readline()
             # Verifica se acabou:
             if "PRODUTIBILIDADES ACUMULADAS PARA CALCULO DE" in linha:
+                if cfg_atual != 0:
+                    df_atual = self.__fecha_configuracao(
+                        df_usinas,
+                        df_reservatorios,
+                        df_acumuladas,
+                        cfg_atual,
+                        df_atual,
+                    )
                 self.data = df_atual.rename(columns={"index": "nome_usina"})[
                     [
                         "nome_usina",
                         "configuracao",
                         "produtibilidade_equivalente_volmin_volmax",
                     ]
                     + self.__colunas_produtibilidades_reservatorios()
                     + self.__colunas_produtibilidades_acumuladas()
                 ]
                 break
             if "CONFIGURACAO :   " in linha:
                 if cfg_atual != 0:
-                    todas_usinas = list(
-                        set(
-                            df_usinas.index.tolist()
-                            + df_reservatorios.index.tolist()
-                            + df_acumuladas.index.tolist()
-                        )
-                    )
-                    todas_usinas.sort()
-                    df_agregado = pd.DataFrame(index=todas_usinas)
-                    df_agregado.loc[
-                        df_usinas.index,
-                        "produtibilidade_equivalente_volmin_volmax",
-                    ] = df_usinas["produtibilidade_equivalente_volmin_volmax"]
-                    for col in self.__colunas_produtibilidades_reservatorios():
-                        df_agregado.loc[
-                            df_reservatorios.index,
-                            col,
-                        ] = df_reservatorios[col]
-                    for col in self.__colunas_produtibilidades_acumuladas():
-                        df_agregado.loc[
-                            df_acumuladas.index,
-                            col,
-                        ] = df_acumuladas[col]
-                    df_agregado["configuracao"] = cfg_atual
-                    df_atual = pd.concat(
-                        [df_atual, df_agregado.reset_index()],
-                        ignore_index=True,
+                    df_atual = self.__fecha_configuracao(
+                        df_usinas,
+                        df_reservatorios,
+                        df_acumuladas,
+                        cfg_atual,
+                        df_atual,
                     )
                 cfg_atual = self.__cfg_line.read(linha)[0]
             if "PRODUTIBILIDADES DAS USINAS (MW/m3/s)" in linha:
                 df_usinas = self.__le_produtibilidade_usinas(file)
                 df_usinas.set_index("nome_usina", inplace=True)
             if "USINA      PRODTM   PDTMIN   PDTMED   PDTMAX" in linha:
                 df_reservatorios = self.__le_produtibilidade_reservatorios(
```

### Comparing `inewave-0.0.94/inewave/newave/modelos/re.py` & `inewave-0.0.95/inewave/newave/modelos/re.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/ree.py` & `inewave-0.0.95/inewave/newave/modelos/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/sistema.py` & `inewave-0.0.95/inewave/newave/modelos/sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/term.py` & `inewave-0.0.95/inewave/newave/modelos/term.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/vazaob.py` & `inewave-0.0.95/inewave/newave/modelos/vazaob.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/vazaof.py` & `inewave-0.0.95/inewave/newave/modelos/vazaof.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/vazaos.py` & `inewave-0.0.95/inewave/newave/modelos/vazaos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/vazoes.py` & `inewave-0.0.95/inewave/newave/modelos/vazoes.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modelos/vazpast.py` & `inewave-0.0.95/inewave/newave/modelos/vazpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/modif.py` & `inewave-0.0.95/inewave/newave/modif.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/newavetim.py` & `inewave-0.0.95/inewave/newave/newavetim.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/nwv_avl_evap.py` & `inewave-0.0.95/inewave/newave/nwv_avl_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/nwv_cortes_evap.py` & `inewave-0.0.95/inewave/newave/nwv_cortes_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/nwv_eco_evap.py` & `inewave-0.0.95/inewave/newave/nwv_eco_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/parp.py` & `inewave-0.0.95/inewave/newave/parp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/parpeol.py` & `inewave-0.0.95/inewave/newave/parpeol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/parpvaz.py` & `inewave-0.0.95/inewave/newave/parpvaz.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/patamar.py` & `inewave-0.0.95/inewave/newave/patamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/penalid.py` & `inewave-0.0.95/inewave/newave/penalid.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/perda.py` & `inewave-0.0.95/inewave/newave/perda.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/pmo.py` & `inewave-0.0.95/inewave/newave/pmo.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/re.py` & `inewave-0.0.95/inewave/newave/re.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/ree.py` & `inewave-0.0.95/inewave/newave/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/sar.py` & `inewave-0.0.95/inewave/newave/sar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/shist.py` & `inewave-0.0.95/inewave/newave/shist.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/sistema.py` & `inewave-0.0.95/inewave/newave/sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/tecno.py` & `inewave-0.0.95/inewave/newave/tecno.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/term.py` & `inewave-0.0.95/inewave/newave/term.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/vazaob.py` & `inewave-0.0.95/inewave/newave/vazaob.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/vazaof.py` & `inewave-0.0.95/inewave/newave/vazaof.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/vazaos.py` & `inewave-0.0.95/inewave/newave/vazaos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/vazoes.py` & `inewave-0.0.95/inewave/newave/vazoes.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/newave/vazpast.py` & `inewave-0.0.95/inewave/newave/vazpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistcf/estados.py` & `inewave-0.0.95/inewave/nwlistcf/estados.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistcf/modelos/estados.py` & `inewave-0.0.95/inewave/nwlistcf/modelos/estados.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistcf/modelos/nwlistcf.py` & `inewave-0.0.95/inewave/nwlistcf/modelos/nwlistcf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistcf/nwlistcf.py` & `inewave-0.0.95/inewave/nwlistcf/nwlistcf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/__init__.py` & `inewave-0.0.95/inewave/nwlistop/__init__.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/cdef.py` & `inewave-0.0.95/inewave/nwlistop/cdef.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/cdefsin.py` & `inewave-0.0.95/inewave/nwlistop/cdefsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/cmarg.py` & `inewave-0.0.95/inewave/nwlistop/cmarg.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/cmargmed.py` & `inewave-0.0.95/inewave/nwlistop/cmargmed.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/coper.py` & `inewave-0.0.95/inewave/nwlistop/coper.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/corteolm.py` & `inewave-0.0.95/inewave/nwlistop/corteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/cterm.py` & `inewave-0.0.95/inewave/nwlistop/cterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/ctermsin.py` & `inewave-0.0.95/inewave/nwlistop/ctermsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/deficit.py` & `inewave-0.0.95/inewave/nwlistop/deficit.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/defsin.py` & `inewave-0.0.95/inewave/nwlistop/defsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/depminuh.py` & `inewave-0.0.95/inewave/nwlistop/depminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/dfphauh.py` & `inewave-0.0.95/inewave/nwlistop/dfphauh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/dlppdfmax.py` & `inewave-0.0.95/inewave/nwlistop/dlppdfmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/dlppdfmaxm.py` & `inewave-0.0.95/inewave/nwlistop/dlppdfmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/dlppdfmaxs.py` & `inewave-0.0.95/inewave/nwlistop/dlppdfmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/dlpptbmax.py` & `inewave-0.0.95/inewave/nwlistop/dlpptbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/dlpptbmaxm.py` & `inewave-0.0.95/inewave/nwlistop/dlpptbmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/dlpptbmaxs.py` & `inewave-0.0.95/inewave/nwlistop/dlpptbmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/dtbmax.py` & `inewave-0.0.95/inewave/nwlistop/dtbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/dtbmin.py` & `inewave-0.0.95/inewave/nwlistop/dtbmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/dvazmax.py` & `inewave-0.0.95/inewave/nwlistop/dvazmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/eaf.py` & `inewave-0.0.95/inewave/nwlistop/eaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/eafb.py` & `inewave-0.0.95/inewave/nwlistop/eafb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/eafbm.py` & `inewave-0.0.95/inewave/nwlistop/eafbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/eafbsin.py` & `inewave-0.0.95/inewave/nwlistop/eafbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/eafm.py` & `inewave-0.0.95/inewave/nwlistop/eafm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/earmf.py` & `inewave-0.0.95/inewave/nwlistop/earmf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/earmfm.py` & `inewave-0.0.95/inewave/nwlistop/earmfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/earmfp.py` & `inewave-0.0.95/inewave/nwlistop/earmfp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/earmfpm.py` & `inewave-0.0.95/inewave/nwlistop/earmfpm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/earmfpsin.py` & `inewave-0.0.95/inewave/nwlistop/earmfpsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/earmfsin.py` & `inewave-0.0.95/inewave/nwlistop/earmfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/evert.py` & `inewave-0.0.95/inewave/nwlistop/evert.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/evertm.py` & `inewave-0.0.95/inewave/nwlistop/evertm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/evertsin.py` & `inewave-0.0.95/inewave/nwlistop/evertsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/exces.py` & `inewave-0.0.95/inewave/nwlistop/exces.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/excessin.py` & `inewave-0.0.95/inewave/nwlistop/excessin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/fteolm.py` & `inewave-0.0.95/inewave/nwlistop/fteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/fteolsin.py` & `inewave-0.0.95/inewave/nwlistop/fteolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/geol.py` & `inewave-0.0.95/inewave/nwlistop/geol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/geolm.py` & `inewave-0.0.95/inewave/nwlistop/geolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/geolsin.py` & `inewave-0.0.95/inewave/nwlistop/geolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/ghiduh.py` & `inewave-0.0.95/inewave/nwlistop/ghiduh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/ghmax.py` & `inewave-0.0.95/inewave/nwlistop/ghmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/ghmaxm.py` & `inewave-0.0.95/inewave/nwlistop/ghmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/ghmaxmr.py` & `inewave-0.0.95/inewave/nwlistop/ghmaxmr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/ghmaxr.py` & `inewave-0.0.95/inewave/nwlistop/ghmaxr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/ghmaxrsin.py` & `inewave-0.0.95/inewave/nwlistop/ghmaxrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/ghmaxsin.py` & `inewave-0.0.95/inewave/nwlistop/ghmaxsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/ghtot.py` & `inewave-0.0.95/inewave/nwlistop/ghtot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/ghtotm.py` & `inewave-0.0.95/inewave/nwlistop/ghtotm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/ghtotsin.py` & `inewave-0.0.95/inewave/nwlistop/ghtotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/gttot.py` & `inewave-0.0.95/inewave/nwlistop/gttot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/gttotsin.py` & `inewave-0.0.95/inewave/nwlistop/gttotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/intercambio.py` & `inewave-0.0.95/inewave/nwlistop/intercambio.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/invade.py` & `inewave-0.0.95/inewave/nwlistop/invade.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/invadem.py` & `inewave-0.0.95/inewave/nwlistop/invadem.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/mediasmerc.py` & `inewave-0.0.95/inewave/nwlistop/mediasmerc.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/mediassin.py` & `inewave-0.0.95/inewave/nwlistop/mediassin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/mercl.py` & `inewave-0.0.95/inewave/nwlistop/mercl.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/merclsin.py` & `inewave-0.0.95/inewave/nwlistop/merclsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py` & `inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/arquivos/arquivoree.py` & `inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivoree.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py` & `inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/arquivos/arquivosin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivosin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py` & `inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py` & `inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py` & `inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/arquivos/arquivousina.py` & `inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivousina.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py` & `inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/blocos/parsubmercados.py` & `inewave-0.0.95/inewave/nwlistop/modelos/blocos/parsubmercados.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/blocos/ree.py` & `inewave-0.0.95/inewave/nwlistop/modelos/blocos/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/blocos/submercado.py` & `inewave-0.0.95/inewave/nwlistop/modelos/blocos/submercado.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/blocos/usina.py` & `inewave-0.0.95/inewave/nwlistop/modelos/blocos/usina.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/blocos/valoresserie.py` & `inewave-0.0.95/inewave/nwlistop/modelos/blocos/valoresserie.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py` & `inewave-0.0.95/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/cdef.py` & `inewave-0.0.95/inewave/nwlistop/modelos/cdef.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/cdefsin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/cdefsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/cmarg.py` & `inewave-0.0.95/inewave/nwlistop/modelos/cmarg.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/cmargmed.py` & `inewave-0.0.95/inewave/nwlistop/modelos/cmargmed.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/coper.py` & `inewave-0.0.95/inewave/nwlistop/modelos/coper.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/corteolm.py` & `inewave-0.0.95/inewave/nwlistop/modelos/corteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/cterm.py` & `inewave-0.0.95/inewave/nwlistop/modelos/cterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/ctermsin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/ctermsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/def.py` & `inewave-0.0.95/inewave/nwlistop/modelos/def.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/defsin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/defsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/depminuh.py` & `inewave-0.0.95/inewave/nwlistop/modelos/depminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/dflppdfmaxm.py` & `inewave-0.0.95/inewave/nwlistop/modelos/dflppdfmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/dflpptbmaxm.py` & `inewave-0.0.95/inewave/nwlistop/modelos/dflpptbmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/dfphauh.py` & `inewave-0.0.95/inewave/nwlistop/modelos/dfphauh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/dlppdfmax.py` & `inewave-0.0.95/inewave/nwlistop/modelos/dlppdfmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/dlppdfmaxs.py` & `inewave-0.0.95/inewave/nwlistop/modelos/dlppdfmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/dlpptbmax.py` & `inewave-0.0.95/inewave/nwlistop/modelos/dlpptbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/dlpptbmaxs.py` & `inewave-0.0.95/inewave/nwlistop/modelos/dlpptbmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/dtbmax.py` & `inewave-0.0.95/inewave/nwlistop/modelos/dtbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/dtbmin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/dtbmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/dvazmax.py` & `inewave-0.0.95/inewave/nwlistop/modelos/dvazmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/eaf.py` & `inewave-0.0.95/inewave/nwlistop/modelos/eaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/eafb.py` & `inewave-0.0.95/inewave/nwlistop/modelos/eafb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/eafbm.py` & `inewave-0.0.95/inewave/nwlistop/modelos/eafbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/eafbsin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/eafbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/eafm.py` & `inewave-0.0.95/inewave/nwlistop/modelos/eafm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/earmf.py` & `inewave-0.0.95/inewave/nwlistop/modelos/earmf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/earmfm.py` & `inewave-0.0.95/inewave/nwlistop/modelos/earmfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/earmfp.py` & `inewave-0.0.95/inewave/nwlistop/modelos/earmfp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/earmfpm.py` & `inewave-0.0.95/inewave/nwlistop/modelos/earmfpm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/earmfpsin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/earmfpsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/earmfsin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/earmfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/evert.py` & `inewave-0.0.95/inewave/nwlistop/modelos/evert.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/evertm.py` & `inewave-0.0.95/inewave/nwlistop/modelos/evertm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/evertsin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/evertsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/exces.py` & `inewave-0.0.95/inewave/nwlistop/modelos/exces.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/excessin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/excessin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/fteolm.py` & `inewave-0.0.95/inewave/nwlistop/modelos/fteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/fteolsin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/fteolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/geol.py` & `inewave-0.0.95/inewave/nwlistop/modelos/geol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/geolm.py` & `inewave-0.0.95/inewave/nwlistop/modelos/geolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/geolsin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/geolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/ghiduh.py` & `inewave-0.0.95/inewave/nwlistop/modelos/ghiduh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/ghmax.py` & `inewave-0.0.95/inewave/nwlistop/modelos/ghmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/ghmaxm.py` & `inewave-0.0.95/inewave/nwlistop/modelos/ghmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/ghmaxmr.py` & `inewave-0.0.95/inewave/nwlistop/modelos/ghmaxmr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/ghmaxr.py` & `inewave-0.0.95/inewave/nwlistop/modelos/ghmaxr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/ghmaxrsin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/ghmaxrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/ghmaxsin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/ghmaxsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/ghtot.py` & `inewave-0.0.95/inewave/nwlistop/modelos/ghtot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/ghtotm.py` & `inewave-0.0.95/inewave/nwlistop/modelos/ghtotm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/ghtotsin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/ghtotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/gttot.py` & `inewave-0.0.95/inewave/nwlistop/modelos/gttot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/gttotsin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/gttotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/intercambio.py` & `inewave-0.0.95/inewave/nwlistop/modelos/intercambio.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/invade.py` & `inewave-0.0.95/inewave/nwlistop/modelos/invade.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/invadem.py` & `inewave-0.0.95/inewave/nwlistop/modelos/invadem.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/mediasmerc.py` & `inewave-0.0.95/inewave/nwlistop/modelos/mediasmerc.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/mediassin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/mediassin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/mercl.py` & `inewave-0.0.95/inewave/nwlistop/modelos/mercl.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/merclsin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/merclsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/perdf.py` & `inewave-0.0.95/inewave/nwlistop/modelos/perdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/perdfm.py` & `inewave-0.0.95/inewave/nwlistop/modelos/perdfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/perdfsin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/perdfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/qafluh.py` & `inewave-0.0.95/inewave/nwlistop/modelos/qafluh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/qincruh.py` & `inewave-0.0.95/inewave/nwlistop/modelos/qincruh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/rhslppdf.py` & `inewave-0.0.95/inewave/nwlistop/modelos/rhslppdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/rhslpptb.py` & `inewave-0.0.95/inewave/nwlistop/modelos/rhslpptb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/vagua.py` & `inewave-0.0.95/inewave/nwlistop/modelos/vagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/varmpuh.py` & `inewave-0.0.95/inewave/nwlistop/modelos/varmpuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/varmuh.py` & `inewave-0.0.95/inewave/nwlistop/modelos/varmuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/vento.py` & `inewave-0.0.95/inewave/nwlistop/modelos/vento.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/vertuh.py` & `inewave-0.0.95/inewave/nwlistop/modelos/vertuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/verturb.py` & `inewave-0.0.95/inewave/nwlistop/modelos/verturb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/verturbm.py` & `inewave-0.0.95/inewave/nwlistop/modelos/verturbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/verturbsin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/verturbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/vevmin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/vevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/vevminm.py` & `inewave-0.0.95/inewave/nwlistop/modelos/vevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/vevminsin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/vevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/vghmin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/vghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/vghminm.py` & `inewave-0.0.95/inewave/nwlistop/modelos/vghminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/vghminsin.py` & `inewave-0.0.95/inewave/nwlistop/modelos/vghminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/vghminuh.py` & `inewave-0.0.95/inewave/nwlistop/modelos/vghminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/modelos/vturuh.py` & `inewave-0.0.95/inewave/nwlistop/modelos/vturuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/perdf.py` & `inewave-0.0.95/inewave/nwlistop/perdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/perdfm.py` & `inewave-0.0.95/inewave/nwlistop/perdfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/perdfsin.py` & `inewave-0.0.95/inewave/nwlistop/perdfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/qafluh.py` & `inewave-0.0.95/inewave/nwlistop/qafluh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/qincruh.py` & `inewave-0.0.95/inewave/nwlistop/qincruh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/rhslppdf.py` & `inewave-0.0.95/inewave/nwlistop/rhslppdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/rhslpptb.py` & `inewave-0.0.95/inewave/nwlistop/rhslpptb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/vagua.py` & `inewave-0.0.95/inewave/nwlistop/vagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/varmpuh.py` & `inewave-0.0.95/inewave/nwlistop/varmpuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/varmuh.py` & `inewave-0.0.95/inewave/nwlistop/varmuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/vento.py` & `inewave-0.0.95/inewave/nwlistop/vento.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/vertuh.py` & `inewave-0.0.95/inewave/nwlistop/vertuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/verturb.py` & `inewave-0.0.95/inewave/nwlistop/verturb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/verturbm.py` & `inewave-0.0.95/inewave/nwlistop/verturbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/verturbsin.py` & `inewave-0.0.95/inewave/nwlistop/verturbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/vevmin.py` & `inewave-0.0.95/inewave/nwlistop/vevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/vevminm.py` & `inewave-0.0.95/inewave/nwlistop/vevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/vevminsin.py` & `inewave-0.0.95/inewave/nwlistop/vevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/vghmin.py` & `inewave-0.0.95/inewave/nwlistop/vghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/vghminm.py` & `inewave-0.0.95/inewave/nwlistop/vghminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/vghminsin.py` & `inewave-0.0.95/inewave/nwlistop/vghminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/vghminuh.py` & `inewave-0.0.95/inewave/nwlistop/vghminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave/nwlistop/vturuh.py` & `inewave-0.0.95/inewave/nwlistop/vturuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/inewave.egg-info/PKG-INFO` & `inewave-0.0.95/inewave.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inewave
-Version: 0.0.94
+Version: 0.0.95
 Summary: Interface para arquivos do NEWAVE
 Home-page: https://github.com/rjmalves/inewave
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `inewave-0.0.94/inewave.egg-info/SOURCES.txt` & `inewave-0.0.95/inewave.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 inewave/newave/eafpast.py
 inewave/newave/elnino.py
 inewave/newave/enavazb.py
 inewave/newave/enavazf.py
 inewave/newave/energiab.py
 inewave/newave/energiaf.py
 inewave/newave/energias.py
+inewave/newave/engnat.py
 inewave/newave/ensoaux.py
 inewave/newave/eolicacadastro.py
 inewave/newave/eolicaconfiguracao.py
 inewave/newave/eolicafte.py
 inewave/newave/eolicageracao.py
 inewave/newave/eolicahistorico.py
 inewave/newave/eolicaposto.py
@@ -67,14 +68,17 @@
 inewave/newave/parpvaz.py
 inewave/newave/patamar.py
 inewave/newave/penalid.py
 inewave/newave/perda.py
 inewave/newave/pmo.py
 inewave/newave/re.py
 inewave/newave/ree.py
+inewave/newave/restricaoeletrica.py
+inewave/newave/restricaoenergia.py
+inewave/newave/restricaovazao.py
 inewave/newave/sar.py
 inewave/newave/shist.py
 inewave/newave/sistema.py
 inewave/newave/tecno.py
 inewave/newave/term.py
 inewave/newave/vazaob.py
 inewave/newave/vazaof.py
@@ -104,14 +108,15 @@
 inewave/newave/modelos/eafpast.py
 inewave/newave/modelos/elnino.py
 inewave/newave/modelos/enavazb.py
 inewave/newave/modelos/enavazf.py
 inewave/newave/modelos/energiab.py
 inewave/newave/modelos/energiaf.py
 inewave/newave/modelos/energias.py
+inewave/newave/modelos/engnat.py
 inewave/newave/modelos/ensoaux.py
 inewave/newave/modelos/eolicacadastro.py
 inewave/newave/modelos/eolicaconfiguracao.py
 inewave/newave/modelos/eolicafte.py
 inewave/newave/modelos/eolicageracao.py
 inewave/newave/modelos/eolicahistorico.py
 inewave/newave/modelos/eolicaposto.py
@@ -134,14 +139,17 @@
 inewave/newave/modelos/parpvaz.py
 inewave/newave/modelos/patamar.py
 inewave/newave/modelos/penalid.py
 inewave/newave/modelos/perda.py
 inewave/newave/modelos/pmo.py
 inewave/newave/modelos/re.py
 inewave/newave/modelos/ree.py
+inewave/newave/modelos/restricaoeletrica.py
+inewave/newave/modelos/restricaoenergia.py
+inewave/newave/modelos/restricaovazao.py
 inewave/newave/modelos/sar.py
 inewave/newave/modelos/shist.py
 inewave/newave/modelos/sistema.py
 inewave/newave/modelos/tecno.py
 inewave/newave/modelos/term.py
 inewave/newave/modelos/vazaob.py
 inewave/newave/modelos/vazaof.py
@@ -449,14 +457,17 @@
 tests/mocks/arquivos/perdfm.py
 tests/mocks/arquivos/perdfsin.py
 tests/mocks/arquivos/pmo.py
 tests/mocks/arquivos/qafluh.py
 tests/mocks/arquivos/qincruh.py
 tests/mocks/arquivos/re.py
 tests/mocks/arquivos/ree.py
+tests/mocks/arquivos/restricaoeletrica.py
+tests/mocks/arquivos/restricaoenergia.py
+tests/mocks/arquivos/restricaovazao.py
 tests/mocks/arquivos/rhslppdf.py
 tests/mocks/arquivos/rhslpptb.py
 tests/mocks/arquivos/sistema.py
 tests/mocks/arquivos/term.py
 tests/mocks/arquivos/vagua.py
 tests/mocks/arquivos/varmpuh.py
 tests/mocks/arquivos/varmuh.py
@@ -491,14 +502,15 @@
 tests/newave/test_dsvagua.py
 tests/newave/test_eafpast.py
 tests/newave/test_enavazb.py
 tests/newave/test_enavazf.py
 tests/newave/test_energiab.py
 tests/newave/test_energiaf.py
 tests/newave/test_energias.py
+tests/newave/test_engnat.py
 tests/newave/test_eolicacadastro.py
 tests/newave/test_eolicaconfiguracao.py
 tests/newave/test_eolicafte.py
 tests/newave/test_eolicageracao.py
 tests/newave/test_eolicahistorico.py
 tests/newave/test_eolicaposto.py
 tests/newave/test_eolicasubmercado.py
@@ -513,14 +525,17 @@
 tests/newave/test_parpeol.py
 tests/newave/test_parpvaz.py
 tests/newave/test_patamar.py
 tests/newave/test_penalid.py
 tests/newave/test_pmo.py
 tests/newave/test_re.py
 tests/newave/test_ree.py
+tests/newave/test_restricaoeletrica.py
+tests/newave/test_restricaoenergia.py
+tests/newave/test_restricaovazao.py
 tests/newave/test_sistema.py
 tests/newave/test_term.py
 tests/newave/test_vazaob.py
 tests/newave/test_vazaof.py
 tests/newave/test_vazaos.py
 tests/newave/test_vazoes.py
 tests/newave/test_vazpast.py
```

### Comparing `inewave-0.0.94/setup.py` & `inewave-0.0.95/setup.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/adterm.py` & `inewave-0.0.95/tests/mocks/arquivos/adterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/arquivos.py` & `inewave-0.0.95/tests/mocks/arquivos/arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/avl_cortesfpha_nwv.py` & `inewave-0.0.95/tests/mocks/arquivos/avl_cortesfpha_nwv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/avl_desvfpha_s.py` & `inewave-0.0.95/tests/mocks/arquivos/avl_desvfpha_s.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/avl_desvfpha_v_q.py` & `inewave-0.0.95/tests/mocks/arquivos/avl_desvfpha_v_q.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/cadic.py` & `inewave-0.0.95/tests/mocks/arquivos/cadic.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/cdef.py` & `inewave-0.0.95/tests/mocks/arquivos/cdef.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/cdefsin.py` & `inewave-0.0.95/tests/mocks/arquivos/cdefsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/clast.py` & `inewave-0.0.95/tests/mocks/arquivos/clast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/cmarg.py` & `inewave-0.0.95/tests/mocks/arquivos/cmarg.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/cmargmed.py` & `inewave-0.0.95/tests/mocks/arquivos/cmargmed.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/confhd.py` & `inewave-0.0.95/tests/mocks/arquivos/confhd.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/conft.py` & `inewave-0.0.95/tests/mocks/arquivos/conft.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/coper.py` & `inewave-0.0.95/tests/mocks/arquivos/coper.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/corteolm.py` & `inewave-0.0.95/tests/mocks/arquivos/corteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/cterm.py` & `inewave-0.0.95/tests/mocks/arquivos/cterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/ctermsin.py` & `inewave-0.0.95/tests/mocks/arquivos/ctermsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/curva.py` & `inewave-0.0.95/tests/mocks/arquivos/curva.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/cvar.py` & `inewave-0.0.95/tests/mocks/arquivos/cvar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/deficit.py` & `inewave-0.0.95/tests/mocks/arquivos/deficit.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/defsin.py` & `inewave-0.0.95/tests/mocks/arquivos/defsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/depminuh.py` & `inewave-0.0.95/tests/mocks/arquivos/depminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/dfphauh.py` & `inewave-0.0.95/tests/mocks/arquivos/dfphauh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/dger.py` & `inewave-0.0.95/tests/mocks/arquivos/dger.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/dlppdfmax.py` & `inewave-0.0.95/tests/mocks/arquivos/dlppdfmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/dlppdfmaxm.py` & `inewave-0.0.95/tests/mocks/arquivos/dlppdfmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/dlppdfmaxs.py` & `inewave-0.0.95/tests/mocks/arquivos/dlppdfmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/dlpptbmax.py` & `inewave-0.0.95/tests/mocks/arquivos/dlpptbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/dlpptbmaxm.py` & `inewave-0.0.95/tests/mocks/arquivos/dlpptbmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/dlpptbmaxs.py` & `inewave-0.0.95/tests/mocks/arquivos/dlpptbmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/dsvagua.py` & `inewave-0.0.95/tests/mocks/arquivos/dsvagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/dtbmax.py` & `inewave-0.0.95/tests/mocks/arquivos/dtbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/dtbmin.py` & `inewave-0.0.95/tests/mocks/arquivos/dtbmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/dvazmax.py` & `inewave-0.0.95/tests/mocks/arquivos/dvazmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/eaf.py` & `inewave-0.0.95/tests/mocks/arquivos/eaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/eafb.py` & `inewave-0.0.95/tests/mocks/arquivos/eafb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/eafbm.py` & `inewave-0.0.95/tests/mocks/arquivos/eafbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/eafbsin.py` & `inewave-0.0.95/tests/mocks/arquivos/eafbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/eafm.py` & `inewave-0.0.95/tests/mocks/arquivos/eafm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/eafpast.py` & `inewave-0.0.95/tests/mocks/arquivos/eafpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/earmf.py` & `inewave-0.0.95/tests/mocks/arquivos/earmf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/earmfm.py` & `inewave-0.0.95/tests/mocks/arquivos/earmfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/earmfp.py` & `inewave-0.0.95/tests/mocks/arquivos/earmfp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/earmfpm.py` & `inewave-0.0.95/tests/mocks/arquivos/earmfpm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/earmfpsin.py` & `inewave-0.0.95/tests/mocks/arquivos/earmfpsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/earmfsin.py` & `inewave-0.0.95/tests/mocks/arquivos/earmfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/eolicacadastro.py` & `inewave-0.0.95/tests/mocks/arquivos/eolicacadastro.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/eolicaconfig.py` & `inewave-0.0.95/tests/mocks/arquivos/eolicaconfig.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/eolicafte.py` & `inewave-0.0.95/tests/mocks/arquivos/eolicafte.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/eolicageracao.py` & `inewave-0.0.95/tests/mocks/arquivos/eolicageracao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/eolicahistorico.py` & `inewave-0.0.95/tests/mocks/arquivos/eolicahistorico.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/eolicaposto.py` & `inewave-0.0.95/tests/mocks/arquivos/eolicaposto.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/estados.py` & `inewave-0.0.95/tests/mocks/arquivos/estados.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/evert.py` & `inewave-0.0.95/tests/mocks/arquivos/evert.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/evertm.py` & `inewave-0.0.95/tests/mocks/arquivos/evertm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/evertsin.py` & `inewave-0.0.95/tests/mocks/arquivos/evertsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/exces.py` & `inewave-0.0.95/tests/mocks/arquivos/exces.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/excessin.py` & `inewave-0.0.95/tests/mocks/arquivos/excessin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/exph.py` & `inewave-0.0.95/tests/mocks/arquivos/exph.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/fteolm.py` & `inewave-0.0.95/tests/mocks/arquivos/fteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/fteolsin.py` & `inewave-0.0.95/tests/mocks/arquivos/fteolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/geol.py` & `inewave-0.0.95/tests/mocks/arquivos/geol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/geolm.py` & `inewave-0.0.95/tests/mocks/arquivos/geolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/geolsin.py` & `inewave-0.0.95/tests/mocks/arquivos/geolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/ghiduh.py` & `inewave-0.0.95/tests/mocks/arquivos/ghiduh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/ghmax.py` & `inewave-0.0.95/tests/mocks/arquivos/ghmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/ghmaxm.py` & `inewave-0.0.95/tests/mocks/arquivos/ghmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/ghmaxmr.py` & `inewave-0.0.95/tests/mocks/arquivos/ghmaxmr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/ghmaxr.py` & `inewave-0.0.95/tests/mocks/arquivos/ghmaxr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/ghmaxrsin.py` & `inewave-0.0.95/tests/mocks/arquivos/ghmaxrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/ghmaxsin.py` & `inewave-0.0.95/tests/mocks/arquivos/ghmaxsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/ghtot.py` & `inewave-0.0.95/tests/mocks/arquivos/ghtot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/ghtotm.py` & `inewave-0.0.95/tests/mocks/arquivos/ghtotm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/ghtotsin.py` & `inewave-0.0.95/tests/mocks/arquivos/ghtotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/gttot.py` & `inewave-0.0.95/tests/mocks/arquivos/gttot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/gttotsin.py` & `inewave-0.0.95/tests/mocks/arquivos/gttotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/intercambio.py` & `inewave-0.0.95/tests/mocks/arquivos/intercambio.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/invade.py` & `inewave-0.0.95/tests/mocks/arquivos/invade.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/invadem.py` & `inewave-0.0.95/tests/mocks/arquivos/invadem.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/mercl.py` & `inewave-0.0.95/tests/mocks/arquivos/mercl.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/merclsin.py` & `inewave-0.0.95/tests/mocks/arquivos/merclsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/modif.py` & `inewave-0.0.95/tests/mocks/arquivos/modif.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/newavetim.py` & `inewave-0.0.95/tests/mocks/arquivos/newavetim.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/nwlistcf.py` & `inewave-0.0.95/tests/mocks/arquivos/nwlistcf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/nwv_avl_evap.py` & `inewave-0.0.95/tests/mocks/arquivos/nwv_avl_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/nwv_cortes_evap.py` & `inewave-0.0.95/tests/mocks/arquivos/nwv_cortes_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/nwv_eco_evap.py` & `inewave-0.0.95/tests/mocks/arquivos/nwv_eco_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/parp.py` & `inewave-0.0.95/tests/mocks/arquivos/parp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/parpeol.py` & `inewave-0.0.95/tests/mocks/arquivos/parpeol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/parpvaz.py` & `inewave-0.0.95/tests/mocks/arquivos/parpvaz.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/patamar.py` & `inewave-0.0.95/tests/mocks/arquivos/patamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/penalid.py` & `inewave-0.0.95/tests/mocks/arquivos/penalid.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/perdf.py` & `inewave-0.0.95/tests/mocks/arquivos/perdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/perdfm.py` & `inewave-0.0.95/tests/mocks/arquivos/perdfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/perdfsin.py` & `inewave-0.0.95/tests/mocks/arquivos/perdfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/pmo.py` & `inewave-0.0.95/tests/mocks/arquivos/pmo.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/qafluh.py` & `inewave-0.0.95/tests/mocks/arquivos/qafluh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/qincruh.py` & `inewave-0.0.95/tests/mocks/arquivos/qincruh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/re.py` & `inewave-0.0.95/tests/mocks/arquivos/re.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/ree.py` & `inewave-0.0.95/tests/mocks/arquivos/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/rhslppdf.py` & `inewave-0.0.95/tests/mocks/arquivos/rhslppdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/rhslpptb.py` & `inewave-0.0.95/tests/mocks/arquivos/rhslpptb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/sistema.py` & `inewave-0.0.95/tests/mocks/arquivos/sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/term.py` & `inewave-0.0.95/tests/mocks/arquivos/term.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/vagua.py` & `inewave-0.0.95/tests/mocks/arquivos/vagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/varmpuh.py` & `inewave-0.0.95/tests/mocks/arquivos/varmpuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/varmuh.py` & `inewave-0.0.95/tests/mocks/arquivos/varmuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/vazpast.py` & `inewave-0.0.95/tests/mocks/arquivos/vazpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/vento.py` & `inewave-0.0.95/tests/mocks/arquivos/vento.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/vertuh.py` & `inewave-0.0.95/tests/mocks/arquivos/vertuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/verturb.py` & `inewave-0.0.95/tests/mocks/arquivos/verturb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/verturbm.py` & `inewave-0.0.95/tests/mocks/arquivos/verturbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/verturbsin.py` & `inewave-0.0.95/tests/mocks/arquivos/verturbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/vevmin.py` & `inewave-0.0.95/tests/mocks/arquivos/vevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/vevminm.py` & `inewave-0.0.95/tests/mocks/arquivos/vevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/vevminsin.py` & `inewave-0.0.95/tests/mocks/arquivos/vevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/vghmin.py` & `inewave-0.0.95/tests/mocks/arquivos/vghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/vghminm.py` & `inewave-0.0.95/tests/mocks/arquivos/vghminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/vghminsin.py` & `inewave-0.0.95/tests/mocks/arquivos/vghminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/vghminuh.py` & `inewave-0.0.95/tests/mocks/arquivos/vghminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/arquivos/vturuh.py` & `inewave-0.0.95/tests/mocks/arquivos/vturuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/mocks/mock_open.py` & `inewave-0.0.95/tests/mocks/mock_open.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_adterm.py` & `inewave-0.0.95/tests/newave/test_adterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_arquivos.py` & `inewave-0.0.95/tests/newave/test_arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_avl_cortesfpha_nwv.py` & `inewave-0.0.95/tests/newave/test_avl_cortesfpha_nwv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_avl_desvfpha_s.py` & `inewave-0.0.95/tests/newave/test_avl_desvfpha_s.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_avl_desvfpha_v_q.py` & `inewave-0.0.95/tests/newave/test_avl_desvfpha_v_q.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_cadic.py` & `inewave-0.0.95/tests/newave/test_cadic.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_caso.py` & `inewave-0.0.95/tests/newave/test_caso.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_clast.py` & `inewave-0.0.95/tests/newave/test_clast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_confhd.py` & `inewave-0.0.95/tests/newave/test_confhd.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_conft.py` & `inewave-0.0.95/tests/newave/test_conft.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_curva.py` & `inewave-0.0.95/tests/newave/test_curva.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_cvar.py` & `inewave-0.0.95/tests/newave/test_cvar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_dger.py` & `inewave-0.0.95/tests/newave/test_dger.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_dsvagua.py` & `inewave-0.0.95/tests/newave/test_dsvagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_eafpast.py` & `inewave-0.0.95/tests/newave/test_eafpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_enavazb.py` & `inewave-0.0.95/tests/newave/test_enavazb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_enavazf.py` & `inewave-0.0.95/tests/newave/test_enavazf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_energiab.py` & `inewave-0.0.95/tests/newave/test_energiab.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_energiaf.py` & `inewave-0.0.95/tests/newave/test_energiaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_energias.py` & `inewave-0.0.95/tests/newave/test_energias.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_eolicacadastro.py` & `inewave-0.0.95/tests/newave/test_eolicacadastro.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_eolicaconfiguracao.py` & `inewave-0.0.95/tests/newave/test_eolicaconfiguracao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_eolicafte.py` & `inewave-0.0.95/tests/newave/test_eolicafte.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_eolicageracao.py` & `inewave-0.0.95/tests/newave/test_eolicageracao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_eolicahistorico.py` & `inewave-0.0.95/tests/newave/test_eolicahistorico.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_eolicaposto.py` & `inewave-0.0.95/tests/newave/test_eolicaposto.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_eolicasubmercado.py` & `inewave-0.0.95/tests/newave/test_eolicasubmercado.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_exph.py` & `inewave-0.0.95/tests/newave/test_exph.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_hidr.py` & `inewave-0.0.95/tests/newave/test_hidr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_modif.py` & `inewave-0.0.95/tests/newave/test_modif.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_newavetim.py` & `inewave-0.0.95/tests/newave/test_newavetim.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_nwv_avl_evap.py` & `inewave-0.0.95/tests/newave/test_nwv_avl_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_nwv_cortes_evap.py` & `inewave-0.0.95/tests/newave/test_nwv_cortes_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_nwv_eco_evap.py` & `inewave-0.0.95/tests/newave/test_nwv_eco_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_parp.py` & `inewave-0.0.95/tests/newave/test_parp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_parpeol.py` & `inewave-0.0.95/tests/newave/test_parpeol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_parpvaz.py` & `inewave-0.0.95/tests/newave/test_parpvaz.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_patamar.py` & `inewave-0.0.95/tests/newave/test_patamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_penalid.py` & `inewave-0.0.95/tests/newave/test_penalid.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_pmo.py` & `inewave-0.0.95/tests/newave/test_pmo.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 def test_leitura_produtibilidades():
     m: MagicMock = mock_open(read_data="".join(MockBlocoProdutibilidadesPMO))
     b = BlocoProdutibilidadesConfiguracaoPMO()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
-    assert len(list(b.data.index)) == 1148
+    assert len(list(b.data.index)) == 1312
     assert b.data.iloc[1, 1] == 1
     assert b.data.iloc[1, 2] == 0.4483
     assert b.data.iloc[1, 3] == 0.4334
     assert b.data.iloc[1, 4] == 0.4005
     assert b.data.iloc[1, 5] == 0.4625
     assert b.data.iloc[1, 6] == 0.4886
     assert b.data.iloc[1, 7] == 2.2083
```

### Comparing `inewave-0.0.94/tests/newave/test_re.py` & `inewave-0.0.95/tests/newave/test_re.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_ree.py` & `inewave-0.0.95/tests/newave/test_ree.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_sistema.py` & `inewave-0.0.95/tests/newave/test_sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_term.py` & `inewave-0.0.95/tests/newave/test_term.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_vazaob.py` & `inewave-0.0.95/tests/newave/test_vazaob.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_vazaof.py` & `inewave-0.0.95/tests/newave/test_vazaof.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_vazaos.py` & `inewave-0.0.95/tests/newave/test_vazaos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_vazoes.py` & `inewave-0.0.95/tests/newave/test_vazoes.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/newave/test_vazpast.py` & `inewave-0.0.95/tests/newave/test_vazpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistcf/test_estados.py` & `inewave-0.0.95/tests/nwlistcf/test_estados.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistcf/test_nwlistcf.py` & `inewave-0.0.95/tests/nwlistcf/test_nwlistcf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_cdef.py` & `inewave-0.0.95/tests/nwlistop/test_cdef.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_cdefsin.py` & `inewave-0.0.95/tests/nwlistop/test_cdefsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_cmarg.py` & `inewave-0.0.95/tests/nwlistop/test_cmarg.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_cmargmed.py` & `inewave-0.0.95/tests/nwlistop/test_cmargmed.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_coper.py` & `inewave-0.0.95/tests/nwlistop/test_coper.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_corteolm.py` & `inewave-0.0.95/tests/nwlistop/test_corteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_cterm.py` & `inewave-0.0.95/tests/nwlistop/test_cterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_ctermsin.py` & `inewave-0.0.95/tests/nwlistop/test_ctermsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_deficit.py` & `inewave-0.0.95/tests/nwlistop/test_deficit.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_defsin.py` & `inewave-0.0.95/tests/nwlistop/test_defsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_depminuh.py` & `inewave-0.0.95/tests/nwlistop/test_depminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_dfphauh.py` & `inewave-0.0.95/tests/nwlistop/test_dfphauh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_dlppdfmax.py` & `inewave-0.0.95/tests/nwlistop/test_dlppdfmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_dlppdfmaxm.py` & `inewave-0.0.95/tests/nwlistop/test_dlppdfmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_dlppdfmaxs.py` & `inewave-0.0.95/tests/nwlistop/test_dlppdfmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_dlpptbmax.py` & `inewave-0.0.95/tests/nwlistop/test_dlpptbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_dlpptbmaxm.py` & `inewave-0.0.95/tests/nwlistop/test_dlpptbmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_dlpptbmaxs.py` & `inewave-0.0.95/tests/nwlistop/test_dlpptbmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_dtbmax.py` & `inewave-0.0.95/tests/nwlistop/test_dtbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_dtbmin.py` & `inewave-0.0.95/tests/nwlistop/test_dtbmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_dvazmax.py` & `inewave-0.0.95/tests/nwlistop/test_dvazmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_eaf.py` & `inewave-0.0.95/tests/nwlistop/test_eaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_eafb.py` & `inewave-0.0.95/tests/nwlistop/test_eafb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_eafbm.py` & `inewave-0.0.95/tests/nwlistop/test_eafbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_eafbsin.py` & `inewave-0.0.95/tests/nwlistop/test_eafbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_eafm.py` & `inewave-0.0.95/tests/nwlistop/test_eafm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_earmf.py` & `inewave-0.0.95/tests/nwlistop/test_earmf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_earmfm.py` & `inewave-0.0.95/tests/nwlistop/test_earmfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_earmfp.py` & `inewave-0.0.95/tests/nwlistop/test_earmfp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_earmfpm.py` & `inewave-0.0.95/tests/nwlistop/test_earmfpm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_earmfpsin.py` & `inewave-0.0.95/tests/nwlistop/test_earmfpsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_earmfsin.py` & `inewave-0.0.95/tests/nwlistop/test_earmfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_evert.py` & `inewave-0.0.95/tests/nwlistop/test_evert.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_evertm.py` & `inewave-0.0.95/tests/nwlistop/test_evertm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_evertsin.py` & `inewave-0.0.95/tests/nwlistop/test_evertsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_exces.py` & `inewave-0.0.95/tests/nwlistop/test_exces.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_excessin.py` & `inewave-0.0.95/tests/nwlistop/test_excessin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_fteolm.py` & `inewave-0.0.95/tests/nwlistop/test_fteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_fteolsin.py` & `inewave-0.0.95/tests/nwlistop/test_fteolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_geol.py` & `inewave-0.0.95/tests/nwlistop/test_geol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_geolm.py` & `inewave-0.0.95/tests/nwlistop/test_geolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_geolsin.py` & `inewave-0.0.95/tests/nwlistop/test_geolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_ghiduh.py` & `inewave-0.0.95/tests/nwlistop/test_ghiduh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_ghmax.py` & `inewave-0.0.95/tests/nwlistop/test_ghmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_ghmaxm.py` & `inewave-0.0.95/tests/nwlistop/test_ghmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_ghmaxmr.py` & `inewave-0.0.95/tests/nwlistop/test_ghmaxmr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_ghmaxr.py` & `inewave-0.0.95/tests/nwlistop/test_ghmaxr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_ghmaxrsin.py` & `inewave-0.0.95/tests/nwlistop/test_ghmaxrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_ghmaxsin.py` & `inewave-0.0.95/tests/nwlistop/test_ghmaxsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_ghtot.py` & `inewave-0.0.95/tests/nwlistop/test_ghtot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_ghtotm.py` & `inewave-0.0.95/tests/nwlistop/test_ghtotm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_ghtotsin.py` & `inewave-0.0.95/tests/nwlistop/test_ghtotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_gttot.py` & `inewave-0.0.95/tests/nwlistop/test_gttot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_gttotsin.py` & `inewave-0.0.95/tests/nwlistop/test_gttotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_intercambio.py` & `inewave-0.0.95/tests/nwlistop/test_intercambio.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_invade.py` & `inewave-0.0.95/tests/nwlistop/test_invade.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_invadem.py` & `inewave-0.0.95/tests/nwlistop/test_invadem.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_mercl.py` & `inewave-0.0.95/tests/nwlistop/test_mercl.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_merclsin.py` & `inewave-0.0.95/tests/nwlistop/test_merclsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_perdf.py` & `inewave-0.0.95/tests/nwlistop/test_perdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_perdfm.py` & `inewave-0.0.95/tests/nwlistop/test_perdfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_perdfsin.py` & `inewave-0.0.95/tests/nwlistop/test_perdfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_qafluh.py` & `inewave-0.0.95/tests/nwlistop/test_qafluh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_qincruh.py` & `inewave-0.0.95/tests/nwlistop/test_qincruh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_rhslppdf.py` & `inewave-0.0.95/tests/nwlistop/test_rhslppdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_rhslpptb.py` & `inewave-0.0.95/tests/nwlistop/test_rhslpptb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_vagua.py` & `inewave-0.0.95/tests/nwlistop/test_vagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_varmpuh.py` & `inewave-0.0.95/tests/nwlistop/test_varmpuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_varmuh.py` & `inewave-0.0.95/tests/nwlistop/test_varmuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_vento.py` & `inewave-0.0.95/tests/nwlistop/test_vento.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_vertuh.py` & `inewave-0.0.95/tests/nwlistop/test_vertuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_verturb.py` & `inewave-0.0.95/tests/nwlistop/test_verturb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_verturbm.py` & `inewave-0.0.95/tests/nwlistop/test_verturbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_verturbsin.py` & `inewave-0.0.95/tests/nwlistop/test_verturbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_vevmin.py` & `inewave-0.0.95/tests/nwlistop/test_vevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_vevminm.py` & `inewave-0.0.95/tests/nwlistop/test_vevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_vevminsin.py` & `inewave-0.0.95/tests/nwlistop/test_vevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_vghmin.py` & `inewave-0.0.95/tests/nwlistop/test_vghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_vghminm.py` & `inewave-0.0.95/tests/nwlistop/test_vghminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_vghminsin.py` & `inewave-0.0.95/tests/nwlistop/test_vghminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_vghminuh.py` & `inewave-0.0.95/tests/nwlistop/test_vghminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.94/tests/nwlistop/test_vturuh.py` & `inewave-0.0.95/tests/nwlistop/test_vturuh.py`

 * *Files identical despite different names*

