# Comparing `tmp/ypricemagic-2.2.0.tar.gz` & `tmp/ypricemagic-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ypricemagic-2.2.0.tar", last modified: Mon Apr 24 20:25:19 2023, max compression
+gzip compressed data, was "ypricemagic-2.2.1.tar", last modified: Wed Apr 26 20:51:15 2023, max compression
```

## Comparing `ypricemagic-2.2.0.tar` & `ypricemagic-2.2.1.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.352266 ypricemagic-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/.env.sample
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.336266 ypricemagic-2.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.340266 ypricemagic-2.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2891 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-04-24 20:25:19.352266 ypricemagic-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      776 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-24 20:25:19.352266 ypricemagic-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.340266 ypricemagic-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.340266 ypricemagic-2.2.0/tests/classes/
--rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/classes/test_erc20.py
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/classes/test_singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.340266 ypricemagic-2.2.0/tests/prices/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/tests/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/dex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/dex/test_balancer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/dex/test_uniswap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/tests/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6458 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/lending/test_aave.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/lending/test_compound.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/tests/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/stable_swap/test_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/test_chainlink.py
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/test_gearbox.py
--rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/test_magic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/test_popsicle.py
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/test_synthetix.py
--rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/test_yearn.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/tests/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/tokenized_fund/test_piedao.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/tests/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/utils/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/test_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/y/
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/y/classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7773 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/classes/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/classes/singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)     9873 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    20009 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/contracts.py
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/convert.py
--rw-r--r--   0 runner    (1001) docker     (122)      576 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/erc20.py
--rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/y/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)     6400 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/ERC20.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/y/interfaces/balancer/
--rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/balancer/WeightedPool.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/balancer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/y/interfaces/compound/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32517 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/compound/unitroller.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/y/interfaces/curve/
--rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/curve/CurveRegistry.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/curve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/multicall2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/y/interfaces/uniswap/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/uniswap/factoryv2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/uniswap/quoterv3.py
--rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/networks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.348266 ypricemagic-2.2.0/y/prices/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/band.py
--rw-r--r--   0 runner    (1001) docker     (122)    19656 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/chainlink.py
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/convex.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.348266 ypricemagic-2.2.0/y/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.348266 ypricemagic-2.2.0/y/prices/dex/balancer/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/balancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/balancer/balancer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/balancer/v1.py
--rw-r--r--   0 runner    (1001) docker     (122)    10453 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/balancer/v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/genericamm.py
--rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/mooniswap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.348266 ypricemagic-2.2.0/y/prices/dex/uniswap/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6370 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/uniswap/uniswap.py
--rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/uniswap/v1.py
--rw-r--r--   0 runner    (1001) docker     (122)    23291 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/uniswap/v2.py
--rw-r--r--   0 runner    (1001) docker     (122)    12588 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/uniswap/v2_forks.py
--rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/uniswap/v3.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.348266 ypricemagic-2.2.0/y/prices/eth_derivs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/eth_derivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/eth_derivs/creth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/eth_derivs/wsteth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2940 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/gearbox.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.348266 ypricemagic-2.2.0/y/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6880 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/lending/aave.py
--rw-r--r--   0 runner    (1001) docker     (122)    10528 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/lending/compound.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/lending/ib.py
--rw-r--r--   0 runner    (1001) docker     (122)    11292 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/magic.py
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/one_to_one.py
--rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/popsicle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.348266 ypricemagic-2.2.0/y/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/stable_swap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/stable_swap/belt.py
--rw-r--r--   0 runner    (1001) docker     (122)    21688 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/stable_swap/curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/stable_swap/ellipsis.py
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/stable_swap/froyo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/stable_swap/mstablefeederpool.py
--rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/stable_swap/saddle.py
--rw-r--r--   0 runner    (1001) docker     (122)     3852 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/synthetix.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.348266 ypricemagic-2.2.0/y/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/tokenized_fund/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/tokenized_fund/basketdao.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/tokenized_fund/gelato.py
--rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/tokenized_fund/piedao.py
--rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/tokenized_fund/tokensets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.348266 ypricemagic-2.2.0/y/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4650 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/utils/buckets.py
--rw-r--r--   0 runner    (1001) docker     (122)     8555 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/utils/sense_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     3853 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/utils/ypriceapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     5853 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/yearn.py
--rw-r--r--   0 runner    (1001) docker     (122)     4343 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.352266 ypricemagic-2.2.0/y/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/utils/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/utils/dank_mids.py
--rw-r--r--   0 runner    (1001) docker     (122)     7970 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/utils/events.py
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/utils/fakes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     2560 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/utils/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)    11228 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/utils/multicall.py
--rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/utils/raw_calls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.352266 ypricemagic-2.2.0/ypricemagic/
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/ypricemagic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/ypricemagic/magic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.352266 ypricemagic-2.2.0/ypricemagic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-04-24 20:25:19.000000 ypricemagic-2.2.0/ypricemagic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-04-24 20:25:19.000000 ypricemagic-2.2.0/ypricemagic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-24 20:25:19.000000 ypricemagic-2.2.0/ypricemagic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-24 20:25:19.000000 ypricemagic-2.2.0/ypricemagic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-24 20:25:19.000000 ypricemagic-2.2.0/ypricemagic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.026847 ypricemagic-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/.env.sample
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:14.994847 ypricemagic-2.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.006847 ypricemagic-2.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2891 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-04-26 20:51:15.026847 ypricemagic-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      776 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-26 20:51:15.026847 ypricemagic-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.006847 ypricemagic-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.006847 ypricemagic-2.2.1/tests/classes/
+-rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/tests/classes/test_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/tests/classes/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.010847 ypricemagic-2.2.1/tests/prices/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/tests/prices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.010847 ypricemagic-2.2.1/tests/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/tests/prices/dex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/tests/prices/dex/test_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/tests/prices/dex/test_uniswap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.010847 ypricemagic-2.2.1/tests/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/tests/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6458 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/tests/prices/lending/test_aave.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/tests/prices/lending/test_compound.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.010847 ypricemagic-2.2.1/tests/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/tests/prices/stable_swap/test_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/tests/prices/test_chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/tests/prices/test_gearbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/tests/prices/test_magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/tests/prices/test_popsicle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/tests/prices/test_synthetix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/tests/prices/test_yearn.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.010847 ypricemagic-2.2.1/tests/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/tests/prices/tokenized_fund/test_piedao.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.010847 ypricemagic-2.2.1/tests/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/tests/prices/utils/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/tests/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.010847 ypricemagic-2.2.1/y/
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.014847 ypricemagic-2.2.1/y/classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7773 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/classes/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/classes/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9873 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20058 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      576 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/erc20.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.014847 ypricemagic-2.2.1/y/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     6400 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/interfaces/ERC20.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.014847 ypricemagic-2.2.1/y/interfaces/balancer/
+-rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/interfaces/balancer/WeightedPool.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/interfaces/balancer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.014847 ypricemagic-2.2.1/y/interfaces/compound/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/interfaces/compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32517 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/interfaces/compound/unitroller.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.014847 ypricemagic-2.2.1/y/interfaces/curve/
+-rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/interfaces/curve/CurveRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/interfaces/curve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/interfaces/multicall2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.014847 ypricemagic-2.2.1/y/interfaces/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/interfaces/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/interfaces/uniswap/factoryv2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/interfaces/uniswap/quoterv3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/networks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.018847 ypricemagic-2.2.1/y/prices/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/band.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19845 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/convex.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.018847 ypricemagic-2.2.1/y/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/dex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.018847 ypricemagic-2.2.1/y/prices/dex/balancer/
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/dex/balancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/dex/balancer/balancer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/dex/balancer/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10453 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/dex/balancer/v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/dex/genericamm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/dex/mooniswap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.018847 ypricemagic-2.2.1/y/prices/dex/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/dex/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6370 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/dex/uniswap/uniswap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/dex/uniswap/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23291 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/dex/uniswap/v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12588 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/dex/uniswap/v2_forks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/dex/uniswap/v3.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.018847 ypricemagic-2.2.1/y/prices/eth_derivs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/eth_derivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/eth_derivs/creth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/eth_derivs/wsteth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2940 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/gearbox.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.018847 ypricemagic-2.2.1/y/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6880 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/lending/aave.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10528 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/lending/compound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/lending/ib.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11292 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/one_to_one.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/popsicle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.022847 ypricemagic-2.2.1/y/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/stable_swap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/stable_swap/belt.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21801 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/stable_swap/curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/stable_swap/ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/stable_swap/froyo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/stable_swap/mstablefeederpool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/stable_swap/saddle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3852 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.022847 ypricemagic-2.2.1/y/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/tokenized_fund/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/tokenized_fund/basketdao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/tokenized_fund/gelato.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/tokenized_fund/piedao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/tokenized_fund/tokensets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.022847 ypricemagic-2.2.1/y/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4650 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/utils/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8555 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/utils/sense_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3853 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/utils/ypriceapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5853 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/prices/yearn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4343 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.022847 ypricemagic-2.2.1/y/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/utils/dank_mids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7970 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/utils/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/utils/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2560 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/utils/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11228 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/utils/multicall.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/y/utils/raw_calls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.022847 ypricemagic-2.2.1/ypricemagic/
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/ypricemagic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-04-26 20:50:59.000000 ypricemagic-2.2.1/ypricemagic/magic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:51:15.026847 ypricemagic-2.2.1/ypricemagic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-04-26 20:51:14.000000 ypricemagic-2.2.1/ypricemagic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-04-26 20:51:14.000000 ypricemagic-2.2.1/ypricemagic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 20:51:14.000000 ypricemagic-2.2.1/ypricemagic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-26 20:51:14.000000 ypricemagic-2.2.1/ypricemagic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-26 20:51:14.000000 ypricemagic-2.2.1/ypricemagic.egg-info/top_level.txt
```

### Comparing `ypricemagic-2.2.0/.github/workflows/codeql-analysis.yml` & `ypricemagic-2.2.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/.github/workflows/pytest.yaml` & `ypricemagic-2.2.1/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/.github/workflows/release.yaml` & `ypricemagic-2.2.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/LICENSE.txt` & `ypricemagic-2.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/README.md` & `ypricemagic-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/setup.py` & `ypricemagic-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/tests/classes/test_erc20.py` & `ypricemagic-2.2.1/tests/classes/test_erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/tests/classes/test_singleton.py` & `ypricemagic-2.2.1/tests/classes/test_singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/tests/fixtures.py` & `ypricemagic-2.2.1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/tests/prices/dex/test_uniswap.py` & `ypricemagic-2.2.1/tests/prices/dex/test_uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/tests/prices/lending/test_aave.py` & `ypricemagic-2.2.1/tests/prices/lending/test_aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/tests/prices/lending/test_compound.py` & `ypricemagic-2.2.1/tests/prices/lending/test_compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/tests/prices/test_chainlink.py` & `ypricemagic-2.2.1/tests/prices/test_chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/tests/prices/test_magic.py` & `ypricemagic-2.2.1/tests/prices/test_magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/tests/prices/test_popsicle.py` & `ypricemagic-2.2.1/tests/prices/test_popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/tests/prices/test_synthetix.py` & `ypricemagic-2.2.1/tests/prices/test_synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/tests/prices/test_yearn.py` & `ypricemagic-2.2.1/tests/prices/test_yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/tests/prices/utils/test_buckets.py` & `ypricemagic-2.2.1/tests/prices/utils/test_buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/__init__.py` & `ypricemagic-2.2.1/y/__init__.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/classes/common.py` & `ypricemagic-2.2.1/y/classes/common.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/classes/singleton.py` & `ypricemagic-2.2.1/y/classes/singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/constants.py` & `ypricemagic-2.2.1/y/constants.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/contracts.py` & `ypricemagic-2.2.1/y/contracts.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,14 +207,15 @@
             except IndexError as e:
                 if str(e) == "pop from an empty deque":
                     raise CompilerError("y.Contract objects work best when we bypass compilers. In this case, it will *only* work when we bypass. Please ensure autofetch_sources=False in your brownie-config.yaml and rerun your script.")
                 raise e
             # If we don't already have the contract in the db, we'll try to fetch it from the explorer.
             except ValueError as e:
                 # TODO catch the specific error we expect, not all ValueErrors
+                logger.warning(f"{address} {e}")
                 try:                  
                     name, abi = _resolve_proxy(address)
                     build = {"abi": abi, "address": address, "contractName": name, "type": "contract"}
                     self.__init_from_abi__(build, owner=owner, persist=True)
                 except (ContractNotFound, ContractNotVerified) as e:
                     if require_success:
                         raise
```

### Comparing `ypricemagic-2.2.0/y/datatypes.py` & `ypricemagic-2.2.1/y/datatypes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/decorators.py` & `ypricemagic-2.2.1/y/decorators.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/erc20.py` & `ypricemagic-2.2.1/y/erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/exceptions.py` & `ypricemagic-2.2.1/y/exceptions.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/interfaces/ERC20.py` & `ypricemagic-2.2.1/y/interfaces/ERC20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/interfaces/balancer/WeightedPool.py` & `ypricemagic-2.2.1/y/interfaces/balancer/WeightedPool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/interfaces/compound/unitroller.py` & `ypricemagic-2.2.1/y/interfaces/compound/unitroller.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/interfaces/curve/CurveRegistry.py` & `ypricemagic-2.2.1/y/interfaces/curve/CurveRegistry.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/interfaces/multicall2.py` & `ypricemagic-2.2.1/y/interfaces/multicall2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/interfaces/uniswap/factoryv2.py` & `ypricemagic-2.2.1/y/interfaces/uniswap/factoryv2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/interfaces/uniswap/quoterv3.py` & `ypricemagic-2.2.1/y/interfaces/uniswap/quoterv3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/networks.py` & `ypricemagic-2.2.1/y/networks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/band.py` & `ypricemagic-2.2.1/y/prices/band.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/chainlink.py` & `ypricemagic-2.2.1/y/prices/chainlink.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,37 +172,37 @@
     def __init__(self, asynchronous: bool = False) -> None:
         self.asynchronous = asynchronous
         if chain.id in registries:
             self.registry = Contract(registries[chain.id])
         elif len(FEEDS) == 0:
             raise UnsupportedNetwork('chainlink is not supported on this network')
         self._cached_feeds = {ERC20(token, asynchronous=self.asynchronous): feed for token, feed in FEEDS.items()}
-        self._feeds_loaded = False
+        self._feeds_loaded = asyncio.Event()
         self._loading = False
     
     async def _start_feed_loop(self) -> Union[None, NoReturn]:
         if self._loading:
             return
 
         self._loading = True
         # for non-mainnet, we have no registry so must get feeds manually
         if chain.id not in registries:
-            self._feeds_loaded = True
+            self._feeds_loaded.set()
             self._loading = False
             return
 
         block = await dank_w3.eth.block_number
         # for mainnet, we have some extra feeds to pull in
         # cache feeds thru current block, log results.
         async for logs in get_logs_asap_generator(str(self.registry), [self.registry.topics['FeedConfirmed']], to_block=block):
             for log in decode_logs(logs):
                 if log['denomination'] == DENOMINATIONS['USD'] and log['latestAggregator'] != ZERO_ADDRESS:
                     self._cached_feeds[log["asset"]] = ERC20(log["latestAggregator"], asynchronous=self.asynchronous)
         
-        self._feeds_loaded = True
+        self._feeds_loaded.set()
         logger.info(f'loaded {len(self._cached_feeds)} feeds')
         
         while await dank_w3.eth.block_number < block+1:
             await asyncio.sleep(15)
 
         # leave coroutine running for future blocks
         async for logs in get_logs_asap_generator(str(self.registry), [self.registry.topics['FeedConfirmed']], from_block=block+1, run_forever=True):
@@ -210,18 +210,22 @@
                 if log['denomination'] == DENOMINATIONS['USD'] and log['latestAggregator'] != ZERO_ADDRESS:
                     asset, latest_aggregator = log["asset"], log["latestAggregator"]
                     self._cached_feeds[asset] = ERC20(latest_aggregator, asynchronous=self.asynchronous)
                     logger.info(f'loaded new feed {latest_aggregator}')
 
     @a_sync.aka.property
     async def feeds(self) -> Dict[ERC20, str]:
-        if not self._feeds_loaded:
-            asyncio.get_event_loop().create_task(self._start_feed_loop())
-        while not self._feeds_loaded:
-            await asyncio.sleep(0)
+        if not self._feeds_loaded.is_set():
+            task = asyncio.get_event_loop().create_task(self._start_feed_loop())
+            def _on_completion(fut):
+                if e:=fut.exception():
+                    self._loading = False
+                    raise e
+            task.add_done_callback(_on_completion)
+        await self._feeds_loaded.wait():
         return self._cached_feeds
     
     async def get_feed(self, asset: Address) -> Optional[Contract]:
         feeds = await self.__feeds__(sync=False)
         try:
             return await Contract.coroutine(feeds[convert.to_address(asset)])
         except ContractNotVerified:
```

### Comparing `ypricemagic-2.2.0/y/prices/convex.py` & `ypricemagic-2.2.1/y/prices/convex.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/dex/balancer/balancer.py` & `ypricemagic-2.2.1/y/prices/dex/balancer/balancer.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/dex/balancer/v1.py` & `ypricemagic-2.2.1/y/prices/dex/balancer/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/dex/balancer/v2.py` & `ypricemagic-2.2.1/y/prices/dex/balancer/v2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/dex/genericamm.py` & `ypricemagic-2.2.1/y/prices/dex/genericamm.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/dex/mooniswap.py` & `ypricemagic-2.2.1/y/prices/dex/mooniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/dex/uniswap/uniswap.py` & `ypricemagic-2.2.1/y/prices/dex/uniswap/uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/dex/uniswap/v1.py` & `ypricemagic-2.2.1/y/prices/dex/uniswap/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/dex/uniswap/v2.py` & `ypricemagic-2.2.1/y/prices/dex/uniswap/v2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/dex/uniswap/v2_forks.py` & `ypricemagic-2.2.1/y/prices/dex/uniswap/v2_forks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/dex/uniswap/v3.py` & `ypricemagic-2.2.1/y/prices/dex/uniswap/v3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/eth_derivs/creth.py` & `ypricemagic-2.2.1/y/prices/eth_derivs/creth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/eth_derivs/wsteth.py` & `ypricemagic-2.2.1/y/prices/eth_derivs/wsteth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/gearbox.py` & `ypricemagic-2.2.1/y/prices/gearbox.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/lending/aave.py` & `ypricemagic-2.2.1/y/prices/lending/aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/lending/compound.py` & `ypricemagic-2.2.1/y/prices/lending/compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/lending/ib.py` & `ypricemagic-2.2.1/y/prices/lending/ib.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/magic.py` & `ypricemagic-2.2.1/y/prices/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/one_to_one.py` & `ypricemagic-2.2.1/y/prices/one_to_one.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/popsicle.py` & `ypricemagic-2.2.1/y/prices/popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/stable_swap/belt.py` & `ypricemagic-2.2.1/y/prices/stable_swap/belt.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/stable_swap/curve.py` & `ypricemagic-2.2.1/y/prices/stable_swap/curve.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,19 +217,19 @@
         self.identifiers = defaultdict(list)
         self.registries = defaultdict(set)  # registry -> pools
         self.factories = defaultdict(set)  # factory -> pools
         self.pools = set()
         self.token_to_pool = dict()  # lp_token -> pool
 
         self._address_providers_loading = asyncio.Event()
-        self._address_providers_loaded = threading.Event()
-        self._registries_loaded = threading.Event()
+        self._address_providers_loaded = asyncio.Event()
+        self._registries_loaded = asyncio.Event()
         self._loaded_registries = set()
-        self._all_loading = threading.Event()
-        self._all_loaded = threading.Event()
+        self._all_loading = asyncio.Event()
+        self._all_loaded = asyncio.Event()
     
     def __repr__(self) -> str:
         return "<CurveRegistry>"
     
     def _load_address_provider_event(self, event) -> None:
         if event.name == 'NewAddressIdentifier':
             self.identifiers[Ids(event['id'])].append(event['addr'])
@@ -237,15 +237,15 @@
             self.identifiers[Ids(event['id'])].append(event['new_address'])
 
     async def _load_address_providers(self) -> NoReturn:
         """ Fetch all address providers. """
         if self._address_providers_loading.is_set():
             return
         self._address_providers_loading.set()
-        block = await dank_w3.eth.block_number            
+        block = await dank_w3.eth.block_number     
         async for logs in get_logs_asap_generator(str(self.address_provider), None, to_block=block, chronological=True):
             for event in decode_logs(logs):
                 self._load_address_provider_event(event)
         self._address_providers_loaded.set()
 
         while await dank_w3.eth.block_number < block+1:
             await asyncio.sleep(15)
@@ -278,17 +278,21 @@
                 await self._load_registry_event(contract, event)
 
     async def _load_registries(self) -> None:
         if self._all_loading.is_set():
             return
         self._all_loading.set()
         if not self._address_providers_loading.is_set():
-            asyncio.get_event_loop().create_task(self._load_address_providers())
-        while not self._address_providers_loaded.is_set():
-            await asyncio.sleep(0)
+            task = asyncio.get_event_loop().create_task(self._load_address_providers())
+            def _on_completion(fut):
+                if e := fut.exception():
+                    self._all_loading.clear()
+                    raise e
+            task.add_done_callback(_on_completion)
+        await self._address_providers_loaded.wait():
         
         known_registries = []
         while True:
             # NOTE: Gnosis chain's address provider fails to provide registry via events. Maybe other chains as well.
             if not self.identifiers[Ids.Main_Registry]:
                 self.identifiers[Ids.Main_Registry] = [await self.address_provider.get_registry.coroutine()]
             
@@ -351,16 +355,15 @@
         if not self._all_loaded.is_set():
             logger.info(f'loaded {len(self.token_to_pool)} pools from {len(self.registries)} registries and {len(self.factories)} factories')
             self._all_loaded.set()
     
     async def load_all(self) -> None:
         if not self._all_loading.is_set():
             asyncio.get_event_loop().create_task(self._load_registries())
-        while not self._all_loaded.is_set():
-            await asyncio.sleep(0)
+        await self._all_loaded.wait():
     
     async def read_pools(self, registry: Address) -> List[EthAddress]:
         try:
             registry = await Contract.coroutine(registry)
         except ContractNotVerified:
             if chain.id == Network.xDai:
                 registry = Contract.from_abi("Vyper_contract", registry, CURVE_REGISTRY_ABI)
```

### Comparing `ypricemagic-2.2.0/y/prices/stable_swap/ellipsis.py` & `ypricemagic-2.2.1/y/prices/stable_swap/ellipsis.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/stable_swap/froyo.py` & `ypricemagic-2.2.1/y/prices/stable_swap/froyo.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/stable_swap/mstablefeederpool.py` & `ypricemagic-2.2.1/y/prices/stable_swap/mstablefeederpool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/stable_swap/saddle.py` & `ypricemagic-2.2.1/y/prices/stable_swap/saddle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/synthetix.py` & `ypricemagic-2.2.1/y/prices/synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/tokenized_fund/basketdao.py` & `ypricemagic-2.2.1/y/prices/tokenized_fund/basketdao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/tokenized_fund/gelato.py` & `ypricemagic-2.2.1/y/prices/tokenized_fund/gelato.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/tokenized_fund/piedao.py` & `ypricemagic-2.2.1/y/prices/tokenized_fund/piedao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/tokenized_fund/tokensets.py` & `ypricemagic-2.2.1/y/prices/tokenized_fund/tokensets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/utils/buckets.py` & `ypricemagic-2.2.1/y/prices/utils/buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/utils/sense_check.py` & `ypricemagic-2.2.1/y/prices/utils/sense_check.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/utils/ypriceapi.py` & `ypricemagic-2.2.1/y/prices/utils/ypriceapi.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/prices/yearn.py` & `ypricemagic-2.2.1/y/prices/yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/time.py` & `ypricemagic-2.2.1/y/time.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/utils/client.py` & `ypricemagic-2.2.1/y/utils/client.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/utils/events.py` & `ypricemagic-2.2.1/y/utils/events.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/utils/fakes.py` & `ypricemagic-2.2.1/y/utils/fakes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/utils/logging.py` & `ypricemagic-2.2.1/y/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/utils/middleware.py` & `ypricemagic-2.2.1/y/utils/middleware.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/utils/multicall.py` & `ypricemagic-2.2.1/y/utils/multicall.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/y/utils/raw_calls.py` & `ypricemagic-2.2.1/y/utils/raw_calls.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/ypricemagic/magic.py` & `ypricemagic-2.2.1/ypricemagic/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.0/ypricemagic.egg-info/SOURCES.txt` & `ypricemagic-2.2.1/ypricemagic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

