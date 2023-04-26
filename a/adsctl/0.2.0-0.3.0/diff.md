# Comparing `tmp/adsctl-0.2.0.tar.gz` & `tmp/adsctl-0.3.0.tar.gz`

## Comparing `adsctl-0.2.0.tar` & `adsctl-0.3.0.tar`

### file list

```diff
@@ -1,164 +1,53 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 adsctl-0.2.0/.DS_Store
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 adsctl-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 adsctl-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 adsctl-0.2.0/RELEASE.md
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 adsctl-0.2.0/TESTING.md
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 adsctl-0.2.0/Taskfile.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/10a9dd0e5adddaf1
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/11af71fc41104902
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/1300821ef2397b8d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/1be09cc27d42825f
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/1e390bbfc98b1261
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/22278fc9e9c974d5
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/24388c23bc4581e1
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/24acd61f3a44e711
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/2ba7bbb13c6f1ff8
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/2e4287c1d42ae99c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/2e4ce798cc3fd5c2
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/2f05f6e2846725b8
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/32f05a3164dd0e5a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/338d67eba4c6bdff
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/37f0b12d8cc64a26
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/39f306ac02bb02fa
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/3bcf9dd6e88c27a8
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/41f825a5216815cb
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/420c14a4d8a7f822
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/4691c6c53ef9d50d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/4700a2e8f34df580
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/491adfbad040a642
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/4c5b056d04e904b7
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/4d6dfedc7028d85
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/506f573dae839856
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/50b72c98509d0f16
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/5156a6d1dfdea5e8
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/5174206c231b427
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/51d580e429e3c0f5
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/5485e4285df788f5
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/54aac7aa945b4eea
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/5d98ccd9a6b9e57a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/5e6c26dd85411a59
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/5eb2b7708bbab22a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/5ef45ad255bebe9e
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/61324e2abd2c7394
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/6139ab745a83e112
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/634372ab84fcdbcb
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/644e31599b8e9334
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/6473c7264aba3c11
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/65f8915ba82563dd
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/662c884e1aefe68d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/6e683bae26a97070
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/705ad6d5d08ac102
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/76e36826debb321d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/7c353c43b7a6e871
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/7c65e05ccd1c9bbb
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/7c7f5cce4e0443cf
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/7cfb88373125310
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/7d23289c78f54ae7
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/7da3ad5bdc699672
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/7e83f2c6e8c1dc3
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/7efbe30ba86ed60b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/806660ee4170b006
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/8292eaab4ba08922
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/866b0f436c6ea144
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/86f500196eb4093e
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/8b253cb47ea728f9
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/8e892b62735c3a22
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/909a15d3b4e8bcbe
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/90ca96135238d641
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/964e56fea98ed0c6
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/a020f1733d5f27cc
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/a05682a3f626f2e7
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/a0dc9ebbc118cbd2
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/a0f5216d10acefbc
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/a4f06cb80811dab6
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/a5299cf723a9da9e
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/a7f2dbf98501bf26
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/aa77d19237682150
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/af875b2351696f9a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/afe656e26213792b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/b23c85d45df72a6c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/b5a6e95177cca536
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/b6a151cd5537a666
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/b7702dd98a1c8feb
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/b8add4ae18edf8fe
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/b8e51ba641007cd3
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/b8f20db2cdf13bf4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/b9a17aed4565a2f5
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/b9a912145a8666c7
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/b9bf929caeb8d5ff
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/bd8f2eb377cc390c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/bec3eace26d48273
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/c2a7e3dbe51acec0
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/c2ee9df2906b0aad
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/c31a4240613aba4c
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/c437a7deb9dca0d3
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/c4b9b21845be4e2a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/c61e2bc2e3e68985
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/c7f894b3b4ff1101
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/cce24d291c5926a7
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/cffd6ef4b335e577
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/d57ff28381b694dc
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/d6354cd37adec7f1
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/d8303c677b348538
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/db007523aa142218
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/dc9700eebaedaae0
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/df687802e9f41b67
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/e0049588e7dd3930
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/e48ea691d4c154c6
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/e96ac9b6b71a0fcc
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/ea412e3c1f88c72
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/eb207793d135be20
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/ebf4a69dc4e4ce0b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/ed35824412324ce
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/ed553939ec479479
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/edc9e85377061c71
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/ee2280db6dd3b108
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/eebc50e7c61565df
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/eec97c7fbb7b4aac
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/f05e950057371d2
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/f71c91fb9f374a7f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/f83993ce009dfcc3
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/fbb7edc21512479d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/fd7b9dc341c04ff5
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 adsctl-0.2.0/requirements/linting.in
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 adsctl-0.2.0/requirements/linting.txt
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 adsctl-0.2.0/requirements/pyproject.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/__about__.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/__init__.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/application.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/client.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/parse.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/queries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/api/__init__.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/api/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/api/campaign/__init__.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/api/campaign/budget.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/api/campaign/main.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/api/campaign/status.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/cli/__init__.py
--rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/cli/auth.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/cli/cli.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/cli/config.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/cli/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/cli/edit/__init__.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/cli/edit/campaign.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/cli/edit/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/config/__init__.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/config/config_file.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/config/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/prompt/__init__.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/prompt/cli.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/prompt/prompt.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/utils/__init__.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/utils/fs.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 adsctl-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 adsctl-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 adsctl-0.2.0/tests/test_parse.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 adsctl-0.2.0/tests/test_pkg.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 adsctl-0.2.0/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 adsctl-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 adsctl-0.2.0/README.md
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 adsctl-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6655 2020-02-02 00:00:00.000000 adsctl-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 adsctl-0.3.0/.DS_Store
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 adsctl-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 adsctl-0.3.0/.python-version
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 adsctl-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 adsctl-0.3.0/RELEASE.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 adsctl-0.3.0/TESTING.md
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 adsctl-0.3.0/Taskfile.yml
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 adsctl-0.3.0/requirements-dev.lock
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 adsctl-0.3.0/requirements.lock
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 adsctl-0.3.0/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 adsctl-0.3.0/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/__about__.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/__init__.py
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/application.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/client.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/parse.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/queries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/api/__init__.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/api/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/api/campaign/__init__.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/api/campaign/budget.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/api/campaign/main.py
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/api/campaign/status.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/cli/__init__.py
+-rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/cli/auth.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/cli/cli.py
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/cli/config.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/cli/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/cli/edit/__init__.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/cli/edit/campaign.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/cli/edit/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/config/__init__.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/config/config_file.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/config/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/prompt/__init__.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/prompt/cli.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/prompt/completer.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/prompt/key_bindings.py
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/prompt/prompt.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/utils/__init__.py
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/utils/fs.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 adsctl-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 adsctl-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 adsctl-0.3.0/tests/test_config_file.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 adsctl-0.3.0/tests/test_parse.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 adsctl-0.3.0/tests/test_pkg.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 adsctl-0.3.0/tests/templates/config_1.toml
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 adsctl-0.3.0/tests/templates/config_invalid_id.toml
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 adsctl-0.3.0/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 adsctl-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 adsctl-0.3.0/README.md
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 adsctl-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 adsctl-0.3.0/PKG-INFO
```

### Comparing `adsctl-0.2.0/.DS_Store` & `adsctl-0.3.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `adsctl-0.2.0/src/adsctl/application.py` & `adsctl-0.3.0/src/adsctl/application.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,92 @@
-from typing import Optional
-
 from google.ads.googleads.client import GoogleAdsClient
 
-from adsctl import client
+from adsctl import client as client_utils
 from adsctl.config.config_file import ConfigFile
-from adsctl.config.model import RootConfig
+from adsctl.config.model import AccountConfig, RootConfig
 from adsctl.parse import parseStream
+from adsctl.utils.fs import Path
 
 
 class Application:
+    config_file_path: Path | None
     config_file: ConfigFile
     client: GoogleAdsClient | None
-    _customer_id: Optional[str]
+    _customer_id: str | None
     params: dict = {}
 
-    def __init__(self, config_file=None, customer_id=None, create_client=True):
-        self.config_file = config_file or ConfigFile()
-        self.config_file.load()
-        self._customer_id = customer_id or self.config_file.model.customer_id
+    def __init__(
+        self,
+        config_file: str | None = None,  # Path to config file
+        account: str | None = None,
+        customer_id: str | None = None,
+        load_config=True,
+    ):
+
+        self._customer_id = customer_id
+        if config_file is None:
+            self.config_file_path = ConfigFile.get_default_location()
+            self.config_file = ConfigFile(account=account)
+        else:
+            self.config_file_path = Path(config_file)
+            path_ = None if config_file is None else Path(config_file)
+            self.config_file = ConfigFile(path=path_, account=account)
 
-        self.client = None
-        if create_client:
-            self.create_client()
+        if load_config:
+            self.load_config()
 
     @property
     def config(self) -> RootConfig:
         return self.config_file.model
 
     @property
+    def account(self) -> AccountConfig:
+        return self.config_file.account
+
+    @property
     def customer_id(self) -> str | None:
-        if self._customer_id is not None:
+        if self._customer_id:
             return self._customer_id.replace("-", "")
+        else:
+            return self.account.customer_id.replace("-", "")
 
-    @customer_id.setter
-    def customer_id_set(self, value: str | None):
-        if value is not None:
-            self._customer_id = value
+    def load_config(self):
+        self.config_file.load()
 
     def create_client(self):
-        if self.client is None:
-            gads_config = self.config_file.model.clientSettings()
-            self.client = client.get_client(gads_config)
-
-    def search(self, query, customer_id=None):
-        customer_id = customer_id or self.config_file.model.customer_id
-        stream = client.search(query.strip(), self.client, customer_id)
-        return stream
-
-    def search_stream(self, query, customer_id=None):
-        customer_id = customer_id or self.config_file.model.customer_id
-        stream = client.search_stream(query.strip(), self.client, customer_id)
-        return stream
-
-    def query(self, query, customer_id=None):
-        stream = self.search_stream(query, customer_id=customer_id)
+        gads_config = self.config_file.account.clientSettings()
+        client_ = client_utils.get_client(gads_config)
+        self.client = client_
+        return client_
+
+    def query(self, query, customer_id=None, params: dict | None = None):
+        if params is None:
+            params = {}
+        customer_id = customer_id or self.config_file.account.customer_id
+        myclient = self.create_client()
+        stream = self.search_stream(query=query, client=myclient, params=params)
         tables = parseStream(stream)
         return tables
 
+    def search(self, query, client, customer_id=None, params: dict | None = None):
+        if params is None:
+            params = {}
+        customer_id = customer_id or self.customer_id or self.account.customer_id
+        query_ = client_utils.render_template(query.strip(), **params)
+
+        ga_service = client.get_service("GoogleAdsService")
+        return ga_service.search(query=query_, customer_id=customer_id)
+
+    def search_stream(
+        self, query, client, customer_id=None, params: dict | None = None
+    ):
+        if params is None:
+            params = {}
+        customer_id = customer_id or self.customer_id or self.account.customer_id
+        query_ = client_utils.render_template(query.strip(), **params)
+
+        ga_service = client.get_service("GoogleAdsService")
+        return ga_service.search_stream(query=query_, customer_id=customer_id)
+
 
 # Alias
 GoogleAds = Application
-GoogleAds = Application
```

### Comparing `adsctl-0.2.0/src/adsctl/client.py` & `adsctl-0.3.0/src/adsctl/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import sys
 
+import jinja2
 from google.ads.googleads.client import GoogleAdsClient
 from google.ads.googleads.errors import GoogleAdsException
 
 
 def get_client(config, version="v13"):
     try:
         googleads_client = GoogleAdsClient.load_from_dict(config, version=version)
@@ -17,17 +18,25 @@
             print(f'\tError with message "{error.message}".')
             if error.location:
                 for field_path_element in error.location.field_path_elements:
                     print(f"\t\tOn field: {field_path_element.field_name}")
         sys.exit(1)
 
 
-def search(query, client, customer_id):
-    customer_id = customer_id.replace("-", "")
-    ga_service = client.get_service("GoogleAdsService")
-    return ga_service.search(customer_id=customer_id, query=query)
-
-
-def search_stream(query, client, customer_id):
-    customer_id = customer_id.replace("-", "")
-    ga_service = client.get_service("GoogleAdsService")
-    return ga_service.search_stream(customer_id=customer_id, query=query)
+# def search(query, client, customer_id):
+#     customer_id = customer_id.replace("-", "")
+#     ga_service = client.get_service("GoogleAdsService")
+#     return ga_service.search(customer_id=customer_id, query=query)
+
+
+# def search_stream(query, client, customer_id):
+#     customer_id = customer_id.replace("-", "")
+#     ga_service = client.get_service("GoogleAdsService")
+#     return ga_service.search_stream(customer_id=customer_id, query=query)
+
+
+def render_template(template: str, **params):
+    if params is None:
+        params = {}
+    environment = jinja2.Environment()
+    template_ = environment.from_string(template)
+    return template_.render(**params)
```

### Comparing `adsctl-0.2.0/src/adsctl/parse.py` & `adsctl-0.3.0/src/adsctl/parse.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.2.0/src/adsctl/queries.py` & `adsctl-0.3.0/src/adsctl/queries.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.2.0/src/adsctl/api/campaign/budget.py` & `adsctl-0.3.0/src/adsctl/api/campaign/budget.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,34 +7,34 @@
 
     query = f"""
         SELECT campaign.id, campaign.campaign_budget
         FROM campaign
         WHERE campaign.id = {campaign_id}
     """
 
-    response = app.search(query)
+    client = app.create_client()
+    response = app.search(query, client)
     for row in response:
         return row.campaign.campaign_budget
     return None
 
 
 def mutate(budget, resource_name: str, app: Application):
     """Set campaign budget."""
-    client = app.client
-
+    client = app.create_client()
     campaign_budget_service = client.get_service("CampaignBudgetService")
     campaign_budget_operation = client.get_type("CampaignBudgetOperation")
 
     updated = campaign_budget_operation.update
     updated.resource_name = resource_name
 
     # Changes
     updated.amount_micros = int(budget * 1000000)
 
     # Boilerplate:
     mask_operation(campaign_budget_operation, updated, client)
 
     response = campaign_budget_service.mutate_campaign_budgets(
-        customer_id=app.customer_id, operations=[campaign_budget_operation]
+        customer_id=app.account.customer_id, operations=[campaign_budget_operation]
     )
 
     return response
```

### Comparing `adsctl-0.2.0/src/adsctl/api/campaign/status.py` & `adsctl-0.3.0/src/adsctl/api/campaign/status.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from google.ads.googleads.client import GoogleAdsClient
 
 from adsctl.api.utils import mask_operation
 from adsctl.application import Application
 
 
 def get_rn(campaign_id, app: Application) -> str:
-    campaign_service = app.client.get_service("CampaignService")
+    client = app.create_client()
+    campaign_service = client.get_service("CampaignService")
     return campaign_service.campaign_path(app.customer_id, campaign_id)
 
 
 def mutate(status, campaign_id, app: Application):
-    client = app.client
-
+    """Set campaign status."""
+    client = app.create_client()
     campaign_service = client.get_service("CampaignService")
     campaign_operation = client.get_type("CampaignOperation")
 
     resource_name = get_rn(campaign_id, app)
 
     updated = campaign_operation.update
     updated.resource_name = resource_name
```

### Comparing `adsctl-0.2.0/src/adsctl/cli/cli.py` & `adsctl-0.3.0/src/adsctl/cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,16 +32,19 @@
 
     if enable_logging:
         logging.basicConfig(
             level=logging.INFO, format="[%(asctime)s - %(levelname)s] %(message).5000s"
         )
         logging.getLogger("google.ads.googleads.client").setLevel(logging.INFO)
 
-    app = create_app(config_file_path)
-    ctx.obj = app
+    try:
+        app = create_app(config_file_path)
+        ctx.obj = app
+    except Exception as e:
+        click.echo(f"Error loading config: {e}")
 
 
 main.add_command(auth)
 main.add_command(edit)
 main.add_command(config)
```

### Comparing `adsctl-0.2.0/src/adsctl/cli/utils.py` & `adsctl-0.3.0/src/adsctl/cli/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,90 @@
 import sys
-from typing import Optional
 
 import click
 
 from adsctl.application import Application
+from adsctl.cli.utils import replace_field
 from adsctl.config.config_file import ConfigFile
-from adsctl.utils.fs import Path
 
 
-def create_app(
-    config_file_path: Optional[str] = None, customer_id: Optional[str] = None
-) -> Application:
-    used_config_file = Path()
-    app = Application(
-        config_file=ConfigFile(), customer_id=customer_id, create_client=False
-    )
-
-    if config_file_path:
-        used_config_file = Path(config_file_path).resolve()
-        if not used_config_file.is_file():
-            click.echo(
-                f"The selected config file `{str(config_file_path)}` does not exist."
-            )
-            sys.exit(1)
-        app.config_file = ConfigFile(used_config_file)
-    elif not app.config_file.path.is_file():
-        click.echo("No config file found, creating one with default settings now...")
+@click.group()
+@click.pass_obj
+def config(app: Application):
+    """View and manage configuration"""
+
+
+@config.command()
+@click.pass_obj
+def init(app: Application):
+    """Create a base config file"""
+    # TODO: Add force flag to overwrite existing config file
 
+    if not app.config_file.path.is_file():
         try:
             app.config_file.restore()
             click.echo(f"Default config file created at: {app.config_file.path}")
             click.echo("Edit that file to include your Google Ads credentials.")
             sys.exit(0)
         except OSError:  # no cov
             click.echo(
                 f"Unable to create config file located at"
                 f"`{str(app.config_file.path)}`. Please check your permissions.",
                 err=True,
             )
-
-    return app
-
-
-def get_first_row(response):
-    for row in response:
-        return row
-    return None
+    else:
+        click.echo(
+            f"Config file already exists at: {app.config_file.path}.\n"
+            "If you want to overwrite it, delete it first."
+        )
+
+
+@config.command("get-account")
+@click.pass_obj
+def get_account(app: Application):
+    """Display the current account"""
+    app.load_config()
+
+    account_name = app.config.current_account
+    click.echo(account_name)
+
+
+@config.command("set-account")
+@click.argument("account_name")
+@click.pass_obj
+def set_account(app: Application, account_name):
+    """Set the current account"""
+    app.load_config()
+
+    if account_name in app.config.accounts.keys():
+        new_content = replace_field(
+            app.config_file.read(),
+            "current_account",
+            app.config.current_account,
+            account_name,
+        )
+        app.config_file.path.write(new_content)
+        click.echo(f"Current account set to: {account_name}")
+    else:
+        click.echo(f"Account `{account_name}` does not exist in the config file.")
+
+
+@config.command()
+@click.pass_obj
+def explore(app: Application):
+    """Open the config location in your file manager"""
+    try:
+        click.launch(str(app.config_file.path), locate=True)
+    except Exception:
+        click.launch(str(ConfigFile.get_default_location().parent), locate=True)
+
+
+@config.command()
+@click.pass_obj
+def view(app: Application):
+    """Show the contents of the config file"""
+    click.echo(f"# Config file: {app.config_file.path}\n")
+
+    if not app.config_file.path.is_file():  # no cov
+        app.display_critical("No config file found! Try: `adsctl config restore`.")
+    else:
+        click.echo(app.config_file.read())
```

### Comparing `adsctl-0.2.0/src/adsctl/cli/edit/campaign.py` & `adsctl-0.3.0/src/adsctl/cli/edit/campaign.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,45 +7,41 @@
 import adsctl.api.campaign.status as status_api
 from adsctl.application import Application
 
 
 @click.group()
 @click.option("--campaign-id", "-i", required=True, help="Campaign ID.")
 @click.pass_obj
-def campaign(obj, campaign_id):
-    obj.params["campaign_id"] = campaign_id
+def campaign(app: Application, campaign_id):
+    app.params["campaign_id"] = campaign_id
 
 
 @campaign.command("status")
 @click.argument("status", type=click.Choice(["enabled", "paused"]))
 @click.pass_obj
-def status(obj: Application, status):
+def status(app: Application, status):
     """Set campaign budget."""
-    obj.create_client()
-
-    campaign_id = obj.params["campaign_id"]
-    campaign_rn = campaign_api.get_rn(campaign_id, app=obj)
+    campaign_id = app.params["campaign_id"]
+    campaign_rn = campaign_api.get_rn(campaign_id, app=app)
 
     if campaign_rn is None:
         click.echo(f"Campaign with id '{campaign_id}' not found.")
         sys.exit(1)
 
-    r = status_api.mutate(status, campaign_id=campaign_id, app=obj)
+    r = status_api.mutate(status, campaign_id=campaign_id, app=app)
     click.echo(f"Campaign updated: {r.results[0].resource_name}")
 
 
 @campaign.command("budget")
 @click.argument("budget", type=float)
 @click.pass_obj
-def budget_(obj: Application, budget):
+def budget_(app: Application, budget):
     """Set campaign budget."""
-    obj.create_client()
-
-    campaign_id = obj.params["campaign_id"]
-    budget_rn = budget_api.get_rn(campaign_id=campaign_id, app=obj)
+    campaign_id = app.params["campaign_id"]
+    budget_rn = budget_api.get_rn(campaign_id=campaign_id, app=app)
 
     if budget_rn is None:
         click.echo(f"Budget not found for campaign {campaign_id}")
         sys.exit(1)
 
-    r = budget_api.mutate(budget, resource_name=budget_rn, app=obj)
+    r = budget_api.mutate(budget, resource_name=budget_rn, app=app)
     click.echo(f"Budget updated: {r.results[0].resource_name}")
```

### Comparing `adsctl-0.2.0/src/adsctl/prompt/cli.py` & `adsctl-0.3.0/src/adsctl/prompt/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,85 @@
 import click
 
 from adsctl.__about__ import __version__
 from adsctl.cli.utils import create_app
-from adsctl.prompt.prompt import make_query, print_results, prompt_loop
+from adsctl.prompt.prompt import print_results, prompt_loop
 
 
 @click.command()
 @click.option(
     "--config-file",
     "-f",
     "config_file_path",
     envvar="ADSCTL_CONFIG",
     help="The path to a custom config file to use [env var: `ADSCTL_CONFIG`]",
 )
-@click.option("--customer-id", "-c", "customer_id_opt", help="Google Ads Customer ID.")
+@click.option(
+    "--account",
+    "-a",
+    "account",
+    help="The account to use. Defaults to the current_account in the config file.",
+)
+@click.option("--customer-id", "-i", "customer_id_opt", help="Google Ads Customer ID.")
 @click.option(
     "--output",
     "-o",
     default="table",
     type=click.Choice(["table", "plain", "csv", "csv-files"], case_sensitive=False),
 )
 @click.option(
     "--command",
     "-c",
+    help="Inline command to run. If not provided, will enter interactive mode.",
+)
+@click.option(
+    "--filename",
+    "-f",
+    "input_file",
+    type=click.File("rb"),
+    help="File to read query from.",
+)
+@click.option(
+    "--var",
+    "-v",
+    "variables",
+    multiple=True,
+    help="Variables to render the query before sending it.",
 )
-@click.option("--filename", "-f", "input_file", type=click.File("rb"))
 @click.version_option(version=__version__, prog_name="AdsCTL")
 @click.pass_context
 def main(
-    ctx: click.Context, config_file_path, customer_id_opt, output, command, input_file
+    ctx: click.Context,
+    config_file_path,
+    account,
+    customer_id_opt,
+    output,
+    command,
+    input_file,
+    variables,
 ):
-    """Interactive GAQL prompt."""
-
-    app = create_app(config_file_path, customer_id=customer_id_opt)
-    # click.echo(f"Using config: {app.config_file.path}")
-
-    app.create_client()
+    """Interactive GAQL prompt"""
 
+    app = create_app(config_file_path, account=account, customer_id=customer_id_opt)
+    app.load_config()
     ctx.obj = app
-    ga_service = app.client.get_service("GoogleAdsService")
+
+    variables = dict(v.split("=") for v in variables)
 
     if command or input_file:
         if input_file is not None:
             command = input_file.read()
 
-        results = make_query(ga_service, app.customer_id, command, output=output)
+        results = app.query(query=command, params=variables)
+
         if output == "csv-files":
             for table, df in results.items():
                 fname = f"{table}.csv"
                 df.to_csv(fname, index=False)
         else:
             print_results(results, output=output)
     else:
-        prompt_loop(ga_service, app.customer_id, output=output)
+        prompt_loop(app, output=output, params=variables)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `adsctl-0.2.0/src/adsctl/prompt/prompt.py` & `adsctl-0.3.0/src/adsctl/prompt/prompt.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,51 @@
 import sys
 
 import click
 from google.ads.googleads.errors import GoogleAdsException
 from prompt_toolkit import PromptSession
+from prompt_toolkit.completion import FuzzyCompleter, ThreadedCompleter
+from prompt_toolkit.history import FileHistory
 from tabulate import tabulate
 
+from adsctl.application import Application
 from adsctl.parse import parseStream
+from adsctl.prompt.completer import MyCustomCompleter
+from adsctl.prompt.key_bindings import adsctl_bindings
 
 
-def prompt_loop(ga_service, customer_id, output="table"):
-    session = PromptSession()
+def prompt_loop(app: Application, output="table", params: dict | None = None):
+    if app.config_file_path is None:
+        my_history = None
+    else:
+        history_file = app.config_file_path.parent / "history.txt"
+        my_history = FileHistory(str(history_file))
+
+    key_bindings = adsctl_bindings()
+    completer = ThreadedCompleter(FuzzyCompleter(MyCustomCompleter()))
+    session = PromptSession(
+        history=my_history,
+        completer=completer,
+        complete_while_typing=True,
+        key_bindings=key_bindings,
+        multiline=True,
+    )
 
     while True:
         try:
             query = session.prompt(">>> ").strip()
 
             if not query:
                 continue
 
             if query == "exit":
                 sys.exit(0)
 
-            results = make_query(ga_service, customer_id, query, output=output)
+            results = app.query(query=query, params=params)
+            # results = make_query(ga_service, customer_id, query, output=output)
 
             if results is None:
                 continue
 
             print_results(results, output=output)
 
         except GoogleAdsException as ex:
@@ -34,18 +54,19 @@
         except KeyboardInterrupt:
             pass
         except EOFError:
             # Control-D pressed
             sys.exit()
 
 
-def make_query(ga_service, customer_id, query, output="table") -> None | list | dict:
-    stream = ga_service.search_stream(customer_id=customer_id, query=query)
-
+def make_query(
+    app: Application, query, output="table", params: dict | None = None
+) -> None | list | dict:
     results = None
+    stream = app.search_stream(query, params=params)
 
     if output == "plain":
         results = []
         for batch in stream:
             for row in batch.results:
                 results.append(row)
     elif output in ("table", "csv", "csv-files"):
@@ -71,7 +92,12 @@
                 click.echo("No results found")
             else:
                 click.echo(tabulate(df, headers="keys", tablefmt="psql"))
     elif output == "csv":
         for _, df in results.items():
             if len(df) > 0:
                 click.echo(df.to_csv(index=False))
+                click.echo(df.to_csv(index=False))
+        for _, df in results.items():
+            if len(df) > 0:
+                click.echo(df.to_csv(index=False))
+                click.echo(df.to_csv(index=False))
```

### Comparing `adsctl-0.2.0/src/adsctl/utils/fs.py` & `adsctl-0.3.0/src/adsctl/utils/fs.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,33 +7,30 @@
 
 if sys.version_info >= (3, 11):
     import tomllib
 else:
     import tomli as tomllib
 
 
-if sys.platform == "win32":
-    _PathBase = pathlib.WindowsPath
-else:
-    _PathBase = pathlib.PosixPath
-
-
 disk_sync = os.fsync
 # https://mjtsai.com/blog/2022/02/17/apple-ssd-benchmarks-and-f_fullsync/
 # https://developer.apple.com/library/archive/documentation/System/Conceptual/ManPages_iPhoneOS/man2/fsync.2.html
 if sys.platform == "darwin":
     import fcntl
 
     if hasattr(fcntl, "F_FULLFSYNC"):
 
         def disk_sync(fd) -> None:
             fcntl.fcntl(fd, fcntl.F_FULLFSYNC)
 
 
-class Path(_PathBase):
+class Path(type(pathlib.Path())):
+    def __new__(cls, *pathsegments):
+        return super().__new__(cls, *pathsegments)
+
     def ensure_dir_exists(self) -> None:
         self.mkdir(parents=True, exist_ok=True)
 
     def ensure_parent_dir_exists(self) -> None:
         self.parent.mkdir(parents=True, exist_ok=True)
 
     def expand(self) -> Path:
@@ -47,14 +44,19 @@
         if self.is_file():
             os.remove(self)
         elif self.is_dir():
             import shutil
 
             shutil.rmtree(self, ignore_errors=False)
 
+    def write(self, data: str) -> None:
+        self.parent.mkdir(parents=True, exist_ok=True)
+        with self.open("w") as f:
+            f.write(data)
+
     def write_atomic(self, data: str | bytes, *args: Any, **kwargs: Any) -> None:
         from tempfile import mkstemp
 
         fd, path = mkstemp(dir=self.parent)
         with os.fdopen(fd, *args, **kwargs) as f:
             f.write(data)
             f.flush()
```

### Comparing `adsctl-0.2.0/tests/test_parse.py` & `adsctl-0.3.0/tests/test_parse.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 pytestmark = [pytest.mark.adsapi]
 
 
 def test_parse_1():
     google_ads = adsctl.GoogleAds()
 
-    tables = google_ads.query(queries.GET_CAMPAIGNS_LIST)
+    google_ads.query(queries.GET_CAMPAIGNS_LIST)
 
     # for table_name, table in tables.items():
     #     print(table_name)
     #     print(table, "\n")
 
 
 def test_parse_2():
```

### Comparing `adsctl-0.2.0/.gitignore` & `adsctl-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adsctl-0.2.0/LICENSE.txt` & `adsctl-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adsctl-0.2.0/README.md` & `adsctl-0.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -12,60 +12,96 @@
     </a>
     </a>
     <a href="https://github.com/danielfrg/adsctl/blob/main/LICENSE.txt">
         <img src="https://img.shields.io/:license-Apache%202-blue.svg">
     </a>
 </p>
 
+Google Ads Interface for humans.
+
+_This is a work in progress, please open an issue if you find any bugs or have any suggestions._
+
 Features:
 
 - A command line tool for executing GAQL queries against the Google Ads API.
   Like [psql](https://www.postgresql.org/docs/current/app-psql.html) for the Google Ads API.
 - A command line tool for managing Google Ads resources.
   Like [kubectl](https://kubernetes.io/docs/reference/kubectl/) for the Google Ads API.
-- Centralized configuration with _(soon)_ multiple config file management
+- Centralized configuration with multiple account management
 - Automatically update refresh token
-- Simple Python API with Pandas integration
-
-Google Ads Interface for humans.
+- Python API with Pandas integration
 
 ## Installation
 
 ```shell
 pip install adsctl
 ```
 
 ## Getting started
 
 Requirements:
 
-- All the requirements to use the Google Ads API including Ads Developer Token and OAuth2 credentials
+- All the requirements to use the Google Ads API including a Developer Token and OAuth2 credentials
 - See [Google Ads API Quickstart](https://developers.google.com/google-ads/api/docs/first-call/overview) for more details.
 
+### Configuration
+
 This project manages it's own configuration files.
 To create the configuration file run:
 
 ```shell
 adsctl config
 
 # Open the location of the config files
 adsctl config explore
 ```
 
-Open the generated config file and fill it with your credentials:
+Open the new default config file and fill it with your credentials:
 Dev Token, Client ID, Client Secret and Customer ID.
-Don't add the `refresh_token`.
 
 To login and get a refresh token:
 
 ```shell
 adsctl auth <path-to-secret.json>
 ```
 
-The token is saved automatically in the configuration file.
+The token is saved automatically in the config file.
+You can see it by running:
+
+```shell
+# View config
+adsctl config view
+```
+
+### Multiple Accounts
+
+You can manage multiple accounts in the config file by adding TOML sections.
+
+```toml
+current_account = "default"
+
+[... default account ...]
+
+[accounts.another]
+developer_token = ""
+customer_id = ""
+login_customer_id = ""
+
+[accounts.another.oauth]
+client_id = ""
+client_secret = ""
+```
+
+Set the current account:
+
+```shell
+$ adsctl config set-account another
+$ adsctl config get-account
+another
+```
 
 ## GAQL Prompt
 
 An interactive shell for executing GAQL queries against the Google Ads API.
 
 ```shell
 $ gaql
@@ -76,43 +112,66 @@
 |----+-----------------------------+---------+-------------|
 |  0 | customers/XXX/campaigns/YYY | name1   | 10000000000 |
 |  1 | customers/XXX/campaigns/YYY | name2   | 10000000000 |
 |  2 | customers/XXX/campaigns/YYY | name3   | 10000000000 |
 +----+-----------------------------+---------+-------------+
 ```
 
-By default adsctl prints it in "table" format but you can control the output
-format with the `-o` flag:
+By default it uses the it in `table` format but you can control the output
+format with the `-o` option:
 
 ```shell
 # Print the plain protobuf response
 $ gaql -o plain
 
-# Print a CSV response
+# Print the contents of a CSV file
 $ gaql -o csv
 ```
 
-You can also run a single commands and save the output to a file in the specified format:
+You can also run a single inline command and redirect the output to a file:
 
 ```shell
-$ gaql -c 'SELECT campaign.id, campaign.name FROM campaign ORDER BY campaign.id' -o csv > my-query.csv
+gaql -c 'SELECT campaign.id, campaign.name FROM campaign ORDER BY campaign.id' -o csv > my-query.csv
 ```
 
 This assumes only table is returned but in more complex queries that include other
 resources or when using metrics or segments multiple tables are created.
 On those cases use the -o csv-files flag to save each table to a different file
 based on the table name.
 
 ```shell
 $ gaql -c 'SELECT campaign.id, campaign.name FROM campaign ORDER BY campaign.id' -o csv-files
 
 $ ls
 campaign.csv
 ```
 
+### Query variables
+
+You can specify one or more variables using the jinja syntax, those
+variables will be replaced with the values specified in the `-v` options.
+
+```shell
+gaql -c 'SELECT campaign.id, campaign.name FROM campaign WHERE campaign.id = {{ id }} ORDER BY campaign.id' -v id=123456789
+```
+
+You can also pass `-v` without a command and use this the variables in the prompt
+queries:
+
+```shell
+$ gaql -v id=123456789 -v field=name
+
+>>> SELECT campaign.id, campaign.{{ field }} FROM campaign WHERE campaign.id = {{ id }} ORDER BY campaign.id
+```
+
+### Other options
+
+You can overwrite the account and customer ID using the `-a` and `-i` options.
+See `gaql --help` for more details.
+
 ## CLI
 
 ### Campaign Management
 
 #### Status management
 
 ```shell
@@ -122,29 +181,23 @@
 
 #### Update budget
 
 ```shell
 adsctl campaign -i <campaign-id> budget <amount>
 ```
 
-### Config
-
-```shell
-adsctl config show
-```
-
-## Programmatic API
+## Python API
 
 You can also use the Python API to easily execute GAQL queries
 and get the results as a Python dict or pandas DataFrame.
 
 ```python
 import adsctl as ads
 
-# Read config file and create client
+# Read config file and creates the Google Ads client
 google_ads = ads.GoogleAds()
 
 # Execute GAQL query
 get_campaigns_query = """
 SELECT campaign.name,
   campaign_budget.amount_micros,
   campaign.status,
@@ -154,18 +207,18 @@
   metrics.impressions,
   metrics.ctr,
   metrics.average_cpc,
   metrics.cost_micros,
   campaign.bidding_strategy_type
 FROM campaign
 WHERE segments.date DURING LAST_7_DAYS
-  AND campaign.status != 'REMOVED'
+  AND campaign.status != '{{ status }}'
 """
 
-tables = adsctl.query(get_campaigns_query)
+tables = adsctl.query(get_campaigns_query, params={"status": "REMOVED"}})
 
 # Print Pandas DataFrames
 for table_name, table in tables.items():
     print(table_name)
     print(table, "\n")
 ```
 
@@ -180,18 +233,19 @@
 0    210    6730050  0.011457  32047.857143       18330
 
 campaignBudget
                                        resourceName amountMicros
 0  customers/XXXXXXXXXX/campaignBudgets/ZZZZZZZZZZZ      1000000
 ```
 
-Or just directly make a `search_stream` request:
+Or directly get a client to use search_stream directly:
 
 ```python
-stream = app.search_stream(query)
+gads_client = google_ads.create_client()
+stream = self.search_stream(query, client=myclient)
 
 for batch in stream:
     for row in batch.results:
         ...
 ```
 
 ## Disclaimer
```

#### html2text {}

```diff
@@ -1,64 +1,81 @@
 # Google Ads API CLI and Prompt
    [https://img.shields.io/pypi/v/adsctl.svg] [https://img.shields.io/pypi/
   pyversions/adsctl.svg] [https://github.com/danielfrg/adsctl/workflows/test/
                                   badge.svg]
  [https://img.shields.io/:license-Apache%202-blue.svg]
-Features: - A command line tool for executing GAQL queries against the Google
-Ads API. Like [psql](https://www.postgresql.org/docs/current/app-psql.html) for
-the Google Ads API. - A command line tool for managing Google Ads resources.
-Like [kubectl](https://kubernetes.io/docs/reference/kubectl/) for the Google
-Ads API. - Centralized configuration with _(soon)_ multiple config file
-management - Automatically update refresh token - Simple Python API with Pandas
-integration Google Ads Interface for humans. ## Installation ```shell pip
-install adsctl ``` ## Getting started Requirements: - All the requirements to
-use the Google Ads API including Ads Developer Token and OAuth2 credentials -
-See [Google Ads API Quickstart](https://developers.google.com/google-ads/api/
-docs/first-call/overview) for more details. This project manages it's own
-configuration files. To create the configuration file run: ```shell adsctl
+Google Ads Interface for humans. _This is a work in progress, please open an
+issue if you find any bugs or have any suggestions._ Features: - A command line
+tool for executing GAQL queries against the Google Ads API. Like [psql](https:/
+/www.postgresql.org/docs/current/app-psql.html) for the Google Ads API. - A
+command line tool for managing Google Ads resources. Like [kubectl](https://
+kubernetes.io/docs/reference/kubectl/) for the Google Ads API. - Centralized
+configuration with multiple account management - Automatically update refresh
+token - Python API with Pandas integration ## Installation ```shell pip install
+adsctl ``` ## Getting started Requirements: - All the requirements to use the
+Google Ads API including a Developer Token and OAuth2 credentials - See [Google
+Ads API Quickstart](https://developers.google.com/google-ads/api/docs/first-
+call/overview) for more details. ### Configuration This project manages it's
+own configuration files. To create the configuration file run: ```shell adsctl
 config # Open the location of the config files adsctl config explore ``` Open
-the generated config file and fill it with your credentials: Dev Token, Client
-ID, Client Secret and Customer ID. Don't add the `refresh_token`. To login and
-get a refresh token: ```shell adsctl auth
-json> ``` The token is saved automatically in the configuration file. ## GAQL
-Prompt An interactive shell for executing GAQL queries against the Google Ads
-API. ```shell $ gaql >>> SELECT campaign.id, campaign.name FROM campaign ORDER
-BY campaign.id +----+-----------------------------+---------+-------------+ | |
-resourceName | name | id | |----+-----------------------------+---------+------
--------| | 0 | customers/XXX/campaigns/YYY | name1 | 10000000000 | | 1 |
-customers/XXX/campaigns/YYY | name2 | 10000000000 | | 2 | customers/XXX/
-campaigns/YYY | name3 | 10000000000 | +----+-----------------------------+-----
-----+-------------+ ``` By default adsctl prints it in "table" format but you
-can control the output format with the `-o` flag: ```shell # Print the plain
-protobuf response $ gaql -o plain # Print a CSV response $ gaql -o csv ``` You
-can also run a single commands and save the output to a file in the specified
-format: ```shell $ gaql -c 'SELECT campaign.id, campaign.name FROM campaign
-ORDER BY campaign.id' -o csv > my-query.csv ``` This assumes only table is
-returned but in more complex queries that include other resources or when using
-metrics or segments multiple tables are created. On those cases use the -o csv-
-files flag to save each table to a different file based on the table name.
-```shell $ gaql -c 'SELECT campaign.id, campaign.name FROM campaign ORDER BY
-campaign.id' -o csv-files $ ls campaign.csv ``` ## CLI ### Campaign Management
-#### Status management ```shell adsctl campaign -i  status enabled adsctl
-campaign -i  status paused ``` #### Update budget ```shell adsctl campaign -
-i  budget  ``` ### Config ```shell adsctl config show ``` ## Programmatic API
-You can also use the Python API to easily execute GAQL queries and get the
-results as a Python dict or pandas DataFrame. ```python import adsctl as ads #
-Read config file and create client google_ads = ads.GoogleAds() # Execute GAQL
-query get_campaigns_query = """ SELECT campaign.name,
+the new default config file and fill it with your credentials: Dev Token,
+Client ID, Client Secret and Customer ID. To login and get a refresh token:
+```shell adsctl auth
+json> ``` The token is saved automatically in the config file. You can see it
+by running: ```shell # View config adsctl config view ``` ### Multiple Accounts
+You can manage multiple accounts in the config file by adding TOML sections.
+```toml current_account = "default" [... default account ...]
+[accounts.another] developer_token = "" customer_id = "" login_customer_id = ""
+[accounts.another.oauth] client_id = "" client_secret = "" ``` Set the current
+account: ```shell $ adsctl config set-account another $ adsctl config get-
+account another ``` ## GAQL Prompt An interactive shell for executing GAQL
+queries against the Google Ads API. ```shell $ gaql >>> SELECT campaign.id,
+campaign.name FROM campaign ORDER BY campaign.id +----+------------------------
+-----+---------+-------------+ | | resourceName | name | id | |----+-----------
+------------------+---------+-------------| | 0 | customers/XXX/campaigns/YYY |
+name1 | 10000000000 | | 1 | customers/XXX/campaigns/YYY | name2 | 10000000000 |
+| 2 | customers/XXX/campaigns/YYY | name3 | 10000000000 | +----+---------------
+--------------+---------+-------------+ ``` By default it uses the it in
+`table` format but you can control the output format with the `-o` option:
+```shell # Print the plain protobuf response $ gaql -o plain # Print the
+contents of a CSV file $ gaql -o csv ``` You can also run a single inline
+command and redirect the output to a file: ```shell gaql -c 'SELECT
+campaign.id, campaign.name FROM campaign ORDER BY campaign.id' -o csv > my-
+query.csv ``` This assumes only table is returned but in more complex queries
+that include other resources or when using metrics or segments multiple tables
+are created. On those cases use the -o csv-files flag to save each table to a
+different file based on the table name. ```shell $ gaql -c 'SELECT campaign.id,
+campaign.name FROM campaign ORDER BY campaign.id' -o csv-files $ ls
+campaign.csv ``` ### Query variables You can specify one or more variables
+using the jinja syntax, those variables will be replaced with the values
+specified in the `-v` options. ```shell gaql -c 'SELECT campaign.id,
+campaign.name FROM campaign WHERE campaign.id = {{ id }} ORDER BY campaign.id'
+-v id=123456789 ``` You can also pass `-v` without a command and use this the
+variables in the prompt queries: ```shell $ gaql -v id=123456789 -v field=name
+>>> SELECT campaign.id, campaign.{{ field }} FROM campaign WHERE campaign.id =
+{{ id }} ORDER BY campaign.id ``` ### Other options You can overwrite the
+account and customer ID using the `-a` and `-i` options. See `gaql --help` for
+more details. ## CLI ### Campaign Management #### Status management ```shell
+adsctl campaign -i  status enabled adsctl campaign -i  status paused ``` ####
+Update budget ```shell adsctl campaign -i  budget  ``` ## Python API You can
+also use the Python API to easily execute GAQL queries and get the results as a
+Python dict or pandas DataFrame. ```python import adsctl as ads # Read config
+file and creates the Google Ads client google_ads = ads.GoogleAds() # Execute
+GAQL query get_campaigns_query = """ SELECT campaign.name,
 campaign_budget.amount_micros, campaign.status, campaign.optimization_score,
 campaign.advertising_channel_type, metrics.clicks, metrics.impressions,
 metrics.ctr, metrics.average_cpc, metrics.cost_micros,
 campaign.bidding_strategy_type FROM campaign WHERE segments.date DURING
-LAST_7_DAYS AND campaign.status != 'REMOVED' """ tables = adsctl.query
-(get_campaigns_query) # Print Pandas DataFrames for table_name, table in
-tables.items(): print(table_name) print(table, "\n") ``` ```plain campaign
-resourceName status ... name optimizationScore 0 customers/XXXXXXXXXX/
-campaigns/YYYYYYYYYYY ENABLED ... my-campaign 0.839904 [1 rows x 6 columns]
-metrics clicks costMicros ctr averageCpc impressions 0 210 6730050 0.011457
-32047.857143 18330 campaignBudget resourceName amountMicros 0 customers/
-XXXXXXXXXX/campaignBudgets/ZZZZZZZZZZZ 1000000 ``` Or just directly make a
-`search_stream` request: ```python stream = app.search_stream(query) for batch
-in stream: for row in batch.results: ... ``` ## Disclaimer _This is not an
-official Google product_. This repository is maintained by a Googler but is not
-a supported Google product. Code and issues here are answered by maintainers
-and other community members on GitHub on a best-effort basis.
+LAST_7_DAYS AND campaign.status != '{{ status }}' """ tables = adsctl.query
+(get_campaigns_query, params={"status": "REMOVED"}}) # Print Pandas DataFrames
+for table_name, table in tables.items(): print(table_name) print(table, "\n")
+``` ```plain campaign resourceName status ... name optimizationScore 0
+customers/XXXXXXXXXX/campaigns/YYYYYYYYYYY ENABLED ... my-campaign 0.839904 [1
+rows x 6 columns] metrics clicks costMicros ctr averageCpc impressions 0 210
+6730050 0.011457 32047.857143 18330 campaignBudget resourceName amountMicros 0
+customers/XXXXXXXXXX/campaignBudgets/ZZZZZZZZZZZ 1000000 ``` Or directly get a
+client to use search_stream directly: ```python gads_client =
+google_ads.create_client() stream = self.search_stream(query, client=myclient)
+for batch in stream: for row in batch.results: ... ``` ## Disclaimer _This is
+not an official Google product_. This repository is maintained by a Googler but
+is not a supported Google product. Code and issues here are answered by
+maintainers and other community members on GitHub on a best-effort basis.
```

### Comparing `adsctl-0.2.0/pyproject.toml` & `adsctl-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -13,55 +13,45 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "google-ads>=20.0.0",
   "click>=8.1",
+  "jinja2>=3.1.0",
   "pandas>=2.0.0",
   "pydantic>=1.10.0,<2.0.0",
   "tabulate>=0.9.0",
   "prompt_toolkit>=3.0.38",
   "tomli-w>=1.0",
   "tomlkit>=0.11.1",
 ]
 dynamic = ["version"]
 
-[project.urls]
-Documentation = "https://github.com/danielfrg/adsctl#readme"
-Issues = "https://github.com/danielfrg/adsctl/issues"
-Source = "https://github.com/danielfrg/adsctl"
-
-[project.optional-dependencies]
-test = ["coverage[toml]", "pytest", "pytest-cov"]
+# [project.optional-dependencies]
+# test = []
 
 [project.scripts]
 gaql = "adsctl.prompt.cli:main"
 adsctl = "adsctl.cli.cli:main"
 
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[tool.hatch.build]
-exclude = [".github"]
-
-[tool.hatch.version]
-path = "src/adsctl/__about__.py"
-
-[tool.hatch.envs.default]
-features = ["test"]
-dependencies = ["black", "isort", "mypy", "pip-tools", "ruff"]
-
-[tool.hatch.envs.default.scripts]
-check-style = ["ruff {args:.}", "black --check --diff {args:.}"]
-fmt = ["black {args:.}", "ruff --fix {args:.}", "style"]
-test = "cov --no-cov {args}"
-test-adsapi = "cov --no-cov --ads-api {args}"
-cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=src/adsctl --cov=tests {args}"
+[tool.rye]
+dev-dependencies = [
+  "black~=23.3.0",
+  "hatch~=1.7.0",
+  "isort~=6.0.0b2",
+  "mypy~=1.2.0",
+  "ruff~=0.0.262",
+  "coverage[toml]", "pytest", "pytest-cov"
+, "ipython~=8.12.0"]
+
+[tool.rye.scripts]
+test = "pytest --no-cov"
+testall = "pytest --no-cov --ads-api"
+cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=src/adsctl --cov=tests"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 addopts = ["-s", "-vv", "--strict-config", "--strict-markers"]
 markers = [
   "pkg: marks tests as Packaging tests",
   "adsapi: mark test that require connection to the API",
@@ -87,7 +77,22 @@
 ]
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 strict = true
+
+[tool.hatch.build]
+exclude = [".github"]
+
+[tool.hatch.version]
+path = "src/adsctl/__about__.py"
+
+[project.urls]
+Documentation = "https://github.com/danielfrg/adsctl#readme"
+Issues = "https://github.com/danielfrg/adsctl/issues"
+Source = "https://github.com/danielfrg/adsctl"
+
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
```

### Comparing `adsctl-0.2.0/PKG-INFO` & `adsctl-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adsctl
-Version: 0.2.0
+Version: 0.3.0
 Summary: Google Ads Control CLI and Prompt
 Project-URL: Documentation, https://github.com/danielfrg/adsctl#readme
 Project-URL: Issues, https://github.com/danielfrg/adsctl/issues
 Project-URL: Source, https://github.com/danielfrg/adsctl
 Author-email: Daniel Rodriguez <daniel@danielfrg.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
@@ -14,24 +14,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: click>=8.1
 Requires-Dist: google-ads>=20.0.0
+Requires-Dist: jinja2>=3.1.0
 Requires-Dist: pandas>=2.0.0
 Requires-Dist: prompt-toolkit>=3.0.38
 Requires-Dist: pydantic<2.0.0,>=1.10.0
 Requires-Dist: tabulate>=0.9.0
 Requires-Dist: tomli-w>=1.0
 Requires-Dist: tomlkit>=0.11.1
-Provides-Extra: test
-Requires-Dist: coverage[toml]; extra == 'test'
-Requires-Dist: pytest; extra == 'test'
-Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Google Ads API CLI and Prompt
 
 <p align="center">
     <a href="https://pypi.org/project/adsctl/">
         <img src="https://img.shields.io/pypi/v/adsctl.svg">
@@ -44,60 +41,96 @@
     </a>
     </a>
     <a href="https://github.com/danielfrg/adsctl/blob/main/LICENSE.txt">
         <img src="https://img.shields.io/:license-Apache%202-blue.svg">
     </a>
 </p>
 
+Google Ads Interface for humans.
+
+_This is a work in progress, please open an issue if you find any bugs or have any suggestions._
+
 Features:
 
 - A command line tool for executing GAQL queries against the Google Ads API.
   Like [psql](https://www.postgresql.org/docs/current/app-psql.html) for the Google Ads API.
 - A command line tool for managing Google Ads resources.
   Like [kubectl](https://kubernetes.io/docs/reference/kubectl/) for the Google Ads API.
-- Centralized configuration with _(soon)_ multiple config file management
+- Centralized configuration with multiple account management
 - Automatically update refresh token
-- Simple Python API with Pandas integration
-
-Google Ads Interface for humans.
+- Python API with Pandas integration
 
 ## Installation
 
 ```shell
 pip install adsctl
 ```
 
 ## Getting started
 
 Requirements:
 
-- All the requirements to use the Google Ads API including Ads Developer Token and OAuth2 credentials
+- All the requirements to use the Google Ads API including a Developer Token and OAuth2 credentials
 - See [Google Ads API Quickstart](https://developers.google.com/google-ads/api/docs/first-call/overview) for more details.
 
+### Configuration
+
 This project manages it's own configuration files.
 To create the configuration file run:
 
 ```shell
 adsctl config
 
 # Open the location of the config files
 adsctl config explore
 ```
 
-Open the generated config file and fill it with your credentials:
+Open the new default config file and fill it with your credentials:
 Dev Token, Client ID, Client Secret and Customer ID.
-Don't add the `refresh_token`.
 
 To login and get a refresh token:
 
 ```shell
 adsctl auth <path-to-secret.json>
 ```
 
-The token is saved automatically in the configuration file.
+The token is saved automatically in the config file.
+You can see it by running:
+
+```shell
+# View config
+adsctl config view
+```
+
+### Multiple Accounts
+
+You can manage multiple accounts in the config file by adding TOML sections.
+
+```toml
+current_account = "default"
+
+[... default account ...]
+
+[accounts.another]
+developer_token = ""
+customer_id = ""
+login_customer_id = ""
+
+[accounts.another.oauth]
+client_id = ""
+client_secret = ""
+```
+
+Set the current account:
+
+```shell
+$ adsctl config set-account another
+$ adsctl config get-account
+another
+```
 
 ## GAQL Prompt
 
 An interactive shell for executing GAQL queries against the Google Ads API.
 
 ```shell
 $ gaql
@@ -108,43 +141,66 @@
 |----+-----------------------------+---------+-------------|
 |  0 | customers/XXX/campaigns/YYY | name1   | 10000000000 |
 |  1 | customers/XXX/campaigns/YYY | name2   | 10000000000 |
 |  2 | customers/XXX/campaigns/YYY | name3   | 10000000000 |
 +----+-----------------------------+---------+-------------+
 ```
 
-By default adsctl prints it in "table" format but you can control the output
-format with the `-o` flag:
+By default it uses the it in `table` format but you can control the output
+format with the `-o` option:
 
 ```shell
 # Print the plain protobuf response
 $ gaql -o plain
 
-# Print a CSV response
+# Print the contents of a CSV file
 $ gaql -o csv
 ```
 
-You can also run a single commands and save the output to a file in the specified format:
+You can also run a single inline command and redirect the output to a file:
 
 ```shell
-$ gaql -c 'SELECT campaign.id, campaign.name FROM campaign ORDER BY campaign.id' -o csv > my-query.csv
+gaql -c 'SELECT campaign.id, campaign.name FROM campaign ORDER BY campaign.id' -o csv > my-query.csv
 ```
 
 This assumes only table is returned but in more complex queries that include other
 resources or when using metrics or segments multiple tables are created.
 On those cases use the -o csv-files flag to save each table to a different file
 based on the table name.
 
 ```shell
 $ gaql -c 'SELECT campaign.id, campaign.name FROM campaign ORDER BY campaign.id' -o csv-files
 
 $ ls
 campaign.csv
 ```
 
+### Query variables
+
+You can specify one or more variables using the jinja syntax, those
+variables will be replaced with the values specified in the `-v` options.
+
+```shell
+gaql -c 'SELECT campaign.id, campaign.name FROM campaign WHERE campaign.id = {{ id }} ORDER BY campaign.id' -v id=123456789
+```
+
+You can also pass `-v` without a command and use this the variables in the prompt
+queries:
+
+```shell
+$ gaql -v id=123456789 -v field=name
+
+>>> SELECT campaign.id, campaign.{{ field }} FROM campaign WHERE campaign.id = {{ id }} ORDER BY campaign.id
+```
+
+### Other options
+
+You can overwrite the account and customer ID using the `-a` and `-i` options.
+See `gaql --help` for more details.
+
 ## CLI
 
 ### Campaign Management
 
 #### Status management
 
 ```shell
@@ -154,29 +210,23 @@
 
 #### Update budget
 
 ```shell
 adsctl campaign -i <campaign-id> budget <amount>
 ```
 
-### Config
-
-```shell
-adsctl config show
-```
-
-## Programmatic API
+## Python API
 
 You can also use the Python API to easily execute GAQL queries
 and get the results as a Python dict or pandas DataFrame.
 
 ```python
 import adsctl as ads
 
-# Read config file and create client
+# Read config file and creates the Google Ads client
 google_ads = ads.GoogleAds()
 
 # Execute GAQL query
 get_campaigns_query = """
 SELECT campaign.name,
   campaign_budget.amount_micros,
   campaign.status,
@@ -186,18 +236,18 @@
   metrics.impressions,
   metrics.ctr,
   metrics.average_cpc,
   metrics.cost_micros,
   campaign.bidding_strategy_type
 FROM campaign
 WHERE segments.date DURING LAST_7_DAYS
-  AND campaign.status != 'REMOVED'
+  AND campaign.status != '{{ status }}'
 """
 
-tables = adsctl.query(get_campaigns_query)
+tables = adsctl.query(get_campaigns_query, params={"status": "REMOVED"}})
 
 # Print Pandas DataFrames
 for table_name, table in tables.items():
     print(table_name)
     print(table, "\n")
 ```
 
@@ -212,18 +262,19 @@
 0    210    6730050  0.011457  32047.857143       18330
 
 campaignBudget
                                        resourceName amountMicros
 0  customers/XXXXXXXXXX/campaignBudgets/ZZZZZZZZZZZ      1000000
 ```
 
-Or just directly make a `search_stream` request:
+Or directly get a client to use search_stream directly:
 
 ```python
-stream = app.search_stream(query)
+gads_client = google_ads.create_client()
+stream = self.search_stream(query, client=myclient)
 
 for batch in stream:
     for row in batch.results:
         ...
 ```
 
 ## Disclaimer
```

#### html2text {}

```diff
@@ -1,81 +1,96 @@
-Metadata-Version: 2.1 Name: adsctl Version: 0.2.0 Summary: Google Ads Control
+Metadata-Version: 2.1 Name: adsctl Version: 0.3.0 Summary: Google Ads Control
 CLI and Prompt Project-URL: Documentation, https://github.com/danielfrg/
 adsctl#readme Project-URL: Issues, https://github.com/danielfrg/adsctl/issues
 Project-URL: Source, https://github.com/danielfrg/adsctl Author-email: Daniel
 Rodriguez
 danielfrg.com> License-Expression: Apache-2.0 License-File: LICENSE.txt
 Keywords: cli,google ads,google ads api,prompt Classifier: Development Status
 :: 4 - Beta Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
 Python: >=3.10 Requires-Dist: click>=8.1 Requires-Dist: google-ads>=20.0.0
-Requires-Dist: pandas>=2.0.0 Requires-Dist: prompt-toolkit>=3.0.38 Requires-
-Dist: pydantic<2.0.0,>=1.10.0 Requires-Dist: tabulate>=0.9.0 Requires-Dist:
-tomli-w>=1.0 Requires-Dist: tomlkit>=0.11.1 Provides-Extra: test Requires-Dist:
-coverage[toml]; extra == 'test' Requires-Dist: pytest; extra == 'test'
-Requires-Dist: pytest-cov; extra == 'test' Description-Content-Type: text/
-markdown # Google Ads API CLI and Prompt
+Requires-Dist: jinja2>=3.1.0 Requires-Dist: pandas>=2.0.0 Requires-Dist:
+prompt-toolkit>=3.0.38 Requires-Dist: pydantic<2.0.0,>=1.10.0 Requires-Dist:
+tabulate>=0.9.0 Requires-Dist: tomli-w>=1.0 Requires-Dist: tomlkit>=0.11.1
+Description-Content-Type: text/markdown # Google Ads API CLI and Prompt
    [https://img.shields.io/pypi/v/adsctl.svg] [https://img.shields.io/pypi/
   pyversions/adsctl.svg] [https://github.com/danielfrg/adsctl/workflows/test/
                                   badge.svg]
  [https://img.shields.io/:license-Apache%202-blue.svg]
-Features: - A command line tool for executing GAQL queries against the Google
-Ads API. Like [psql](https://www.postgresql.org/docs/current/app-psql.html) for
-the Google Ads API. - A command line tool for managing Google Ads resources.
-Like [kubectl](https://kubernetes.io/docs/reference/kubectl/) for the Google
-Ads API. - Centralized configuration with _(soon)_ multiple config file
-management - Automatically update refresh token - Simple Python API with Pandas
-integration Google Ads Interface for humans. ## Installation ```shell pip
-install adsctl ``` ## Getting started Requirements: - All the requirements to
-use the Google Ads API including Ads Developer Token and OAuth2 credentials -
-See [Google Ads API Quickstart](https://developers.google.com/google-ads/api/
-docs/first-call/overview) for more details. This project manages it's own
-configuration files. To create the configuration file run: ```shell adsctl
+Google Ads Interface for humans. _This is a work in progress, please open an
+issue if you find any bugs or have any suggestions._ Features: - A command line
+tool for executing GAQL queries against the Google Ads API. Like [psql](https:/
+/www.postgresql.org/docs/current/app-psql.html) for the Google Ads API. - A
+command line tool for managing Google Ads resources. Like [kubectl](https://
+kubernetes.io/docs/reference/kubectl/) for the Google Ads API. - Centralized
+configuration with multiple account management - Automatically update refresh
+token - Python API with Pandas integration ## Installation ```shell pip install
+adsctl ``` ## Getting started Requirements: - All the requirements to use the
+Google Ads API including a Developer Token and OAuth2 credentials - See [Google
+Ads API Quickstart](https://developers.google.com/google-ads/api/docs/first-
+call/overview) for more details. ### Configuration This project manages it's
+own configuration files. To create the configuration file run: ```shell adsctl
 config # Open the location of the config files adsctl config explore ``` Open
-the generated config file and fill it with your credentials: Dev Token, Client
-ID, Client Secret and Customer ID. Don't add the `refresh_token`. To login and
-get a refresh token: ```shell adsctl auth
-json> ``` The token is saved automatically in the configuration file. ## GAQL
-Prompt An interactive shell for executing GAQL queries against the Google Ads
-API. ```shell $ gaql >>> SELECT campaign.id, campaign.name FROM campaign ORDER
-BY campaign.id +----+-----------------------------+---------+-------------+ | |
-resourceName | name | id | |----+-----------------------------+---------+------
--------| | 0 | customers/XXX/campaigns/YYY | name1 | 10000000000 | | 1 |
-customers/XXX/campaigns/YYY | name2 | 10000000000 | | 2 | customers/XXX/
-campaigns/YYY | name3 | 10000000000 | +----+-----------------------------+-----
-----+-------------+ ``` By default adsctl prints it in "table" format but you
-can control the output format with the `-o` flag: ```shell # Print the plain
-protobuf response $ gaql -o plain # Print a CSV response $ gaql -o csv ``` You
-can also run a single commands and save the output to a file in the specified
-format: ```shell $ gaql -c 'SELECT campaign.id, campaign.name FROM campaign
-ORDER BY campaign.id' -o csv > my-query.csv ``` This assumes only table is
-returned but in more complex queries that include other resources or when using
-metrics or segments multiple tables are created. On those cases use the -o csv-
-files flag to save each table to a different file based on the table name.
-```shell $ gaql -c 'SELECT campaign.id, campaign.name FROM campaign ORDER BY
-campaign.id' -o csv-files $ ls campaign.csv ``` ## CLI ### Campaign Management
-#### Status management ```shell adsctl campaign -i  status enabled adsctl
-campaign -i  status paused ``` #### Update budget ```shell adsctl campaign -
-i  budget  ``` ### Config ```shell adsctl config show ``` ## Programmatic API
-You can also use the Python API to easily execute GAQL queries and get the
-results as a Python dict or pandas DataFrame. ```python import adsctl as ads #
-Read config file and create client google_ads = ads.GoogleAds() # Execute GAQL
-query get_campaigns_query = """ SELECT campaign.name,
+the new default config file and fill it with your credentials: Dev Token,
+Client ID, Client Secret and Customer ID. To login and get a refresh token:
+```shell adsctl auth
+json> ``` The token is saved automatically in the config file. You can see it
+by running: ```shell # View config adsctl config view ``` ### Multiple Accounts
+You can manage multiple accounts in the config file by adding TOML sections.
+```toml current_account = "default" [... default account ...]
+[accounts.another] developer_token = "" customer_id = "" login_customer_id = ""
+[accounts.another.oauth] client_id = "" client_secret = "" ``` Set the current
+account: ```shell $ adsctl config set-account another $ adsctl config get-
+account another ``` ## GAQL Prompt An interactive shell for executing GAQL
+queries against the Google Ads API. ```shell $ gaql >>> SELECT campaign.id,
+campaign.name FROM campaign ORDER BY campaign.id +----+------------------------
+-----+---------+-------------+ | | resourceName | name | id | |----+-----------
+------------------+---------+-------------| | 0 | customers/XXX/campaigns/YYY |
+name1 | 10000000000 | | 1 | customers/XXX/campaigns/YYY | name2 | 10000000000 |
+| 2 | customers/XXX/campaigns/YYY | name3 | 10000000000 | +----+---------------
+--------------+---------+-------------+ ``` By default it uses the it in
+`table` format but you can control the output format with the `-o` option:
+```shell # Print the plain protobuf response $ gaql -o plain # Print the
+contents of a CSV file $ gaql -o csv ``` You can also run a single inline
+command and redirect the output to a file: ```shell gaql -c 'SELECT
+campaign.id, campaign.name FROM campaign ORDER BY campaign.id' -o csv > my-
+query.csv ``` This assumes only table is returned but in more complex queries
+that include other resources or when using metrics or segments multiple tables
+are created. On those cases use the -o csv-files flag to save each table to a
+different file based on the table name. ```shell $ gaql -c 'SELECT campaign.id,
+campaign.name FROM campaign ORDER BY campaign.id' -o csv-files $ ls
+campaign.csv ``` ### Query variables You can specify one or more variables
+using the jinja syntax, those variables will be replaced with the values
+specified in the `-v` options. ```shell gaql -c 'SELECT campaign.id,
+campaign.name FROM campaign WHERE campaign.id = {{ id }} ORDER BY campaign.id'
+-v id=123456789 ``` You can also pass `-v` without a command and use this the
+variables in the prompt queries: ```shell $ gaql -v id=123456789 -v field=name
+>>> SELECT campaign.id, campaign.{{ field }} FROM campaign WHERE campaign.id =
+{{ id }} ORDER BY campaign.id ``` ### Other options You can overwrite the
+account and customer ID using the `-a` and `-i` options. See `gaql --help` for
+more details. ## CLI ### Campaign Management #### Status management ```shell
+adsctl campaign -i  status enabled adsctl campaign -i  status paused ``` ####
+Update budget ```shell adsctl campaign -i  budget  ``` ## Python API You can
+also use the Python API to easily execute GAQL queries and get the results as a
+Python dict or pandas DataFrame. ```python import adsctl as ads # Read config
+file and creates the Google Ads client google_ads = ads.GoogleAds() # Execute
+GAQL query get_campaigns_query = """ SELECT campaign.name,
 campaign_budget.amount_micros, campaign.status, campaign.optimization_score,
 campaign.advertising_channel_type, metrics.clicks, metrics.impressions,
 metrics.ctr, metrics.average_cpc, metrics.cost_micros,
 campaign.bidding_strategy_type FROM campaign WHERE segments.date DURING
-LAST_7_DAYS AND campaign.status != 'REMOVED' """ tables = adsctl.query
-(get_campaigns_query) # Print Pandas DataFrames for table_name, table in
-tables.items(): print(table_name) print(table, "\n") ``` ```plain campaign
-resourceName status ... name optimizationScore 0 customers/XXXXXXXXXX/
-campaigns/YYYYYYYYYYY ENABLED ... my-campaign 0.839904 [1 rows x 6 columns]
-metrics clicks costMicros ctr averageCpc impressions 0 210 6730050 0.011457
-32047.857143 18330 campaignBudget resourceName amountMicros 0 customers/
-XXXXXXXXXX/campaignBudgets/ZZZZZZZZZZZ 1000000 ``` Or just directly make a
-`search_stream` request: ```python stream = app.search_stream(query) for batch
-in stream: for row in batch.results: ... ``` ## Disclaimer _This is not an
-official Google product_. This repository is maintained by a Googler but is not
-a supported Google product. Code and issues here are answered by maintainers
-and other community members on GitHub on a best-effort basis.
+LAST_7_DAYS AND campaign.status != '{{ status }}' """ tables = adsctl.query
+(get_campaigns_query, params={"status": "REMOVED"}}) # Print Pandas DataFrames
+for table_name, table in tables.items(): print(table_name) print(table, "\n")
+``` ```plain campaign resourceName status ... name optimizationScore 0
+customers/XXXXXXXXXX/campaigns/YYYYYYYYYYY ENABLED ... my-campaign 0.839904 [1
+rows x 6 columns] metrics clicks costMicros ctr averageCpc impressions 0 210
+6730050 0.011457 32047.857143 18330 campaignBudget resourceName amountMicros 0
+customers/XXXXXXXXXX/campaignBudgets/ZZZZZZZZZZZ 1000000 ``` Or directly get a
+client to use search_stream directly: ```python gads_client =
+google_ads.create_client() stream = self.search_stream(query, client=myclient)
+for batch in stream: for row in batch.results: ... ``` ## Disclaimer _This is
+not an official Google product_. This repository is maintained by a Googler but
+is not a supported Google product. Code and issues here are answered by
+maintainers and other community members on GitHub on a best-effort basis.
```

