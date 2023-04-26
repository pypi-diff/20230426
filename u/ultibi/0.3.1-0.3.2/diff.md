# Comparing `tmp/ultibi-0.3.1.tar.gz` & `tmp/ultibi-0.3.2.tar.gz`

## Comparing `ultibi-0.3.1.tar` & `ultibi-0.3.2.tar`

### file list

```diff
@@ -1,150 +1,153 @@
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 ultibi-0.3.1/local_dependencies/ultibi/Cargo.toml
--rw-r--r--   0     1001      123        0 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi/README.md
--rw-r--r--   0     1001      123       73 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi/src/lib.rs
--rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 ultibi-0.3.1/local_dependencies/ultibi_server/Cargo.toml
--rw-r--r--   0     1001      123      219 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_server/build.rs
--rw-r--r--   0     1001      123       35 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_server/src/api/mod.rs
--rw-r--r--   0     1001      123      638 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_server/src/api/open_api.rs
--rw-r--r--   0     1001      123     6651 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_server/src/api/routers.rs
--rw-r--r--   0     1001      123     1264 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_server/src/app.rs
--rw-r--r--   0     1001      123     2593 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_server/src/helpers.rs
--rw-r--r--   0     1001      123     1432 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_server/src/lib.rs
--rw-r--r--   0     1001      123      433 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_server/src/visual.rs
--rw-r--r--   0        0        0     1379 1970-01-01 00:00:00.000000 ultibi-0.3.1/local_dependencies/ultibi_core/Cargo.toml
--rw-r--r--   0     1001      123     2031 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/src/add_row.rs
--rw-r--r--   0     1001      123     3486 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/src/aggregations.rs
--rw-r--r--   0     1001      123      654 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/src/cache.rs
--rw-r--r--   0     1001      123     4244 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/src/datarequest.rs
--rw-r--r--   0     1001      123     9751 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/src/dataset.rs
--rw-r--r--   0     1001      123     1782 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/src/datasource/acquire.rs
--rw-r--r--   0     1001      123     2059 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/src/datasource/awss3.rs
--rw-r--r--   0     1001      123     5329 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/src/datasource/helpers.rs
--rw-r--r--   0     1001      123     7509 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/src/datasource/mod.rs
--rw-r--r--   0     1001      123        9 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/src/errors.rs
--rw-r--r--   0     1001      123    10956 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/src/execution/execute_agg.rs
--rw-r--r--   0     1001      123     4594 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs
--rw-r--r--   0     1001      123      464 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/src/execution/mod.rs
--rw-r--r--   0     1001      123     2585 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/src/filters.rs
--rw-r--r--   0     1001      123       18 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/src/helpers/mod.rs
--rw-r--r--   0     1001      123      545 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/src/helpers/searches.rs
--rw-r--r--   0     1001      123      358 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/src/lib.rs
--rw-r--r--   0     1001      123    11996 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/src/measure.rs
--rw-r--r--   0     1001      123     5459 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/src/overrides.rs
--rw-r--r--   0     1001      123      230 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/src/prelude.rs
--rw-r--r--   0     1001      123     1884 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/tests/add_row.rs
--rw-r--r--   0     1001      123      741 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/tests/agg_request.rs
--rw-r--r--   0     1001      123     1543 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/tests/aggregations.rs
--rw-r--r--   0     1001      123        1 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/tests/cache.rs
--rw-r--r--   0     1001      123     2067 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/tests/common/mod.rs
--rw-r--r--   0     1001      123       95 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/tests/data/bad_config.toml
--rw-r--r--   0     1001      123      553 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/tests/data/bad_config2.toml
--rw-r--r--   0     1001      123      116 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/tests/data/test_config.toml
--rw-r--r--   0     1001      123      354 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/tests/data/testset.csv
--rw-r--r--   0     1001      123     1250 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/tests/datasource.rs
--rw-r--r--   0     1001      123     3115 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/tests/dependants.rs
--rw-r--r--   0     1001      123     1485 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/tests/filters.rs
--rw-r--r--   0     1001      123        1 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/ultibi_core/tests/overrides.rs
--rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 ultibi-0.3.1/local_dependencies/frtb_engine/Cargo.toml
--rw-r--r--   0     1001      123      481 2023-04-19 16:50:58.000000 ultibi-0.3.1/local_dependencies/frtb_engine/README.md
--rw-r--r--   0     1001      123    14931 2023-04-19 16:50:58.000000 ultibi-0.3.1/local_dependencies/frtb_engine/data/frtb/Delta.csv
--rw-r--r--   0     1001      123      541 2023-04-19 16:50:58.000000 ultibi-0.3.1/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv
--rw-r--r--   0     1001      123     2160 2023-04-19 16:50:58.000000 ultibi-0.3.1/local_dependencies/frtb_engine/data/frtb/datasource_config.toml
--rw-r--r--   0     1001      123      159 2023-04-19 16:50:58.000000 ultibi-0.3.1/local_dependencies/frtb_engine/data/frtb/hms.csv
--rw-r--r--   0     1001      123      177 2023-04-19 16:50:58.000000 ultibi-0.3.1/local_dependencies/frtb_engine/data/frtb/vega_risk_weights.csv
--rw-r--r--   0     1001      123    20066 2023-04-19 16:50:58.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/calc_params.rs
--rw-r--r--   0     1001      123       25 2023-04-19 16:50:58.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/docs/mod.rs
--rw-r--r--   0     1001      123     1226 2023-04-19 16:50:58.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/docs/optional_params.rs
--rw-r--r--   0     1001      123     1424 2023-04-19 16:50:58.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/drc/common.rs
--rw-r--r--   0     1001      123    11840 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs
--rw-r--r--   0     1001      123     9483 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs
--rw-r--r--   0     1001      123     7606 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/drc/drc_weights.rs
--rw-r--r--   0     1001      123       96 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/drc/mod.rs
--rw-r--r--   0     1001      123      787 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/drc/totals.rs
--rw-r--r--   0     1001      123     4811 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/helpers.rs
--rw-r--r--   0     1001      123     8968 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/lib.rs
--rw-r--r--   0     1001      123     3780 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/measures.rs
--rw-r--r--   0     1001      123      188 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/prelude.rs
--rw-r--r--   0     1001      123    26516 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/risk_weights.rs
--rw-r--r--   0     1001      123     5408 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/risk_weights_crr2.rs
--rw-r--r--   0     1001      123     5268 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/rrao/mod.rs
--rw-r--r--   0     1001      123     1374 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/buckets.rs
--rw-r--r--   0     1001      123    14177 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs
--rw-r--r--   0     1001      123    13866 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs
--rw-r--r--   0     1001      123       64 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/commodity/mod.rs
--rw-r--r--   0     1001      123     3699 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs
--rw-r--r--   0     1001      123     7432 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs
--rw-r--r--   0     1001      123    29827 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/common.rs
--rw-r--r--   0     1001      123     9793 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/common_curv.rs
--rw-r--r--   0     1001      123    19318 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs
--rw-r--r--   0     1001      123    17703 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs
--rw-r--r--   0     1001      123       64 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/mod.rs
--rw-r--r--   0     1001      123     3841 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs
--rw-r--r--   0     1001      123    11803 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs
--rw-r--r--   0     1001      123    15617 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs
--rw-r--r--   0     1001      123    12459 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs
--rw-r--r--   0     1001      123       64 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/mod.rs
--rw-r--r--   0     1001      123     2904 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs
--rw-r--r--   0     1001      123     8782 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs
--rw-r--r--   0     1001      123    15261 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs
--rw-r--r--   0     1001      123    13479 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs
--rw-r--r--   0     1001      123       64 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/mod.rs
--rw-r--r--   0     1001      123     2988 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs
--rw-r--r--   0     1001      123     8063 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs
--rw-r--r--   0     1001      123    17052 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs
--rw-r--r--   0     1001      123    10900 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/equity/delta.rs
--rw-r--r--   0     1001      123       64 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/equity/mod.rs
--rw-r--r--   0     1001      123     2162 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/equity/totals.rs
--rw-r--r--   0     1001      123    10428 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/equity/vega.rs
--rw-r--r--   0     1001      123    14289 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs
--rw-r--r--   0     1001      123    11992 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/fx/delta.rs
--rw-r--r--   0     1001      123       64 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/fx/mod.rs
--rw-r--r--   0     1001      123     2162 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/fx/totals.rs
--rw-r--r--   0     1001      123    10166 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/fx/vega.rs
--rw-r--r--   0     1001      123    14030 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs
--rw-r--r--   0     1001      123    21887 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/girr/delta.rs
--rw-r--r--   0     1001      123       64 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/girr/mod.rs
--rw-r--r--   0     1001      123     2295 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/girr/totals.rs
--rw-r--r--   0     1001      123    15657 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/girr/vega.rs
--rw-r--r--   0     1001      123      221 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/mod.rs
--rw-r--r--   0     1001      123     5170 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/totals.rs
--rw-r--r--   0     1001      123    28643 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/statics.rs
--rw-r--r--   0     1001      123      753 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/totals.rs
--rw-r--r--   0     1001      123     1881 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/src/validate.rs
--rw-r--r--   0     1001      123     1756 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/tests/common/mod.rs
--rw-r--r--   0     1001      123     1486 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/tests/dependant.rs
--rw-r--r--   0     1001      123     4487 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/tests/drc.rs
--rw-r--r--   0     1001      123      420 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/tests/rrao.rs
--rw-r--r--   0     1001      123    18903 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/tests/sbm.rs
--rw-r--r--   0     1001      123      744 2023-04-19 16:50:59.000000 ultibi-0.3.1/local_dependencies/frtb_engine/tests/sbm_totals.rs
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 ultibi-0.3.1/Cargo.toml
--rw-r--r--   0     1001      123      728 2023-04-19 16:50:59.000000 ultibi-0.3.1/.gitignore
--rw-r--r--   0     1001      123     2403 2023-04-19 16:50:59.000000 ultibi-0.3.1/Makefile
--rw-r--r--   0     1001      123     4606 2023-04-19 16:50:59.000000 ultibi-0.3.1/README.md
--rw-r--r--   0     1001      123     1559 2023-04-19 16:50:59.000000 ultibi-0.3.1/example.py
--rw-r--r--   0     1001      123     1429 2023-04-19 16:50:59.000000 ultibi-0.3.1/pyproject.toml
--rw-r--r--   0     1001      123       36 2023-04-19 16:50:59.000000 ultibi-0.3.1/requirements-lint.txt
--rw-r--r--   0     1001      123      307 2023-04-19 16:50:59.000000 ultibi-0.3.1/requirements.txt
--rw-r--r--   0     1001      123     3682 2023-04-19 16:50:59.000000 ultibi-0.3.1/src/calculator.rs
--rw-r--r--   0     1001      123       48 2023-04-19 16:50:59.000000 ultibi-0.3.1/src/conversions/mod.rs
--rw-r--r--   0     1001      123     3542 2023-04-19 16:50:59.000000 ultibi-0.3.1/src/conversions/series.rs
--rw-r--r--   0     1001      123     3049 2023-04-19 16:50:59.000000 ultibi-0.3.1/src/conversions/wrappers.rs
--rw-r--r--   0     1001      123     7737 2023-04-19 16:50:59.000000 ultibi-0.3.1/src/dataset.rs
--rw-r--r--   0     1001      123     3303 2023-04-19 16:50:59.000000 ultibi-0.3.1/src/errors.rs
--rw-r--r--   0     1001      123      693 2023-04-19 16:50:59.000000 ultibi-0.3.1/src/filter.rs
--rw-r--r--   0     1001      123     1986 2023-04-19 16:50:59.000000 ultibi-0.3.1/src/lib.rs
--rw-r--r--   0     1001      123     2521 2023-04-19 16:50:59.000000 ultibi-0.3.1/src/measure.rs
--rw-r--r--   0     1001      123     1353 2023-04-19 16:50:59.000000 ultibi-0.3.1/src/requests.rs
--rw-r--r--   0     1001      123     1762 2023-04-19 16:50:59.000000 ultibi-0.3.1/tests/data/datasource_config.toml
--rw-r--r--   0     1001      123     4042 2023-04-19 16:50:59.000000 ultibi-0.3.1/tests/docs/run_doc_examples.py
--rw-r--r--   0     1001      123      591 2023-04-19 16:50:59.000000 ultibi-0.3.1/tests/unit/test_compute.py
--rw-r--r--   0     1001      123     1507 2023-04-19 16:50:59.000000 ultibi-0.3.1/tests/unit/test_ds.py
--rw-r--r--   0     1001      123     2658 2023-04-19 16:50:59.000000 ultibi-0.3.1/tests/unit/test_measure.py
--rw-r--r--   0     1001      123      848 2023-04-19 16:50:59.000000 ultibi-0.3.1/ultibi/__init__.py
--rw-r--r--   0     1001      123     1062 2023-04-19 16:50:59.000000 ultibi-0.3.1/ultibi/internals/__init__.py
--rw-r--r--   0     1001      123     6735 2023-04-19 16:50:59.000000 ultibi-0.3.1/ultibi/internals/dataset.py
--rw-r--r--   0     1001      123     3133 2023-04-19 16:50:59.000000 ultibi-0.3.1/ultibi/internals/filters.py
--rw-r--r--   0     1001      123     5202 2023-04-19 16:50:59.000000 ultibi-0.3.1/ultibi/internals/measure.py
--rw-r--r--   0     1001      123     2952 2023-04-19 16:50:59.000000 ultibi-0.3.1/ultibi/internals/requests.py
--rw-r--r--   0     1001      123        0 2023-04-19 16:50:59.000000 ultibi-0.3.1/ultibi/rust_module/__init__.py
--rw-r--r--   0        0        0   101983 2023-04-19 16:52:52.000000 ultibi-0.3.1/Cargo.lock
--rw-r--r--   0        0        0     5039 1970-01-01 00:00:00.000000 ultibi-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 ultibi-0.3.2/local_dependencies/ultibi/Cargo.toml
+-rw-r--r--   0     1001      123        0 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi/README.md
+-rw-r--r--   0     1001      123       73 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi/src/lib.rs
+-rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 ultibi-0.3.2/local_dependencies/ultibi_server/Cargo.toml
+-rw-r--r--   0     1001      123      219 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_server/build.rs
+-rw-r--r--   0     1001      123       35 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_server/src/api/mod.rs
+-rw-r--r--   0     1001      123      743 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_server/src/api/open_api.rs
+-rw-r--r--   0     1001      123     6651 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_server/src/api/routers.rs
+-rw-r--r--   0     1001      123     1264 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_server/src/app.rs
+-rw-r--r--   0     1001      123     2593 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_server/src/helpers.rs
+-rw-r--r--   0     1001      123     1432 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_server/src/lib.rs
+-rw-r--r--   0     1001      123      433 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_server/src/visual.rs
+-rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 ultibi-0.3.2/local_dependencies/frtb_engine/Cargo.toml
+-rw-r--r--   0     1001      123      481 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/README.md
+-rw-r--r--   0     1001      123    14931 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/data/frtb/Delta.csv
+-rw-r--r--   0     1001      123      541 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv
+-rw-r--r--   0     1001      123     2160 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/data/frtb/datasource_config.toml
+-rw-r--r--   0     1001      123      159 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/data/frtb/hms.csv
+-rw-r--r--   0     1001      123      177 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/data/frtb/vega_risk_weights.csv
+-rw-r--r--   0     1001      123    20066 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/calc_params.rs
+-rw-r--r--   0     1001      123       25 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/docs/mod.rs
+-rw-r--r--   0     1001      123     1226 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/docs/optional_params.rs
+-rw-r--r--   0     1001      123     1424 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/drc/common.rs
+-rw-r--r--   0     1001      123    11840 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs
+-rw-r--r--   0     1001      123     9483 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs
+-rw-r--r--   0     1001      123     7606 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/drc/drc_weights.rs
+-rw-r--r--   0     1001      123       96 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/drc/mod.rs
+-rw-r--r--   0     1001      123      787 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/drc/totals.rs
+-rw-r--r--   0     1001      123     4811 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/helpers.rs
+-rw-r--r--   0     1001      123     8968 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/lib.rs
+-rw-r--r--   0     1001      123     3780 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/measures.rs
+-rw-r--r--   0     1001      123      188 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/prelude.rs
+-rw-r--r--   0     1001      123    26516 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/risk_weights.rs
+-rw-r--r--   0     1001      123     5408 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/risk_weights_crr2.rs
+-rw-r--r--   0     1001      123     5268 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/rrao/mod.rs
+-rw-r--r--   0     1001      123     1374 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/buckets.rs
+-rw-r--r--   0     1001      123    14177 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs
+-rw-r--r--   0     1001      123    13866 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs
+-rw-r--r--   0     1001      123       64 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/commodity/mod.rs
+-rw-r--r--   0     1001      123     3699 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs
+-rw-r--r--   0     1001      123     7432 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs
+-rw-r--r--   0     1001      123    29827 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/common.rs
+-rw-r--r--   0     1001      123     9793 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/common_curv.rs
+-rw-r--r--   0     1001      123    19318 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs
+-rw-r--r--   0     1001      123    17703 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs
+-rw-r--r--   0     1001      123       64 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/mod.rs
+-rw-r--r--   0     1001      123     3841 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs
+-rw-r--r--   0     1001      123    11803 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs
+-rw-r--r--   0     1001      123    15617 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs
+-rw-r--r--   0     1001      123    12459 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs
+-rw-r--r--   0     1001      123       64 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/mod.rs
+-rw-r--r--   0     1001      123     2904 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs
+-rw-r--r--   0     1001      123     8782 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs
+-rw-r--r--   0     1001      123    15261 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs
+-rw-r--r--   0     1001      123    13479 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs
+-rw-r--r--   0     1001      123       64 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/mod.rs
+-rw-r--r--   0     1001      123     2988 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs
+-rw-r--r--   0     1001      123     8063 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs
+-rw-r--r--   0     1001      123    17052 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs
+-rw-r--r--   0     1001      123    10900 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/equity/delta.rs
+-rw-r--r--   0     1001      123       64 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/equity/mod.rs
+-rw-r--r--   0     1001      123     2162 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/equity/totals.rs
+-rw-r--r--   0     1001      123    10428 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/equity/vega.rs
+-rw-r--r--   0     1001      123    14289 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs
+-rw-r--r--   0     1001      123    11992 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/fx/delta.rs
+-rw-r--r--   0     1001      123       64 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/fx/mod.rs
+-rw-r--r--   0     1001      123     2162 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/fx/totals.rs
+-rw-r--r--   0     1001      123    10166 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/fx/vega.rs
+-rw-r--r--   0     1001      123    14030 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs
+-rw-r--r--   0     1001      123    21887 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/girr/delta.rs
+-rw-r--r--   0     1001      123       64 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/girr/mod.rs
+-rw-r--r--   0     1001      123     2295 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/girr/totals.rs
+-rw-r--r--   0     1001      123    15657 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/girr/vega.rs
+-rw-r--r--   0     1001      123      221 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/mod.rs
+-rw-r--r--   0     1001      123     5170 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/totals.rs
+-rw-r--r--   0     1001      123    28643 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/statics.rs
+-rw-r--r--   0     1001      123      753 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/totals.rs
+-rw-r--r--   0     1001      123     1881 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/validate.rs
+-rw-r--r--   0     1001      123     1756 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/tests/common/mod.rs
+-rw-r--r--   0     1001      123     1486 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/tests/dependant.rs
+-rw-r--r--   0     1001      123     4487 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/tests/drc.rs
+-rw-r--r--   0     1001      123      420 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/tests/rrao.rs
+-rw-r--r--   0     1001      123    18903 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/tests/sbm.rs
+-rw-r--r--   0     1001      123      744 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/tests/sbm_totals.rs
+-rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 ultibi-0.3.2/local_dependencies/ultibi_core/Cargo.toml
+-rw-r--r--   0     1001      123     2031 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/add_row.rs
+-rw-r--r--   0     1001      123     3486 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/aggregations.rs
+-rw-r--r--   0     1001      123      654 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/cache.rs
+-rw-r--r--   0     1001      123     4244 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/datarequest.rs
+-rw-r--r--   0     1001      123     9751 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/dataset.rs
+-rw-r--r--   0     1001      123     1782 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/datasource/acquire.rs
+-rw-r--r--   0     1001      123     2059 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/datasource/awss3.rs
+-rw-r--r--   0     1001      123     5329 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/datasource/helpers.rs
+-rw-r--r--   0     1001      123     7509 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/datasource/mod.rs
+-rw-r--r--   0     1001      123      699 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/errors.rs
+-rw-r--r--   0     1001      123    10956 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/execution/execute_agg.rs
+-rw-r--r--   0     1001      123     4594 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs
+-rw-r--r--   0     1001      123      464 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/execution/mod.rs
+-rw-r--r--   0     1001      123     2585 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/filters.rs
+-rw-r--r--   0     1001      123       18 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/helpers/mod.rs
+-rw-r--r--   0     1001      123      545 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/helpers/searches.rs
+-rw-r--r--   0     1001      123      375 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/lib.rs
+-rw-r--r--   0     1001      123    11996 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/measure.rs
+-rw-r--r--   0     1001      123     5459 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/overrides.rs
+-rw-r--r--   0     1001      123      230 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/prelude.rs
+-rw-r--r--   0     1001      123       15 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/reports/mod.rs
+-rw-r--r--   0     1001      123      645 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/reports/report.rs
+-rw-r--r--   0     1001      123     1884 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/add_row.rs
+-rw-r--r--   0     1001      123      741 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/agg_request.rs
+-rw-r--r--   0     1001      123     1543 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/aggregations.rs
+-rw-r--r--   0     1001      123        1 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/cache.rs
+-rw-r--r--   0     1001      123     2067 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/common/mod.rs
+-rw-r--r--   0     1001      123       95 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/data/bad_config.toml
+-rw-r--r--   0     1001      123      553 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/data/bad_config2.toml
+-rw-r--r--   0     1001      123      116 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/data/test_config.toml
+-rw-r--r--   0     1001      123      354 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/data/testset.csv
+-rw-r--r--   0     1001      123     1250 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/datasource.rs
+-rw-r--r--   0     1001      123     3115 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/dependants.rs
+-rw-r--r--   0     1001      123     1485 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/filters.rs
+-rw-r--r--   0     1001      123        1 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/overrides.rs
+-rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 ultibi-0.3.2/Cargo.toml
+-rw-r--r--   0     1001      123      728 2023-04-25 16:53:29.000000 ultibi-0.3.2/.gitignore
+-rw-r--r--   0     1001      123     5183 2023-04-25 16:53:29.000000 ultibi-0.3.2/LICENSE
+-rw-r--r--   0     1001      123     2403 2023-04-25 16:53:29.000000 ultibi-0.3.2/Makefile
+-rw-r--r--   0     1001      123     4968 2023-04-25 16:53:29.000000 ultibi-0.3.2/README.md
+-rw-r--r--   0     1001      123     1559 2023-04-25 16:53:29.000000 ultibi-0.3.2/example.py
+-rw-r--r--   0     1001      123     2045 2023-04-25 16:53:55.000000 ultibi-0.3.2/pyproject.toml
+-rw-r--r--   0     1001      123       36 2023-04-25 16:53:29.000000 ultibi-0.3.2/requirements-lint.txt
+-rw-r--r--   0     1001      123      307 2023-04-25 16:53:29.000000 ultibi-0.3.2/requirements.txt
+-rw-r--r--   0     1001      123     3682 2023-04-25 16:53:29.000000 ultibi-0.3.2/src/calculator.rs
+-rw-r--r--   0     1001      123       48 2023-04-25 16:53:29.000000 ultibi-0.3.2/src/conversions/mod.rs
+-rw-r--r--   0     1001      123     3542 2023-04-25 16:53:29.000000 ultibi-0.3.2/src/conversions/series.rs
+-rw-r--r--   0     1001      123     3049 2023-04-25 16:53:29.000000 ultibi-0.3.2/src/conversions/wrappers.rs
+-rw-r--r--   0     1001      123     7737 2023-04-25 16:53:29.000000 ultibi-0.3.2/src/dataset.rs
+-rw-r--r--   0     1001      123     3303 2023-04-25 16:53:29.000000 ultibi-0.3.2/src/errors.rs
+-rw-r--r--   0     1001      123      693 2023-04-25 16:53:29.000000 ultibi-0.3.2/src/filter.rs
+-rw-r--r--   0     1001      123     1986 2023-04-25 16:53:29.000000 ultibi-0.3.2/src/lib.rs
+-rw-r--r--   0     1001      123     2521 2023-04-25 16:53:29.000000 ultibi-0.3.2/src/measure.rs
+-rw-r--r--   0     1001      123     1353 2023-04-25 16:53:29.000000 ultibi-0.3.2/src/requests.rs
+-rw-r--r--   0     1001      123     1762 2023-04-25 16:53:29.000000 ultibi-0.3.2/tests/data/datasource_config.toml
+-rw-r--r--   0     1001      123     4042 2023-04-25 16:53:29.000000 ultibi-0.3.2/tests/docs/run_doc_examples.py
+-rw-r--r--   0     1001      123      591 2023-04-25 16:53:29.000000 ultibi-0.3.2/tests/unit/test_compute.py
+-rw-r--r--   0     1001      123     1507 2023-04-25 16:53:29.000000 ultibi-0.3.2/tests/unit/test_ds.py
+-rw-r--r--   0     1001      123     2658 2023-04-25 16:53:29.000000 ultibi-0.3.2/tests/unit/test_measure.py
+-rw-r--r--   0     1001      123      848 2023-04-25 16:53:29.000000 ultibi-0.3.2/ultibi/__init__.py
+-rw-r--r--   0     1001      123     1062 2023-04-25 16:53:29.000000 ultibi-0.3.2/ultibi/internals/__init__.py
+-rw-r--r--   0     1001      123     6735 2023-04-25 16:53:29.000000 ultibi-0.3.2/ultibi/internals/dataset.py
+-rw-r--r--   0     1001      123     3133 2023-04-25 16:53:29.000000 ultibi-0.3.2/ultibi/internals/filters.py
+-rw-r--r--   0     1001      123     5202 2023-04-25 16:53:29.000000 ultibi-0.3.2/ultibi/internals/measure.py
+-rw-r--r--   0     1001      123     2952 2023-04-25 16:53:29.000000 ultibi-0.3.2/ultibi/internals/requests.py
+-rw-r--r--   0     1001      123        0 2023-04-25 16:53:29.000000 ultibi-0.3.2/ultibi/rust_module/__init__.py
+-rw-r--r--   0        0        0   101994 2023-04-25 16:55:32.000000 ultibi-0.3.2/Cargo.lock
+-rw-r--r--   0        0        0     5891 1970-01-01 00:00:00.000000 ultibi-0.3.2/PKG-INFO
```

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_server/Cargo.toml` & `ultibi-0.3.2/local_dependencies/ultibi_server/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ultibi_server"
-version= "0.3.1"
+version= "0.3.2"
 edition = "2021"
 publish = true
 license-file= "LICENSE"
 description= "Ultibi is a BI tool for no code data analysis"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_server/src/api/routers.rs` & `ultibi-0.3.2/local_dependencies/ultibi_server/src/api/routers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_server/src/app.rs` & `ultibi-0.3.2/local_dependencies/ultibi_server/src/app.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_server/src/helpers.rs` & `ultibi-0.3.2/local_dependencies/ultibi_server/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_server/src/lib.rs` & `ultibi-0.3.2/local_dependencies/ultibi_server/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/Cargo.toml` & `ultibi-0.3.2/local_dependencies/ultibi_core/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ultibi_core"
-version= "0.3.1"
+version= "0.3.2"
 edition = "2021"
 publish = true
 license-file= "LICENSE"
 description= "Ultibi is a BI tool for no code data analysis"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
@@ -32,14 +32,15 @@
     "csv-file",
     "diagonal_concat",
     "describe"] }
 serde_json = "1.0"
 toml = "0.7.2"
 once_cell = "1.12"
 derivative = "2.2"
+thiserror = "*"
 #AWS S3
 aws-config = { version = "0.49.0", optional = true }
 aws-sdk-s3 = { version = "0.19.0", optional = true }
 tokio = { version = "1.21.2", features = ["rt-multi-thread"], optional = true }
 futures = { version = "0.3", optional = true }
 #Cache
 #May be make optional
```

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/src/add_row.rs` & `ultibi-0.3.2/local_dependencies/ultibi_core/src/add_row.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/src/aggregations.rs` & `ultibi-0.3.2/local_dependencies/ultibi_core/src/aggregations.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/src/cache.rs` & `ultibi-0.3.2/local_dependencies/ultibi_core/src/cache.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/src/datarequest.rs` & `ultibi-0.3.2/local_dependencies/ultibi_core/src/datarequest.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/src/dataset.rs` & `ultibi-0.3.2/local_dependencies/ultibi_core/src/dataset.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/src/datasource/acquire.rs` & `ultibi-0.3.2/local_dependencies/ultibi_core/src/datasource/acquire.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/src/datasource/awss3.rs` & `ultibi-0.3.2/local_dependencies/ultibi_core/src/datasource/awss3.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/src/datasource/helpers.rs` & `ultibi-0.3.2/local_dependencies/ultibi_core/src/datasource/helpers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/src/datasource/mod.rs` & `ultibi-0.3.2/local_dependencies/ultibi_core/src/datasource/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/src/execution/execute_agg.rs` & `ultibi-0.3.2/local_dependencies/ultibi_core/src/execution/execute_agg.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs` & `ultibi-0.3.2/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/src/filters.rs` & `ultibi-0.3.2/local_dependencies/ultibi_core/src/filters.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/src/helpers/searches.rs` & `ultibi-0.3.2/local_dependencies/ultibi_core/src/helpers/searches.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/src/measure.rs` & `ultibi-0.3.2/local_dependencies/ultibi_core/src/measure.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/src/overrides.rs` & `ultibi-0.3.2/local_dependencies/ultibi_core/src/overrides.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/tests/add_row.rs` & `ultibi-0.3.2/local_dependencies/ultibi_core/tests/add_row.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/tests/agg_request.rs` & `ultibi-0.3.2/local_dependencies/ultibi_core/tests/agg_request.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/tests/aggregations.rs` & `ultibi-0.3.2/local_dependencies/ultibi_core/tests/aggregations.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/tests/common/mod.rs` & `ultibi-0.3.2/local_dependencies/ultibi_core/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/tests/data/bad_config2.toml` & `ultibi-0.3.2/local_dependencies/ultibi_core/tests/data/bad_config2.toml`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/tests/datasource.rs` & `ultibi-0.3.2/local_dependencies/ultibi_core/tests/datasource.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/tests/dependants.rs` & `ultibi-0.3.2/local_dependencies/ultibi_core/tests/dependants.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/ultibi_core/tests/filters.rs` & `ultibi-0.3.2/local_dependencies/ultibi_core/tests/filters.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/Cargo.toml` & `ultibi-0.3.2/local_dependencies/frtb_engine/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "frtb_engine"
-version= "0.3.1"
+version= "0.3.2"
 edition = "2021"
 publish = false
 license-file= "LICENSE"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
```

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/data/frtb/Delta.csv` & `ultibi-0.3.2/local_dependencies/frtb_engine/data/frtb/Delta.csv`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv` & `ultibi-0.3.2/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/data/frtb/datasource_config.toml` & `ultibi-0.3.2/local_dependencies/frtb_engine/data/frtb/datasource_config.toml`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/calc_params.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/calc_params.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/docs/optional_params.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/docs/optional_params.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/drc/common.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/drc/common.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/drc/drc_weights.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/drc/drc_weights.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/drc/totals.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/drc/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/helpers.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/lib.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/measures.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/measures.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/risk_weights.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/risk_weights.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/risk_weights_crr2.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/risk_weights_crr2.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/rrao/mod.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/rrao/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/buckets.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/buckets.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/common.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/common.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/common_curv.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/common_curv.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/equity/delta.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/equity/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/equity/totals.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/equity/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/equity/vega.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/equity/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/fx/delta.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/fx/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/fx/totals.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/fx/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/fx/vega.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/fx/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/girr/delta.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/girr/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/girr/totals.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/girr/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/girr/vega.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/girr/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/sbm/totals.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/statics.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/statics.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/totals.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/src/validate.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/src/validate.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/tests/common/mod.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/tests/dependant.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/tests/dependant.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/tests/drc.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/tests/drc.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/tests/sbm.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/tests/sbm.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/local_dependencies/frtb_engine/tests/sbm_totals.rs` & `ultibi-0.3.2/local_dependencies/frtb_engine/tests/sbm_totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/Cargo.toml` & `ultibi-0.3.2/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyultima"
-version= "0.3.1"
+version= "0.3.2"
 edition = "2021"
 publish = false
 repository= "https://github.com/ultima-ib/ultima/"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "ultibi"
```

### Comparing `ultibi-0.3.1/.gitignore` & `ultibi-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/Makefile` & `ultibi-0.3.2/Makefile`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/README.md` & `ultibi-0.3.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # The Ultimate BI tool
 With `Ultibi` you can turn your `DataFrame` into a pivot table with a UI and share it across organisation. You can also define measures applicable to your `DataFrame`.  This means your colleagues/consumers don't have to write any code to analyse the data.
 
 <br>
 
 <p align="center">
     <a href="https://frtb.demo.ultimabi.uk/" target="_blank">
-    <img width="900" src="https://ultima-bi.s3.eu-west-2.amazonaws.com/imgs/titanic_gif.gif" alt="Ultima Logo">
+    <img width="900" src="https://ultima-bi.s3.eu-west-2.amazonaws.com/imgs/UltimaScreenshotExplained.jpg" alt="Ultima Logo">
     </a>
 </p>
 
 <br>
 
 Ultibi leverages on the giants: [Actix](https://github.com/actix/actix-web), [Polars](https://github.com/pola-rs/polars) and Rust which make this possible. We use TypeScript for the frontend.
 
@@ -40,23 +40,30 @@
 os.environ["RUST_LOG"] = "info" # enable logs
 os.environ["ADDRESS"] = "0.0.0.0:8000" # host on this address
 
 # Read Data
 # for more details: https://pola-rs.github.io/polars/py-polars/html/reference/api/polars.read_csv.html
 df = pl.read_csv("titanic.csv")
 
+# Let's add some Custom/Bespoke Calculations to our UI
+
 # Standard Calculator
 def survival_mean_age(kwargs: dict[str, str]) -> pl.Expr:
     """Mean Age of Survivals
     pl.col("survived") is 0 or 1
     pl.col("age") * pl.col("survived") - age of survived person, otherwise 0
     pl.col("survived").sum() - number of survived
     """
     return pl.col("age") * pl.col("survived") / pl.col("survived").sum()
 
+# Also a Standard Calculator
+def example_dep_calc(kwargs: dict[str, str]) -> pl.Expr:
+    return pl.col("SurvivalMeanAge_sum") + pl.col("SouthamptonFareDivAge_sum")
+
+# When we need more involved calculations we go for a Custom Calculator
 def custom_calculator(
             srs: list[pl.Series], kwargs: dict[str, str]
         ) -> pl.Series:
         """
         Southampton Fare/Age*multiplier
         """
         df = pl.DataFrame({"age": srs[0], 
@@ -64,34 +71,32 @@
                            "e": srs[2]}) 
         # Add Indicator Column for Southampton
         df = df.with_columns(pl.when(pl.col("e")=="S").then(1).otherwise(0).alias("S")) 
         multiplier = float(kwargs.get("multiplier", 1))
         res = df["S"] * df["fare"] / df["age"] * multiplier
         return res
 
-def example_dep_calc(kwargs: dict[str, str]) -> pl.Expr:
-    return pl.col("SurvivalMeanAge_sum") + pl.col("SouthamptonFareDivAge_sum")
-
 # inputs for the custom_calculator srs param
 inputs = ["age", "fare", "embarked"]
-# (Optional) - we are only interested in Southampton
-# unless other measures requested
-precompute_filter = ul.EqFilter("embarked", "S")
 # We return Floats
 res_type = pl.Float64
 # We return a Series, not a scalar (which otherwise would be auto exploded)
 returns_scalar = False
 
 measures = [
             ul.BaseMeasure(
                 "SouthamptonFareDivAge",
                 ul.CustomCalculator(
                     custom_calculator, res_type, inputs, returns_scalar
                 ),
-                [[precompute_filter]],
+                # (Optional) - we are only interested in Southampton, so
+                # unless other measures requested we might as well filter for Southampton only
+                # However, if if multiple measures requested, their precompute_filters will be joined as OR.
+                [[ul.EqFilter("embarked", "S")]],
+                # PARAMS tab of the UI
                 calc_params=[ul.CalcParam("mltplr", "1", "float")]
             ),
             ul.BaseMeasure(
                 "SurvivalMeanAge",
                 ul.StandardCalculator(survival_mean_age),
                 aggregation_restriction="sum",
             ),
```

#### html2text {}

```diff
@@ -14,34 +14,38 @@
 [Polars](https://github.com/pola-rs/polars) and Rust which make this possible.
 We use TypeScript for the frontend. # Examples Our userguide is under
 development. In the mean time refer to FRTB [userguide](https://ultimabi.uk/
 ultibi-frtb-book/). ## Python ```python import ultibi as ul import polars as pl
 import os os.environ["RUST_LOG"] = "info" # enable logs os.environ["ADDRESS"] =
 "0.0.0.0:8000" # host on this address # Read Data # for more details: https://
 pola-rs.github.io/polars/py-polars/html/reference/api/polars.read_csv.html df =
-pl.read_csv("titanic.csv") # Standard Calculator def survival_mean_age(kwargs:
-dict[str, str]) -> pl.Expr: """Mean Age of Survivals pl.col("survived") is 0 or
-1 pl.col("age") * pl.col("survived") - age of survived person, otherwise 0
-pl.col("survived").sum() - number of survived """ return pl.col("age") * pl.col
-("survived") / pl.col("survived").sum() def custom_calculator( srs: list
-[pl.Series], kwargs: dict[str, str] ) -> pl.Series: """ Southampton Fare/
-Age*multiplier """ df = pl.DataFrame({"age": srs[0], "fare": srs[1], "e": srs
-[2]}) # Add Indicator Column for Southampton df = df.with_columns(pl.when
+pl.read_csv("titanic.csv") # Let's add some Custom/Bespoke Calculations to our
+UI # Standard Calculator def survival_mean_age(kwargs: dict[str, str]) -
+> pl.Expr: """Mean Age of Survivals pl.col("survived") is 0 or 1 pl.col("age")
+* pl.col("survived") - age of survived person, otherwise 0 pl.col
+("survived").sum() - number of survived """ return pl.col("age") * pl.col
+("survived") / pl.col("survived").sum() # Also a Standard Calculator def
+example_dep_calc(kwargs: dict[str, str]) -> pl.Expr: return pl.col
+("SurvivalMeanAge_sum") + pl.col("SouthamptonFareDivAge_sum") # When we need
+more involved calculations we go for a Custom Calculator def custom_calculator
+( srs: list[pl.Series], kwargs: dict[str, str] ) -> pl.Series: """ Southampton
+Fare/Age*multiplier """ df = pl.DataFrame({"age": srs[0], "fare": srs[1], "e":
+srs[2]}) # Add Indicator Column for Southampton df = df.with_columns(pl.when
 (pl.col("e")=="S").then(1).otherwise(0).alias("S")) multiplier = float
 (kwargs.get("multiplier", 1)) res = df["S"] * df["fare"] / df["age"] *
-multiplier return res def example_dep_calc(kwargs: dict[str, str]) -> pl.Expr:
-return pl.col("SurvivalMeanAge_sum") + pl.col("SouthamptonFareDivAge_sum") #
-inputs for the custom_calculator srs param inputs = ["age", "fare", "embarked"]
-# (Optional) - we are only interested in Southampton # unless other measures
-requested precompute_filter = ul.EqFilter("embarked", "S") # We return Floats
-res_type = pl.Float64 # We return a Series, not a scalar (which otherwise would
-be auto exploded) returns_scalar = False measures = [ ul.BaseMeasure
-( "SouthamptonFareDivAge", ul.CustomCalculator( custom_calculator, res_type,
-inputs, returns_scalar ), [[precompute_filter]], calc_params=[ul.CalcParam
-("mltplr", "1", "float")] ), ul.BaseMeasure( "SurvivalMeanAge",
+multiplier return res # inputs for the custom_calculator srs param inputs =
+["age", "fare", "embarked"] # We return Floats res_type = pl.Float64 # We
+return a Series, not a scalar (which otherwise would be auto exploded)
+returns_scalar = False measures = [ ul.BaseMeasure( "SouthamptonFareDivAge",
+ul.CustomCalculator( custom_calculator, res_type, inputs, returns_scalar ), #
+(Optional) - we are only interested in Southampton, so # unless other measures
+requested we might as well filter for Southampton only # However, if if
+multiple measures requested, their precompute_filters will be joined as OR. [
+[ul.EqFilter("embarked", "S")]], # PARAMS tab of the UI calc_params=
+[ul.CalcParam("mltplr", "1", "float")] ), ul.BaseMeasure( "SurvivalMeanAge",
 ul.StandardCalculator(survival_mean_age), aggregation_restriction="sum", ),
 ul.DependantMeasure( "A_Dependant_Measure", ul.StandardCalculator
 (example_dep_calc), [("SurvivalMeanAge", "sum"), ("SouthamptonFareDivAge",
 "sum")], ), ] # Convert it into an Ultibi DataSet ds = ul.DataSet.from_frame
 (df, bespoke_measures=measures) # By default (might change in the future) #
 Fields are Utf8 (non numerics) and integers # Measures are numeric columns.
 ds.ui() ``` Then navigate to `http://localhost:8000` or checkout `http://
```

### Comparing `ultibi-0.3.1/example.py` & `ultibi-0.3.2/example.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/src/calculator.rs` & `ultibi-0.3.2/src/calculator.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/src/conversions/series.rs` & `ultibi-0.3.2/src/conversions/series.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/src/conversions/wrappers.rs` & `ultibi-0.3.2/src/conversions/wrappers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/src/dataset.rs` & `ultibi-0.3.2/src/dataset.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/src/errors.rs` & `ultibi-0.3.2/src/errors.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/src/filter.rs` & `ultibi-0.3.2/src/filter.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/src/lib.rs` & `ultibi-0.3.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/src/measure.rs` & `ultibi-0.3.2/src/measure.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/src/requests.rs` & `ultibi-0.3.2/src/requests.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/tests/data/datasource_config.toml` & `ultibi-0.3.2/tests/data/datasource_config.toml`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/tests/docs/run_doc_examples.py` & `ultibi-0.3.2/tests/docs/run_doc_examples.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/tests/unit/test_compute.py` & `ultibi-0.3.2/tests/unit/test_compute.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/tests/unit/test_ds.py` & `ultibi-0.3.2/tests/unit/test_ds.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/tests/unit/test_measure.py` & `ultibi-0.3.2/tests/unit/test_measure.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/ultibi/__init__.py` & `ultibi-0.3.2/ultibi/__init__.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/ultibi/internals/__init__.py` & `ultibi-0.3.2/ultibi/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/ultibi/internals/dataset.py` & `ultibi-0.3.2/ultibi/internals/dataset.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/ultibi/internals/filters.py` & `ultibi-0.3.2/ultibi/internals/filters.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/ultibi/internals/measure.py` & `ultibi-0.3.2/ultibi/internals/measure.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/ultibi/internals/requests.py` & `ultibi-0.3.2/ultibi/internals/requests.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.1/Cargo.lock` & `ultibi-0.3.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -260,17 +260,17 @@
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "alloc-no-stdlib"
 version = "2.0.4"
@@ -293,17 +293,17 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anstream"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e579a7752471abc2a8268df8b20005e3eadd975f585398f17efcfd8d4927371"
+checksum = "6342bd4f5a1205d7f41e94a41a901f5647c938cdfa96036338e8533c9d6c2450"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
  "is-terminal",
@@ -332,17 +332,17 @@
 checksum = "5ca11d4be1bab0c8bc8734a9aa7bf4ee8316d462a08c6ac5052f888fef5b494b"
 dependencies = [
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "anstyle-wincon"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4bcd8291a340dd8ac70e18878bc4501dd7b4ff970cfa21c207d36ece51ea88fd"
+checksum = "180abfa45703aebe0093f79badacc01b8fd4ea2e35118747e5811127f926e188"
 dependencies = [
  "anstyle",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "anyhow"
@@ -808,17 +808,17 @@
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.12.0"
+version = "3.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
+checksum = "9b1ce199063694f33ffb7dd4e0ee620741495c32833cde5aa08f02a0bf96f0c8"
 
 [[package]]
 name = "bytemuck"
 version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
 dependencies = [
@@ -1009,17 +1009,17 @@
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.6"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "280a9f2d8b3a38871a3c8a46fb80db65e5e5ed97da80c4d08bf27fb63e35e181"
+checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32c"
 version = "0.6.3"
@@ -1374,15 +1374,15 @@
 checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "frtb_engine"
-version = "0.3.1"
+version = "0.3.2"
 dependencies = [
  "log",
  "ndarray",
  "once_cell",
  "polars",
  "rayon",
  "serde",
@@ -1907,17 +1907,17 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.141"
+version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "libm"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
 
@@ -1938,17 +1938,17 @@
 checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.3.2"
+version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3f508063cc7bb32987c71511216bd5a32be15bccb6a80b52df8b9d7f01fc3aa2"
+checksum = "36eb31c1778188ae1e64398743890d0877fef36d11521ac60406b42016e8c2cf"
 
 [[package]]
 name = "local-channel"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f303ec0e94c6c54447f84f3b0ef7af769858a9c4ef56ef2a986d3dcd4c3fc9c"
 dependencies = [
@@ -2001,17 +2001,17 @@
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "matrixmultiply"
-version = "0.3.2"
+version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "add85d4dd35074e6fedc608f8c8f513a3548619a9024b751949ef0e8e45a4d84"
+checksum = "bb99c395ae250e1bf9133673f03ca9f97b7e71b705436bf8f089453445d1e9fe"
 dependencies = [
  "num_cpus",
  "once_cell",
  "rawpointer",
  "thread-tree",
 ]
 
@@ -2156,17 +2156,17 @@
 checksum = "6d89e9874397a1f0a52fc1f197a8effd9735223cb2390e9dcc83ac6cd02923d0"
 dependencies = [
  "chrono",
 ]
 
 [[package]]
 name = "ntapi"
-version = "0.4.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bc51db7b362b205941f71232e56c625156eb9a929f8cf74a428fd5bc094a4afc"
+checksum = "e8a3895c6391c39d7fe7ebc444a87eb2991b2a0bc718fdabd071eec617fc68e4"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "num-complex"
 version = "0.4.3"
@@ -2210,17 +2210,17 @@
 name = "once_cell"
 version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "openssl"
-version = "0.10.50"
+version = "0.10.52"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e30d8bc91859781f0a943411186324d580f2bbeb71b452fe91ae344806af3f1"
+checksum = "01b8574602df80f7b85fdfc5392fa884a4e3b3f4f35402c070ab34c3d3f78d56"
 dependencies = [
  "bitflags",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
@@ -2242,17 +2242,17 @@
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.85"
+version = "0.9.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d3d193fb1488ad46ffe3aaabc912cc931d02ee8518fe2959aea8ef52718b0c0"
+checksum = "8e17f59264b2809d77ae94f0e1ebabc434773f370d6ca667bd223ea10e06cc7e"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
@@ -2711,15 +2711,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyultima"
-version = "0.3.1"
+version = "0.3.2"
 dependencies = [
  "frtb_engine",
  "once_cell",
  "polars",
  "polars-arrow",
  "pyo3",
  "serde_json",
@@ -2837,28 +2837,28 @@
  "getrandom",
  "redox_syscall 0.2.16",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.3"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b1f693b24f6ac912f4893ef08244d70b6067480d2f1a46e950c9691e6749d1d"
+checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.29"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
 
 [[package]]
 name = "reqwest"
 version = "0.11.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "27b71749df584b7f4cac2c426c127a7c785a5106cc98f7a8feb044115f0fa254"
 dependencies = [
@@ -2950,17 +2950,17 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.37.12"
+version = "0.37.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "722529a737f5a942fdbac3a46cee213053196737c5eaa3386d52e85b786f2659"
+checksum = "d9b864d3c18a5785a05953adeed93e2dca37ed30f18e69bba9f30079d51f363f"
 dependencies = [
  "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.48.0",
@@ -3325,17 +3325,17 @@
 name = "target-features"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "24840de800c1707d75c800893dbd727a5e1501ce921944e602f0698167491e36"
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tempfile"
 version = "3.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9fbec84f381d5795b08656e4912bec604d162bff9291d6189a78f4c8ab87998"
 dependencies = [
@@ -3344,15 +3344,15 @@
  "redox_syscall 0.3.5",
  "rustix",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "template_drivers"
-version = "0.3.1"
+version = "0.3.2"
 dependencies = [
  "actix-files",
  "actix-web",
  "actix-web-httpauth",
  "actix-web-static-files",
  "anyhow",
  "clap",
@@ -3614,21 +3614,21 @@
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4017f8f45139870ca7e672686113917c71c7a6e02d4924eda67186083c03081a"
+checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
@@ -3646,42 +3646,43 @@
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "ultibi"
-version = "0.3.1"
+version = "0.3.2"
 dependencies = [
  "ultibi_core",
  "ultibi_server",
 ]
 
 [[package]]
 name = "ultibi_core"
-version = "0.3.1"
+version = "0.3.2"
 dependencies = [
  "aws-config",
  "aws-sdk-s3",
  "dashmap",
  "derivative",
  "futures",
  "once_cell",
  "polars",
  "quote",
  "serde",
  "serde_json",
+ "thiserror",
  "tokio",
  "toml",
  "utoipa",
 ]
 
 [[package]]
 name = "ultibi_server"
-version = "0.3.1"
+version = "0.3.2"
 dependencies = [
  "actix-web",
  "actix-web-static-files",
  "anyhow",
  "dotenv",
  "log",
  "mime",
```

### Comparing `ultibi-0.3.1/PKG-INFO` & `ultibi-0.3.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 Metadata-Version: 2.1
 Name: ultibi
-Version: 0.3.1
+Version: 0.3.2
 Classifier: Programming Language :: Rust
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: License :: Free for non-commercial use
+Classifier: Topic :: Scientific/Engineering
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: polars
 Requires-Dist: pyarrow
+License-File: LICENSE
+Summary: Flexible DataFrame Operations via UI
+Keywords: dataframe,visualization,aggregation,calculation,chart,data,dataviz,pivot-table,frtb,risk
+Author-email: Anatoly Bugakov <anatoly@ultimabi.uk>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Source Code, https://github.com/ultima-ib/ultima/
+Project-URL: Documentation, https://ultimabi.uk/ultibi-frtb-book/
+Project-URL: Homepage, https://ultimabi.uk/
+Project-URL: Repository, https://github.com/ultima-ib/ultibi-frtb-book
 
 <br>
 
 <p align="center">
     <a href="https://ultimabi.uk/" target="_blank">
     <img width="900" src="https://ultima-bi.s3.eu-west-2.amazonaws.com/imgs/logo.png" alt="Ultima Logo">
     </a>
@@ -26,15 +36,15 @@
 # The Ultimate BI tool
 With `Ultibi` you can turn your `DataFrame` into a pivot table with a UI and share it across organisation. You can also define measures applicable to your `DataFrame`.  This means your colleagues/consumers don't have to write any code to analyse the data.
 
 <br>
 
 <p align="center">
     <a href="https://frtb.demo.ultimabi.uk/" target="_blank">
-    <img width="900" src="https://ultima-bi.s3.eu-west-2.amazonaws.com/imgs/titanic_gif.gif" alt="Ultima Logo">
+    <img width="900" src="https://ultima-bi.s3.eu-west-2.amazonaws.com/imgs/UltimaScreenshotExplained.jpg" alt="Ultima Logo">
     </a>
 </p>
 
 <br>
 
 Ultibi leverages on the giants: [Actix](https://github.com/actix/actix-web), [Polars](https://github.com/pola-rs/polars) and Rust which make this possible. We use TypeScript for the frontend.
 
@@ -52,23 +62,30 @@
 os.environ["RUST_LOG"] = "info" # enable logs
 os.environ["ADDRESS"] = "0.0.0.0:8000" # host on this address
 
 # Read Data
 # for more details: https://pola-rs.github.io/polars/py-polars/html/reference/api/polars.read_csv.html
 df = pl.read_csv("titanic.csv")
 
+# Let's add some Custom/Bespoke Calculations to our UI
+
 # Standard Calculator
 def survival_mean_age(kwargs: dict[str, str]) -> pl.Expr:
     """Mean Age of Survivals
     pl.col("survived") is 0 or 1
     pl.col("age") * pl.col("survived") - age of survived person, otherwise 0
     pl.col("survived").sum() - number of survived
     """
     return pl.col("age") * pl.col("survived") / pl.col("survived").sum()
 
+# Also a Standard Calculator
+def example_dep_calc(kwargs: dict[str, str]) -> pl.Expr:
+    return pl.col("SurvivalMeanAge_sum") + pl.col("SouthamptonFareDivAge_sum")
+
+# When we need more involved calculations we go for a Custom Calculator
 def custom_calculator(
             srs: list[pl.Series], kwargs: dict[str, str]
         ) -> pl.Series:
         """
         Southampton Fare/Age*multiplier
         """
         df = pl.DataFrame({"age": srs[0], 
@@ -76,34 +93,32 @@
                            "e": srs[2]}) 
         # Add Indicator Column for Southampton
         df = df.with_columns(pl.when(pl.col("e")=="S").then(1).otherwise(0).alias("S")) 
         multiplier = float(kwargs.get("multiplier", 1))
         res = df["S"] * df["fare"] / df["age"] * multiplier
         return res
 
-def example_dep_calc(kwargs: dict[str, str]) -> pl.Expr:
-    return pl.col("SurvivalMeanAge_sum") + pl.col("SouthamptonFareDivAge_sum")
-
 # inputs for the custom_calculator srs param
 inputs = ["age", "fare", "embarked"]
-# (Optional) - we are only interested in Southampton
-# unless other measures requested
-precompute_filter = ul.EqFilter("embarked", "S")
 # We return Floats
 res_type = pl.Float64
 # We return a Series, not a scalar (which otherwise would be auto exploded)
 returns_scalar = False
 
 measures = [
             ul.BaseMeasure(
                 "SouthamptonFareDivAge",
                 ul.CustomCalculator(
                     custom_calculator, res_type, inputs, returns_scalar
                 ),
-                [[precompute_filter]],
+                # (Optional) - we are only interested in Southampton, so
+                # unless other measures requested we might as well filter for Southampton only
+                # However, if if multiple measures requested, their precompute_filters will be joined as OR.
+                [[ul.EqFilter("embarked", "S")]],
+                # PARAMS tab of the UI
                 calc_params=[ul.CalcParam("mltplr", "1", "float")]
             ),
             ul.BaseMeasure(
                 "SurvivalMeanAge",
                 ul.StandardCalculator(survival_mean_age),
                 aggregation_restriction="sum",
             ),
```

#### html2text {}

```diff
@@ -1,13 +1,20 @@
-Metadata-Version: 2.1 Name: ultibi Version: 0.3.1 Classifier: Programming
-Language :: Rust Classifier: Programming Language :: Python :: Implementation
-:: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: polars Requires-Dist: pyarrow Requires-Python: >=3.7
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM Project-
-URL: Source Code, https://github.com/ultima-ib/ultima/
+Metadata-Version: 2.1 Name: ultibi Version: 0.3.2 Classifier: Programming
+Language :: Rust Classifier: License :: Free for non-commercial use Classifier:
+Topic :: Scientific/Engineering Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: polars Requires-Dist: pyarrow License-File: LICENSE Summary:
+Flexible DataFrame Operations via UI Keywords:
+dataframe,visualization,aggregation,calculation,chart,data,dataviz,pivot-
+table,frtb,risk Author-email: Anatoly Bugakov
+ultimabi.uk> Requires-Python: >=3.7 Description-Content-Type: text/markdown;
+charset=UTF-8; variant=GFM Project-URL: Documentation, https://ultimabi.uk/
+ultibi-frtb-book/ Project-URL: Homepage, https://ultimabi.uk/ Project-URL:
+Repository, https://github.com/ultima-ib/ultibi-frtb-book
                                  [Ultima_Logo]
 
                     **** the ultimate data analytics tool
          for no code visualisation and collaborative exploration. ****
          **** Present easier.   Dig deeper.   Review together.   ****
 # The Ultimate BI tool With `Ultibi` you can turn your `DataFrame` into a pivot
 table with a UI and share it across organisation. You can also define measures
@@ -19,34 +26,38 @@
 [Polars](https://github.com/pola-rs/polars) and Rust which make this possible.
 We use TypeScript for the frontend. # Examples Our userguide is under
 development. In the mean time refer to FRTB [userguide](https://ultimabi.uk/
 ultibi-frtb-book/). ## Python ```python import ultibi as ul import polars as pl
 import os os.environ["RUST_LOG"] = "info" # enable logs os.environ["ADDRESS"] =
 "0.0.0.0:8000" # host on this address # Read Data # for more details: https://
 pola-rs.github.io/polars/py-polars/html/reference/api/polars.read_csv.html df =
-pl.read_csv("titanic.csv") # Standard Calculator def survival_mean_age(kwargs:
-dict[str, str]) -> pl.Expr: """Mean Age of Survivals pl.col("survived") is 0 or
-1 pl.col("age") * pl.col("survived") - age of survived person, otherwise 0
-pl.col("survived").sum() - number of survived """ return pl.col("age") * pl.col
-("survived") / pl.col("survived").sum() def custom_calculator( srs: list
-[pl.Series], kwargs: dict[str, str] ) -> pl.Series: """ Southampton Fare/
-Age*multiplier """ df = pl.DataFrame({"age": srs[0], "fare": srs[1], "e": srs
-[2]}) # Add Indicator Column for Southampton df = df.with_columns(pl.when
+pl.read_csv("titanic.csv") # Let's add some Custom/Bespoke Calculations to our
+UI # Standard Calculator def survival_mean_age(kwargs: dict[str, str]) -
+> pl.Expr: """Mean Age of Survivals pl.col("survived") is 0 or 1 pl.col("age")
+* pl.col("survived") - age of survived person, otherwise 0 pl.col
+("survived").sum() - number of survived """ return pl.col("age") * pl.col
+("survived") / pl.col("survived").sum() # Also a Standard Calculator def
+example_dep_calc(kwargs: dict[str, str]) -> pl.Expr: return pl.col
+("SurvivalMeanAge_sum") + pl.col("SouthamptonFareDivAge_sum") # When we need
+more involved calculations we go for a Custom Calculator def custom_calculator
+( srs: list[pl.Series], kwargs: dict[str, str] ) -> pl.Series: """ Southampton
+Fare/Age*multiplier """ df = pl.DataFrame({"age": srs[0], "fare": srs[1], "e":
+srs[2]}) # Add Indicator Column for Southampton df = df.with_columns(pl.when
 (pl.col("e")=="S").then(1).otherwise(0).alias("S")) multiplier = float
 (kwargs.get("multiplier", 1)) res = df["S"] * df["fare"] / df["age"] *
-multiplier return res def example_dep_calc(kwargs: dict[str, str]) -> pl.Expr:
-return pl.col("SurvivalMeanAge_sum") + pl.col("SouthamptonFareDivAge_sum") #
-inputs for the custom_calculator srs param inputs = ["age", "fare", "embarked"]
-# (Optional) - we are only interested in Southampton # unless other measures
-requested precompute_filter = ul.EqFilter("embarked", "S") # We return Floats
-res_type = pl.Float64 # We return a Series, not a scalar (which otherwise would
-be auto exploded) returns_scalar = False measures = [ ul.BaseMeasure
-( "SouthamptonFareDivAge", ul.CustomCalculator( custom_calculator, res_type,
-inputs, returns_scalar ), [[precompute_filter]], calc_params=[ul.CalcParam
-("mltplr", "1", "float")] ), ul.BaseMeasure( "SurvivalMeanAge",
+multiplier return res # inputs for the custom_calculator srs param inputs =
+["age", "fare", "embarked"] # We return Floats res_type = pl.Float64 # We
+return a Series, not a scalar (which otherwise would be auto exploded)
+returns_scalar = False measures = [ ul.BaseMeasure( "SouthamptonFareDivAge",
+ul.CustomCalculator( custom_calculator, res_type, inputs, returns_scalar ), #
+(Optional) - we are only interested in Southampton, so # unless other measures
+requested we might as well filter for Southampton only # However, if if
+multiple measures requested, their precompute_filters will be joined as OR. [
+[ul.EqFilter("embarked", "S")]], # PARAMS tab of the UI calc_params=
+[ul.CalcParam("mltplr", "1", "float")] ), ul.BaseMeasure( "SurvivalMeanAge",
 ul.StandardCalculator(survival_mean_age), aggregation_restriction="sum", ),
 ul.DependantMeasure( "A_Dependant_Measure", ul.StandardCalculator
 (example_dep_calc), [("SurvivalMeanAge", "sum"), ("SouthamptonFareDivAge",
 "sum")], ), ] # Convert it into an Ultibi DataSet ds = ul.DataSet.from_frame
 (df, bespoke_measures=measures) # By default (might change in the future) #
 Fields are Utf8 (non numerics) and integers # Measures are numeric columns.
 ds.ui() ``` Then navigate to `http://localhost:8000` or checkout `http://
```

