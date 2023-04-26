# Comparing `tmp/fastly-1.3.0.tar.gz` & `tmp/fastly-1.3.1.tar.gz`

## Comparing `fastly-1.3.0.tar` & `fastly-1.3.1.tar`

### file list

```diff
@@ -1,1441 +1,1419 @@
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 fastly-1.3.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 fastly-1.3.0/CHANGELOG.md
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 fastly-1.3.0/MANIFEST.in
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 fastly-1.3.0/SECURITY.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fastly-1.3.0/requirements.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fastly-1.3.0/setup.cfg
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 fastly-1.3.0/setup.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastly-1.3.0/sig.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 fastly-1.3.0/test-requirements.txt
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 fastly-1.3.0/tox.ini
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 fastly-1.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rwxr-xr-x   0        0        0      619 2020-02-02 00:00:00.000000 fastly-1.3.0/.github/scripts/pack.sh
--rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 fastly-1.3.0/.github/scripts/prepare.sh
--rwxr-xr-x   0        0        0      812 2020-02-02 00:00:00.000000 fastly-1.3.0/.github/scripts/publish_env.sh
--rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 fastly-1.3.0/.github/scripts/release_body.sh
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 fastly-1.3.0/.github/workflows/ci-release.yaml
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Acl.md
--rw-r--r--   0        0        0    15695 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/AclApi.md
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/AclEntry.md
--rw-r--r--   0        0        0    20447 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/AclEntryApi.md
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/AclEntryResponse.md
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/AclEntryResponseAllOf.md
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/AclResponse.md
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/AclResponseAllOf.md
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ApexRedirect.md
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ApexRedirectAllOf.md
--rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ApexRedirectApi.md
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/AwsRegion.md
--rw-r--r--   0        0        0     5836 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Backend.md
--rw-r--r--   0        0        0    38224 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BackendApi.md
--rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BackendResponse.md
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BackendResponseAllOf.md
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Billing.md
--rw-r--r--   0        0        0    13259 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BillingAddressApi.md
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BillingAddressAttributes.md
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BillingAddressRequest.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BillingAddressRequestData.md
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BillingAddressResponse.md
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BillingAddressResponseData.md
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BillingAddressVerificationErrorResponse.md
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BillingAddressVerificationErrorResponseErrors.md
--rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BillingApi.md
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BillingEstimateResponse.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BillingEstimateResponseAllOf.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BillingEstimateResponseAllOfLine.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BillingEstimateResponseAllOfLines.md
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BillingResponse.md
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BillingResponseAllOf.md
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BillingResponseLineItem.md
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BillingResponseLineItemAllOf.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BillingStatus.md
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BillingTotal.md
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BillingTotalExtras.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BulkUpdateAclEntriesRequest.md
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BulkUpdateAclEntry.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BulkUpdateAclEntryAllOf.md
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BulkUpdateDictionaryItem.md
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BulkUpdateDictionaryItemAllOf.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BulkUpdateDictionaryListRequest.md
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BulkWafActiveRule.md
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/BulkWafActiveRules.md
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/CacheSetting.md
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/CacheSettingResponse.md
--rw-r--r--   0        0        0    18846 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/CacheSettingsApi.md
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Condition.md
--rw-r--r--   0        0        0    17741 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ConditionApi.md
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ConditionResponse.md
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ConditionsResponse.md
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Contact.md
--rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ContactApi.md
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ContactResponse.md
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ContactResponseAllOf.md
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Content.md
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ContentApi.md
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Customer.md
--rw-r--r--   0        0        0    18926 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/CustomerApi.md
--rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/CustomerResponse.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/CustomerResponseAllOf.md
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Dictionary.md
--rw-r--r--   0        0        0    17237 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/DictionaryApi.md
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/DictionaryInfoApi.md
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/DictionaryInfoResponse.md
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/DictionaryItem.md
--rw-r--r--   0        0        0    22127 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/DictionaryItemApi.md
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/DictionaryItemResponse.md
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/DictionaryItemResponseAllOf.md
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/DictionaryResponse.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/DictionaryResponseAllOf.md
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/DiffApi.md
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/DiffResponse.md
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Director.md
--rw-r--r--   0        0        0    15015 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/DirectorApi.md
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/DirectorBackend.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/DirectorBackendAllOf.md
--rw-r--r--   0        0        0     9981 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/DirectorBackendApi.md
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/DirectorResponse.md
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Domain.md
--rw-r--r--   0        0        0    21769 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/DomainApi.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/DomainCheckItem.md
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/DomainCheckResponse.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/DomainCheckResponseList.md
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/DomainOwnershipsApi.md
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/DomainResponse.md
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/DomainsResponse.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/EnabledProductResponse.md
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/EnabledProductResponseLinks.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/EnabledProductResponseProduct.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/EnabledProductResponseService.md
--rw-r--r--   0        0        0     8351 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/EnabledProductsApi.md
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ErrorResponse.md
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ErrorResponseData.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Event.md
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/EventAttributes.md
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/EventResponse.md
--rw-r--r--   0        0        0     7243 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/EventsApi.md
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/EventsResponse.md
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/EventsResponseAllOf.md
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/GenericTokenError.md
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Gzip.md
--rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/GzipApi.md
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/GzipResponse.md
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Header.md
--rw-r--r--   0        0        0    20925 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HeaderApi.md
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HeaderResponse.md
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Healthcheck.md
--rw-r--r--   0        0        0    20120 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HealthcheckApi.md
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HealthcheckResponse.md
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Historical.md
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HistoricalAggregateResponse.md
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HistoricalAggregateResponseAllOf.md
--rw-r--r--   0        0        0    39081 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HistoricalApi.md
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HistoricalFieldAggregateResponse.md
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HistoricalFieldAggregateResponseAllOf.md
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HistoricalFieldResponse.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HistoricalFieldResponseAllOf.md
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HistoricalFieldResults.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HistoricalMeta.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HistoricalRegionsResponse.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HistoricalRegionsResponseAllOf.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HistoricalResponse.md
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HistoricalResponseAllOf.md
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HistoricalResults.md
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HistoricalServices.md
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HistoricalUsageAggregateResponse.md
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HistoricalUsageMonthResponse.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HistoricalUsageMonthResponseAllOf.md
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HistoricalUsageMonthResponseAllOfData.md
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HistoricalUsageResults.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HistoricalUsageServiceResponse.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HistoricalUsageServiceResponseAllOf.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Http3.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Http3AllOf.md
--rw-r--r--   0        0        0     9629 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Http3Api.md
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HttpResponseFormat.md
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/HttpStreamFormat.md
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/IamPermission.md
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/IamPermissionsApi.md
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/IamRole.md
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/IamRoleAllOf.md
--rw-r--r--   0        0        0     9918 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/IamRolesApi.md
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/IamServiceGroup.md
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/IamServiceGroupAllOf.md
--rw-r--r--   0        0        0    11406 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/IamServiceGroupsApi.md
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/IamUserGroup.md
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/IamUserGroupAllOf.md
--rw-r--r--   0        0        0    17911 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/IamUserGroupsApi.md
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/IncludedWithWafActiveRule.md
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/IncludedWithWafActiveRuleItem.md
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/IncludedWithWafExclusion.md
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/IncludedWithWafExclusionItem.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/IncludedWithWafFirewall.md
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/IncludedWithWafFirewallVersion.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/IncludedWithWafFirewallVersionItem.md
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/IncludedWithWafRule.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/IncludedWithWafRuleItem.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/IncludedWithWafRuleRevision.md
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/InlineObject.md
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/InlineObject1.md
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/InlineResponse200.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/InlineResponse2001.md
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/InlineResponse2002.md
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/InlineResponse2002Meta.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/InlineResponse2003.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/InlineResponse2003Meta.md
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Invitation.md
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/InvitationData.md
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/InvitationDataAttributes.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/InvitationResponse.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/InvitationResponseAllOf.md
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/InvitationResponseData.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/InvitationResponseDataAllOf.md
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/InvitationsApi.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/InvitationsResponse.md
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/InvitationsResponseAllOf.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingAddressAndPort.md
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingAzureblob.md
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingAzureblobAllOf.md
--rw-r--r--   0        0        0    29125 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingAzureblobApi.md
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingAzureblobResponse.md
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingBigquery.md
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingBigqueryAllOf.md
--rw-r--r--   0        0        0    24678 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingBigqueryApi.md
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingBigqueryResponse.md
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingCloudfiles.md
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingCloudfilesAllOf.md
--rw-r--r--   0        0        0    27524 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingCloudfilesApi.md
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingCloudfilesResponse.md
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingCommon.md
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingDatadog.md
--rw-r--r--   0        0        0     3883 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingDatadogAllOf.md
--rw-r--r--   0        0        0    38955 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingDatadogApi.md
--rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingDatadogResponse.md
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingDigitalocean.md
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingDigitaloceanAllOf.md
--rw-r--r--   0        0        0    28174 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingDigitaloceanApi.md
--rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingDigitaloceanResponse.md
--rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingElasticsearch.md
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingElasticsearchAllOf.md
--rw-r--r--   0        0        0    30259 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingElasticsearchApi.md
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingElasticsearchResponse.md
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingFormatVersion.md
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingFtp.md
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingFtpAllOf.md
--rw-r--r--   0        0        0    27244 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingFtpApi.md
--rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingFtpResponse.md
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingGcs.md
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingGcsAllOf.md
--rw-r--r--   0        0        0    28487 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingGcsApi.md
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingGcsCommon.md
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingGcsResponse.md
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingGenericCommon.md
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingGooglePubsub.md
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingGooglePubsubAllOf.md
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingGooglePubsubResponse.md
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingHeroku.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingHerokuAllOf.md
--rw-r--r--   0        0        0    21127 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingHerokuApi.md
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingHerokuResponse.md
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingHoneycomb.md
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingHoneycombAllOf.md
--rw-r--r--   0        0        0    20986 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingHoneycombApi.md
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingHoneycombResponse.md
--rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingHttps.md
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingHttpsAllOf.md
--rw-r--r--   0        0        0    29036 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingHttpsApi.md
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingHttpsResponse.md
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingKafka.md
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingKafkaAllOf.md
--rw-r--r--   0        0        0    18733 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingKafkaApi.md
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingKafkaResponse.md
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingKinesis.md
--rw-r--r--   0        0        0    17289 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingKinesisApi.md
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingKinesisResponse.md
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingLogentries.md
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingLogentriesAllOf.md
--rw-r--r--   0        0        0    22258 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingLogentriesApi.md
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingLogentriesResponse.md
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingLoggly.md
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingLogglyAllOf.md
--rw-r--r--   0        0        0    20871 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingLogglyApi.md
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingLogglyResponse.md
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingLogshuttle.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingLogshuttleAllOf.md
--rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingLogshuttleApi.md
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingLogshuttleResponse.md
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingMessageType.md
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingNewrelic.md
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingNewrelicAllOf.md
--rw-r--r--   0        0        0    25794 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingNewrelicApi.md
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingNewrelicResponse.md
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingOpenstack.md
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingOpenstackAllOf.md
--rw-r--r--   0        0        0    27216 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingOpenstackApi.md
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingOpenstackResponse.md
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingPapertrail.md
--rw-r--r--   0        0        0    21189 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingPapertrailApi.md
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingPapertrailResponse.md
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingPlacement.md
--rw-r--r--   0        0        0    24358 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingPubsubApi.md
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingRequestCapsCommon.md
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingS3.md
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingS3AllOf.md
--rw-r--r--   0        0        0    31697 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingS3Api.md
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingS3Response.md
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingScalyr.md
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingScalyrAllOf.md
--rw-r--r--   0        0        0    21715 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingScalyrApi.md
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingScalyrResponse.md
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingSftp.md
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingSftpAllOf.md
--rw-r--r--   0        0        0    28475 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingSftpApi.md
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingSftpResponse.md
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingSplunk.md
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingSplunkAllOf.md
--rw-r--r--   0        0        0    26444 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingSplunkApi.md
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingSplunkResponse.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingSumologic.md
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingSumologicAllOf.md
--rw-r--r--   0        0        0    21088 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingSumologicApi.md
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingSumologicResponse.md
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingSyslog.md
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingSyslogAllOf.md
--rw-r--r--   0        0        0    26805 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingSyslogApi.md
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingSyslogResponse.md
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingTlsCommon.md
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/LoggingUseTls.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/MutualAuthentication.md
--rw-r--r--   0        0        0    17143 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/MutualAuthenticationApi.md
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/MutualAuthenticationData.md
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/MutualAuthenticationDataAttributes.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/MutualAuthenticationResponse.md
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/MutualAuthenticationResponseAttributes.md
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/MutualAuthenticationResponseAttributesAllOf.md
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/MutualAuthenticationResponseData.md
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/MutualAuthenticationResponseDataAllOf.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/MutualAuthenticationsResponse.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/MutualAuthenticationsResponseAllOf.md
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/NumberVersion.md
--rw-r--r--   0        0        0    10438 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ObjectStoreApi.md
--rw-r--r--   0        0        0    12896 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ObjectStoreItemApi.md
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Package.md
--rw-r--r--   0        0        0     6678 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/PackageApi.md
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/PackageMetadata.md
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/PackageResponse.md
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/PackageResponseAllOf.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Pagination.md
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/PaginationLinks.md
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/PaginationMeta.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Permission.md
--rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Pool.md
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/PoolAllOf.md
--rw-r--r--   0        0        0    29387 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/PoolApi.md
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/PoolResponse.md
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/PoolResponseAllOf.md
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Pop.md
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/PopApi.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/PopCoordinates.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/PublicIpList.md
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/PublicIpListApi.md
--rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/PublishApi.md
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/PublishItem.md
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/PublishItemFormats.md
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/PublishRequest.md
--rw-r--r--   0        0        0    10418 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/PurgeApi.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/PurgeKeys.md
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/PurgeKeysResponse.md
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/PurgeResponse.md
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RateLimiter.md
--rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RateLimiterApi.md
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RateLimiterResponse.md
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RateLimiterResponse1.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RateLimiterResponseAllOf.md
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Realtime.md
--rw-r--r--   0        0        0     8759 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RealtimeApi.md
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RealtimeEntry.md
--rw-r--r--   0        0        0    27181 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RealtimeMeasurements.md
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipCommonName.md
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipCustomer.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipCustomerCustomer.md
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipMemberCustomer.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipMemberMutualAuthentication.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipMemberService.md
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipMemberServiceInvitation.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipMemberTlsActivation.md
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipMemberTlsBulkCertificate.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipMemberTlsCertificate.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipMemberTlsConfiguration.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipMemberTlsDnsRecord.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipMemberTlsDomain.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipMemberTlsPrivateKey.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipMemberTlsSubscription.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipMemberWafActiveRule.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipMemberWafFirewall.md
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipMemberWafFirewallVersion.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipMemberWafRule.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipMemberWafRuleRevision.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipMemberWafTag.md
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipMutualAuthentication.md
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipMutualAuthenticationMutualAuthentication.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipMutualAuthentications.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipMutualAuthenticationsMutualAuthentications.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipService.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipServiceInvitations.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipServiceInvitationsCreate.md
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipServiceInvitationsCreateServiceInvitations.md
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipServiceInvitationsServiceInvitations.md
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipServices.md
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipServicesServices.md
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsActivation.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsActivationTlsActivation.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsActivations.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsBulkCertificate.md
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsBulkCertificateTlsBulkCertificate.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsBulkCertificates.md
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsCertificate.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsCertificateTlsCertificate.md
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsCertificates.md
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsCertificatesTlsCertificates.md
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsConfiguration.md
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsConfigurationTlsConfiguration.md
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsConfigurations.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsConfigurationsTlsConfigurations.md
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsDnsRecord.md
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsDnsRecordDnsRecord.md
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsDnsRecords.md
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsDomain.md
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsDomainTlsDomain.md
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsDomains.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsDomainsTlsDomains.md
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsPrivateKey.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsPrivateKeyTlsPrivateKey.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsPrivateKeys.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsPrivateKeysTlsPrivateKeys.md
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsSubscription.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsSubscriptionTlsSubscription.md
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipTlsSubscriptions.md
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipUser.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipUserUser.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipWafActiveRules.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipWafActiveRulesWafActiveRules.md
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipWafFirewall.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipWafFirewallVersion.md
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipWafFirewallVersionWafFirewallVersion.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipWafFirewallVersions.md
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipWafFirewallWafFirewall.md
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipWafRule.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipWafRuleRevision.md
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipWafRuleRevisionWafRuleRevisions.md
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipWafRuleRevisions.md
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipWafRuleWafRule.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipWafRules.md
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipWafTags.md
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipWafTagsWafTags.md
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipsForInvitation.md
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipsForMutualAuthentication.md
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipsForStar.md
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipsForTlsActivation.md
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipsForTlsBulkCertificate.md
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipsForTlsConfiguration.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipsForTlsCsr.md
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipsForTlsDomain.md
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipsForTlsPrivateKey.md
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipsForTlsSubscription.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipsForWafActiveRule.md
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipsForWafExclusion.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipsForWafFirewallVersion.md
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RelationshipsForWafRule.md
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RequestSettings.md
--rw-r--r--   0        0        0    15635 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RequestSettingsApi.md
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RequestSettingsResponse.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Resource.md
--rw-r--r--   0        0        0    15552 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ResourceApi.md
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ResourceResponse.md
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ResourceResponseAllOf.md
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ResponseObject.md
--rw-r--r--   0        0        0     8900 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ResponseObjectApi.md
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ResponseObjectResponse.md
--rw-r--r--   0        0        0    27069 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Results.md
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/RoleUser.md
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/SchemasContactResponse.md
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/SchemasSnippetResponse.md
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/SchemasUserResponse.md
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/SchemasVclResponse.md
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/SchemasVersion.md
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/SchemasVersionResponse.md
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/SchemasWafFirewallVersion.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/SchemasWafFirewallVersionData.md
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Server.md
--rw-r--r--   0        0        0    19968 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServerApi.md
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServerResponse.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServerResponseAllOf.md
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Service.md
--rw-r--r--   0        0        0    22475 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceApi.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceAuthorization.md
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceAuthorizationData.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceAuthorizationDataAttributes.md
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceAuthorizationDataRelationships.md
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceAuthorizationDataRelationshipsUser.md
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceAuthorizationDataRelationshipsUserData.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceAuthorizationResponse.md
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceAuthorizationResponseData.md
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceAuthorizationResponseDataAllOf.md
--rw-r--r--   0        0        0    16177 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceAuthorizationsApi.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceAuthorizationsResponse.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceAuthorizationsResponseAllOf.md
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceCreate.md
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceCreateAllOf.md
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceDetail.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceDetailAllOf.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceIdAndVersion.md
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceInvitation.md
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceInvitationData.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceInvitationDataAttributes.md
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceInvitationDataRelationships.md
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceInvitationResponse.md
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceInvitationResponseAllOf.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceInvitationResponseAllOfData.md
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceListResponse.md
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceListResponseAllOf.md
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceResponse.md
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceResponseAllOf.md
--rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceVersionDetail.md
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ServiceVersionDetailOrNull.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Settings.md
--rw-r--r--   0        0        0     7419 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/SettingsApi.md
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/SettingsResponse.md
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Snippet.md
--rw-r--r--   0        0        0    19425 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/SnippetApi.md
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/SnippetResponse.md
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/SnippetResponseAllOf.md
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Star.md
--rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/StarApi.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/StarData.md
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/StarResponse.md
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/StarResponseAllOf.md
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Stats.md
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/StatsApi.md
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Store.md
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/StoreResponse.md
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Timestamps.md
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TimestampsNoDelete.md
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsActivation.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsActivationData.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsActivationResponse.md
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsActivationResponseData.md
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsActivationResponseDataAllOf.md
--rw-r--r--   0        0        0    16586 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsActivationsApi.md
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsActivationsResponse.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsActivationsResponseAllOf.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsBulkCertificate.md
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsBulkCertificateData.md
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsBulkCertificateDataAttributes.md
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsBulkCertificateResponse.md
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsBulkCertificateResponseAttributes.md
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsBulkCertificateResponseAttributesAllOf.md
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsBulkCertificateResponseData.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsBulkCertificateResponseDataAllOf.md
--rw-r--r--   0        0        0    16217 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsBulkCertificatesApi.md
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsBulkCertificatesResponse.md
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsBulkCertificatesResponseAllOf.md
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsCertificate.md
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsCertificateData.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsCertificateDataAttributes.md
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsCertificateResponse.md
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsCertificateResponseAttributes.md
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsCertificateResponseAttributesAllOf.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsCertificateResponseData.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsCertificateResponseDataAllOf.md
--rw-r--r--   0        0        0    16715 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsCertificatesApi.md
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsCertificatesResponse.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsCertificatesResponseAllOf.md
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsCommon.md
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsConfiguration.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsConfigurationData.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsConfigurationDataAttributes.md
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsConfigurationResponse.md
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsConfigurationResponseAttributes.md
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsConfigurationResponseAttributesAllOf.md
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsConfigurationResponseData.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsConfigurationResponseDataAllOf.md
--rw-r--r--   0        0        0    10339 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsConfigurationsApi.md
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsConfigurationsResponse.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsConfigurationsResponseAllOf.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsCsr.md
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsCsrData.md
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsCsrDataAttributes.md
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsCsrResponse.md
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsCsrResponseAttributes.md
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsCsrResponseData.md
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsCsrsApi.md
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsDnsRecord.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsDomainData.md
--rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsDomainsApi.md
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsDomainsResponse.md
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsDomainsResponseAllOf.md
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsPrivateKey.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsPrivateKeyData.md
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsPrivateKeyDataAttributes.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsPrivateKeyResponse.md
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsPrivateKeyResponseAttributes.md
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsPrivateKeyResponseAttributesAllOf.md
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsPrivateKeyResponseData.md
--rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsPrivateKeysApi.md
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsPrivateKeysResponse.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsPrivateKeysResponseAllOf.md
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsSubscription.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsSubscriptionData.md
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsSubscriptionDataAttributes.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsSubscriptionResponse.md
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsSubscriptionResponseAttributes.md
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsSubscriptionResponseAttributesAllOf.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsSubscriptionResponseData.md
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsSubscriptionResponseDataAllOf.md
--rw-r--r--   0        0        0    26148 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsSubscriptionsApi.md
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsSubscriptionsResponse.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TlsSubscriptionsResponseAllOf.md
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Token.md
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TokenCreatedResponse.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TokenCreatedResponseAllOf.md
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TokenResponse.md
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TokenResponseAllOf.md
--rw-r--r--   0        0        0    12243 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TokensApi.md
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeBillingAddress.md
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeContact.md
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeCustomer.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeEvent.md
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeInvitation.md
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeMutualAuthentication.md
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeResource.md
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeService.md
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeServiceAuthorization.md
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeServiceInvitation.md
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeStar.md
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeTlsActivation.md
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeTlsBulkCertificate.md
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeTlsCertificate.md
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeTlsConfiguration.md
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeTlsCsr.md
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeTlsDnsRecord.md
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeTlsDomain.md
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeTlsPrivateKey.md
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeTlsSubscription.md
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeUser.md
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeWafActiveRule.md
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeWafExclusion.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeWafFirewall.md
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeWafFirewallVersion.md
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeWafRule.md
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeWafRuleRevision.md
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/TypeWafTag.md
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/UpdateBillingAddressRequest.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/UpdateBillingAddressRequestData.md
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/User.md
--rw-r--r--   0        0        0    20765 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/UserApi.md
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/UserResponse.md
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/UserResponseAllOf.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ValidatorResult.md
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/ValidatorResultMessages.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Vcl.md
--rw-r--r--   0        0        0    32742 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/VclApi.md
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/VclDiff.md
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/VclDiffApi.md
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/VclResponse.md
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/Version.md
--rw-r--r--   0        0        0    26131 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/VersionApi.md
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/VersionCreateResponse.md
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/VersionDetail.md
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/VersionDetailSettings.md
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/VersionResponse.md
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/VersionResponseAllOf.md
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafActiveRule.md
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafActiveRuleCreationResponse.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafActiveRuleData.md
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafActiveRuleDataAttributes.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafActiveRuleResponse.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafActiveRuleResponseData.md
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafActiveRuleResponseDataAllOf.md
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafActiveRuleResponseDataAttributes.md
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafActiveRuleResponseDataAttributesAllOf.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafActiveRuleResponseDataRelationships.md
--rw-r--r--   0        0        0    27789 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafActiveRulesApi.md
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafActiveRulesResponse.md
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafActiveRulesResponseAllOf.md
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafExclusion.md
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafExclusionData.md
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafExclusionDataAttributes.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafExclusionResponse.md
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafExclusionResponseData.md
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafExclusionResponseDataAllOf.md
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafExclusionResponseDataAttributes.md
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafExclusionResponseDataAttributesAllOf.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafExclusionResponseDataRelationships.md
--rw-r--r--   0        0        0    19155 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafExclusionsApi.md
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafExclusionsResponse.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafExclusionsResponseAllOf.md
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafFirewall.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafFirewallData.md
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafFirewallDataAttributes.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafFirewallResponse.md
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafFirewallResponseData.md
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafFirewallResponseDataAllOf.md
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafFirewallResponseDataAttributes.md
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafFirewallResponseDataAttributesAllOf.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafFirewallVersion.md
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafFirewallVersionData.md
--rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafFirewallVersionDataAttributes.md
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafFirewallVersionResponse.md
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafFirewallVersionResponseData.md
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafFirewallVersionResponseDataAllOf.md
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafFirewallVersionResponseDataAttributes.md
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafFirewallVersionResponseDataAttributesAllOf.md
--rw-r--r--   0        0        0    24852 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafFirewallVersionsApi.md
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafFirewallVersionsResponse.md
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafFirewallVersionsResponseAllOf.md
--rw-r--r--   0        0        0    17211 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafFirewallsApi.md
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafFirewallsResponse.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafFirewallsResponseAllOf.md
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafRule.md
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafRuleAttributes.md
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafRuleResponse.md
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafRuleResponseData.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafRuleResponseDataAllOf.md
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafRuleRevision.md
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafRuleRevisionAttributes.md
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafRuleRevisionOrLatest.md
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafRuleRevisionResponse.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafRuleRevisionResponseData.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafRuleRevisionResponseDataAllOf.md
--rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafRuleRevisionsApi.md
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafRuleRevisionsResponse.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafRuleRevisionsResponseAllOf.md
--rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafRulesApi.md
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafRulesResponse.md
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafRulesResponseAllOf.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafTag.md
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafTagAttributes.md
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafTagsApi.md
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafTagsResponse.md
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafTagsResponseAllOf.md
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WafTagsResponseDataItem.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-1.3.0/docs/WsMessageFormat.md
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/__init__.py
--rw-r--r--   0        0        0    39346 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api_client.py
--rw-r--r--   0        0        0    18987 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/configuration.py
--rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/exceptions.py
--rw-r--r--   0        0        0    82524 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model_utils.py
--rw-r--r--   0        0        0    14634 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/rest.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/__init__.py
--rw-r--r--   0        0        0    29655 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/acl_api.py
--rw-r--r--   0        0        0    36324 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/acl_entry_api.py
--rw-r--r--   0        0        0    24178 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/apex_redirect_api.py
--rw-r--r--   0        0        0    53093 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/backend_api.py
--rw-r--r--   0        0        0    21781 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/billing_address_api.py
--rw-r--r--   0        0        0    18043 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/billing_api.py
--rw-r--r--   0        0        0    33343 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/cache_settings_api.py
--rw-r--r--   0        0        0    33323 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/condition_api.py
--rw-r--r--   0        0        0    11415 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/contact_api.py
--rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/content_api.py
--rw-r--r--   0        0        0    33521 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/customer_api.py
--rw-r--r--   0        0        0    30822 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/dictionary_api.py
--rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/dictionary_info_api.py
--rw-r--r--   0        0        0    38750 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/dictionary_item_api.py
--rw-r--r--   0        0        0     7805 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/diff_api.py
--rw-r--r--   0        0        0    26135 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/director_api.py
--rw-r--r--   0        0        0    20052 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/director_backend_api.py
--rw-r--r--   0        0        0    41462 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/domain_api.py
--rw-r--r--   0        0        0     5727 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/domain_ownerships_api.py
--rw-r--r--   0        0        0    17158 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/enabled_products_api.py
--rw-r--r--   0        0        0    13773 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/events_api.py
--rw-r--r--   0        0        0    31746 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/gzip_api.py
--rw-r--r--   0        0        0    37636 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/header_api.py
--rw-r--r--   0        0        0    36204 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/healthcheck_api.py
--rw-r--r--   0        0        0    58830 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/historical_api.py
--rw-r--r--   0        0        0    19004 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/http3_api.py
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/iam_permissions_api.py
--rw-r--r--   0        0        0    20715 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/iam_roles_api.py
--rw-r--r--   0        0        0    22040 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/iam_service_groups_api.py
--rw-r--r--   0        0        0    33266 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/iam_user_groups_api.py
--rw-r--r--   0        0        0    15947 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/invitations_api.py
--rw-r--r--   0        0        0    44535 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_azureblob_api.py
--rw-r--r--   0        0        0    39192 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_bigquery_api.py
--rw-r--r--   0        0        0    44242 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_cloudfiles_api.py
--rw-r--r--   0        0        0    41953 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_datadog_api.py
--rw-r--r--   0        0        0    43696 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_digitalocean_api.py
--rw-r--r--   0        0        0    44319 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_elasticsearch_api.py
--rw-r--r--   0        0        0    43522 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_ftp_api.py
--rw-r--r--   0        0        0    43855 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_gcs_api.py
--rw-r--r--   0        0        0    35557 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_heroku_api.py
--rw-r--r--   0        0        0    35714 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_honeycomb_api.py
--rw-r--r--   0        0        0    45205 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_https_api.py
--rw-r--r--   0        0        0    31840 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_kafka_api.py
--rw-r--r--   0        0        0    27552 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_kinesis_api.py
--rw-r--r--   0        0        0    37579 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_logentries_api.py
--rw-r--r--   0        0        0    35171 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_loggly_api.py
--rw-r--r--   0        0        0    35860 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_logshuttle_api.py
--rw-r--r--   0        0        0    37648 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_newrelic_api.py
--rw-r--r--   0        0        0    43132 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_openstack_api.py
--rw-r--r--   0        0        0    35725 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_papertrail_api.py
--rw-r--r--   0        0        0    38355 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_pubsub_api.py
--rw-r--r--   0        0        0    47867 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_s3_api.py
--rw-r--r--   0        0        0    36559 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_scalyr_api.py
--rw-r--r--   0        0        0    44447 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_sftp_api.py
--rw-r--r--   0        0        0    41345 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_splunk_api.py
--rw-r--r--   0        0        0    35657 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_sumologic_api.py
--rw-r--r--   0        0        0    42123 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/logging_syslog_api.py
--rw-r--r--   0        0        0    27942 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/mutual_authentication_api.py
--rw-r--r--   0        0        0    20697 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/object_store_api.py
--rw-r--r--   0        0        0    24093 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/object_store_item_api.py
--rw-r--r--   0        0        0    12532 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/package_api.py
--rw-r--r--   0        0        0    46444 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/pool_api.py
--rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/pop_api.py
--rw-r--r--   0        0        0     5681 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/public_ip_list_api.py
--rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/publish_api.py
--rw-r--r--   0        0        0    17849 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/purge_api.py
--rw-r--r--   0        0        0    16399 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/rate_limiter_api.py
--rw-r--r--   0        0        0    17309 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/realtime_api.py
--rw-r--r--   0        0        0    28563 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/request_settings_api.py
--rw-r--r--   0        0        0    29580 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/resource_api.py
--rw-r--r--   0        0        0    18201 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/response_object_api.py
--rw-r--r--   0        0        0    34128 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/server_api.py
--rw-r--r--   0        0        0    42868 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/service_api.py
--rw-r--r--   0        0        0    27001 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/service_authorizations_api.py
--rw-r--r--   0        0        0    13576 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/settings_api.py
--rw-r--r--   0        0        0    37746 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/snippet_api.py
--rw-r--r--   0        0        0    19785 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/star_api.py
--rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/stats_api.py
--rw-r--r--   0        0        0    28369 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/tls_activations_api.py
--rw-r--r--   0        0        0    27785 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/tls_bulk_certificates_api.py
--rw-r--r--   0        0        0    28246 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/tls_certificates_api.py
--rw-r--r--   0        0        0    17747 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/tls_configurations_api.py
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/tls_csrs_api.py
--rw-r--r--   0        0        0     8628 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/tls_domains_api.py
--rw-r--r--   0        0        0    21392 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/tls_private_keys_api.py
--rw-r--r--   0        0        0    42634 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/tls_subscriptions_api.py
--rw-r--r--   0        0        0    24152 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/tokens_api.py
--rw-r--r--   0        0        0    39118 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/user_api.py
--rw-r--r--   0        0        0    62802 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/vcl_api.py
--rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/vcl_diff_api.py
--rw-r--r--   0        0        0    50043 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/version_api.py
--rw-r--r--   0        0        0    44729 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/waf_active_rules_api.py
--rw-r--r--   0        0        0    33076 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/waf_exclusions_api.py
--rw-r--r--   0        0        0    35544 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/waf_firewall_versions_api.py
--rw-r--r--   0        0        0    28691 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/waf_firewalls_api.py
--rw-r--r--   0        0        0    13476 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/waf_rule_revisions_api.py
--rw-r--r--   0        0        0    13599 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/waf_rules_api.py
--rw-r--r--   0        0        0     7121 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/api/waf_tags_api.py
--rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/apis/__init__.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/__init__.py
--rw-r--r--   0        0        0    11622 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/acl.py
--rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/acl_entry.py
--rw-r--r--   0        0        0    17351 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/acl_entry_response.py
--rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/acl_entry_response_all_of.py
--rw-r--r--   0        0        0    15941 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/acl_response.py
--rw-r--r--   0        0        0    11415 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/acl_response_all_of.py
--rw-r--r--   0        0        0    16586 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/apex_redirect.py
--rw-r--r--   0        0        0    12580 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/apex_redirect_all_of.py
--rw-r--r--   0        0        0    14660 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/aws_region.py
--rw-r--r--   0        0        0    26110 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/backend.py
--rw-r--r--   0        0        0    30674 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/backend_response.py
--rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/backend_response_all_of.py
--rw-r--r--   0        0        0    14085 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/billing.py
--rw-r--r--   0        0        0    13567 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/billing_address_attributes.py
--rw-r--r--   0        0        0    12075 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/billing_address_request.py
--rw-r--r--   0        0        0    12080 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/billing_address_request_data.py
--rw-r--r--   0        0        0    11707 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/billing_address_response.py
--rw-r--r--   0        0        0    12794 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/billing_address_response_data.py
--rw-r--r--   0        0        0    11909 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/billing_address_verification_error_response.py
--rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/billing_address_verification_error_response_errors.py
--rw-r--r--   0        0        0    16877 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/billing_estimate_response.py
--rw-r--r--   0        0        0    11787 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/billing_estimate_response_all_of.py
--rw-r--r--   0        0        0    13188 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/billing_estimate_response_all_of_line.py
--rw-r--r--   0        0        0    11784 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/billing_estimate_response_all_of_lines.py
--rw-r--r--   0        0        0    16765 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/billing_response.py
--rw-r--r--   0        0        0    11716 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/billing_response_all_of.py
--rw-r--r--   0        0        0    18617 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/billing_response_line_item.py
--rw-r--r--   0        0        0    15190 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/billing_response_line_item_all_of.py
--rw-r--r--   0        0        0    12041 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/billing_status.py
--rw-r--r--   0        0        0    16362 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/billing_total.py
--rw-r--r--   0        0        0    12157 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/billing_total_extras.py
--rw-r--r--   0        0        0    11687 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/bulk_update_acl_entries_request.py
--rw-r--r--   0        0        0    15994 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/bulk_update_acl_entry.py
--rw-r--r--   0        0        0    11730 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/bulk_update_acl_entry_all_of.py
--rw-r--r--   0        0        0    14503 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/bulk_update_dictionary_item.py
--rw-r--r--   0        0        0    11584 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/bulk_update_dictionary_item_all_of.py
--rw-r--r--   0        0        0    11731 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/bulk_update_dictionary_list_request.py
--rw-r--r--   0        0        0    11735 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/bulk_waf_active_rule.py
--rw-r--r--   0        0        0    11638 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/bulk_waf_active_rules.py
--rw-r--r--   0        0        0    13506 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/cache_setting.py
--rw-r--r--   0        0        0    17524 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/cache_setting_response.py
--rw-r--r--   0        0        0    13530 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/condition.py
--rw-r--r--   0        0        0    16896 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/condition_response.py
--rw-r--r--   0        0        0    11911 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/conditions_response.py
--rw-r--r--   0        0        0    13577 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/contact.py
--rw-r--r--   0        0        0    17300 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/contact_response.py
--rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/contact_response_all_of.py
--rw-r--r--   0        0        0    12747 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/content.py
--rw-r--r--   0        0        0    20398 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/customer.py
--rw-r--r--   0        0        0    24131 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/customer_response.py
--rw-r--r--   0        0        0    11430 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/customer_response_all_of.py
--rw-r--r--   0        0        0    12110 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/dictionary.py
--rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/dictionary_info_response.py
--rw-r--r--   0        0        0    11765 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/dictionary_item.py
--rw-r--r--   0        0        0    15870 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/dictionary_item_response.py
--rw-r--r--   0        0        0    11758 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/dictionary_item_response_all_of.py
--rw-r--r--   0        0        0    16499 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/dictionary_response.py
--rw-r--r--   0        0        0    11436 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/dictionary_response_all_of.py
--rw-r--r--   0        0        0    12481 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/diff_response.py
--rw-r--r--   0        0        0    14620 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/director.py
--rw-r--r--   0        0        0    15768 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/director_backend.py
--rw-r--r--   0        0        0    11747 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/director_backend_all_of.py
--rw-r--r--   0        0        0    18553 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/director_response.py
--rw-r--r--   0        0        0    11783 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/domain.py
--rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/domain_check_item.py
--rw-r--r--   0        0        0    11897 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/domain_check_response.py
--rw-r--r--   0        0        0    11945 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/domain_check_response_list.py
--rw-r--r--   0        0        0    15770 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/domain_response.py
--rw-r--r--   0        0        0    11875 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/domains_response.py
--rw-r--r--   0        0        0    12604 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/enabled_product_response.py
--rw-r--r--   0        0        0    11739 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/enabled_product_response_links.py
--rw-r--r--   0        0        0    11694 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/enabled_product_response_product.py
--rw-r--r--   0        0        0    11694 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/enabled_product_response_service.py
--rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/error_response.py
--rw-r--r--   0        0        0    11593 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/error_response_data.py
--rw-r--r--   0        0        0    12088 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/event.py
--rw-r--r--   0        0        0    21129 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/event_attributes.py
--rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/event_response.py
--rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/events_response.py
--rw-r--r--   0        0        0    11554 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/events_response_all_of.py
--rw-r--r--   0        0        0    11395 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/generic_token_error.py
--rw-r--r--   0        0        0    12758 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/gzip.py
--rw-r--r--   0        0        0    16735 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/gzip_response.py
--rw-r--r--   0        0        0    15905 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/header.py
--rw-r--r--   0        0        0    19828 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/header_response.py
--rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/healthcheck.py
--rw-r--r--   0        0        0    18979 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/healthcheck_response.py
--rw-r--r--   0        0        0    12267 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/historical.py
--rw-r--r--   0        0        0    14970 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/historical_aggregate_response.py
--rw-r--r--   0        0        0    11672 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/historical_aggregate_response_all_of.py
--rw-r--r--   0        0        0    15047 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/historical_field_aggregate_response.py
--rw-r--r--   0        0        0    11723 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/historical_field_aggregate_response_all_of.py
--rw-r--r--   0        0        0    15004 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/historical_field_response.py
--rw-r--r--   0        0        0    11726 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/historical_field_response_all_of.py
--rw-r--r--   0        0        0    11740 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/historical_field_results.py
--rw-r--r--   0        0        0    11919 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/historical_meta.py
--rw-r--r--   0        0        0    14797 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/historical_regions_response.py
--rw-r--r--   0        0        0    11445 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/historical_regions_response_all_of.py
--rw-r--r--   0        0        0    15199 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/historical_response.py
--rw-r--r--   0        0        0    11947 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/historical_response_all_of.py
--rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/historical_results.py
--rw-r--r--   0        0        0    11403 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/historical_services.py
--rw-r--r--   0        0        0    15037 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/historical_usage_aggregate_response.py
--rw-r--r--   0        0        0    15124 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/historical_usage_month_response.py
--rw-r--r--   0        0        0    11820 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/historical_usage_month_response_all_of.py
--rw-r--r--   0        0        0    12346 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/historical_usage_month_response_all_of_data.py
--rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/historical_usage_results.py
--rw-r--r--   0        0        0    15031 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/historical_usage_service_response.py
--rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/historical_usage_service_response_all_of.py
--rw-r--r--   0        0        0    15675 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/http3.py
--rw-r--r--   0        0        0    11705 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/http3_all_of.py
--rw-r--r--   0        0        0    12796 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/http_response_format.py
--rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/http_stream_format.py
--rw-r--r--   0        0        0    13211 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/iam_permission.py
--rw-r--r--   0        0        0    15987 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/iam_role.py
--rw-r--r--   0        0        0    12962 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/iam_role_all_of.py
--rw-r--r--   0        0        0    15636 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/iam_service_group.py
--rw-r--r--   0        0        0    12570 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/iam_service_group_all_of.py
--rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/iam_user_group.py
--rw-r--r--   0        0        0    12926 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/iam_user_group_all_of.py
--rw-r--r--   0        0        0    12044 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/included_with_waf_active_rule.py
--rw-r--r--   0        0        0    15142 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/included_with_waf_active_rule_item.py
--rw-r--r--   0        0        0    12031 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/included_with_waf_exclusion.py
--rw-r--r--   0        0        0    14619 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/included_with_waf_exclusion_item.py
--rw-r--r--   0        0        0    12000 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/included_with_waf_firewall.py
--rw-r--r--   0        0        0    12104 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/included_with_waf_firewall_version.py
--rw-r--r--   0        0        0    13972 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/included_with_waf_firewall_version_item.py
--rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/included_with_waf_rule.py
--rw-r--r--   0        0        0    14599 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/included_with_waf_rule_item.py
--rw-r--r--   0        0        0    11848 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/included_with_waf_rule_revision.py
--rw-r--r--   0        0        0    11416 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/inline_object.py
--rw-r--r--   0        0        0    11419 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/inline_object1.py
--rw-r--r--   0        0        0    11418 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/inline_response200.py
--rw-r--r--   0        0        0    11605 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/inline_response2001.py
--rw-r--r--   0        0        0    11985 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/inline_response2002.py
--rw-r--r--   0        0        0    11725 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/inline_response2002_meta.py
--rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/inline_response2003.py
--rw-r--r--   0        0        0    11633 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/inline_response2003_meta.py
--rw-r--r--   0        0        0    11585 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/invitation.py
--rw-r--r--   0        0        0    12539 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/invitation_data.py
--rw-r--r--   0        0        0    12611 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/invitation_data_attributes.py
--rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/invitation_response.py
--rw-r--r--   0        0        0    11681 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/invitation_response_all_of.py
--rw-r--r--   0        0        0    14895 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/invitation_response_data.py
--rw-r--r--   0        0        0    12283 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/invitation_response_data_all_of.py
--rw-r--r--   0        0        0    14597 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/invitations_response.py
--rw-r--r--   0        0        0    11690 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/invitations_response_all_of.py
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_address_and_port.py
--rw-r--r--   0        0        0    22489 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_azureblob.py
--rw-r--r--   0        0        0    14206 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_azureblob_all_of.py
--rw-r--r--   0        0        0    24022 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_azureblob_response.py
--rw-r--r--   0        0        0    19390 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_bigquery.py
--rw-r--r--   0        0        0    13195 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_bigquery_all_of.py
--rw-r--r--   0        0        0    20943 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_bigquery_response.py
--rw-r--r--   0        0        0    21831 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_cloudfiles.py
--rw-r--r--   0        0        0    13543 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_cloudfiles_all_of.py
--rw-r--r--   0        0        0    23364 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_cloudfiles_response.py
--rw-r--r--   0        0        0    14144 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_common.py
--rw-r--r--   0        0        0    23211 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_datadog.py
--rw-r--r--   0        0        0    18487 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_datadog_all_of.py
--rw-r--r--   0        0        0    24914 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_datadog_response.py
--rw-r--r--   0        0        0    21812 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_digitalocean.py
--rw-r--r--   0        0        0    13514 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_digitalocean_all_of.py
--rw-r--r--   0        0        0    23345 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_digitalocean_response.py
--rw-r--r--   0        0        0    22734 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_elasticsearch.py
--rw-r--r--   0        0        0    14289 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_elasticsearch_all_of.py
--rw-r--r--   0        0        0    24096 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_elasticsearch_response.py
--rw-r--r--   0        0        0    12403 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_format_version.py
--rw-r--r--   0        0        0    22023 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_ftp.py
--rw-r--r--   0        0        0    13770 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_ftp_all_of.py
--rw-r--r--   0        0        0    23556 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_ftp_response.py
--rw-r--r--   0        0        0    22679 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_gcs.py
--rw-r--r--   0        0        0    12744 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_gcs_all_of.py
--rw-r--r--   0        0        0    12815 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_gcs_common.py
--rw-r--r--   0        0        0    24062 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_gcs_response.py
--rw-r--r--   0        0        0    14090 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_generic_common.py
--rw-r--r--   0        0        0    18898 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_google_pubsub.py
--rw-r--r--   0        0        0    12402 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_google_pubsub_all_of.py
--rw-r--r--   0        0        0    20451 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_google_pubsub_response.py
--rw-r--r--   0        0        0    17238 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_heroku.py
--rw-r--r--   0        0        0    11999 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_heroku_all_of.py
--rw-r--r--   0        0        0    18941 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_heroku_response.py
--rw-r--r--   0        0        0    17018 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_honeycomb.py
--rw-r--r--   0        0        0    12284 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_honeycomb_all_of.py
--rw-r--r--   0        0        0    18721 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_honeycomb_response.py
--rw-r--r--   0        0        0    23100 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_https.py
--rw-r--r--   0        0        0    15781 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_https_all_of.py
--rw-r--r--   0        0        0    24462 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_https_response.py
--rw-r--r--   0        0        0    23053 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_kafka.py
--rw-r--r--   0        0        0    15405 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_kafka_all_of.py
--rw-r--r--   0        0        0    24606 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_kafka_response.py
--rw-r--r--   0        0        0    16368 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_kinesis.py
--rw-r--r--   0        0        0    20332 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_kinesis_response.py
--rw-r--r--   0        0        0    18046 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_logentries.py
--rw-r--r--   0        0        0    12851 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_logentries_all_of.py
--rw-r--r--   0        0        0    19749 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_logentries_response.py
--rw-r--r--   0        0        0    16993 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_loggly.py
--rw-r--r--   0        0        0    11754 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_loggly_all_of.py
--rw-r--r--   0        0        0    18696 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_loggly_response.py
--rw-r--r--   0        0        0    17065 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_logshuttle.py
--rw-r--r--   0        0        0    11806 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_logshuttle_all_of.py
--rw-r--r--   0        0        0    18768 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_logshuttle_response.py
--rw-r--r--   0        0        0    11945 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_message_type.py
--rw-r--r--   0        0        0    18795 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_newrelic.py
--rw-r--r--   0        0        0    14066 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_newrelic_all_of.py
--rw-r--r--   0        0        0    20498 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_newrelic_response.py
--rw-r--r--   0        0        0    21509 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_openstack.py
--rw-r--r--   0        0        0    13226 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_openstack_all_of.py
--rw-r--r--   0        0        0    23042 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_openstack_response.py
--rw-r--r--   0        0        0    17068 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_papertrail.py
--rw-r--r--   0        0        0    18776 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_papertrail_response.py
--rw-r--r--   0        0        0    12818 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_placement.py
--rw-r--r--   0        0        0    12265 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_request_caps_common.py
--rw-r--r--   0        0        0    24622 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_s3.py
--rw-r--r--   0        0        0    16374 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_s3_all_of.py
--rw-r--r--   0        0        0    26155 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_s3_response.py
--rw-r--r--   0        0        0    17727 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_scalyr.py
--rw-r--r--   0        0        0    12488 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_scalyr_all_of.py
--rw-r--r--   0        0        0    19430 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_scalyr_response.py
--rw-r--r--   0        0        0    22808 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_sftp.py
--rw-r--r--   0        0        0    14123 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_sftp_all_of.py
--rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_sftp_response.py
--rw-r--r--   0        0        0    21030 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_splunk.py
--rw-r--r--   0        0        0    12164 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_splunk_all_of.py
--rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_splunk_response.py
--rw-r--r--   0        0        0    17102 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_sumologic.py
--rw-r--r--   0        0        0    11912 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_sumologic_all_of.py
--rw-r--r--   0        0        0    18805 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_sumologic_response.py
--rw-r--r--   0        0        0    21452 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_syslog.py
--rw-r--r--   0        0        0    13046 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_syslog_all_of.py
--rw-r--r--   0        0        0    22829 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_syslog_response.py
--rw-r--r--   0        0        0    13547 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_tls_common.py
--rw-r--r--   0        0        0    11595 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/logging_use_tls.py
--rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/mutual_authentication.py
--rw-r--r--   0        0        0    12711 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/mutual_authentication_data.py
--rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/mutual_authentication_data_attributes.py
--rw-r--r--   0        0        0    11767 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/mutual_authentication_response.py
--rw-r--r--   0        0        0    15149 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/mutual_authentication_response_attributes.py
--rw-r--r--   0        0        0    11647 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/mutual_authentication_response_attributes_all_of.py
--rw-r--r--   0        0        0    15368 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/mutual_authentication_response_data.py
--rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/mutual_authentication_response_data_all_of.py
--rw-r--r--   0        0        0    14749 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/mutual_authentications_response.py
--rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/mutual_authentications_response_all_of.py
--rw-r--r--   0        0        0    11906 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/number_version.py
--rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/package.py
--rw-r--r--   0        0        0    12863 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/package_metadata.py
--rw-r--r--   0        0        0    15990 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/package_response.py
--rw-r--r--   0        0        0    11519 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/package_response_all_of.py
--rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/pagination.py
--rw-r--r--   0        0        0    12267 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/pagination_links.py
--rw-r--r--   0        0        0    12484 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/pagination_meta.py
--rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/permission.py
--rw-r--r--   0        0        0    23511 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/pool.py
--rw-r--r--   0        0        0    18578 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/pool_all_of.py
--rw-r--r--   0        0        0    25586 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/pool_response.py
--rw-r--r--   0        0        0    11418 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/pool_response_all_of.py
--rw-r--r--   0        0        0    15216 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/pop.py
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/pop_coordinates.py
--rw-r--r--   0        0        0    11742 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/public_ip_list.py
--rw-r--r--   0        0        0    12528 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/publish_item.py
--rw-r--r--   0        0        0    12411 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/publish_item_formats.py
--rw-r--r--   0        0        0    11685 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/publish_request.py
--rw-r--r--   0        0        0    11432 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/purge_keys.py
--rw-r--r--   0        0        0    11165 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/purge_keys_response.py
--rw-r--r--   0        0        0    11594 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/purge_response.py
--rw-r--r--   0        0        0    19002 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/rate_limiter.py
--rw-r--r--   0        0        0    23413 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/rate_limiter_response.py
--rw-r--r--   0        0        0    12394 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/rate_limiter_response1.py
--rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/rate_limiter_response_all_of.py
--rw-r--r--   0        0        0    12619 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/realtime.py
--rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/realtime_entry.py
--rw-r--r--   0        0        0    97542 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/realtime_measurements.py
--rw-r--r--   0        0        0    11749 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_common_name.py
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_customer.py
--rw-r--r--   0        0        0    11730 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_customer_customer.py
--rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_member_customer.py
--rw-r--r--   0        0        0    11936 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_member_mutual_authentication.py
--rw-r--r--   0        0        0    11805 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_member_service.py
--rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_member_service_invitation.py
--rw-r--r--   0        0        0    11866 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_member_tls_activation.py
--rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_member_tls_bulk_certificate.py
--rw-r--r--   0        0        0    11876 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_member_tls_certificate.py
--rw-r--r--   0        0        0    11896 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_member_tls_configuration.py
--rw-r--r--   0        0        0    11857 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_member_tls_dns_record.py
--rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_member_tls_domain.py
--rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_member_tls_private_key.py
--rw-r--r--   0        0        0    11886 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_member_tls_subscription.py
--rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_member_waf_active_rule.py
--rw-r--r--   0        0        0    11846 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_member_waf_firewall.py
--rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_member_waf_firewall_version.py
--rw-r--r--   0        0        0    11806 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_member_waf_rule.py
--rw-r--r--   0        0        0    11995 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_member_waf_rule_revision.py
--rw-r--r--   0        0        0    11884 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_member_waf_tag.py
--rw-r--r--   0        0        0    12005 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_mutual_authentication.py
--rw-r--r--   0        0        0    11881 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_mutual_authentication_mutual_authentication.py
--rw-r--r--   0        0        0    12027 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_mutual_authentications.py
--rw-r--r--   0        0        0    11893 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_mutual_authentications_mutual_authentications.py
--rw-r--r--   0        0        0    11705 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_service.py
--rw-r--r--   0        0        0    11961 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_service_invitations.py
--rw-r--r--   0        0        0    12022 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_service_invitations_create.py
--rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_service_invitations_create_service_invitations.py
--rw-r--r--   0        0        0    11854 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_service_invitations_service_invitations.py
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_services.py
--rw-r--r--   0        0        0    11723 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_services_services.py
--rw-r--r--   0        0        0    11851 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_activation.py
--rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_activation_tls_activation.py
--rw-r--r--   0        0        0    11859 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_activations.py
--rw-r--r--   0        0        0    11968 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_bulk_certificate.py
--rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_bulk_certificate_tls_bulk_certificate.py
--rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_bulk_certificates.py
--rw-r--r--   0        0        0    11873 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_certificate.py
--rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_certificate_tls_certificate.py
--rw-r--r--   0        0        0    11895 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_certificates.py
--rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_certificates_tls_certificates.py
--rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_configuration.py
--rw-r--r--   0        0        0    11829 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_configuration_tls_configuration.py
--rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_configurations.py
--rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_configurations_tls_configurations.py
--rw-r--r--   0        0        0    11794 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_dns_record.py
--rw-r--r--   0        0        0    11775 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_dns_record_dns_record.py
--rw-r--r--   0        0        0    11802 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_dns_records.py
--rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_domain.py
--rw-r--r--   0        0        0    11738 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_domain_tls_domain.py
--rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_domains.py
--rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_domains_tls_domains.py
--rw-r--r--   0        0        0    11858 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_private_key.py
--rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_private_key_tls_private_key.py
--rw-r--r--   0        0        0    11880 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_private_keys.py
--rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_private_keys_tls_private_keys.py
--rw-r--r--   0        0        0    11895 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_subscription.py
--rw-r--r--   0        0        0    11822 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_subscription_tls_subscription.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_tls_subscriptions.py
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_user.py
--rw-r--r--   0        0        0    11836 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_user_user.py
--rw-r--r--   0        0        0    11880 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_waf_active_rules.py
--rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_waf_active_rules_waf_active_rules.py
--rw-r--r--   0        0        0    11807 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_waf_firewall.py
--rw-r--r--   0        0        0    11968 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_waf_firewall_version.py
--rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_waf_firewall_version_waf_firewall_version.py
--rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_waf_firewall_versions.py
--rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_waf_firewall_waf_firewall.py
--rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_waf_rule.py
--rw-r--r--   0        0        0    11914 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_waf_rule_revision.py
--rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_waf_rule_revision_waf_rule_revisions.py
--rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_waf_rule_revisions.py
--rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_waf_rule_waf_rule.py
--rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_waf_rules.py
--rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_waf_tags.py
--rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationship_waf_tags_waf_tags.py
--rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationships_for_invitation.py
--rw-r--r--   0        0        0    14050 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationships_for_mutual_authentication.py
--rw-r--r--   0        0        0    14345 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationships_for_star.py
--rw-r--r--   0        0        0    11882 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationships_for_tls_activation.py
--rw-r--r--   0        0        0    14690 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationships_for_tls_bulk_certificate.py
--rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationships_for_tls_configuration.py
--rw-r--r--   0        0        0    14006 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationships_for_tls_csr.py
--rw-r--r--   0        0        0    14687 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationships_for_tls_domain.py
--rw-r--r--   0        0        0    14589 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationships_for_tls_private_key.py
--rw-r--r--   0        0        0    15411 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationships_for_tls_subscription.py
--rw-r--r--   0        0        0    14951 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationships_for_waf_active_rule.py
--rw-r--r--   0        0        0    14691 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationships_for_waf_exclusion.py
--rw-r--r--   0        0        0    14940 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationships_for_waf_firewall_version.py
--rw-r--r--   0        0        0    14666 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/relationships_for_waf_rule.py
--rw-r--r--   0        0        0    15858 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/request_settings.py
--rw-r--r--   0        0        0    19891 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/request_settings_response.py
--rw-r--r--   0        0        0    11736 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/resource.py
--rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/resource_response.py
--rw-r--r--   0        0        0    12732 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/resource_response_all_of.py
--rw-r--r--   0        0        0    13673 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/response_object.py
--rw-r--r--   0        0        0    17701 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/response_object_response.py
--rw-r--r--   0        0        0    96777 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/results.py
--rw-r--r--   0        0        0    12451 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/role_user.py
--rw-r--r--   0        0        0    17321 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/schemas_contact_response.py
--rw-r--r--   0        0        0    17541 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/schemas_snippet_response.py
--rw-r--r--   0        0        0    18068 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/schemas_user_response.py
--rw-r--r--   0        0        0    15953 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/schemas_vcl_response.py
--rw-r--r--   0        0        0    13626 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/schemas_version.py
--rw-r--r--   0        0        0    17433 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/schemas_version_response.py
--rw-r--r--   0        0        0    11738 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/schemas_waf_firewall_version.py
--rw-r--r--   0        0        0    12179 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/schemas_waf_firewall_version_data.py
--rw-r--r--   0        0        0    14569 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/server.py
--rw-r--r--   0        0        0    18752 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/server_response.py
--rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/server_response_all_of.py
--rw-r--r--   0        0        0    12015 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service.py
--rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_authorization.py
--rw-r--r--   0        0        0    12718 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_authorization_data.py
--rw-r--r--   0        0        0    11658 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_authorization_data_attributes.py
--rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_authorization_data_relationships.py
--rw-r--r--   0        0        0    11899 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_authorization_data_relationships_user.py
--rw-r--r--   0        0        0    11844 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_authorization_data_relationships_user_data.py
--rw-r--r--   0        0        0    11767 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_authorization_response.py
--rw-r--r--   0        0        0    15176 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_authorization_response_data.py
--rw-r--r--   0        0        0    11863 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_authorization_response_data_all_of.py
--rw-r--r--   0        0        0    14749 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_authorizations_response.py
--rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_authorizations_response_all_of.py
--rw-r--r--   0        0        0    14640 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_create.py
--rw-r--r--   0        0        0    11543 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_create_all_of.py
--rw-r--r--   0        0        0    18255 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_detail.py
--rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_detail_all_of.py
--rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_id_and_version.py
--rw-r--r--   0        0        0    11656 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_invitation.py
--rw-r--r--   0        0        0    12646 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_invitation_data.py
--rw-r--r--   0        0        0    11922 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_invitation_data_attributes.py
--rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_invitation_data_relationships.py
--rw-r--r--   0        0        0    14111 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_invitation_response.py
--rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_invitation_response_all_of.py
--rw-r--r--   0        0        0    11854 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_invitation_response_all_of_data.py
--rw-r--r--   0        0        0    17024 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_list_response.py
--rw-r--r--   0        0        0    12407 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_list_response_all_of.py
--rw-r--r--   0        0        0    17544 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_response.py
--rw-r--r--   0        0        0    12948 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_response_all_of.py
--rw-r--r--   0        0        0    23835 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_version_detail.py
--rw-r--r--   0        0        0    23852 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/service_version_detail_or_null.py
--rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/settings.py
--rw-r--r--   0        0        0    15732 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/settings_response.py
--rw-r--r--   0        0        0    13161 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/snippet.py
--rw-r--r--   0        0        0    17520 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/snippet_response.py
--rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/snippet_response_all_of.py
--rw-r--r--   0        0        0    11525 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/star.py
--rw-r--r--   0        0        0    11945 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/star_data.py
--rw-r--r--   0        0        0    13825 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/star_response.py
--rw-r--r--   0        0        0    11571 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/star_response_all_of.py
--rw-r--r--   0        0        0    11555 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/stats.py
--rw-r--r--   0        0        0    11440 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/store.py
--rw-r--r--   0        0        0    11668 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/store_response.py
--rw-r--r--   0        0        0    12287 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/timestamps.py
--rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/timestamps_no_delete.py
--rw-r--r--   0        0        0    11616 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_activation.py
--rw-r--r--   0        0        0    12100 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_activation_data.py
--rw-r--r--   0        0        0    11697 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_activation_response.py
--rw-r--r--   0        0        0    14980 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_activation_response_data.py
--rw-r--r--   0        0        0    11842 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_activation_response_data_all_of.py
--rw-r--r--   0        0        0    14644 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_activations_response.py
--rw-r--r--   0        0        0    11721 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_activations_response_all_of.py
--rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_bulk_certificate.py
--rw-r--r--   0        0        0    12666 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_bulk_certificate_data.py
--rw-r--r--   0        0        0    12407 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_bulk_certificate_data_attributes.py
--rw-r--r--   0        0        0    11748 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_bulk_certificate_response.py
--rw-r--r--   0        0        0    16192 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_bulk_certificate_response_attributes.py
--rw-r--r--   0        0        0    12699 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_bulk_certificate_response_attributes_all_of.py
--rw-r--r--   0        0        0    15305 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_bulk_certificate_response_data.py
--rw-r--r--   0        0        0    12043 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_bulk_certificate_response_data_all_of.py
--rw-r--r--   0        0        0    14721 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_bulk_certificates_response.py
--rw-r--r--   0        0        0    11772 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_bulk_certificates_response_all_of.py
--rw-r--r--   0        0        0    11626 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_certificate.py
--rw-r--r--   0        0        0    12510 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_certificate_data.py
--rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_certificate_data_attributes.py
--rw-r--r--   0        0        0    11707 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_certificate_response.py
--rw-r--r--   0        0        0    17609 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_certificate_response_attributes.py
--rw-r--r--   0        0        0    14137 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_certificate_response_attributes_all_of.py
--rw-r--r--   0        0        0    15107 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_certificate_response_data.py
--rw-r--r--   0        0        0    12002 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_certificate_response_data_all_of.py
--rw-r--r--   0        0        0    14659 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_certificates_response.py
--rw-r--r--   0        0        0    11731 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_certificates_response_all_of.py
--rw-r--r--   0        0        0    13892 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_common.py
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_configuration.py
--rw-r--r--   0        0        0    12615 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_configuration_data.py
--rw-r--r--   0        0        0    11525 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_configuration_data_attributes.py
--rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_configuration_response.py
--rw-r--r--   0        0        0    16408 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_configuration_response_attributes.py
--rw-r--r--   0        0        0    12926 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_configuration_response_attributes_all_of.py
--rw-r--r--   0        0        0    15232 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_configuration_response_data.py
--rw-r--r--   0        0        0    12022 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_configuration_response_data_all_of.py
--rw-r--r--   0        0        0    14689 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_configurations_response.py
--rw-r--r--   0        0        0    11751 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_configurations_response_all_of.py
--rw-r--r--   0        0        0    11546 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_csr.py
--rw-r--r--   0        0        0    12375 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_csr_data.py
--rw-r--r--   0        0        0    15331 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_csr_data_attributes.py
--rw-r--r--   0        0        0    11627 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_csr_response.py
--rw-r--r--   0        0        0    11480 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_csr_response_attributes.py
--rw-r--r--   0        0        0    12595 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_csr_response_data.py
--rw-r--r--   0        0        0    13196 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_dns_record.py
--rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_domain_data.py
--rw-r--r--   0        0        0    14527 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_domains_response.py
--rw-r--r--   0        0        0    11624 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_domains_response_all_of.py
--rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_private_key.py
--rw-r--r--   0        0        0    12546 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_private_key_data.py
--rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_private_key_data_attributes.py
--rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_private_key_response.py
--rw-r--r--   0        0        0    16480 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_private_key_response_attributes.py
--rw-r--r--   0        0        0    13012 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_private_key_response_attributes_all_of.py
--rw-r--r--   0        0        0    12321 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_private_key_response_data.py
--rw-r--r--   0        0        0    14646 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_private_keys_response.py
--rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_private_keys_response_all_of.py
--rw-r--r--   0        0        0    11636 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_subscription.py
--rw-r--r--   0        0        0    12591 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_subscription_data.py
--rw-r--r--   0        0        0    11818 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_subscription_data_attributes.py
--rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_subscription_response.py
--rw-r--r--   0        0        0    15234 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_subscription_response_attributes.py
--rw-r--r--   0        0        0    11757 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_subscription_response_attributes_all_of.py
--rw-r--r--   0        0        0    14191 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_subscription_response_data.py
--rw-r--r--   0        0        0    12012 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_subscription_response_data_all_of.py
--rw-r--r--   0        0        0    14645 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_subscriptions_response.py
--rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/tls_subscriptions_response_all_of.py
--rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/token.py
--rw-r--r--   0        0        0    18055 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/token_created_response.py
--rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/token_created_response_all_of.py
--rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/token_response.py
--rw-r--r--   0        0        0    13237 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/token_response_all_of.py
--rw-r--r--   0        0        0    11733 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_billing_address.py
--rw-r--r--   0        0        0    11616 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_contact.py
--rw-r--r--   0        0        0    11631 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_customer.py
--rw-r--r--   0        0        0    11586 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_event.py
--rw-r--r--   0        0        0    11661 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_invitation.py
--rw-r--r--   0        0        0    11823 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_mutual_authentication.py
--rw-r--r--   0        0        0    11895 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_resource.py
--rw-r--r--   0        0        0    11616 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_service.py
--rw-r--r--   0        0        0    11823 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_service_authorization.py
--rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_service_invitation.py
--rw-r--r--   0        0        0    11571 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_star.py
--rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_tls_activation.py
--rw-r--r--   0        0        0    11805 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_tls_bulk_certificate.py
--rw-r--r--   0        0        0    11733 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_tls_certificate.py
--rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_tls_configuration.py
--rw-r--r--   0        0        0    11581 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_tls_csr.py
--rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_tls_dns_record.py
--rw-r--r--   0        0        0    11658 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_tls_domain.py
--rw-r--r--   0        0        0    11730 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_tls_private_key.py
--rw-r--r--   0        0        0    11748 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_tls_subscription.py
--rw-r--r--   0        0        0    11571 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_user.py
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_waf_active_rule.py
--rw-r--r--   0        0        0    11707 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_waf_exclusion.py
--rw-r--r--   0        0        0    11692 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_waf_firewall.py
--rw-r--r--   0        0        0    11809 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_waf_firewall_version.py
--rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_waf_rule.py
--rw-r--r--   0        0        0    11764 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_waf_rule_revision.py
--rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/type_waf_tag.py
--rw-r--r--   0        0        0    12136 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/update_billing_address_request.py
--rw-r--r--   0        0        0    12402 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/update_billing_address_request_data.py
--rw-r--r--   0        0        0    13820 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/user.py
--rw-r--r--   0        0        0    18047 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/user_response.py
--rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/user_response_all_of.py
--rw-r--r--   0        0        0    12570 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/validator_result.py
--rw-r--r--   0        0        0    12325 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/validator_result_messages.py
--rw-r--r--   0        0        0    11960 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/vcl.py
--rw-r--r--   0        0        0    12644 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/vcl_diff.py
--rw-r--r--   0        0        0    15932 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/vcl_response.py
--rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/version.py
--rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/version_create_response.py
--rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/version_detail.py
--rw-r--r--   0        0        0    12978 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/version_detail_settings.py
--rw-r--r--   0        0        0    17376 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/version_response.py
--rw-r--r--   0        0        0    11475 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/version_response_all_of.py
--rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_active_rule.py
--rw-r--r--   0        0        0    15118 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_active_rule_creation_response.py
--rw-r--r--   0        0        0    12546 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_active_rule_data.py
--rw-r--r--   0        0        0    12548 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_active_rule_data_attributes.py
--rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_active_rule_response.py
--rw-r--r--   0        0        0    15228 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_active_rule_response_data.py
--rw-r--r--   0        0        0    12559 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_active_rule_response_data_all_of.py
--rw-r--r--   0        0        0    15589 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_active_rule_response_data_attributes.py
--rw-r--r--   0        0        0    12100 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_active_rule_response_data_attributes_all_of.py
--rw-r--r--   0        0        0    14978 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_active_rule_response_data_relationships.py
--rw-r--r--   0        0        0    15066 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_active_rules_response.py
--rw-r--r--   0        0        0    12142 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_active_rules_response_all_of.py
--rw-r--r--   0        0        0    11606 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_exclusion.py
--rw-r--r--   0        0        0    12519 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_exclusion_data.py
--rw-r--r--   0        0        0    13837 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_exclusion_data_attributes.py
--rw-r--r--   0        0        0    11687 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_exclusion_response.py
--rw-r--r--   0        0        0    15289 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_exclusion_response_data.py
--rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_exclusion_response_data_all_of.py
--rw-r--r--   0        0        0    17359 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_exclusion_response_data_attributes.py
--rw-r--r--   0        0        0    13876 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_exclusion_response_data_attributes_all_of.py
--rw-r--r--   0        0        0    14718 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_exclusion_response_data_relationships.py
--rw-r--r--   0        0        0    15041 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_exclusions_response.py
--rw-r--r--   0        0        0    12123 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_exclusions_response_all_of.py
--rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_firewall.py
--rw-r--r--   0        0        0    12037 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_firewall_data.py
--rw-r--r--   0        0        0    12561 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_firewall_data_attributes.py
--rw-r--r--   0        0        0    12082 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_firewall_response.py
--rw-r--r--   0        0        0    15119 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_firewall_response_data.py
--rw-r--r--   0        0        0    12487 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_firewall_response_data_all_of.py
--rw-r--r--   0        0        0    19383 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_firewall_response_data_attributes.py
--rw-r--r--   0        0        0    15905 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_firewall_response_data_attributes_all_of.py
--rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_firewall_version.py
--rw-r--r--   0        0        0    12158 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_firewall_version_data.py
--rw-r--r--   0        0        0    24857 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_firewall_version_data_attributes.py
--rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_firewall_version_response.py
--rw-r--r--   0        0        0    15440 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_firewall_version_response_data.py
--rw-r--r--   0        0        0    12686 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_firewall_version_response_data_all_of.py
--rw-r--r--   0        0        0    20346 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_firewall_version_response_data_attributes.py
--rw-r--r--   0        0        0    16832 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_firewall_version_response_data_attributes_all_of.py
--rw-r--r--   0        0        0    15176 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_firewall_versions_response.py
--rw-r--r--   0        0        0    12227 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_firewall_versions_response_all_of.py
--rw-r--r--   0        0        0    15019 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_firewalls_response.py
--rw-r--r--   0        0        0    12106 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_firewalls_response_all_of.py
--rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_rule.py
--rw-r--r--   0        0        0    12553 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_rule_attributes.py
--rw-r--r--   0        0        0    12014 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_rule_response.py
--rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_rule_response_data.py
--rw-r--r--   0        0        0    11737 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_rule_response_data_all_of.py
--rw-r--r--   0        0        0    12370 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_rule_revision.py
--rw-r--r--   0        0        0    13775 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_rule_revision_attributes.py
--rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_rule_revision_or_latest.py
--rw-r--r--   0        0        0    12152 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_rule_revision_response.py
--rw-r--r--   0        0        0    15147 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_rule_revision_response_data.py
--rw-r--r--   0        0        0    11732 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_rule_revision_response_data_all_of.py
--rw-r--r--   0        0        0    15110 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_rule_revisions_response.py
--rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_rule_revisions_response_all_of.py
--rw-r--r--   0        0        0    14931 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_rules_response.py
--rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_rules_response_all_of.py
--rw-r--r--   0        0        0    12195 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_tag.py
--rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_tag_attributes.py
--rw-r--r--   0        0        0    14872 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_tags_response.py
--rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_tags_response_all_of.py
--rw-r--r--   0        0        0    14941 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/waf_tags_response_data_item.py
--rw-r--r--   0        0        0    11832 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/model/ws_message_format.py
--rw-r--r--   0        0        0    44657 2020-02-02 00:00:00.000000 fastly-1.3.0/fastly/models/__init__.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 fastly-1.3.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 fastly-1.3.0/LICENSE
--rw-r--r--   0        0        0    88253 2020-02-02 00:00:00.000000 fastly-1.3.0/README.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastly-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    88745 2020-02-02 00:00:00.000000 fastly-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 fastly-1.3.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 fastly-1.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 fastly-1.3.1/MANIFEST.in
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 fastly-1.3.1/SECURITY.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fastly-1.3.1/requirements.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fastly-1.3.1/setup.cfg
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 fastly-1.3.1/setup.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastly-1.3.1/sig.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 fastly-1.3.1/test-requirements.txt
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 fastly-1.3.1/tox.ini
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 fastly-1.3.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rwxr-xr-x   0        0        0      619 2020-02-02 00:00:00.000000 fastly-1.3.1/.github/scripts/pack.sh
+-rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 fastly-1.3.1/.github/scripts/prepare.sh
+-rwxr-xr-x   0        0        0      812 2020-02-02 00:00:00.000000 fastly-1.3.1/.github/scripts/publish_env.sh
+-rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 fastly-1.3.1/.github/scripts/release_body.sh
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 fastly-1.3.1/.github/workflows/ci-release.yaml
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Acl.md
+-rw-r--r--   0        0        0    15695 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/AclApi.md
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/AclEntry.md
+-rw-r--r--   0        0        0    20447 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/AclEntryApi.md
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/AclEntryResponse.md
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/AclEntryResponseAllOf.md
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/AclResponse.md
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/AclResponseAllOf.md
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ApexRedirect.md
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ApexRedirectAllOf.md
+-rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ApexRedirectApi.md
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/AwsRegion.md
+-rw-r--r--   0        0        0     5836 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Backend.md
+-rw-r--r--   0        0        0    38224 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BackendApi.md
+-rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BackendResponse.md
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BackendResponseAllOf.md
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Billing.md
+-rw-r--r--   0        0        0    13259 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BillingAddressApi.md
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BillingAddressAttributes.md
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BillingAddressRequest.md
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BillingAddressRequestData.md
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BillingAddressResponse.md
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BillingAddressResponseData.md
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BillingAddressVerificationErrorResponse.md
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BillingAddressVerificationErrorResponseErrors.md
+-rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BillingApi.md
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BillingEstimateResponse.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BillingEstimateResponseAllOf.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BillingEstimateResponseAllOfLine.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BillingEstimateResponseAllOfLines.md
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BillingResponse.md
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BillingResponseAllOf.md
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BillingResponseLineItem.md
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BillingResponseLineItemAllOf.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BillingStatus.md
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BillingTotal.md
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BillingTotalExtras.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BulkUpdateAclEntriesRequest.md
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BulkUpdateAclEntry.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BulkUpdateAclEntryAllOf.md
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BulkUpdateDictionaryItem.md
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BulkUpdateDictionaryItemAllOf.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BulkUpdateDictionaryListRequest.md
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BulkWafActiveRule.md
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/BulkWafActiveRules.md
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/CacheSetting.md
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/CacheSettingResponse.md
+-rw-r--r--   0        0        0    18846 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/CacheSettingsApi.md
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Condition.md
+-rw-r--r--   0        0        0    17741 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ConditionApi.md
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ConditionResponse.md
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ConditionsResponse.md
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Contact.md
+-rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ContactApi.md
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ContactResponse.md
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ContactResponseAllOf.md
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Content.md
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ContentApi.md
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Customer.md
+-rw-r--r--   0        0        0    18926 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/CustomerApi.md
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/CustomerResponse.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/CustomerResponseAllOf.md
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Dictionary.md
+-rw-r--r--   0        0        0    17237 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/DictionaryApi.md
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/DictionaryInfoApi.md
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/DictionaryInfoResponse.md
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/DictionaryItem.md
+-rw-r--r--   0        0        0    22127 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/DictionaryItemApi.md
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/DictionaryItemResponse.md
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/DictionaryItemResponseAllOf.md
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/DictionaryResponse.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/DictionaryResponseAllOf.md
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/DiffApi.md
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/DiffResponse.md
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Director.md
+-rw-r--r--   0        0        0    15015 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/DirectorApi.md
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/DirectorBackend.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/DirectorBackendAllOf.md
+-rw-r--r--   0        0        0     9981 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/DirectorBackendApi.md
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/DirectorResponse.md
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Domain.md
+-rw-r--r--   0        0        0    21769 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/DomainApi.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/DomainCheckItem.md
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/DomainCheckResponse.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/DomainCheckResponseList.md
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/DomainOwnershipsApi.md
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/DomainResponse.md
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/DomainsResponse.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/EnabledProductResponse.md
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/EnabledProductResponseLinks.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/EnabledProductResponseProduct.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/EnabledProductResponseService.md
+-rw-r--r--   0        0        0     8351 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/EnabledProductsApi.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Event.md
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/EventAttributes.md
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/EventResponse.md
+-rw-r--r--   0        0        0     7243 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/EventsApi.md
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/EventsResponse.md
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/EventsResponseAllOf.md
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/GenericTokenError.md
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Gzip.md
+-rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/GzipApi.md
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/GzipResponse.md
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Header.md
+-rw-r--r--   0        0        0    20925 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HeaderApi.md
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HeaderResponse.md
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Healthcheck.md
+-rw-r--r--   0        0        0    20120 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HealthcheckApi.md
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HealthcheckResponse.md
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Historical.md
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HistoricalAggregateResponse.md
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HistoricalAggregateResponseAllOf.md
+-rw-r--r--   0        0        0    39081 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HistoricalApi.md
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HistoricalFieldAggregateResponse.md
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HistoricalFieldAggregateResponseAllOf.md
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HistoricalFieldResponse.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HistoricalFieldResponseAllOf.md
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HistoricalFieldResults.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HistoricalMeta.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HistoricalRegionsResponse.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HistoricalRegionsResponseAllOf.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HistoricalResponse.md
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HistoricalResponseAllOf.md
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HistoricalResults.md
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HistoricalServices.md
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HistoricalUsageAggregateResponse.md
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HistoricalUsageMonthResponse.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HistoricalUsageMonthResponseAllOf.md
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HistoricalUsageMonthResponseAllOfData.md
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HistoricalUsageResults.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HistoricalUsageServiceResponse.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HistoricalUsageServiceResponseAllOf.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Http3.md
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Http3AllOf.md
+-rw-r--r--   0        0        0     9629 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Http3Api.md
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HttpResponseFormat.md
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/HttpStreamFormat.md
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/IamPermission.md
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/IamPermissionsApi.md
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/IamRole.md
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/IamRoleAllOf.md
+-rw-r--r--   0        0        0     9918 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/IamRolesApi.md
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/IamServiceGroup.md
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/IamServiceGroupAllOf.md
+-rw-r--r--   0        0        0    11406 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/IamServiceGroupsApi.md
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/IamUserGroup.md
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/IamUserGroupAllOf.md
+-rw-r--r--   0        0        0    17911 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/IamUserGroupsApi.md
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/IncludedWithWafActiveRule.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/IncludedWithWafActiveRuleItem.md
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/IncludedWithWafExclusion.md
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/IncludedWithWafExclusionItem.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/IncludedWithWafFirewall.md
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/IncludedWithWafFirewallVersion.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/IncludedWithWafFirewallVersionItem.md
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/IncludedWithWafRule.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/IncludedWithWafRuleItem.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/IncludedWithWafRuleRevision.md
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/InlineObject.md
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/InlineObject1.md
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/InlineResponse200.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/InlineResponse2001.md
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/InlineResponse2002.md
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/InlineResponse2002Meta.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/InlineResponse2003.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/InlineResponse2003Meta.md
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Invitation.md
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/InvitationData.md
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/InvitationDataAttributes.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/InvitationResponse.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/InvitationResponseAllOf.md
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/InvitationResponseData.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/InvitationResponseDataAllOf.md
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/InvitationsApi.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/InvitationsResponse.md
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/InvitationsResponseAllOf.md
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingAddressAndPort.md
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingAzureblob.md
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingAzureblobAllOf.md
+-rw-r--r--   0        0        0    29125 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingAzureblobApi.md
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingAzureblobResponse.md
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingBigquery.md
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingBigqueryAllOf.md
+-rw-r--r--   0        0        0    24678 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingBigqueryApi.md
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingBigqueryResponse.md
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingCloudfiles.md
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingCloudfilesAllOf.md
+-rw-r--r--   0        0        0    27524 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingCloudfilesApi.md
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingCloudfilesResponse.md
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingCommon.md
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingDatadog.md
+-rw-r--r--   0        0        0     3883 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingDatadogAllOf.md
+-rw-r--r--   0        0        0    38955 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingDatadogApi.md
+-rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingDatadogResponse.md
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingDigitalocean.md
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingDigitaloceanAllOf.md
+-rw-r--r--   0        0        0    28174 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingDigitaloceanApi.md
+-rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingDigitaloceanResponse.md
+-rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingElasticsearch.md
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingElasticsearchAllOf.md
+-rw-r--r--   0        0        0    30259 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingElasticsearchApi.md
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingElasticsearchResponse.md
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingFormatVersion.md
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingFtp.md
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingFtpAllOf.md
+-rw-r--r--   0        0        0    27244 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingFtpApi.md
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingFtpResponse.md
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingGcs.md
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingGcsAllOf.md
+-rw-r--r--   0        0        0    28487 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingGcsApi.md
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingGcsCommon.md
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingGcsResponse.md
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingGenericCommon.md
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingGooglePubsub.md
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingGooglePubsubAllOf.md
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingGooglePubsubResponse.md
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingHeroku.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingHerokuAllOf.md
+-rw-r--r--   0        0        0    21127 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingHerokuApi.md
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingHerokuResponse.md
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingHoneycomb.md
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingHoneycombAllOf.md
+-rw-r--r--   0        0        0    20986 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingHoneycombApi.md
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingHoneycombResponse.md
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingHttps.md
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingHttpsAllOf.md
+-rw-r--r--   0        0        0    29036 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingHttpsApi.md
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingHttpsResponse.md
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingKafka.md
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingKafkaAllOf.md
+-rw-r--r--   0        0        0    18733 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingKafkaApi.md
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingKafkaResponse.md
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingKinesis.md
+-rw-r--r--   0        0        0    17289 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingKinesisApi.md
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingKinesisResponse.md
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingLogentries.md
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingLogentriesAllOf.md
+-rw-r--r--   0        0        0    22258 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingLogentriesApi.md
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingLogentriesResponse.md
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingLoggly.md
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingLogglyAllOf.md
+-rw-r--r--   0        0        0    20871 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingLogglyApi.md
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingLogglyResponse.md
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingLogshuttle.md
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingLogshuttleAllOf.md
+-rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingLogshuttleApi.md
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingLogshuttleResponse.md
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingMessageType.md
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingNewrelic.md
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingNewrelicAllOf.md
+-rw-r--r--   0        0        0    25794 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingNewrelicApi.md
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingNewrelicResponse.md
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingOpenstack.md
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingOpenstackAllOf.md
+-rw-r--r--   0        0        0    27216 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingOpenstackApi.md
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingOpenstackResponse.md
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingPapertrail.md
+-rw-r--r--   0        0        0    21189 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingPapertrailApi.md
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingPapertrailResponse.md
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingPlacement.md
+-rw-r--r--   0        0        0    24358 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingPubsubApi.md
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingRequestCapsCommon.md
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingS3.md
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingS3AllOf.md
+-rw-r--r--   0        0        0    31697 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingS3Api.md
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingS3Response.md
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingScalyr.md
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingScalyrAllOf.md
+-rw-r--r--   0        0        0    21715 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingScalyrApi.md
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingScalyrResponse.md
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingSftp.md
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingSftpAllOf.md
+-rw-r--r--   0        0        0    28475 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingSftpApi.md
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingSftpResponse.md
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingSplunk.md
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingSplunkAllOf.md
+-rw-r--r--   0        0        0    26444 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingSplunkApi.md
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingSplunkResponse.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingSumologic.md
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingSumologicAllOf.md
+-rw-r--r--   0        0        0    21088 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingSumologicApi.md
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingSumologicResponse.md
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingSyslog.md
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingSyslogAllOf.md
+-rw-r--r--   0        0        0    26805 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingSyslogApi.md
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingSyslogResponse.md
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingTlsCommon.md
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/LoggingUseTls.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/MutualAuthentication.md
+-rw-r--r--   0        0        0    17143 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/MutualAuthenticationApi.md
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/MutualAuthenticationData.md
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/MutualAuthenticationDataAttributes.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/MutualAuthenticationResponse.md
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/MutualAuthenticationResponseAttributes.md
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/MutualAuthenticationResponseAttributesAllOf.md
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/MutualAuthenticationResponseData.md
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/MutualAuthenticationResponseDataAllOf.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/MutualAuthenticationsResponse.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/MutualAuthenticationsResponseAllOf.md
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/NumberVersion.md
+-rw-r--r--   0        0        0    10438 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ObjectStoreApi.md
+-rw-r--r--   0        0        0    12839 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ObjectStoreItemApi.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Package.md
+-rw-r--r--   0        0        0     6678 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/PackageApi.md
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/PackageMetadata.md
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/PackageResponse.md
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/PackageResponseAllOf.md
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Pagination.md
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/PaginationLinks.md
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/PaginationMeta.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Permission.md
+-rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Pool.md
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/PoolAllOf.md
+-rw-r--r--   0        0        0    29387 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/PoolApi.md
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/PoolResponse.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/PoolResponseAllOf.md
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Pop.md
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/PopApi.md
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/PopCoordinates.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/PublicIpList.md
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/PublicIpListApi.md
+-rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/PublishApi.md
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/PublishItem.md
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/PublishItemFormats.md
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/PublishRequest.md
+-rw-r--r--   0        0        0    10418 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/PurgeApi.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/PurgeKeys.md
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/PurgeKeysResponse.md
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/PurgeResponse.md
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RateLimiter.md
+-rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RateLimiterApi.md
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RateLimiterResponse.md
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RateLimiterResponse1.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RateLimiterResponseAllOf.md
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Realtime.md
+-rw-r--r--   0        0        0     8759 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RealtimeApi.md
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RealtimeEntry.md
+-rw-r--r--   0        0        0    27181 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RealtimeMeasurements.md
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipCommonName.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipCustomer.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipCustomerCustomer.md
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipMemberCustomer.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipMemberMutualAuthentication.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipMemberService.md
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipMemberServiceInvitation.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipMemberTlsActivation.md
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipMemberTlsBulkCertificate.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipMemberTlsCertificate.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipMemberTlsConfiguration.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipMemberTlsDnsRecord.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipMemberTlsDomain.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipMemberTlsPrivateKey.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipMemberTlsSubscription.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipMemberWafActiveRule.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipMemberWafFirewall.md
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipMemberWafFirewallVersion.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipMemberWafRule.md
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipMemberWafRuleRevision.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipMemberWafTag.md
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipMutualAuthentication.md
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipMutualAuthenticationMutualAuthentication.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipMutualAuthentications.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipMutualAuthenticationsMutualAuthentications.md
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipService.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipServiceInvitations.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipServiceInvitationsCreate.md
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipServiceInvitationsCreateServiceInvitations.md
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipServiceInvitationsServiceInvitations.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipServices.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipServicesServices.md
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsActivation.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsActivationTlsActivation.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsActivations.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsBulkCertificate.md
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsBulkCertificateTlsBulkCertificate.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsBulkCertificates.md
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsCertificate.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsCertificateTlsCertificate.md
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsCertificates.md
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsCertificatesTlsCertificates.md
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsConfiguration.md
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsConfigurationTlsConfiguration.md
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsConfigurations.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsConfigurationsTlsConfigurations.md
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsDnsRecord.md
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsDnsRecordDnsRecord.md
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsDnsRecords.md
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsDomain.md
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsDomainTlsDomain.md
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsDomains.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsDomainsTlsDomains.md
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsPrivateKey.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsPrivateKeyTlsPrivateKey.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsPrivateKeys.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsPrivateKeysTlsPrivateKeys.md
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsSubscription.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsSubscriptionTlsSubscription.md
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipTlsSubscriptions.md
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipUser.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipUserUser.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipWafActiveRules.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipWafActiveRulesWafActiveRules.md
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipWafFirewall.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipWafFirewallVersion.md
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipWafFirewallVersionWafFirewallVersion.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipWafFirewallVersions.md
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipWafFirewallWafFirewall.md
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipWafRule.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipWafRuleRevision.md
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipWafRuleRevisionWafRuleRevisions.md
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipWafRuleRevisions.md
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipWafRuleWafRule.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipWafRules.md
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipWafTags.md
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipWafTagsWafTags.md
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipsForInvitation.md
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipsForMutualAuthentication.md
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipsForStar.md
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipsForTlsActivation.md
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipsForTlsBulkCertificate.md
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipsForTlsConfiguration.md
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipsForTlsDomain.md
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipsForTlsPrivateKey.md
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipsForTlsSubscription.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipsForWafActiveRule.md
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipsForWafExclusion.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipsForWafFirewallVersion.md
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RelationshipsForWafRule.md
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RequestSettings.md
+-rw-r--r--   0        0        0    15635 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RequestSettingsApi.md
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RequestSettingsResponse.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Resource.md
+-rw-r--r--   0        0        0    15552 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ResourceApi.md
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ResourceResponse.md
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ResourceResponseAllOf.md
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ResponseObject.md
+-rw-r--r--   0        0        0     8900 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ResponseObjectApi.md
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ResponseObjectResponse.md
+-rw-r--r--   0        0        0    27069 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Results.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/RoleUser.md
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/SchemasContactResponse.md
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/SchemasSnippetResponse.md
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/SchemasUserResponse.md
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/SchemasVclResponse.md
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/SchemasVersion.md
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/SchemasVersionResponse.md
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/SchemasWafFirewallVersion.md
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/SchemasWafFirewallVersionData.md
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Server.md
+-rw-r--r--   0        0        0    19968 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServerApi.md
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServerResponse.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServerResponseAllOf.md
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Service.md
+-rw-r--r--   0        0        0    22475 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceApi.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceAuthorization.md
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceAuthorizationData.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceAuthorizationDataAttributes.md
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceAuthorizationDataRelationships.md
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceAuthorizationDataRelationshipsUser.md
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceAuthorizationDataRelationshipsUserData.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceAuthorizationResponse.md
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceAuthorizationResponseData.md
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceAuthorizationResponseDataAllOf.md
+-rw-r--r--   0        0        0    16177 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceAuthorizationsApi.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceAuthorizationsResponse.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceAuthorizationsResponseAllOf.md
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceCreate.md
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceCreateAllOf.md
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceDetail.md
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceDetailAllOf.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceIdAndVersion.md
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceInvitation.md
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceInvitationData.md
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceInvitationDataAttributes.md
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceInvitationDataRelationships.md
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceInvitationResponse.md
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceInvitationResponseAllOf.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceInvitationResponseAllOfData.md
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceListResponse.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceListResponseAllOf.md
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceResponse.md
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceResponseAllOf.md
+-rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceVersionDetail.md
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ServiceVersionDetailOrNull.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Settings.md
+-rw-r--r--   0        0        0     7419 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/SettingsApi.md
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/SettingsResponse.md
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Snippet.md
+-rw-r--r--   0        0        0    19425 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/SnippetApi.md
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/SnippetResponse.md
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/SnippetResponseAllOf.md
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Star.md
+-rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/StarApi.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/StarData.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/StarResponse.md
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/StarResponseAllOf.md
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Stats.md
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/StatsApi.md
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Store.md
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/StoreResponse.md
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Timestamps.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TimestampsNoDelete.md
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsActivation.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsActivationData.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsActivationResponse.md
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsActivationResponseData.md
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsActivationResponseDataAllOf.md
+-rw-r--r--   0        0        0    16586 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsActivationsApi.md
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsActivationsResponse.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsActivationsResponseAllOf.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsBulkCertificate.md
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsBulkCertificateData.md
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsBulkCertificateDataAttributes.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsBulkCertificateResponse.md
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsBulkCertificateResponseAttributes.md
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsBulkCertificateResponseAttributesAllOf.md
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsBulkCertificateResponseData.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsBulkCertificateResponseDataAllOf.md
+-rw-r--r--   0        0        0    16217 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsBulkCertificatesApi.md
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsBulkCertificatesResponse.md
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsBulkCertificatesResponseAllOf.md
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsCertificate.md
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsCertificateData.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsCertificateDataAttributes.md
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsCertificateResponse.md
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsCertificateResponseAttributes.md
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsCertificateResponseAttributesAllOf.md
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsCertificateResponseData.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsCertificateResponseDataAllOf.md
+-rw-r--r--   0        0        0    16715 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsCertificatesApi.md
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsCertificatesResponse.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsCertificatesResponseAllOf.md
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsCommon.md
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsConfiguration.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsConfigurationData.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsConfigurationDataAttributes.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsConfigurationResponse.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsConfigurationResponseAttributes.md
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsConfigurationResponseAttributesAllOf.md
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsConfigurationResponseData.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsConfigurationResponseDataAllOf.md
+-rw-r--r--   0        0        0    10339 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsConfigurationsApi.md
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsConfigurationsResponse.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsConfigurationsResponseAllOf.md
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsDnsRecord.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsDomainData.md
+-rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsDomainsApi.md
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsDomainsResponse.md
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsDomainsResponseAllOf.md
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsPrivateKey.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsPrivateKeyData.md
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsPrivateKeyDataAttributes.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsPrivateKeyResponse.md
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsPrivateKeyResponseAttributes.md
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsPrivateKeyResponseAttributesAllOf.md
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsPrivateKeyResponseData.md
+-rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsPrivateKeysApi.md
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsPrivateKeysResponse.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsPrivateKeysResponseAllOf.md
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsSubscription.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsSubscriptionData.md
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsSubscriptionDataAttributes.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsSubscriptionResponse.md
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsSubscriptionResponseAttributes.md
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsSubscriptionResponseAttributesAllOf.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsSubscriptionResponseData.md
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsSubscriptionResponseDataAllOf.md
+-rw-r--r--   0        0        0    26148 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsSubscriptionsApi.md
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsSubscriptionsResponse.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TlsSubscriptionsResponseAllOf.md
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Token.md
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TokenCreatedResponse.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TokenCreatedResponseAllOf.md
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TokenResponse.md
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TokenResponseAllOf.md
+-rw-r--r--   0        0        0    12243 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TokensApi.md
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeBillingAddress.md
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeContact.md
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeCustomer.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeEvent.md
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeInvitation.md
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeMutualAuthentication.md
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeResource.md
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeService.md
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeServiceAuthorization.md
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeServiceInvitation.md
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeStar.md
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeTlsActivation.md
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeTlsBulkCertificate.md
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeTlsCertificate.md
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeTlsConfiguration.md
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeTlsDnsRecord.md
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeTlsDomain.md
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeTlsPrivateKey.md
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeTlsSubscription.md
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeUser.md
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeWafActiveRule.md
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeWafExclusion.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeWafFirewall.md
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeWafFirewallVersion.md
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeWafRule.md
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeWafRuleRevision.md
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/TypeWafTag.md
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/UpdateBillingAddressRequest.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/UpdateBillingAddressRequestData.md
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/User.md
+-rw-r--r--   0        0        0    20765 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/UserApi.md
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/UserResponse.md
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/UserResponseAllOf.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ValidatorResult.md
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/ValidatorResultMessages.md
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Vcl.md
+-rw-r--r--   0        0        0    32742 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/VclApi.md
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/VclDiff.md
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/VclDiffApi.md
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/VclResponse.md
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/Version.md
+-rw-r--r--   0        0        0    26131 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/VersionApi.md
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/VersionCreateResponse.md
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/VersionDetail.md
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/VersionDetailSettings.md
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/VersionResponse.md
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/VersionResponseAllOf.md
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafActiveRule.md
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafActiveRuleCreationResponse.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafActiveRuleData.md
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafActiveRuleDataAttributes.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafActiveRuleResponse.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafActiveRuleResponseData.md
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafActiveRuleResponseDataAllOf.md
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafActiveRuleResponseDataAttributes.md
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafActiveRuleResponseDataAttributesAllOf.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafActiveRuleResponseDataRelationships.md
+-rw-r--r--   0        0        0    27789 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafActiveRulesApi.md
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafActiveRulesResponse.md
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafActiveRulesResponseAllOf.md
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafExclusion.md
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafExclusionData.md
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafExclusionDataAttributes.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafExclusionResponse.md
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafExclusionResponseData.md
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafExclusionResponseDataAllOf.md
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafExclusionResponseDataAttributes.md
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafExclusionResponseDataAttributesAllOf.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafExclusionResponseDataRelationships.md
+-rw-r--r--   0        0        0    19155 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafExclusionsApi.md
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafExclusionsResponse.md
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafExclusionsResponseAllOf.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafFirewall.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafFirewallData.md
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafFirewallDataAttributes.md
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafFirewallResponse.md
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafFirewallResponseData.md
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafFirewallResponseDataAllOf.md
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafFirewallResponseDataAttributes.md
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafFirewallResponseDataAttributesAllOf.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafFirewallVersion.md
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafFirewallVersionData.md
+-rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafFirewallVersionDataAttributes.md
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafFirewallVersionResponse.md
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafFirewallVersionResponseData.md
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafFirewallVersionResponseDataAllOf.md
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafFirewallVersionResponseDataAttributes.md
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafFirewallVersionResponseDataAttributesAllOf.md
+-rw-r--r--   0        0        0    24852 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafFirewallVersionsApi.md
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafFirewallVersionsResponse.md
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafFirewallVersionsResponseAllOf.md
+-rw-r--r--   0        0        0    17211 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafFirewallsApi.md
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafFirewallsResponse.md
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafFirewallsResponseAllOf.md
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafRule.md
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafRuleAttributes.md
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafRuleResponse.md
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafRuleResponseData.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafRuleResponseDataAllOf.md
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafRuleRevision.md
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafRuleRevisionAttributes.md
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafRuleRevisionOrLatest.md
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafRuleRevisionResponse.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafRuleRevisionResponseData.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafRuleRevisionResponseDataAllOf.md
+-rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafRuleRevisionsApi.md
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafRuleRevisionsResponse.md
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafRuleRevisionsResponseAllOf.md
+-rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafRulesApi.md
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafRulesResponse.md
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafRulesResponseAllOf.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafTag.md
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafTagAttributes.md
+-rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafTagsApi.md
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafTagsResponse.md
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafTagsResponseAllOf.md
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WafTagsResponseDataItem.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-1.3.1/docs/WsMessageFormat.md
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/__init__.py
+-rw-r--r--   0        0        0    39346 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api_client.py
+-rw-r--r--   0        0        0    18987 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/configuration.py
+-rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/exceptions.py
+-rw-r--r--   0        0        0    82524 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model_utils.py
+-rw-r--r--   0        0        0    14634 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/rest.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/__init__.py
+-rw-r--r--   0        0        0    29655 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/acl_api.py
+-rw-r--r--   0        0        0    36324 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/acl_entry_api.py
+-rw-r--r--   0        0        0    24178 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/apex_redirect_api.py
+-rw-r--r--   0        0        0    53093 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/backend_api.py
+-rw-r--r--   0        0        0    21781 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/billing_address_api.py
+-rw-r--r--   0        0        0    18043 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/billing_api.py
+-rw-r--r--   0        0        0    33343 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/cache_settings_api.py
+-rw-r--r--   0        0        0    33323 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/condition_api.py
+-rw-r--r--   0        0        0    11415 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/contact_api.py
+-rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/content_api.py
+-rw-r--r--   0        0        0    33521 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/customer_api.py
+-rw-r--r--   0        0        0    30822 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/dictionary_api.py
+-rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/dictionary_info_api.py
+-rw-r--r--   0        0        0    38750 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/dictionary_item_api.py
+-rw-r--r--   0        0        0     7805 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/diff_api.py
+-rw-r--r--   0        0        0    26135 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/director_api.py
+-rw-r--r--   0        0        0    20052 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/director_backend_api.py
+-rw-r--r--   0        0        0    41462 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/domain_api.py
+-rw-r--r--   0        0        0     5727 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/domain_ownerships_api.py
+-rw-r--r--   0        0        0    17158 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/enabled_products_api.py
+-rw-r--r--   0        0        0    13773 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/events_api.py
+-rw-r--r--   0        0        0    31746 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/gzip_api.py
+-rw-r--r--   0        0        0    37636 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/header_api.py
+-rw-r--r--   0        0        0    36204 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/healthcheck_api.py
+-rw-r--r--   0        0        0    58830 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/historical_api.py
+-rw-r--r--   0        0        0    19004 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/http3_api.py
+-rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/iam_permissions_api.py
+-rw-r--r--   0        0        0    20715 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/iam_roles_api.py
+-rw-r--r--   0        0        0    22040 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/iam_service_groups_api.py
+-rw-r--r--   0        0        0    33266 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/iam_user_groups_api.py
+-rw-r--r--   0        0        0    15947 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/invitations_api.py
+-rw-r--r--   0        0        0    44535 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_azureblob_api.py
+-rw-r--r--   0        0        0    39192 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_bigquery_api.py
+-rw-r--r--   0        0        0    44242 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_cloudfiles_api.py
+-rw-r--r--   0        0        0    41953 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_datadog_api.py
+-rw-r--r--   0        0        0    43696 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_digitalocean_api.py
+-rw-r--r--   0        0        0    44319 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_elasticsearch_api.py
+-rw-r--r--   0        0        0    43522 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_ftp_api.py
+-rw-r--r--   0        0        0    43855 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_gcs_api.py
+-rw-r--r--   0        0        0    35557 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_heroku_api.py
+-rw-r--r--   0        0        0    35714 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_honeycomb_api.py
+-rw-r--r--   0        0        0    45205 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_https_api.py
+-rw-r--r--   0        0        0    31840 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_kafka_api.py
+-rw-r--r--   0        0        0    27552 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_kinesis_api.py
+-rw-r--r--   0        0        0    37579 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_logentries_api.py
+-rw-r--r--   0        0        0    35171 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_loggly_api.py
+-rw-r--r--   0        0        0    35860 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_logshuttle_api.py
+-rw-r--r--   0        0        0    37648 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_newrelic_api.py
+-rw-r--r--   0        0        0    43132 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_openstack_api.py
+-rw-r--r--   0        0        0    35725 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_papertrail_api.py
+-rw-r--r--   0        0        0    38355 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_pubsub_api.py
+-rw-r--r--   0        0        0    47867 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_s3_api.py
+-rw-r--r--   0        0        0    36559 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_scalyr_api.py
+-rw-r--r--   0        0        0    44447 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_sftp_api.py
+-rw-r--r--   0        0        0    41345 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_splunk_api.py
+-rw-r--r--   0        0        0    35657 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_sumologic_api.py
+-rw-r--r--   0        0        0    42123 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/logging_syslog_api.py
+-rw-r--r--   0        0        0    27942 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/mutual_authentication_api.py
+-rw-r--r--   0        0        0    20697 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/object_store_api.py
+-rw-r--r--   0        0        0    24057 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/object_store_item_api.py
+-rw-r--r--   0        0        0    12532 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/package_api.py
+-rw-r--r--   0        0        0    46444 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/pool_api.py
+-rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/pop_api.py
+-rw-r--r--   0        0        0     5681 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/public_ip_list_api.py
+-rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/publish_api.py
+-rw-r--r--   0        0        0    17849 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/purge_api.py
+-rw-r--r--   0        0        0    16399 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/rate_limiter_api.py
+-rw-r--r--   0        0        0    17309 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/realtime_api.py
+-rw-r--r--   0        0        0    28563 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/request_settings_api.py
+-rw-r--r--   0        0        0    29580 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/resource_api.py
+-rw-r--r--   0        0        0    18201 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/response_object_api.py
+-rw-r--r--   0        0        0    34128 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/server_api.py
+-rw-r--r--   0        0        0    42868 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/service_api.py
+-rw-r--r--   0        0        0    27001 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/service_authorizations_api.py
+-rw-r--r--   0        0        0    13576 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/settings_api.py
+-rw-r--r--   0        0        0    37746 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/snippet_api.py
+-rw-r--r--   0        0        0    19785 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/star_api.py
+-rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/stats_api.py
+-rw-r--r--   0        0        0    28369 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/tls_activations_api.py
+-rw-r--r--   0        0        0    27785 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/tls_bulk_certificates_api.py
+-rw-r--r--   0        0        0    28246 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/tls_certificates_api.py
+-rw-r--r--   0        0        0    17747 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/tls_configurations_api.py
+-rw-r--r--   0        0        0     8628 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/tls_domains_api.py
+-rw-r--r--   0        0        0    21392 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/tls_private_keys_api.py
+-rw-r--r--   0        0        0    42634 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/tls_subscriptions_api.py
+-rw-r--r--   0        0        0    24152 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/tokens_api.py
+-rw-r--r--   0        0        0    39118 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/user_api.py
+-rw-r--r--   0        0        0    62802 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/vcl_api.py
+-rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/vcl_diff_api.py
+-rw-r--r--   0        0        0    50043 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/version_api.py
+-rw-r--r--   0        0        0    44729 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/waf_active_rules_api.py
+-rw-r--r--   0        0        0    33076 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/waf_exclusions_api.py
+-rw-r--r--   0        0        0    35544 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/waf_firewall_versions_api.py
+-rw-r--r--   0        0        0    28691 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/waf_firewalls_api.py
+-rw-r--r--   0        0        0    13476 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/waf_rule_revisions_api.py
+-rw-r--r--   0        0        0    13599 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/waf_rules_api.py
+-rw-r--r--   0        0        0     7121 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/api/waf_tags_api.py
+-rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/apis/__init__.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/__init__.py
+-rw-r--r--   0        0        0    11622 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/acl.py
+-rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/acl_entry.py
+-rw-r--r--   0        0        0    17351 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/acl_entry_response.py
+-rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/acl_entry_response_all_of.py
+-rw-r--r--   0        0        0    15941 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/acl_response.py
+-rw-r--r--   0        0        0    11415 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/acl_response_all_of.py
+-rw-r--r--   0        0        0    16586 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/apex_redirect.py
+-rw-r--r--   0        0        0    12580 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/apex_redirect_all_of.py
+-rw-r--r--   0        0        0    14660 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/aws_region.py
+-rw-r--r--   0        0        0    26110 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/backend.py
+-rw-r--r--   0        0        0    30674 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/backend_response.py
+-rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/backend_response_all_of.py
+-rw-r--r--   0        0        0    14085 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/billing.py
+-rw-r--r--   0        0        0    13567 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/billing_address_attributes.py
+-rw-r--r--   0        0        0    12075 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/billing_address_request.py
+-rw-r--r--   0        0        0    12080 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/billing_address_request_data.py
+-rw-r--r--   0        0        0    11707 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/billing_address_response.py
+-rw-r--r--   0        0        0    12794 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/billing_address_response_data.py
+-rw-r--r--   0        0        0    11909 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/billing_address_verification_error_response.py
+-rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/billing_address_verification_error_response_errors.py
+-rw-r--r--   0        0        0    16877 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/billing_estimate_response.py
+-rw-r--r--   0        0        0    11787 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/billing_estimate_response_all_of.py
+-rw-r--r--   0        0        0    13188 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/billing_estimate_response_all_of_line.py
+-rw-r--r--   0        0        0    11784 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/billing_estimate_response_all_of_lines.py
+-rw-r--r--   0        0        0    16765 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/billing_response.py
+-rw-r--r--   0        0        0    11716 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/billing_response_all_of.py
+-rw-r--r--   0        0        0    18617 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/billing_response_line_item.py
+-rw-r--r--   0        0        0    15190 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/billing_response_line_item_all_of.py
+-rw-r--r--   0        0        0    12041 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/billing_status.py
+-rw-r--r--   0        0        0    16362 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/billing_total.py
+-rw-r--r--   0        0        0    12157 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/billing_total_extras.py
+-rw-r--r--   0        0        0    11687 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/bulk_update_acl_entries_request.py
+-rw-r--r--   0        0        0    15994 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/bulk_update_acl_entry.py
+-rw-r--r--   0        0        0    11730 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/bulk_update_acl_entry_all_of.py
+-rw-r--r--   0        0        0    14503 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/bulk_update_dictionary_item.py
+-rw-r--r--   0        0        0    11584 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/bulk_update_dictionary_item_all_of.py
+-rw-r--r--   0        0        0    11731 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/bulk_update_dictionary_list_request.py
+-rw-r--r--   0        0        0    11735 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/bulk_waf_active_rule.py
+-rw-r--r--   0        0        0    11638 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/bulk_waf_active_rules.py
+-rw-r--r--   0        0        0    13506 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/cache_setting.py
+-rw-r--r--   0        0        0    17524 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/cache_setting_response.py
+-rw-r--r--   0        0        0    13530 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/condition.py
+-rw-r--r--   0        0        0    16896 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/condition_response.py
+-rw-r--r--   0        0        0    11911 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/conditions_response.py
+-rw-r--r--   0        0        0    13577 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/contact.py
+-rw-r--r--   0        0        0    17300 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/contact_response.py
+-rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/contact_response_all_of.py
+-rw-r--r--   0        0        0    12747 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/content.py
+-rw-r--r--   0        0        0    20398 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/customer.py
+-rw-r--r--   0        0        0    24131 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/customer_response.py
+-rw-r--r--   0        0        0    11430 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/customer_response_all_of.py
+-rw-r--r--   0        0        0    12110 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/dictionary.py
+-rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/dictionary_info_response.py
+-rw-r--r--   0        0        0    11765 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/dictionary_item.py
+-rw-r--r--   0        0        0    15870 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/dictionary_item_response.py
+-rw-r--r--   0        0        0    11758 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/dictionary_item_response_all_of.py
+-rw-r--r--   0        0        0    16499 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/dictionary_response.py
+-rw-r--r--   0        0        0    11436 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/dictionary_response_all_of.py
+-rw-r--r--   0        0        0    12481 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/diff_response.py
+-rw-r--r--   0        0        0    14620 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/director.py
+-rw-r--r--   0        0        0    15768 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/director_backend.py
+-rw-r--r--   0        0        0    11747 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/director_backend_all_of.py
+-rw-r--r--   0        0        0    18553 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/director_response.py
+-rw-r--r--   0        0        0    11783 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/domain.py
+-rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/domain_check_item.py
+-rw-r--r--   0        0        0    11897 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/domain_check_response.py
+-rw-r--r--   0        0        0    11945 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/domain_check_response_list.py
+-rw-r--r--   0        0        0    15770 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/domain_response.py
+-rw-r--r--   0        0        0    11875 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/domains_response.py
+-rw-r--r--   0        0        0    12604 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/enabled_product_response.py
+-rw-r--r--   0        0        0    11739 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/enabled_product_response_links.py
+-rw-r--r--   0        0        0    11694 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/enabled_product_response_product.py
+-rw-r--r--   0        0        0    11694 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/enabled_product_response_service.py
+-rw-r--r--   0        0        0    12088 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/event.py
+-rw-r--r--   0        0        0    21129 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/event_attributes.py
+-rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/event_response.py
+-rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/events_response.py
+-rw-r--r--   0        0        0    11554 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/events_response_all_of.py
+-rw-r--r--   0        0        0    11395 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/generic_token_error.py
+-rw-r--r--   0        0        0    12758 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/gzip.py
+-rw-r--r--   0        0        0    16735 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/gzip_response.py
+-rw-r--r--   0        0        0    15905 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/header.py
+-rw-r--r--   0        0        0    19828 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/header_response.py
+-rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/healthcheck.py
+-rw-r--r--   0        0        0    18979 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/healthcheck_response.py
+-rw-r--r--   0        0        0    12267 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/historical.py
+-rw-r--r--   0        0        0    14970 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/historical_aggregate_response.py
+-rw-r--r--   0        0        0    11672 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/historical_aggregate_response_all_of.py
+-rw-r--r--   0        0        0    15047 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/historical_field_aggregate_response.py
+-rw-r--r--   0        0        0    11723 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/historical_field_aggregate_response_all_of.py
+-rw-r--r--   0        0        0    15004 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/historical_field_response.py
+-rw-r--r--   0        0        0    11726 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/historical_field_response_all_of.py
+-rw-r--r--   0        0        0    11740 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/historical_field_results.py
+-rw-r--r--   0        0        0    11919 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/historical_meta.py
+-rw-r--r--   0        0        0    14797 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/historical_regions_response.py
+-rw-r--r--   0        0        0    11445 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/historical_regions_response_all_of.py
+-rw-r--r--   0        0        0    15199 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/historical_response.py
+-rw-r--r--   0        0        0    11947 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/historical_response_all_of.py
+-rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/historical_results.py
+-rw-r--r--   0        0        0    11403 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/historical_services.py
+-rw-r--r--   0        0        0    15037 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/historical_usage_aggregate_response.py
+-rw-r--r--   0        0        0    15124 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/historical_usage_month_response.py
+-rw-r--r--   0        0        0    11820 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/historical_usage_month_response_all_of.py
+-rw-r--r--   0        0        0    12346 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/historical_usage_month_response_all_of_data.py
+-rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/historical_usage_results.py
+-rw-r--r--   0        0        0    15031 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/historical_usage_service_response.py
+-rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/historical_usage_service_response_all_of.py
+-rw-r--r--   0        0        0    15675 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/http3.py
+-rw-r--r--   0        0        0    11705 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/http3_all_of.py
+-rw-r--r--   0        0        0    12796 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/http_response_format.py
+-rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/http_stream_format.py
+-rw-r--r--   0        0        0    13211 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/iam_permission.py
+-rw-r--r--   0        0        0    15987 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/iam_role.py
+-rw-r--r--   0        0        0    12962 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/iam_role_all_of.py
+-rw-r--r--   0        0        0    15636 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/iam_service_group.py
+-rw-r--r--   0        0        0    12570 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/iam_service_group_all_of.py
+-rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/iam_user_group.py
+-rw-r--r--   0        0        0    12926 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/iam_user_group_all_of.py
+-rw-r--r--   0        0        0    12044 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/included_with_waf_active_rule.py
+-rw-r--r--   0        0        0    15142 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/included_with_waf_active_rule_item.py
+-rw-r--r--   0        0        0    12031 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/included_with_waf_exclusion.py
+-rw-r--r--   0        0        0    14619 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/included_with_waf_exclusion_item.py
+-rw-r--r--   0        0        0    12000 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/included_with_waf_firewall.py
+-rw-r--r--   0        0        0    12104 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/included_with_waf_firewall_version.py
+-rw-r--r--   0        0        0    13972 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/included_with_waf_firewall_version_item.py
+-rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/included_with_waf_rule.py
+-rw-r--r--   0        0        0    14599 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/included_with_waf_rule_item.py
+-rw-r--r--   0        0        0    11848 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/included_with_waf_rule_revision.py
+-rw-r--r--   0        0        0    11416 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/inline_object.py
+-rw-r--r--   0        0        0    11419 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/inline_object1.py
+-rw-r--r--   0        0        0    11418 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/inline_response200.py
+-rw-r--r--   0        0        0    11605 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/inline_response2001.py
+-rw-r--r--   0        0        0    11985 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/inline_response2002.py
+-rw-r--r--   0        0        0    11725 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/inline_response2002_meta.py
+-rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/inline_response2003.py
+-rw-r--r--   0        0        0    11633 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/inline_response2003_meta.py
+-rw-r--r--   0        0        0    11585 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/invitation.py
+-rw-r--r--   0        0        0    12539 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/invitation_data.py
+-rw-r--r--   0        0        0    12611 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/invitation_data_attributes.py
+-rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/invitation_response.py
+-rw-r--r--   0        0        0    11681 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/invitation_response_all_of.py
+-rw-r--r--   0        0        0    14895 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/invitation_response_data.py
+-rw-r--r--   0        0        0    12283 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/invitation_response_data_all_of.py
+-rw-r--r--   0        0        0    14597 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/invitations_response.py
+-rw-r--r--   0        0        0    11690 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/invitations_response_all_of.py
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_address_and_port.py
+-rw-r--r--   0        0        0    22489 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_azureblob.py
+-rw-r--r--   0        0        0    14206 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_azureblob_all_of.py
+-rw-r--r--   0        0        0    24022 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_azureblob_response.py
+-rw-r--r--   0        0        0    19390 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_bigquery.py
+-rw-r--r--   0        0        0    13195 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_bigquery_all_of.py
+-rw-r--r--   0        0        0    20943 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_bigquery_response.py
+-rw-r--r--   0        0        0    21831 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_cloudfiles.py
+-rw-r--r--   0        0        0    13543 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_cloudfiles_all_of.py
+-rw-r--r--   0        0        0    23364 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_cloudfiles_response.py
+-rw-r--r--   0        0        0    14144 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_common.py
+-rw-r--r--   0        0        0    23211 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_datadog.py
+-rw-r--r--   0        0        0    18487 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_datadog_all_of.py
+-rw-r--r--   0        0        0    24914 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_datadog_response.py
+-rw-r--r--   0        0        0    21812 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_digitalocean.py
+-rw-r--r--   0        0        0    13514 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_digitalocean_all_of.py
+-rw-r--r--   0        0        0    23345 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_digitalocean_response.py
+-rw-r--r--   0        0        0    22734 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_elasticsearch.py
+-rw-r--r--   0        0        0    14289 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_elasticsearch_all_of.py
+-rw-r--r--   0        0        0    24096 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_elasticsearch_response.py
+-rw-r--r--   0        0        0    12403 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_format_version.py
+-rw-r--r--   0        0        0    22023 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_ftp.py
+-rw-r--r--   0        0        0    13770 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_ftp_all_of.py
+-rw-r--r--   0        0        0    23556 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_ftp_response.py
+-rw-r--r--   0        0        0    22679 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_gcs.py
+-rw-r--r--   0        0        0    12744 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_gcs_all_of.py
+-rw-r--r--   0        0        0    12815 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_gcs_common.py
+-rw-r--r--   0        0        0    24062 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_gcs_response.py
+-rw-r--r--   0        0        0    14090 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_generic_common.py
+-rw-r--r--   0        0        0    18898 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_google_pubsub.py
+-rw-r--r--   0        0        0    12402 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_google_pubsub_all_of.py
+-rw-r--r--   0        0        0    20451 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_google_pubsub_response.py
+-rw-r--r--   0        0        0    17238 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_heroku.py
+-rw-r--r--   0        0        0    11999 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_heroku_all_of.py
+-rw-r--r--   0        0        0    18941 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_heroku_response.py
+-rw-r--r--   0        0        0    17018 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_honeycomb.py
+-rw-r--r--   0        0        0    12284 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_honeycomb_all_of.py
+-rw-r--r--   0        0        0    18721 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_honeycomb_response.py
+-rw-r--r--   0        0        0    23100 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_https.py
+-rw-r--r--   0        0        0    15781 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_https_all_of.py
+-rw-r--r--   0        0        0    24462 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_https_response.py
+-rw-r--r--   0        0        0    23053 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_kafka.py
+-rw-r--r--   0        0        0    15405 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_kafka_all_of.py
+-rw-r--r--   0        0        0    24606 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_kafka_response.py
+-rw-r--r--   0        0        0    16368 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_kinesis.py
+-rw-r--r--   0        0        0    20332 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_kinesis_response.py
+-rw-r--r--   0        0        0    18046 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_logentries.py
+-rw-r--r--   0        0        0    12851 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_logentries_all_of.py
+-rw-r--r--   0        0        0    19749 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_logentries_response.py
+-rw-r--r--   0        0        0    16993 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_loggly.py
+-rw-r--r--   0        0        0    11754 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_loggly_all_of.py
+-rw-r--r--   0        0        0    18696 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_loggly_response.py
+-rw-r--r--   0        0        0    17065 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_logshuttle.py
+-rw-r--r--   0        0        0    11806 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_logshuttle_all_of.py
+-rw-r--r--   0        0        0    18768 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_logshuttle_response.py
+-rw-r--r--   0        0        0    11945 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_message_type.py
+-rw-r--r--   0        0        0    18795 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_newrelic.py
+-rw-r--r--   0        0        0    14066 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_newrelic_all_of.py
+-rw-r--r--   0        0        0    20498 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_newrelic_response.py
+-rw-r--r--   0        0        0    21509 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_openstack.py
+-rw-r--r--   0        0        0    13226 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_openstack_all_of.py
+-rw-r--r--   0        0        0    23042 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_openstack_response.py
+-rw-r--r--   0        0        0    17068 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_papertrail.py
+-rw-r--r--   0        0        0    18776 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_papertrail_response.py
+-rw-r--r--   0        0        0    12818 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_placement.py
+-rw-r--r--   0        0        0    12265 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_request_caps_common.py
+-rw-r--r--   0        0        0    24622 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_s3.py
+-rw-r--r--   0        0        0    16374 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_s3_all_of.py
+-rw-r--r--   0        0        0    26155 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_s3_response.py
+-rw-r--r--   0        0        0    17727 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_scalyr.py
+-rw-r--r--   0        0        0    12488 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_scalyr_all_of.py
+-rw-r--r--   0        0        0    19430 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_scalyr_response.py
+-rw-r--r--   0        0        0    22808 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_sftp.py
+-rw-r--r--   0        0        0    14123 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_sftp_all_of.py
+-rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_sftp_response.py
+-rw-r--r--   0        0        0    21030 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_splunk.py
+-rw-r--r--   0        0        0    12164 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_splunk_all_of.py
+-rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_splunk_response.py
+-rw-r--r--   0        0        0    17102 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_sumologic.py
+-rw-r--r--   0        0        0    11912 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_sumologic_all_of.py
+-rw-r--r--   0        0        0    18805 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_sumologic_response.py
+-rw-r--r--   0        0        0    21452 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_syslog.py
+-rw-r--r--   0        0        0    13046 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_syslog_all_of.py
+-rw-r--r--   0        0        0    22829 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_syslog_response.py
+-rw-r--r--   0        0        0    13547 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_tls_common.py
+-rw-r--r--   0        0        0    11595 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/logging_use_tls.py
+-rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/mutual_authentication.py
+-rw-r--r--   0        0        0    12711 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/mutual_authentication_data.py
+-rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/mutual_authentication_data_attributes.py
+-rw-r--r--   0        0        0    11767 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/mutual_authentication_response.py
+-rw-r--r--   0        0        0    15149 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/mutual_authentication_response_attributes.py
+-rw-r--r--   0        0        0    11647 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/mutual_authentication_response_attributes_all_of.py
+-rw-r--r--   0        0        0    15368 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/mutual_authentication_response_data.py
+-rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/mutual_authentication_response_data_all_of.py
+-rw-r--r--   0        0        0    14749 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/mutual_authentications_response.py
+-rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/mutual_authentications_response_all_of.py
+-rw-r--r--   0        0        0    11906 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/number_version.py
+-rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/package.py
+-rw-r--r--   0        0        0    12863 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/package_metadata.py
+-rw-r--r--   0        0        0    15990 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/package_response.py
+-rw-r--r--   0        0        0    11519 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/package_response_all_of.py
+-rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/pagination.py
+-rw-r--r--   0        0        0    12267 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/pagination_links.py
+-rw-r--r--   0        0        0    12484 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/pagination_meta.py
+-rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/permission.py
+-rw-r--r--   0        0        0    23511 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/pool.py
+-rw-r--r--   0        0        0    18578 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/pool_all_of.py
+-rw-r--r--   0        0        0    25586 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/pool_response.py
+-rw-r--r--   0        0        0    11418 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/pool_response_all_of.py
+-rw-r--r--   0        0        0    15216 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/pop.py
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/pop_coordinates.py
+-rw-r--r--   0        0        0    11742 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/public_ip_list.py
+-rw-r--r--   0        0        0    12528 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/publish_item.py
+-rw-r--r--   0        0        0    12411 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/publish_item_formats.py
+-rw-r--r--   0        0        0    11685 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/publish_request.py
+-rw-r--r--   0        0        0    11432 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/purge_keys.py
+-rw-r--r--   0        0        0    11165 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/purge_keys_response.py
+-rw-r--r--   0        0        0    11594 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/purge_response.py
+-rw-r--r--   0        0        0    19002 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/rate_limiter.py
+-rw-r--r--   0        0        0    23413 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/rate_limiter_response.py
+-rw-r--r--   0        0        0    12394 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/rate_limiter_response1.py
+-rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/rate_limiter_response_all_of.py
+-rw-r--r--   0        0        0    12619 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/realtime.py
+-rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/realtime_entry.py
+-rw-r--r--   0        0        0    97542 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/realtime_measurements.py
+-rw-r--r--   0        0        0    11749 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_common_name.py
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_customer.py
+-rw-r--r--   0        0        0    11730 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_customer_customer.py
+-rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_member_customer.py
+-rw-r--r--   0        0        0    11936 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_member_mutual_authentication.py
+-rw-r--r--   0        0        0    11805 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_member_service.py
+-rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_member_service_invitation.py
+-rw-r--r--   0        0        0    11866 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_member_tls_activation.py
+-rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_member_tls_bulk_certificate.py
+-rw-r--r--   0        0        0    11876 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_member_tls_certificate.py
+-rw-r--r--   0        0        0    11896 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_member_tls_configuration.py
+-rw-r--r--   0        0        0    11857 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_member_tls_dns_record.py
+-rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_member_tls_domain.py
+-rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_member_tls_private_key.py
+-rw-r--r--   0        0        0    11886 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_member_tls_subscription.py
+-rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_member_waf_active_rule.py
+-rw-r--r--   0        0        0    11846 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_member_waf_firewall.py
+-rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_member_waf_firewall_version.py
+-rw-r--r--   0        0        0    11806 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_member_waf_rule.py
+-rw-r--r--   0        0        0    11995 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_member_waf_rule_revision.py
+-rw-r--r--   0        0        0    11884 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_member_waf_tag.py
+-rw-r--r--   0        0        0    12005 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_mutual_authentication.py
+-rw-r--r--   0        0        0    11881 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_mutual_authentication_mutual_authentication.py
+-rw-r--r--   0        0        0    12027 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_mutual_authentications.py
+-rw-r--r--   0        0        0    11893 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_mutual_authentications_mutual_authentications.py
+-rw-r--r--   0        0        0    11705 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_service.py
+-rw-r--r--   0        0        0    11961 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_service_invitations.py
+-rw-r--r--   0        0        0    12022 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_service_invitations_create.py
+-rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_service_invitations_create_service_invitations.py
+-rw-r--r--   0        0        0    11854 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_service_invitations_service_invitations.py
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_services.py
+-rw-r--r--   0        0        0    11723 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_services_services.py
+-rw-r--r--   0        0        0    11851 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_activation.py
+-rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_activation_tls_activation.py
+-rw-r--r--   0        0        0    11859 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_activations.py
+-rw-r--r--   0        0        0    11968 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_bulk_certificate.py
+-rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_bulk_certificate_tls_bulk_certificate.py
+-rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_bulk_certificates.py
+-rw-r--r--   0        0        0    11873 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_certificate.py
+-rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_certificate_tls_certificate.py
+-rw-r--r--   0        0        0    11895 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_certificates.py
+-rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_certificates_tls_certificates.py
+-rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_configuration.py
+-rw-r--r--   0        0        0    11829 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_configuration_tls_configuration.py
+-rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_configurations.py
+-rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_configurations_tls_configurations.py
+-rw-r--r--   0        0        0    11794 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_dns_record.py
+-rw-r--r--   0        0        0    11775 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_dns_record_dns_record.py
+-rw-r--r--   0        0        0    11802 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_dns_records.py
+-rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_domain.py
+-rw-r--r--   0        0        0    11738 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_domain_tls_domain.py
+-rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_domains.py
+-rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_domains_tls_domains.py
+-rw-r--r--   0        0        0    11858 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_private_key.py
+-rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_private_key_tls_private_key.py
+-rw-r--r--   0        0        0    11880 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_private_keys.py
+-rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_private_keys_tls_private_keys.py
+-rw-r--r--   0        0        0    11895 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_subscription.py
+-rw-r--r--   0        0        0    11822 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_subscription_tls_subscription.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_tls_subscriptions.py
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_user.py
+-rw-r--r--   0        0        0    11836 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_user_user.py
+-rw-r--r--   0        0        0    11880 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_waf_active_rules.py
+-rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_waf_active_rules_waf_active_rules.py
+-rw-r--r--   0        0        0    11807 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_waf_firewall.py
+-rw-r--r--   0        0        0    11968 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_waf_firewall_version.py
+-rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_waf_firewall_version_waf_firewall_version.py
+-rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_waf_firewall_versions.py
+-rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_waf_firewall_waf_firewall.py
+-rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_waf_rule.py
+-rw-r--r--   0        0        0    11914 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_waf_rule_revision.py
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_waf_rule_revision_waf_rule_revisions.py
+-rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_waf_rule_revisions.py
+-rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_waf_rule_waf_rule.py
+-rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_waf_rules.py
+-rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_waf_tags.py
+-rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationship_waf_tags_waf_tags.py
+-rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationships_for_invitation.py
+-rw-r--r--   0        0        0    14050 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationships_for_mutual_authentication.py
+-rw-r--r--   0        0        0    14345 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationships_for_star.py
+-rw-r--r--   0        0        0    11882 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationships_for_tls_activation.py
+-rw-r--r--   0        0        0    14690 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationships_for_tls_bulk_certificate.py
+-rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationships_for_tls_configuration.py
+-rw-r--r--   0        0        0    14687 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationships_for_tls_domain.py
+-rw-r--r--   0        0        0    14589 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationships_for_tls_private_key.py
+-rw-r--r--   0        0        0    15411 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationships_for_tls_subscription.py
+-rw-r--r--   0        0        0    14951 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationships_for_waf_active_rule.py
+-rw-r--r--   0        0        0    14691 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationships_for_waf_exclusion.py
+-rw-r--r--   0        0        0    14940 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationships_for_waf_firewall_version.py
+-rw-r--r--   0        0        0    14666 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/relationships_for_waf_rule.py
+-rw-r--r--   0        0        0    15858 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/request_settings.py
+-rw-r--r--   0        0        0    19891 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/request_settings_response.py
+-rw-r--r--   0        0        0    11736 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/resource.py
+-rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/resource_response.py
+-rw-r--r--   0        0        0    12732 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/resource_response_all_of.py
+-rw-r--r--   0        0        0    13673 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/response_object.py
+-rw-r--r--   0        0        0    17701 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/response_object_response.py
+-rw-r--r--   0        0        0    96777 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/results.py
+-rw-r--r--   0        0        0    12451 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/role_user.py
+-rw-r--r--   0        0        0    17321 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/schemas_contact_response.py
+-rw-r--r--   0        0        0    17541 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/schemas_snippet_response.py
+-rw-r--r--   0        0        0    18068 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/schemas_user_response.py
+-rw-r--r--   0        0        0    15953 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/schemas_vcl_response.py
+-rw-r--r--   0        0        0    13626 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/schemas_version.py
+-rw-r--r--   0        0        0    17433 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/schemas_version_response.py
+-rw-r--r--   0        0        0    11738 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/schemas_waf_firewall_version.py
+-rw-r--r--   0        0        0    12179 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/schemas_waf_firewall_version_data.py
+-rw-r--r--   0        0        0    14569 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/server.py
+-rw-r--r--   0        0        0    18752 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/server_response.py
+-rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/server_response_all_of.py
+-rw-r--r--   0        0        0    12015 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service.py
+-rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_authorization.py
+-rw-r--r--   0        0        0    12718 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_authorization_data.py
+-rw-r--r--   0        0        0    11658 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_authorization_data_attributes.py
+-rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_authorization_data_relationships.py
+-rw-r--r--   0        0        0    11899 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_authorization_data_relationships_user.py
+-rw-r--r--   0        0        0    11844 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_authorization_data_relationships_user_data.py
+-rw-r--r--   0        0        0    11767 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_authorization_response.py
+-rw-r--r--   0        0        0    15176 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_authorization_response_data.py
+-rw-r--r--   0        0        0    11863 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_authorization_response_data_all_of.py
+-rw-r--r--   0        0        0    14749 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_authorizations_response.py
+-rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_authorizations_response_all_of.py
+-rw-r--r--   0        0        0    14640 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_create.py
+-rw-r--r--   0        0        0    11543 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_create_all_of.py
+-rw-r--r--   0        0        0    18255 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_detail.py
+-rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_detail_all_of.py
+-rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_id_and_version.py
+-rw-r--r--   0        0        0    11656 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_invitation.py
+-rw-r--r--   0        0        0    12646 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_invitation_data.py
+-rw-r--r--   0        0        0    11922 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_invitation_data_attributes.py
+-rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_invitation_data_relationships.py
+-rw-r--r--   0        0        0    14111 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_invitation_response.py
+-rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_invitation_response_all_of.py
+-rw-r--r--   0        0        0    11854 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_invitation_response_all_of_data.py
+-rw-r--r--   0        0        0    17024 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_list_response.py
+-rw-r--r--   0        0        0    12407 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_list_response_all_of.py
+-rw-r--r--   0        0        0    17544 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_response.py
+-rw-r--r--   0        0        0    12948 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_response_all_of.py
+-rw-r--r--   0        0        0    23835 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_version_detail.py
+-rw-r--r--   0        0        0    23852 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/service_version_detail_or_null.py
+-rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/settings.py
+-rw-r--r--   0        0        0    15732 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/settings_response.py
+-rw-r--r--   0        0        0    13161 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/snippet.py
+-rw-r--r--   0        0        0    17520 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/snippet_response.py
+-rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/snippet_response_all_of.py
+-rw-r--r--   0        0        0    11525 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/star.py
+-rw-r--r--   0        0        0    11945 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/star_data.py
+-rw-r--r--   0        0        0    13825 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/star_response.py
+-rw-r--r--   0        0        0    11571 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/star_response_all_of.py
+-rw-r--r--   0        0        0    11555 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/stats.py
+-rw-r--r--   0        0        0    11440 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/store.py
+-rw-r--r--   0        0        0    11668 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/store_response.py
+-rw-r--r--   0        0        0    12287 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/timestamps.py
+-rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/timestamps_no_delete.py
+-rw-r--r--   0        0        0    11616 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_activation.py
+-rw-r--r--   0        0        0    12100 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_activation_data.py
+-rw-r--r--   0        0        0    11697 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_activation_response.py
+-rw-r--r--   0        0        0    14980 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_activation_response_data.py
+-rw-r--r--   0        0        0    11842 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_activation_response_data_all_of.py
+-rw-r--r--   0        0        0    14644 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_activations_response.py
+-rw-r--r--   0        0        0    11721 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_activations_response_all_of.py
+-rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_bulk_certificate.py
+-rw-r--r--   0        0        0    12666 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_bulk_certificate_data.py
+-rw-r--r--   0        0        0    12407 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_bulk_certificate_data_attributes.py
+-rw-r--r--   0        0        0    11748 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_bulk_certificate_response.py
+-rw-r--r--   0        0        0    16192 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_bulk_certificate_response_attributes.py
+-rw-r--r--   0        0        0    12699 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_bulk_certificate_response_attributes_all_of.py
+-rw-r--r--   0        0        0    15305 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_bulk_certificate_response_data.py
+-rw-r--r--   0        0        0    12043 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_bulk_certificate_response_data_all_of.py
+-rw-r--r--   0        0        0    14721 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_bulk_certificates_response.py
+-rw-r--r--   0        0        0    11772 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_bulk_certificates_response_all_of.py
+-rw-r--r--   0        0        0    11626 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_certificate.py
+-rw-r--r--   0        0        0    12510 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_certificate_data.py
+-rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_certificate_data_attributes.py
+-rw-r--r--   0        0        0    11707 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_certificate_response.py
+-rw-r--r--   0        0        0    17609 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_certificate_response_attributes.py
+-rw-r--r--   0        0        0    14137 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_certificate_response_attributes_all_of.py
+-rw-r--r--   0        0        0    15107 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_certificate_response_data.py
+-rw-r--r--   0        0        0    12002 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_certificate_response_data_all_of.py
+-rw-r--r--   0        0        0    14659 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_certificates_response.py
+-rw-r--r--   0        0        0    11731 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_certificates_response_all_of.py
+-rw-r--r--   0        0        0    13892 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_common.py
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_configuration.py
+-rw-r--r--   0        0        0    12615 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_configuration_data.py
+-rw-r--r--   0        0        0    11525 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_configuration_data_attributes.py
+-rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_configuration_response.py
+-rw-r--r--   0        0        0    16408 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_configuration_response_attributes.py
+-rw-r--r--   0        0        0    12926 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_configuration_response_attributes_all_of.py
+-rw-r--r--   0        0        0    15232 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_configuration_response_data.py
+-rw-r--r--   0        0        0    12022 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_configuration_response_data_all_of.py
+-rw-r--r--   0        0        0    14689 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_configurations_response.py
+-rw-r--r--   0        0        0    11751 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_configurations_response_all_of.py
+-rw-r--r--   0        0        0    13196 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_dns_record.py
+-rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_domain_data.py
+-rw-r--r--   0        0        0    14527 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_domains_response.py
+-rw-r--r--   0        0        0    11624 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_domains_response_all_of.py
+-rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_private_key.py
+-rw-r--r--   0        0        0    12546 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_private_key_data.py
+-rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_private_key_data_attributes.py
+-rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_private_key_response.py
+-rw-r--r--   0        0        0    16480 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_private_key_response_attributes.py
+-rw-r--r--   0        0        0    13012 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_private_key_response_attributes_all_of.py
+-rw-r--r--   0        0        0    12321 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_private_key_response_data.py
+-rw-r--r--   0        0        0    14646 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_private_keys_response.py
+-rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_private_keys_response_all_of.py
+-rw-r--r--   0        0        0    11636 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_subscription.py
+-rw-r--r--   0        0        0    12591 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_subscription_data.py
+-rw-r--r--   0        0        0    11818 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_subscription_data_attributes.py
+-rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_subscription_response.py
+-rw-r--r--   0        0        0    15234 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_subscription_response_attributes.py
+-rw-r--r--   0        0        0    11757 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_subscription_response_attributes_all_of.py
+-rw-r--r--   0        0        0    14191 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_subscription_response_data.py
+-rw-r--r--   0        0        0    12012 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_subscription_response_data_all_of.py
+-rw-r--r--   0        0        0    14645 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_subscriptions_response.py
+-rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/tls_subscriptions_response_all_of.py
+-rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/token.py
+-rw-r--r--   0        0        0    18055 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/token_created_response.py
+-rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/token_created_response_all_of.py
+-rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/token_response.py
+-rw-r--r--   0        0        0    13237 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/token_response_all_of.py
+-rw-r--r--   0        0        0    11733 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_billing_address.py
+-rw-r--r--   0        0        0    11616 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_contact.py
+-rw-r--r--   0        0        0    11631 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_customer.py
+-rw-r--r--   0        0        0    11586 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_event.py
+-rw-r--r--   0        0        0    11661 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_invitation.py
+-rw-r--r--   0        0        0    11823 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_mutual_authentication.py
+-rw-r--r--   0        0        0    11895 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_resource.py
+-rw-r--r--   0        0        0    11616 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_service.py
+-rw-r--r--   0        0        0    11823 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_service_authorization.py
+-rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_service_invitation.py
+-rw-r--r--   0        0        0    11571 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_star.py
+-rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_tls_activation.py
+-rw-r--r--   0        0        0    11805 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_tls_bulk_certificate.py
+-rw-r--r--   0        0        0    11733 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_tls_certificate.py
+-rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_tls_configuration.py
+-rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_tls_dns_record.py
+-rw-r--r--   0        0        0    11658 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_tls_domain.py
+-rw-r--r--   0        0        0    11730 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_tls_private_key.py
+-rw-r--r--   0        0        0    11748 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_tls_subscription.py
+-rw-r--r--   0        0        0    11571 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_user.py
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_waf_active_rule.py
+-rw-r--r--   0        0        0    11707 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_waf_exclusion.py
+-rw-r--r--   0        0        0    11692 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_waf_firewall.py
+-rw-r--r--   0        0        0    11809 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_waf_firewall_version.py
+-rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_waf_rule.py
+-rw-r--r--   0        0        0    11764 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_waf_rule_revision.py
+-rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/type_waf_tag.py
+-rw-r--r--   0        0        0    12136 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/update_billing_address_request.py
+-rw-r--r--   0        0        0    12402 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/update_billing_address_request_data.py
+-rw-r--r--   0        0        0    13820 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/user.py
+-rw-r--r--   0        0        0    18047 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/user_response.py
+-rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/user_response_all_of.py
+-rw-r--r--   0        0        0    12570 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/validator_result.py
+-rw-r--r--   0        0        0    12325 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/validator_result_messages.py
+-rw-r--r--   0        0        0    11960 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/vcl.py
+-rw-r--r--   0        0        0    12644 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/vcl_diff.py
+-rw-r--r--   0        0        0    15932 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/vcl_response.py
+-rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/version.py
+-rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/version_create_response.py
+-rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/version_detail.py
+-rw-r--r--   0        0        0    12978 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/version_detail_settings.py
+-rw-r--r--   0        0        0    17376 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/version_response.py
+-rw-r--r--   0        0        0    11475 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/version_response_all_of.py
+-rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_active_rule.py
+-rw-r--r--   0        0        0    15118 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_active_rule_creation_response.py
+-rw-r--r--   0        0        0    12546 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_active_rule_data.py
+-rw-r--r--   0        0        0    12548 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_active_rule_data_attributes.py
+-rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_active_rule_response.py
+-rw-r--r--   0        0        0    15228 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_active_rule_response_data.py
+-rw-r--r--   0        0        0    12559 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_active_rule_response_data_all_of.py
+-rw-r--r--   0        0        0    15589 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_active_rule_response_data_attributes.py
+-rw-r--r--   0        0        0    12100 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_active_rule_response_data_attributes_all_of.py
+-rw-r--r--   0        0        0    14978 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_active_rule_response_data_relationships.py
+-rw-r--r--   0        0        0    15066 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_active_rules_response.py
+-rw-r--r--   0        0        0    12142 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_active_rules_response_all_of.py
+-rw-r--r--   0        0        0    11606 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_exclusion.py
+-rw-r--r--   0        0        0    12519 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_exclusion_data.py
+-rw-r--r--   0        0        0    13837 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_exclusion_data_attributes.py
+-rw-r--r--   0        0        0    11687 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_exclusion_response.py
+-rw-r--r--   0        0        0    15289 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_exclusion_response_data.py
+-rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_exclusion_response_data_all_of.py
+-rw-r--r--   0        0        0    17359 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_exclusion_response_data_attributes.py
+-rw-r--r--   0        0        0    13876 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_exclusion_response_data_attributes_all_of.py
+-rw-r--r--   0        0        0    14718 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_exclusion_response_data_relationships.py
+-rw-r--r--   0        0        0    15041 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_exclusions_response.py
+-rw-r--r--   0        0        0    12123 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_exclusions_response_all_of.py
+-rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_firewall.py
+-rw-r--r--   0        0        0    12037 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_firewall_data.py
+-rw-r--r--   0        0        0    12561 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_firewall_data_attributes.py
+-rw-r--r--   0        0        0    12082 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_firewall_response.py
+-rw-r--r--   0        0        0    15119 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_firewall_response_data.py
+-rw-r--r--   0        0        0    12487 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_firewall_response_data_all_of.py
+-rw-r--r--   0        0        0    19383 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_firewall_response_data_attributes.py
+-rw-r--r--   0        0        0    15905 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_firewall_response_data_attributes_all_of.py
+-rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_firewall_version.py
+-rw-r--r--   0        0        0    12158 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_firewall_version_data.py
+-rw-r--r--   0        0        0    24857 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_firewall_version_data_attributes.py
+-rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_firewall_version_response.py
+-rw-r--r--   0        0        0    15440 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_firewall_version_response_data.py
+-rw-r--r--   0        0        0    12686 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_firewall_version_response_data_all_of.py
+-rw-r--r--   0        0        0    20346 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_firewall_version_response_data_attributes.py
+-rw-r--r--   0        0        0    16832 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_firewall_version_response_data_attributes_all_of.py
+-rw-r--r--   0        0        0    15176 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_firewall_versions_response.py
+-rw-r--r--   0        0        0    12227 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_firewall_versions_response_all_of.py
+-rw-r--r--   0        0        0    15019 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_firewalls_response.py
+-rw-r--r--   0        0        0    12106 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_firewalls_response_all_of.py
+-rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_rule.py
+-rw-r--r--   0        0        0    12553 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_rule_attributes.py
+-rw-r--r--   0        0        0    12014 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_rule_response.py
+-rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_rule_response_data.py
+-rw-r--r--   0        0        0    11737 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_rule_response_data_all_of.py
+-rw-r--r--   0        0        0    12370 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_rule_revision.py
+-rw-r--r--   0        0        0    13775 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_rule_revision_attributes.py
+-rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_rule_revision_or_latest.py
+-rw-r--r--   0        0        0    12152 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_rule_revision_response.py
+-rw-r--r--   0        0        0    15147 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_rule_revision_response_data.py
+-rw-r--r--   0        0        0    11732 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_rule_revision_response_data_all_of.py
+-rw-r--r--   0        0        0    15110 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_rule_revisions_response.py
+-rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_rule_revisions_response_all_of.py
+-rw-r--r--   0        0        0    14931 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_rules_response.py
+-rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_rules_response_all_of.py
+-rw-r--r--   0        0        0    12195 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_tag.py
+-rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_tag_attributes.py
+-rw-r--r--   0        0        0    14872 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_tags_response.py
+-rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_tags_response_all_of.py
+-rw-r--r--   0        0        0    14941 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/waf_tags_response_data_item.py
+-rw-r--r--   0        0        0    11832 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/model/ws_message_format.py
+-rw-r--r--   0        0        0    44057 2020-02-02 00:00:00.000000 fastly-1.3.1/fastly/models/__init__.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 fastly-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 fastly-1.3.1/LICENSE
+-rw-r--r--   0        0        0    87607 2020-02-02 00:00:00.000000 fastly-1.3.1/README.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastly-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0    88099 2020-02-02 00:00:00.000000 fastly-1.3.1/PKG-INFO
```

### Comparing `fastly-1.3.0/CHANGELOG.md` & `fastly-1.3.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## [v1.3.1](https://github.com/fastly/fastly-py/releases/tag/release/v1.3.1) (2023-04-26)
+
+**Bug fixes:**
+
+- fix(object-store-item): use correct type for key value
+- fix(tls-csrs): remove internal endpoint
+
 ## [v1.3.0](https://github.com/fastly/fastly-py/releases/tag/release/v1.3.0) (2023-04-03)
 
 **Bug fixes:**
 
 - fix(purge): avoid escaping URL parameter
 
 **Enhancements:**
```

### Comparing `fastly-1.3.0/SECURITY.md` & `fastly-1.3.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/setup.py` & `fastly-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 from pathlib import Path
 
 NAME = "fastly"
-VERSION = "1.3.0"
+VERSION = "1.3.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `fastly-1.3.0/.github/scripts/pack.sh` & `fastly-1.3.1/.github/scripts/pack.sh`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/.github/scripts/publish_env.sh` & `fastly-1.3.1/.github/scripts/publish_env.sh`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/.github/scripts/release_body.sh` & `fastly-1.3.1/.github/scripts/release_body.sh`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/.github/workflows/ci-release.yaml` & `fastly-1.3.1/.github/workflows/ci-release.yaml`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Acl.md` & `fastly-1.3.1/docs/Acl.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/AclApi.md` & `fastly-1.3.1/docs/AclApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/AclEntry.md` & `fastly-1.3.1/docs/AclEntry.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/AclEntryApi.md` & `fastly-1.3.1/docs/AclEntryApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/AclEntryResponse.md` & `fastly-1.3.1/docs/AclEntryResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/AclEntryResponseAllOf.md` & `fastly-1.3.1/docs/AclEntryResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/AclResponse.md` & `fastly-1.3.1/docs/AclResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ApexRedirect.md` & `fastly-1.3.1/docs/ApexRedirect.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ApexRedirectAllOf.md` & `fastly-1.3.1/docs/ApexRedirectAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ApexRedirectApi.md` & `fastly-1.3.1/docs/ApexRedirectApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/AwsRegion.md` & `fastly-1.3.1/docs/AwsRegion.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Backend.md` & `fastly-1.3.1/docs/Backend.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BackendApi.md` & `fastly-1.3.1/docs/BackendApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BackendResponse.md` & `fastly-1.3.1/docs/BackendResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BackendResponseAllOf.md` & `fastly-1.3.1/docs/BackendResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Billing.md` & `fastly-1.3.1/docs/Billing.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BillingAddressApi.md` & `fastly-1.3.1/docs/BillingAddressApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BillingAddressAttributes.md` & `fastly-1.3.1/docs/BillingAddressAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BillingAddressRequest.md` & `fastly-1.3.1/docs/BillingAddressRequest.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BillingAddressRequestData.md` & `fastly-1.3.1/docs/BillingAddressRequestData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BillingAddressResponse.md` & `fastly-1.3.1/docs/BillingAddressResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BillingAddressResponseData.md` & `fastly-1.3.1/docs/BillingAddressResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BillingAddressVerificationErrorResponse.md` & `fastly-1.3.1/docs/BillingAddressVerificationErrorResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BillingAddressVerificationErrorResponseErrors.md` & `fastly-1.3.1/docs/BillingAddressVerificationErrorResponseErrors.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BillingApi.md` & `fastly-1.3.1/docs/BillingApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BillingEstimateResponse.md` & `fastly-1.3.1/docs/BillingEstimateResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BillingEstimateResponseAllOf.md` & `fastly-1.3.1/docs/BillingEstimateResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BillingEstimateResponseAllOfLine.md` & `fastly-1.3.1/docs/BillingEstimateResponseAllOfLine.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BillingEstimateResponseAllOfLines.md` & `fastly-1.3.1/docs/BillingEstimateResponseAllOfLines.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BillingResponse.md` & `fastly-1.3.1/docs/BillingResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BillingResponseAllOf.md` & `fastly-1.3.1/docs/BillingResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BillingResponseLineItem.md` & `fastly-1.3.1/docs/BillingResponseLineItem.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BillingResponseLineItemAllOf.md` & `fastly-1.3.1/docs/BillingResponseLineItemAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BillingStatus.md` & `fastly-1.3.1/docs/BillingStatus.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BillingTotal.md` & `fastly-1.3.1/docs/BillingTotal.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BillingTotalExtras.md` & `fastly-1.3.1/docs/BillingTotalExtras.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BulkUpdateAclEntriesRequest.md` & `fastly-1.3.1/docs/BulkUpdateAclEntriesRequest.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BulkUpdateAclEntry.md` & `fastly-1.3.1/docs/BulkUpdateAclEntry.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BulkUpdateAclEntryAllOf.md` & `fastly-1.3.1/docs/BulkUpdateAclEntryAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BulkUpdateDictionaryItem.md` & `fastly-1.3.1/docs/BulkUpdateDictionaryItem.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BulkUpdateDictionaryListRequest.md` & `fastly-1.3.1/docs/BulkUpdateDictionaryListRequest.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/BulkWafActiveRules.md` & `fastly-1.3.1/docs/BulkWafActiveRules.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/CacheSetting.md` & `fastly-1.3.1/docs/CacheSetting.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/CacheSettingResponse.md` & `fastly-1.3.1/docs/CacheSettingResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/CacheSettingsApi.md` & `fastly-1.3.1/docs/CacheSettingsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Condition.md` & `fastly-1.3.1/docs/Condition.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ConditionApi.md` & `fastly-1.3.1/docs/ConditionApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ConditionResponse.md` & `fastly-1.3.1/docs/ConditionResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Contact.md` & `fastly-1.3.1/docs/Contact.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ContactApi.md` & `fastly-1.3.1/docs/ContactApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ContactResponse.md` & `fastly-1.3.1/docs/ContactResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ContactResponseAllOf.md` & `fastly-1.3.1/docs/ContactResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Content.md` & `fastly-1.3.1/docs/Content.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ContentApi.md` & `fastly-1.3.1/docs/ContentApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Customer.md` & `fastly-1.3.1/docs/Customer.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/CustomerApi.md` & `fastly-1.3.1/docs/CustomerApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/CustomerResponse.md` & `fastly-1.3.1/docs/CustomerResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/CustomerResponseAllOf.md` & `fastly-1.3.1/docs/CustomerResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Dictionary.md` & `fastly-1.3.1/docs/Dictionary.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/DictionaryApi.md` & `fastly-1.3.1/docs/DictionaryApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/DictionaryInfoApi.md` & `fastly-1.3.1/docs/DictionaryInfoApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/DictionaryInfoResponse.md` & `fastly-1.3.1/docs/DictionaryInfoResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/DictionaryItem.md` & `fastly-1.3.1/docs/DictionaryItem.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/DictionaryItemApi.md` & `fastly-1.3.1/docs/DictionaryItemApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/DictionaryItemResponse.md` & `fastly-1.3.1/docs/DictionaryItemResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/DictionaryItemResponseAllOf.md` & `fastly-1.3.1/docs/DictionaryItemResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/DictionaryResponse.md` & `fastly-1.3.1/docs/DictionaryResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/DictionaryResponseAllOf.md` & `fastly-1.3.1/docs/DictionaryResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/DiffApi.md` & `fastly-1.3.1/docs/DiffApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/DiffResponse.md` & `fastly-1.3.1/docs/DiffResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Director.md` & `fastly-1.3.1/docs/Director.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/DirectorApi.md` & `fastly-1.3.1/docs/DirectorApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/DirectorBackend.md` & `fastly-1.3.1/docs/DirectorBackend.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/DirectorBackendAllOf.md` & `fastly-1.3.1/docs/DirectorBackendAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/DirectorBackendApi.md` & `fastly-1.3.1/docs/DirectorBackendApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/DirectorResponse.md` & `fastly-1.3.1/docs/DirectorResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Domain.md` & `fastly-1.3.1/docs/Domain.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/DomainApi.md` & `fastly-1.3.1/docs/DomainApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/DomainCheckItem.md` & `fastly-1.3.1/docs/DomainCheckItem.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/DomainOwnershipsApi.md` & `fastly-1.3.1/docs/DomainOwnershipsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/DomainResponse.md` & `fastly-1.3.1/docs/DomainResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/EnabledProductResponse.md` & `fastly-1.3.1/docs/EnabledProductResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/EnabledProductResponseLinks.md` & `fastly-1.3.1/docs/EnabledProductResponseLinks.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/EnabledProductResponseProduct.md` & `fastly-1.3.1/docs/EnabledProductResponseProduct.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/EnabledProductResponseService.md` & `fastly-1.3.1/docs/EnabledProductResponseService.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/EnabledProductsApi.md` & `fastly-1.3.1/docs/EnabledProductsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ErrorResponse.md` & `fastly-1.3.1/docs/WafExclusion.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# ErrorResponse
+# WafExclusion
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**errors** | [**[ErrorResponseData]**](ErrorResponseData.md) |  | [optional] 
+**data** | [**WafExclusionData**](WafExclusionData.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/ErrorResponseData.md` & `fastly-1.3.1/docs/SnippetResponseAllOf.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# ErrorResponseData
+# SnippetResponseAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**title** | **str** |  | [optional] 
-**detail** | **str** |  | [optional] 
+**id** | **str** |  | [optional] [readonly] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/Event.md` & `fastly-1.3.1/docs/Event.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/EventAttributes.md` & `fastly-1.3.1/docs/EventAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/EventsApi.md` & `fastly-1.3.1/docs/EventsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/EventsResponse.md` & `fastly-1.3.1/docs/EventsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/EventsResponseAllOf.md` & `fastly-1.3.1/docs/EventsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Gzip.md` & `fastly-1.3.1/docs/Gzip.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/GzipApi.md` & `fastly-1.3.1/docs/GzipApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/GzipResponse.md` & `fastly-1.3.1/docs/GzipResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Header.md` & `fastly-1.3.1/docs/Header.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HeaderApi.md` & `fastly-1.3.1/docs/HeaderApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HeaderResponse.md` & `fastly-1.3.1/docs/HeaderResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Healthcheck.md` & `fastly-1.3.1/docs/Healthcheck.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HealthcheckApi.md` & `fastly-1.3.1/docs/HealthcheckApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HealthcheckResponse.md` & `fastly-1.3.1/docs/HealthcheckResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Historical.md` & `fastly-1.3.1/docs/Historical.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HistoricalAggregateResponse.md` & `fastly-1.3.1/docs/HistoricalAggregateResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HistoricalAggregateResponseAllOf.md` & `fastly-1.3.1/docs/HistoricalAggregateResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HistoricalApi.md` & `fastly-1.3.1/docs/HistoricalApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HistoricalFieldAggregateResponse.md` & `fastly-1.3.1/docs/HistoricalFieldAggregateResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HistoricalFieldAggregateResponseAllOf.md` & `fastly-1.3.1/docs/HistoricalFieldAggregateResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HistoricalFieldResponse.md` & `fastly-1.3.1/docs/HistoricalFieldResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HistoricalFieldResponseAllOf.md` & `fastly-1.3.1/docs/HistoricalFieldResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HistoricalMeta.md` & `fastly-1.3.1/docs/HistoricalMeta.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HistoricalRegionsResponse.md` & `fastly-1.3.1/docs/HistoricalRegionsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HistoricalRegionsResponseAllOf.md` & `fastly-1.3.1/docs/HistoricalRegionsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HistoricalResponse.md` & `fastly-1.3.1/docs/HistoricalResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HistoricalResponseAllOf.md` & `fastly-1.3.1/docs/HistoricalResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HistoricalUsageAggregateResponse.md` & `fastly-1.3.1/docs/HistoricalUsageAggregateResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HistoricalUsageMonthResponse.md` & `fastly-1.3.1/docs/HistoricalUsageMonthResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HistoricalUsageMonthResponseAllOf.md` & `fastly-1.3.1/docs/HistoricalUsageMonthResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HistoricalUsageMonthResponseAllOfData.md` & `fastly-1.3.1/docs/HistoricalUsageMonthResponseAllOfData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HistoricalUsageResults.md` & `fastly-1.3.1/docs/HistoricalUsageResults.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HistoricalUsageServiceResponse.md` & `fastly-1.3.1/docs/HistoricalUsageServiceResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HistoricalUsageServiceResponseAllOf.md` & `fastly-1.3.1/docs/HistoricalUsageServiceResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Http3.md` & `fastly-1.3.1/docs/Http3.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Http3AllOf.md` & `fastly-1.3.1/docs/Http3AllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Http3Api.md` & `fastly-1.3.1/docs/Http3Api.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HttpResponseFormat.md` & `fastly-1.3.1/docs/HttpResponseFormat.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/HttpStreamFormat.md` & `fastly-1.3.1/docs/HttpStreamFormat.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/IamPermission.md` & `fastly-1.3.1/docs/IamPermission.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/IamPermissionsApi.md` & `fastly-1.3.1/docs/IamPermissionsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/IamRole.md` & `fastly-1.3.1/docs/IamRole.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/IamRoleAllOf.md` & `fastly-1.3.1/docs/IamRoleAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/IamRolesApi.md` & `fastly-1.3.1/docs/IamRolesApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/IamServiceGroup.md` & `fastly-1.3.1/docs/IamServiceGroup.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/IamServiceGroupAllOf.md` & `fastly-1.3.1/docs/IamServiceGroupAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/IamServiceGroupsApi.md` & `fastly-1.3.1/docs/IamServiceGroupsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/IamUserGroup.md` & `fastly-1.3.1/docs/IamUserGroup.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/IamUserGroupAllOf.md` & `fastly-1.3.1/docs/IamUserGroupAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/IamUserGroupsApi.md` & `fastly-1.3.1/docs/IamUserGroupsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/IncludedWithWafActiveRuleItem.md` & `fastly-1.3.1/docs/IncludedWithWafActiveRuleItem.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/IncludedWithWafExclusionItem.md` & `fastly-1.3.1/docs/IncludedWithWafExclusionItem.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/IncludedWithWafFirewallVersionItem.md` & `fastly-1.3.1/docs/IncludedWithWafFirewallVersionItem.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/IncludedWithWafRuleItem.md` & `fastly-1.3.1/docs/IncludedWithWafRuleItem.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/InlineResponse2001.md` & `fastly-1.3.1/docs/InlineResponse2001.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/InlineResponse2002.md` & `fastly-1.3.1/docs/InlineResponse2002.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/InlineResponse2002Meta.md` & `fastly-1.3.1/docs/InlineResponse2002Meta.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/InlineResponse2003.md` & `fastly-1.3.1/docs/InlineResponse2003.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/InlineResponse2003Meta.md` & `fastly-1.3.1/docs/InlineResponse2003Meta.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Invitation.md` & `fastly-1.3.1/docs/Invitation.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/InvitationData.md` & `fastly-1.3.1/docs/InvitationData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/InvitationDataAttributes.md` & `fastly-1.3.1/docs/InvitationDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/InvitationResponse.md` & `fastly-1.3.1/docs/InvitationResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/InvitationResponseAllOf.md` & `fastly-1.3.1/docs/InvitationResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/InvitationResponseData.md` & `fastly-1.3.1/docs/InvitationResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/InvitationResponseDataAllOf.md` & `fastly-1.3.1/docs/InvitationResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/InvitationsApi.md` & `fastly-1.3.1/docs/InvitationsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/InvitationsResponse.md` & `fastly-1.3.1/docs/InvitationsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/InvitationsResponseAllOf.md` & `fastly-1.3.1/docs/InvitationsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingAddressAndPort.md` & `fastly-1.3.1/docs/LoggingAddressAndPort.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingAzureblob.md` & `fastly-1.3.1/docs/LoggingAzureblob.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingAzureblobAllOf.md` & `fastly-1.3.1/docs/LoggingAzureblobAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingAzureblobApi.md` & `fastly-1.3.1/docs/LoggingAzureblobApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingAzureblobResponse.md` & `fastly-1.3.1/docs/LoggingAzureblobResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingBigquery.md` & `fastly-1.3.1/docs/LoggingBigquery.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingBigqueryAllOf.md` & `fastly-1.3.1/docs/LoggingBigqueryAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingBigqueryApi.md` & `fastly-1.3.1/docs/LoggingBigqueryApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingBigqueryResponse.md` & `fastly-1.3.1/docs/LoggingBigqueryResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingCloudfiles.md` & `fastly-1.3.1/docs/LoggingCloudfiles.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingCloudfilesAllOf.md` & `fastly-1.3.1/docs/LoggingCloudfilesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingCloudfilesApi.md` & `fastly-1.3.1/docs/LoggingCloudfilesApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingCloudfilesResponse.md` & `fastly-1.3.1/docs/LoggingCloudfilesResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingCommon.md` & `fastly-1.3.1/docs/LoggingCommon.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingDatadog.md` & `fastly-1.3.1/docs/LoggingDatadog.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingDatadogAllOf.md` & `fastly-1.3.1/docs/LoggingDatadogAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingDatadogApi.md` & `fastly-1.3.1/docs/LoggingDatadogApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingDatadogResponse.md` & `fastly-1.3.1/docs/LoggingDatadogResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingDigitalocean.md` & `fastly-1.3.1/docs/LoggingDigitalocean.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingDigitaloceanAllOf.md` & `fastly-1.3.1/docs/LoggingDigitaloceanAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingDigitaloceanApi.md` & `fastly-1.3.1/docs/LoggingDigitaloceanApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingDigitaloceanResponse.md` & `fastly-1.3.1/docs/LoggingDigitaloceanResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingElasticsearch.md` & `fastly-1.3.1/docs/LoggingElasticsearch.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingElasticsearchAllOf.md` & `fastly-1.3.1/docs/LoggingElasticsearchAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingElasticsearchApi.md` & `fastly-1.3.1/docs/LoggingElasticsearchApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingElasticsearchResponse.md` & `fastly-1.3.1/docs/LoggingElasticsearchResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingFormatVersion.md` & `fastly-1.3.1/docs/LoggingFormatVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingFtp.md` & `fastly-1.3.1/docs/LoggingFtp.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingFtpAllOf.md` & `fastly-1.3.1/docs/LoggingFtpAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingFtpApi.md` & `fastly-1.3.1/docs/LoggingFtpApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingFtpResponse.md` & `fastly-1.3.1/docs/LoggingFtpResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingGcs.md` & `fastly-1.3.1/docs/LoggingGcs.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingGcsAllOf.md` & `fastly-1.3.1/docs/LoggingGcsAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingGcsApi.md` & `fastly-1.3.1/docs/LoggingGcsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingGcsCommon.md` & `fastly-1.3.1/docs/LoggingGcsCommon.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingGcsResponse.md` & `fastly-1.3.1/docs/LoggingGcsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingGenericCommon.md` & `fastly-1.3.1/docs/LoggingGenericCommon.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingGooglePubsub.md` & `fastly-1.3.1/docs/LoggingGooglePubsub.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingGooglePubsubAllOf.md` & `fastly-1.3.1/docs/LoggingGooglePubsubAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingGooglePubsubResponse.md` & `fastly-1.3.1/docs/LoggingGooglePubsubResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingHeroku.md` & `fastly-1.3.1/docs/LoggingHeroku.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingHerokuAllOf.md` & `fastly-1.3.1/docs/LoggingHerokuAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingHerokuApi.md` & `fastly-1.3.1/docs/LoggingHerokuApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingHerokuResponse.md` & `fastly-1.3.1/docs/LoggingHerokuResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingHoneycomb.md` & `fastly-1.3.1/docs/LoggingHoneycomb.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingHoneycombAllOf.md` & `fastly-1.3.1/docs/LoggingHoneycombAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingHoneycombApi.md` & `fastly-1.3.1/docs/LoggingHoneycombApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingHoneycombResponse.md` & `fastly-1.3.1/docs/LoggingHoneycombResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingHttps.md` & `fastly-1.3.1/docs/LoggingHttps.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingHttpsAllOf.md` & `fastly-1.3.1/docs/LoggingHttpsAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingHttpsApi.md` & `fastly-1.3.1/docs/LoggingHttpsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingHttpsResponse.md` & `fastly-1.3.1/docs/LoggingHttpsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingKafka.md` & `fastly-1.3.1/docs/LoggingKafka.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingKafkaAllOf.md` & `fastly-1.3.1/docs/LoggingKafkaAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingKafkaApi.md` & `fastly-1.3.1/docs/LoggingKafkaApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingKafkaResponse.md` & `fastly-1.3.1/docs/LoggingKafkaResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingKinesis.md` & `fastly-1.3.1/docs/LoggingKinesis.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingKinesisApi.md` & `fastly-1.3.1/docs/LoggingKinesisApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingKinesisResponse.md` & `fastly-1.3.1/docs/LoggingKinesisResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingLogentries.md` & `fastly-1.3.1/docs/LoggingLogentries.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingLogentriesAllOf.md` & `fastly-1.3.1/docs/LoggingLogentriesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingLogentriesApi.md` & `fastly-1.3.1/docs/LoggingLogentriesApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingLogentriesResponse.md` & `fastly-1.3.1/docs/LoggingLogentriesResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingLoggly.md` & `fastly-1.3.1/docs/LoggingLoggly.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingLogglyAllOf.md` & `fastly-1.3.1/docs/LoggingLogglyAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingLogglyApi.md` & `fastly-1.3.1/docs/LoggingLogglyApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingLogglyResponse.md` & `fastly-1.3.1/docs/LoggingLogglyResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingLogshuttle.md` & `fastly-1.3.1/docs/LoggingLogshuttle.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingLogshuttleAllOf.md` & `fastly-1.3.1/docs/LoggingLogshuttleAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingLogshuttleApi.md` & `fastly-1.3.1/docs/LoggingLogshuttleApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingLogshuttleResponse.md` & `fastly-1.3.1/docs/LoggingLogshuttleResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingNewrelic.md` & `fastly-1.3.1/docs/LoggingNewrelic.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingNewrelicAllOf.md` & `fastly-1.3.1/docs/LoggingNewrelicAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingNewrelicApi.md` & `fastly-1.3.1/docs/LoggingNewrelicApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingNewrelicResponse.md` & `fastly-1.3.1/docs/LoggingNewrelicResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingOpenstack.md` & `fastly-1.3.1/docs/LoggingOpenstack.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingOpenstackAllOf.md` & `fastly-1.3.1/docs/LoggingOpenstackAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingOpenstackApi.md` & `fastly-1.3.1/docs/LoggingOpenstackApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingOpenstackResponse.md` & `fastly-1.3.1/docs/LoggingOpenstackResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingPapertrail.md` & `fastly-1.3.1/docs/LoggingPapertrail.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingPapertrailApi.md` & `fastly-1.3.1/docs/LoggingPapertrailApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingPapertrailResponse.md` & `fastly-1.3.1/docs/LoggingPapertrailResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingPlacement.md` & `fastly-1.3.1/docs/LoggingPlacement.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingPubsubApi.md` & `fastly-1.3.1/docs/LoggingPubsubApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingRequestCapsCommon.md` & `fastly-1.3.1/docs/LoggingRequestCapsCommon.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingS3.md` & `fastly-1.3.1/docs/LoggingS3.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingS3AllOf.md` & `fastly-1.3.1/docs/LoggingS3AllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingS3Api.md` & `fastly-1.3.1/docs/LoggingS3Api.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingS3Response.md` & `fastly-1.3.1/docs/LoggingS3Response.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingScalyr.md` & `fastly-1.3.1/docs/LoggingScalyr.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingScalyrAllOf.md` & `fastly-1.3.1/docs/LoggingScalyrAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingScalyrApi.md` & `fastly-1.3.1/docs/LoggingScalyrApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingScalyrResponse.md` & `fastly-1.3.1/docs/LoggingScalyrResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingSftp.md` & `fastly-1.3.1/docs/LoggingSftp.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingSftpAllOf.md` & `fastly-1.3.1/docs/LoggingSftpAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingSftpApi.md` & `fastly-1.3.1/docs/LoggingSftpApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingSftpResponse.md` & `fastly-1.3.1/docs/LoggingSftpResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingSplunk.md` & `fastly-1.3.1/docs/LoggingSplunk.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingSplunkAllOf.md` & `fastly-1.3.1/docs/LoggingSplunkAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingSplunkApi.md` & `fastly-1.3.1/docs/LoggingSplunkApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingSplunkResponse.md` & `fastly-1.3.1/docs/LoggingSplunkResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingSumologic.md` & `fastly-1.3.1/docs/LoggingSumologic.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingSumologicAllOf.md` & `fastly-1.3.1/docs/LoggingSumologicAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingSumologicApi.md` & `fastly-1.3.1/docs/LoggingSumologicApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingSumologicResponse.md` & `fastly-1.3.1/docs/LoggingSumologicResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingSyslog.md` & `fastly-1.3.1/docs/LoggingSyslog.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingSyslogAllOf.md` & `fastly-1.3.1/docs/LoggingSyslogAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingSyslogApi.md` & `fastly-1.3.1/docs/LoggingSyslogApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingSyslogResponse.md` & `fastly-1.3.1/docs/LoggingSyslogResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/LoggingTlsCommon.md` & `fastly-1.3.1/docs/LoggingTlsCommon.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/MutualAuthentication.md` & `fastly-1.3.1/docs/MutualAuthentication.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/MutualAuthenticationApi.md` & `fastly-1.3.1/docs/MutualAuthenticationApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/MutualAuthenticationData.md` & `fastly-1.3.1/docs/MutualAuthenticationData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/MutualAuthenticationDataAttributes.md` & `fastly-1.3.1/docs/MutualAuthenticationDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/MutualAuthenticationResponse.md` & `fastly-1.3.1/docs/MutualAuthenticationResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/MutualAuthenticationResponseAttributes.md` & `fastly-1.3.1/docs/MutualAuthenticationResponseAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/MutualAuthenticationResponseAttributesAllOf.md` & `fastly-1.3.1/docs/MutualAuthenticationResponseAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/MutualAuthenticationResponseData.md` & `fastly-1.3.1/docs/MutualAuthenticationResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/MutualAuthenticationResponseDataAllOf.md` & `fastly-1.3.1/docs/MutualAuthenticationResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/MutualAuthenticationsResponse.md` & `fastly-1.3.1/docs/MutualAuthenticationsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/MutualAuthenticationsResponseAllOf.md` & `fastly-1.3.1/docs/MutualAuthenticationsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ObjectStoreApi.md` & `fastly-1.3.1/docs/ObjectStoreApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ObjectStoreItemApi.md` & `fastly-1.3.1/docs/ObjectStoreItemApi.md`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 | Status code | Description | Response headers |
 |-------------|-------------|------------------|
 **200** | OK |  -  |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
 # **get_value_for_key**
-> file_type get_value_for_key(store_id, key_name)
+> str get_value_for_key(store_id, key_name)
 
 Get the value of an object store item
 
 Get the value associated with a key.
 
 ### Example
 
@@ -246,15 +246,15 @@
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **store_id** | **str**|  |
  **key_name** | **str**|  |
 
 ### Return type
 
-**file_type**
+**str**
 
 ### Authorization
 
 [token](../README.md#token)
 
 ### HTTP request headers
 
@@ -267,15 +267,15 @@
 | Status code | Description | Response headers |
 |-------------|-------------|------------------|
 **200** | OK |  * generation - A unique, non-serial 32-bit integer that can be used for testing against a specific object store value. <br>  * metadata - An arbitrary data field which can contain up to 2000B of data <br>  |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
 # **set_value_for_key**
-> file_type set_value_for_key(store_id, key_name)
+> str set_value_for_key(store_id, key_name)
 
 Insert an item into an object store
 
 Set a new value for a new or existing key in an object store.
 
 ### Example
 
@@ -312,15 +312,15 @@
     if_generation_match = 1 # int |  (optional)
     time_to_live_sec = 1 # int |  (optional)
     metadata = "metadata_example" # str |  (optional)
     add = True # bool |  (optional)
     append = True # bool |  (optional)
     prepend = True # bool |  (optional)
     background_fetch = True # bool |  (optional)
-    body = open('/path/to/file', 'rb') # file_type |  (optional)
+    body = 'YQ==' # str |  (optional)
 
     # example passing only required values which don't have defaults set
     try:
         # Insert an item into an object store
         api_response = api_instance.set_value_for_key(store_id, key_name)
         pprint(api_response)
     except fastly.ApiException as e:
@@ -346,19 +346,19 @@
  **if_generation_match** | **int**|  | [optional]
  **time_to_live_sec** | **int**|  | [optional]
  **metadata** | **str**|  | [optional]
  **add** | **bool**|  | [optional]
  **append** | **bool**|  | [optional]
  **prepend** | **bool**|  | [optional]
  **background_fetch** | **bool**|  | [optional]
- **body** | **file_type**|  | [optional]
+ **body** | **str**|  | [optional]
 
 ### Return type
 
-**file_type**
+**str**
 
 ### Authorization
 
 [token](../README.md#token)
 
 ### HTTP request headers
```

### Comparing `fastly-1.3.0/docs/Package.md` & `fastly-1.3.1/docs/Package.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/PackageApi.md` & `fastly-1.3.1/docs/PackageApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/PackageMetadata.md` & `fastly-1.3.1/docs/PackageMetadata.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/PackageResponse.md` & `fastly-1.3.1/docs/PackageResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/PackageResponseAllOf.md` & `fastly-1.3.1/docs/PackageResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Pagination.md` & `fastly-1.3.1/docs/Pagination.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/PaginationLinks.md` & `fastly-1.3.1/docs/PaginationLinks.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/PaginationMeta.md` & `fastly-1.3.1/docs/PaginationMeta.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Permission.md` & `fastly-1.3.1/docs/Permission.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Pool.md` & `fastly-1.3.1/docs/Pool.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/PoolAllOf.md` & `fastly-1.3.1/docs/PoolAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/PoolApi.md` & `fastly-1.3.1/docs/PoolApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/PoolResponse.md` & `fastly-1.3.1/docs/PoolResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Pop.md` & `fastly-1.3.1/docs/Pop.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/PopApi.md` & `fastly-1.3.1/docs/PopApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/PopCoordinates.md` & `fastly-1.3.1/docs/PopCoordinates.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/PublicIpList.md` & `fastly-1.3.1/docs/PublicIpList.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/PublicIpListApi.md` & `fastly-1.3.1/docs/PublicIpListApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/PublishApi.md` & `fastly-1.3.1/docs/PublishApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/PublishItem.md` & `fastly-1.3.1/docs/PublishItem.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/PublishItemFormats.md` & `fastly-1.3.1/docs/PublishItemFormats.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/PublishRequest.md` & `fastly-1.3.1/docs/PublishRequest.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/PurgeApi.md` & `fastly-1.3.1/docs/PurgeApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/PurgeKeys.md` & `fastly-1.3.1/docs/PurgeKeys.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/PurgeResponse.md` & `fastly-1.3.1/docs/PurgeResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RateLimiter.md` & `fastly-1.3.1/docs/RateLimiter.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RateLimiterApi.md` & `fastly-1.3.1/docs/RateLimiterApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RateLimiterResponse.md` & `fastly-1.3.1/docs/RateLimiterResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RateLimiterResponse1.md` & `fastly-1.3.1/docs/RateLimiterResponse1.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RateLimiterResponseAllOf.md` & `fastly-1.3.1/docs/RateLimiterResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Realtime.md` & `fastly-1.3.1/docs/Realtime.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RealtimeApi.md` & `fastly-1.3.1/docs/RealtimeApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RealtimeEntry.md` & `fastly-1.3.1/docs/RealtimeEntry.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RealtimeMeasurements.md` & `fastly-1.3.1/docs/RealtimeMeasurements.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipCommonName.md` & `fastly-1.3.1/docs/RelationshipCommonName.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipCustomer.md` & `fastly-1.3.1/docs/RelationshipCustomer.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipCustomerCustomer.md` & `fastly-1.3.1/docs/RelationshipCustomerCustomer.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipMemberCustomer.md` & `fastly-1.3.1/docs/RelationshipMemberCustomer.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipMemberMutualAuthentication.md` & `fastly-1.3.1/docs/RelationshipMemberMutualAuthentication.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipMemberService.md` & `fastly-1.3.1/docs/RelationshipMemberService.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipMemberServiceInvitation.md` & `fastly-1.3.1/docs/RelationshipMemberServiceInvitation.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipMemberTlsActivation.md` & `fastly-1.3.1/docs/RelationshipMemberTlsActivation.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipMemberTlsBulkCertificate.md` & `fastly-1.3.1/docs/RelationshipMemberTlsBulkCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipMemberTlsCertificate.md` & `fastly-1.3.1/docs/RelationshipMemberTlsCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipMemberTlsConfiguration.md` & `fastly-1.3.1/docs/RelationshipMemberTlsConfiguration.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipMemberTlsDnsRecord.md` & `fastly-1.3.1/docs/RelationshipMemberTlsDnsRecord.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipMemberTlsDomain.md` & `fastly-1.3.1/docs/RelationshipMemberTlsDomain.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipMemberTlsPrivateKey.md` & `fastly-1.3.1/docs/RelationshipMemberTlsPrivateKey.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipMemberTlsSubscription.md` & `fastly-1.3.1/docs/RelationshipMemberTlsSubscription.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipMemberWafActiveRule.md` & `fastly-1.3.1/docs/RelationshipMemberWafActiveRule.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipMemberWafFirewall.md` & `fastly-1.3.1/docs/RelationshipMemberWafFirewall.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipMemberWafFirewallVersion.md` & `fastly-1.3.1/docs/RelationshipMemberWafFirewallVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipMemberWafRule.md` & `fastly-1.3.1/docs/RelationshipMemberWafRule.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipMemberWafRuleRevision.md` & `fastly-1.3.1/docs/RelationshipMemberWafRuleRevision.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipMemberWafTag.md` & `fastly-1.3.1/docs/RelationshipMemberWafTag.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipMutualAuthentication.md` & `fastly-1.3.1/docs/RelationshipMutualAuthentication.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipMutualAuthenticationMutualAuthentication.md` & `fastly-1.3.1/docs/RelationshipMutualAuthenticationMutualAuthentication.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipMutualAuthentications.md` & `fastly-1.3.1/docs/RelationshipMutualAuthentications.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipMutualAuthenticationsMutualAuthentications.md` & `fastly-1.3.1/docs/RelationshipMutualAuthenticationsMutualAuthentications.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipService.md` & `fastly-1.3.1/docs/RelationshipService.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipServiceInvitations.md` & `fastly-1.3.1/docs/RelationshipServiceInvitations.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipServiceInvitationsCreate.md` & `fastly-1.3.1/docs/RelationshipServiceInvitationsCreate.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipServiceInvitationsCreateServiceInvitations.md` & `fastly-1.3.1/docs/RelationshipServiceInvitationsCreateServiceInvitations.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipServiceInvitationsServiceInvitations.md` & `fastly-1.3.1/docs/RelationshipServiceInvitationsServiceInvitations.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipServices.md` & `fastly-1.3.1/docs/RelationshipServices.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipServicesServices.md` & `fastly-1.3.1/docs/RelationshipServicesServices.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsActivation.md` & `fastly-1.3.1/docs/RelationshipTlsActivation.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsActivationTlsActivation.md` & `fastly-1.3.1/docs/RelationshipTlsActivationTlsActivation.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsActivations.md` & `fastly-1.3.1/docs/RelationshipTlsActivations.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsBulkCertificate.md` & `fastly-1.3.1/docs/RelationshipTlsBulkCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsBulkCertificateTlsBulkCertificate.md` & `fastly-1.3.1/docs/RelationshipTlsBulkCertificateTlsBulkCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsBulkCertificates.md` & `fastly-1.3.1/docs/RelationshipTlsBulkCertificates.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsCertificate.md` & `fastly-1.3.1/docs/RelationshipTlsCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsCertificateTlsCertificate.md` & `fastly-1.3.1/docs/RelationshipTlsCertificateTlsCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsCertificates.md` & `fastly-1.3.1/docs/RelationshipTlsCertificates.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsCertificatesTlsCertificates.md` & `fastly-1.3.1/docs/RelationshipTlsCertificatesTlsCertificates.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsConfiguration.md` & `fastly-1.3.1/docs/RelationshipTlsConfiguration.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsConfigurationTlsConfiguration.md` & `fastly-1.3.1/docs/RelationshipTlsConfigurationTlsConfiguration.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsConfigurations.md` & `fastly-1.3.1/docs/RelationshipTlsConfigurations.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsConfigurationsTlsConfigurations.md` & `fastly-1.3.1/docs/RelationshipTlsConfigurationsTlsConfigurations.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsDnsRecord.md` & `fastly-1.3.1/docs/RelationshipTlsDnsRecord.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsDnsRecordDnsRecord.md` & `fastly-1.3.1/docs/RelationshipTlsDnsRecordDnsRecord.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsDnsRecords.md` & `fastly-1.3.1/docs/RelationshipTlsDnsRecords.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsDomain.md` & `fastly-1.3.1/docs/RelationshipTlsDomain.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsDomainTlsDomain.md` & `fastly-1.3.1/docs/RelationshipTlsDomainTlsDomain.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsDomains.md` & `fastly-1.3.1/docs/RelationshipTlsDomains.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsDomainsTlsDomains.md` & `fastly-1.3.1/docs/RelationshipTlsDomainsTlsDomains.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsPrivateKey.md` & `fastly-1.3.1/docs/RelationshipTlsPrivateKey.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsPrivateKeyTlsPrivateKey.md` & `fastly-1.3.1/docs/RelationshipTlsPrivateKeyTlsPrivateKey.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsPrivateKeys.md` & `fastly-1.3.1/docs/RelationshipTlsPrivateKeys.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsPrivateKeysTlsPrivateKeys.md` & `fastly-1.3.1/docs/RelationshipTlsPrivateKeysTlsPrivateKeys.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsSubscription.md` & `fastly-1.3.1/docs/RelationshipTlsSubscription.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsSubscriptionTlsSubscription.md` & `fastly-1.3.1/docs/RelationshipTlsSubscriptionTlsSubscription.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipTlsSubscriptions.md` & `fastly-1.3.1/docs/RelationshipTlsSubscriptions.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipUser.md` & `fastly-1.3.1/docs/RelationshipUser.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipUserUser.md` & `fastly-1.3.1/docs/RelationshipUserUser.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipWafActiveRules.md` & `fastly-1.3.1/docs/RelationshipWafActiveRules.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipWafActiveRulesWafActiveRules.md` & `fastly-1.3.1/docs/RelationshipWafActiveRulesWafActiveRules.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipWafFirewall.md` & `fastly-1.3.1/docs/RelationshipWafFirewall.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipWafFirewallVersion.md` & `fastly-1.3.1/docs/RelationshipWafFirewallVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipWafFirewallVersionWafFirewallVersion.md` & `fastly-1.3.1/docs/RelationshipWafFirewallVersionWafFirewallVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipWafFirewallVersions.md` & `fastly-1.3.1/docs/RelationshipWafFirewallVersions.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipWafFirewallWafFirewall.md` & `fastly-1.3.1/docs/RelationshipWafFirewallWafFirewall.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipWafRule.md` & `fastly-1.3.1/docs/RelationshipWafRule.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipWafRuleRevision.md` & `fastly-1.3.1/docs/RelationshipWafRuleRevision.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipWafRuleRevisionWafRuleRevisions.md` & `fastly-1.3.1/docs/RelationshipWafRuleRevisionWafRuleRevisions.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipWafRuleRevisions.md` & `fastly-1.3.1/docs/RelationshipWafRuleRevisions.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipWafRuleWafRule.md` & `fastly-1.3.1/docs/RelationshipWafRuleWafRule.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipWafRules.md` & `fastly-1.3.1/docs/RelationshipWafRules.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipWafTags.md` & `fastly-1.3.1/docs/RelationshipWafTags.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipWafTagsWafTags.md` & `fastly-1.3.1/docs/RelationshipWafTagsWafTags.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipsForInvitation.md` & `fastly-1.3.1/docs/RelationshipsForInvitation.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipsForMutualAuthentication.md` & `fastly-1.3.1/docs/RelationshipsForMutualAuthentication.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipsForStar.md` & `fastly-1.3.1/docs/RelationshipsForStar.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipsForTlsActivation.md` & `fastly-1.3.1/docs/RelationshipsForTlsActivation.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipsForTlsBulkCertificate.md` & `fastly-1.3.1/docs/RelationshipsForTlsBulkCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipsForTlsConfiguration.md` & `fastly-1.3.1/docs/RelationshipsForTlsConfiguration.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipsForTlsCsr.md` & `fastly-1.3.1/docs/TlsPrivateKeyResponse.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# RelationshipsForTlsCsr
+# TlsPrivateKeyResponse
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**tls_private_key** | [**RelationshipTlsPrivateKeyTlsPrivateKey**](RelationshipTlsPrivateKeyTlsPrivateKey.md) |  | [optional] 
+**data** | [**TlsPrivateKeyResponseData**](TlsPrivateKeyResponseData.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/RelationshipsForTlsDomain.md` & `fastly-1.3.1/docs/RelationshipsForTlsDomain.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipsForTlsPrivateKey.md` & `fastly-1.3.1/docs/RelationshipsForTlsPrivateKey.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipsForTlsSubscription.md` & `fastly-1.3.1/docs/RelationshipsForTlsSubscription.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipsForWafActiveRule.md` & `fastly-1.3.1/docs/RelationshipsForWafActiveRule.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipsForWafExclusion.md` & `fastly-1.3.1/docs/RelationshipsForWafExclusion.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipsForWafFirewallVersion.md` & `fastly-1.3.1/docs/RelationshipsForWafFirewallVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RelationshipsForWafRule.md` & `fastly-1.3.1/docs/RelationshipsForWafRule.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RequestSettings.md` & `fastly-1.3.1/docs/RequestSettings.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RequestSettingsApi.md` & `fastly-1.3.1/docs/RequestSettingsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RequestSettingsResponse.md` & `fastly-1.3.1/docs/RequestSettingsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Resource.md` & `fastly-1.3.1/docs/Resource.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ResourceApi.md` & `fastly-1.3.1/docs/ResourceApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ResourceResponse.md` & `fastly-1.3.1/docs/ResourceResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ResourceResponseAllOf.md` & `fastly-1.3.1/docs/ResourceResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ResponseObject.md` & `fastly-1.3.1/docs/ResponseObject.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ResponseObjectApi.md` & `fastly-1.3.1/docs/ResponseObjectApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ResponseObjectResponse.md` & `fastly-1.3.1/docs/ResponseObjectResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Results.md` & `fastly-1.3.1/docs/Results.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/RoleUser.md` & `fastly-1.3.1/docs/RoleUser.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/SchemasContactResponse.md` & `fastly-1.3.1/docs/SchemasContactResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/SchemasSnippetResponse.md` & `fastly-1.3.1/docs/SchemasSnippetResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/SchemasUserResponse.md` & `fastly-1.3.1/docs/SchemasUserResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/SchemasVclResponse.md` & `fastly-1.3.1/docs/SchemasVclResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/SchemasVersion.md` & `fastly-1.3.1/docs/SchemasVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/SchemasVersionResponse.md` & `fastly-1.3.1/docs/SchemasVersionResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/SchemasWafFirewallVersion.md` & `fastly-1.3.1/docs/SchemasWafFirewallVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/SchemasWafFirewallVersionData.md` & `fastly-1.3.1/docs/SchemasWafFirewallVersionData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Server.md` & `fastly-1.3.1/docs/Server.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServerApi.md` & `fastly-1.3.1/docs/ServerApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServerResponse.md` & `fastly-1.3.1/docs/ServerResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServerResponseAllOf.md` & `fastly-1.3.1/docs/ServerResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Service.md` & `fastly-1.3.1/docs/Service.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceApi.md` & `fastly-1.3.1/docs/ServiceApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceAuthorization.md` & `fastly-1.3.1/docs/ServiceAuthorization.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceAuthorizationData.md` & `fastly-1.3.1/docs/ServiceAuthorizationData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceAuthorizationDataAttributes.md` & `fastly-1.3.1/docs/ServiceAuthorizationDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceAuthorizationDataRelationships.md` & `fastly-1.3.1/docs/ServiceAuthorizationDataRelationships.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceAuthorizationDataRelationshipsUser.md` & `fastly-1.3.1/docs/ServiceAuthorizationDataRelationshipsUser.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceAuthorizationDataRelationshipsUserData.md` & `fastly-1.3.1/docs/ServiceAuthorizationDataRelationshipsUserData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceAuthorizationResponse.md` & `fastly-1.3.1/docs/ServiceAuthorizationResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceAuthorizationResponseData.md` & `fastly-1.3.1/docs/ServiceAuthorizationResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceAuthorizationResponseDataAllOf.md` & `fastly-1.3.1/docs/ServiceAuthorizationResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceAuthorizationsApi.md` & `fastly-1.3.1/docs/ServiceAuthorizationsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceAuthorizationsResponse.md` & `fastly-1.3.1/docs/ServiceAuthorizationsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceAuthorizationsResponseAllOf.md` & `fastly-1.3.1/docs/ServiceAuthorizationsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceCreate.md` & `fastly-1.3.1/docs/ServiceCreate.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceCreateAllOf.md` & `fastly-1.3.1/docs/ServiceCreateAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceDetail.md` & `fastly-1.3.1/docs/ServiceDetail.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceDetailAllOf.md` & `fastly-1.3.1/docs/ServiceDetailAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceIdAndVersion.md` & `fastly-1.3.1/docs/ServiceIdAndVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceInvitation.md` & `fastly-1.3.1/docs/ServiceInvitation.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceInvitationData.md` & `fastly-1.3.1/docs/ServiceInvitationData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceInvitationDataAttributes.md` & `fastly-1.3.1/docs/ServiceInvitationDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceInvitationDataRelationships.md` & `fastly-1.3.1/docs/ServiceInvitationDataRelationships.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceInvitationResponse.md` & `fastly-1.3.1/docs/ServiceInvitationResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceInvitationResponseAllOf.md` & `fastly-1.3.1/docs/ServiceInvitationResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceInvitationResponseAllOfData.md` & `fastly-1.3.1/docs/ServiceInvitationResponseAllOfData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceListResponse.md` & `fastly-1.3.1/docs/ServiceListResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceListResponseAllOf.md` & `fastly-1.3.1/docs/ServiceListResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceResponse.md` & `fastly-1.3.1/docs/ServiceResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceResponseAllOf.md` & `fastly-1.3.1/docs/ServiceResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceVersionDetail.md` & `fastly-1.3.1/docs/ServiceVersionDetail.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ServiceVersionDetailOrNull.md` & `fastly-1.3.1/docs/ServiceVersionDetailOrNull.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Settings.md` & `fastly-1.3.1/docs/Settings.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/SettingsApi.md` & `fastly-1.3.1/docs/SettingsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/SettingsResponse.md` & `fastly-1.3.1/docs/SettingsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Snippet.md` & `fastly-1.3.1/docs/Snippet.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/SnippetApi.md` & `fastly-1.3.1/docs/SnippetApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/SnippetResponse.md` & `fastly-1.3.1/docs/SnippetResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/SnippetResponseAllOf.md` & `fastly-1.3.1/docs/VersionResponseAllOf.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# SnippetResponseAllOf
+# VersionResponseAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**id** | **str** |  | [optional] [readonly] 
+**service_id** | **str** |  | [optional] [readonly] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/StarApi.md` & `fastly-1.3.1/docs/StarApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/StarData.md` & `fastly-1.3.1/docs/StarData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/StarResponse.md` & `fastly-1.3.1/docs/StarResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/StarResponseAllOf.md` & `fastly-1.3.1/docs/StarResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Stats.md` & `fastly-1.3.1/docs/Stats.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/StatsApi.md` & `fastly-1.3.1/docs/StatsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Store.md` & `fastly-1.3.1/docs/Store.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/StoreResponse.md` & `fastly-1.3.1/docs/StoreResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Timestamps.md` & `fastly-1.3.1/docs/Timestamps.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TimestampsNoDelete.md` & `fastly-1.3.1/docs/TimestampsNoDelete.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsActivation.md` & `fastly-1.3.1/docs/TlsActivation.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsActivationData.md` & `fastly-1.3.1/docs/TlsActivationData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsActivationResponse.md` & `fastly-1.3.1/docs/TlsActivationResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsActivationResponseData.md` & `fastly-1.3.1/docs/TlsActivationResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsActivationResponseDataAllOf.md` & `fastly-1.3.1/docs/TlsActivationResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsActivationsApi.md` & `fastly-1.3.1/docs/TlsActivationsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsActivationsResponse.md` & `fastly-1.3.1/docs/TlsActivationsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsActivationsResponseAllOf.md` & `fastly-1.3.1/docs/TlsActivationsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsBulkCertificate.md` & `fastly-1.3.1/docs/TlsBulkCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsBulkCertificateData.md` & `fastly-1.3.1/docs/TlsBulkCertificateData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsBulkCertificateDataAttributes.md` & `fastly-1.3.1/docs/TlsBulkCertificateDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsBulkCertificateResponse.md` & `fastly-1.3.1/docs/TlsBulkCertificateResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsBulkCertificateResponseAttributes.md` & `fastly-1.3.1/docs/TlsBulkCertificateResponseAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsBulkCertificateResponseAttributesAllOf.md` & `fastly-1.3.1/docs/TlsBulkCertificateResponseAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsBulkCertificateResponseData.md` & `fastly-1.3.1/docs/TlsBulkCertificateResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsBulkCertificateResponseDataAllOf.md` & `fastly-1.3.1/docs/TlsBulkCertificateResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsBulkCertificatesApi.md` & `fastly-1.3.1/docs/TlsBulkCertificatesApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsBulkCertificatesResponse.md` & `fastly-1.3.1/docs/TlsBulkCertificatesResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsBulkCertificatesResponseAllOf.md` & `fastly-1.3.1/docs/TlsBulkCertificatesResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsCertificate.md` & `fastly-1.3.1/docs/TlsCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsCertificateData.md` & `fastly-1.3.1/docs/TlsCertificateData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsCertificateDataAttributes.md` & `fastly-1.3.1/docs/TlsCertificateDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsCertificateResponse.md` & `fastly-1.3.1/docs/TlsCertificateResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsCertificateResponseAttributes.md` & `fastly-1.3.1/docs/TlsCertificateResponseAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsCertificateResponseAttributesAllOf.md` & `fastly-1.3.1/docs/TlsCertificateResponseAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsCertificateResponseData.md` & `fastly-1.3.1/docs/TlsCertificateResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsCertificateResponseDataAllOf.md` & `fastly-1.3.1/docs/TlsCertificateResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsCertificatesApi.md` & `fastly-1.3.1/docs/TlsCertificatesApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsCertificatesResponse.md` & `fastly-1.3.1/docs/TlsCertificatesResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsCertificatesResponseAllOf.md` & `fastly-1.3.1/docs/TlsCertificatesResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsCommon.md` & `fastly-1.3.1/docs/TlsCommon.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsConfiguration.md` & `fastly-1.3.1/docs/TlsConfiguration.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsConfigurationData.md` & `fastly-1.3.1/docs/TlsConfigurationData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsConfigurationDataAttributes.md` & `fastly-1.3.1/docs/TlsConfigurationDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsConfigurationResponse.md` & `fastly-1.3.1/docs/TlsConfigurationResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsConfigurationResponseAttributes.md` & `fastly-1.3.1/docs/TlsConfigurationResponseAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsConfigurationResponseAttributesAllOf.md` & `fastly-1.3.1/docs/TlsConfigurationResponseAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsConfigurationResponseData.md` & `fastly-1.3.1/docs/TlsConfigurationResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsConfigurationResponseDataAllOf.md` & `fastly-1.3.1/docs/TlsConfigurationResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsConfigurationsApi.md` & `fastly-1.3.1/docs/TlsConfigurationsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsConfigurationsResponse.md` & `fastly-1.3.1/docs/TlsConfigurationsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsConfigurationsResponseAllOf.md` & `fastly-1.3.1/docs/TlsConfigurationsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsCsr.md` & `fastly-1.3.1/docs/WafFirewall.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# TlsCsr
+# WafFirewall
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**TlsCsrData**](TlsCsrData.md) |  | [optional] 
+**data** | [**WafFirewallData**](WafFirewallData.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/TlsCsrData.md` & `fastly-1.3.1/docs/WafExclusionData.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# TlsCsrData
+# WafExclusionData
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**type** | [**TypeTlsCsr**](TypeTlsCsr.md) |  | [optional] 
-**attributes** | [**TlsCsrDataAttributes**](TlsCsrDataAttributes.md) |  | [optional] 
-**relationships** | [**RelationshipsForTlsCsr**](RelationshipsForTlsCsr.md) |  | [optional] 
+**type** | [**TypeWafExclusion**](TypeWafExclusion.md) |  | [optional] 
+**attributes** | [**WafExclusionDataAttributes**](WafExclusionDataAttributes.md) |  | [optional] 
+**relationships** | [**RelationshipsForWafExclusion**](RelationshipsForWafExclusion.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/TlsCsrResponse.md` & `fastly-1.3.1/docs/WafExclusionResponse.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# TlsCsrResponse
+# WafExclusionResponse
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**TlsCsrResponseData**](TlsCsrResponseData.md) |  | [optional] 
+**data** | [**WafExclusionResponseData**](WafExclusionResponseData.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/TlsCsrResponseAttributes.md` & `fastly-1.3.1/docs/TlsPrivateKeyDataAttributes.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-# TlsCsrResponseAttributes
+# TlsPrivateKeyDataAttributes
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**content** | **str** | The PEM encoded CSR. | [optional] 
+**name** | **str** | A customizable name for your private key. Optional. | [optional] 
+**key** | **str** | The contents of the private key. Must be a PEM-formatted key. Not returned in response body. Required. | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/TlsCsrResponseData.md` & `fastly-1.3.1/docs/WafRuleResponseData.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# TlsCsrResponseData
+# WafRuleResponseData
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**id** | **str** |  | [optional] 
-**type** | [**TypeTlsCsr**](TypeTlsCsr.md) |  | [optional] 
-**attributes** | [**TlsCsrResponseAttributes**](TlsCsrResponseAttributes.md) |  | [optional] 
-**relationships** | [**RelationshipsForTlsCsr**](RelationshipsForTlsCsr.md) |  | [optional] 
+**type** | [**TypeWafRule**](TypeWafRule.md) |  | [optional] 
+**id** | **str** |  | [optional] [readonly] 
+**attributes** | [**WafRuleAttributes**](WafRuleAttributes.md) |  | [optional] 
+**relationships** | [**RelationshipsForWafRule**](RelationshipsForWafRule.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/TlsDnsRecord.md` & `fastly-1.3.1/docs/TlsDnsRecord.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsDomainData.md` & `fastly-1.3.1/docs/TlsDomainData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsDomainsApi.md` & `fastly-1.3.1/docs/TlsDomainsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsDomainsResponse.md` & `fastly-1.3.1/docs/TlsDomainsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsDomainsResponseAllOf.md` & `fastly-1.3.1/docs/TlsDomainsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsPrivateKey.md` & `fastly-1.3.1/docs/TlsPrivateKey.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsPrivateKeyData.md` & `fastly-1.3.1/docs/TlsPrivateKeyData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsPrivateKeyDataAttributes.md` & `fastly-1.3.1/docs/WafActiveRuleResponseDataAttributesAllOf.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# TlsPrivateKeyDataAttributes
+# WafActiveRuleResponseDataAttributesAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**name** | **str** | A customizable name for your private key. Optional. | [optional] 
-**key** | **str** | The contents of the private key. Must be a PEM-formatted key. Not returned in response body. Required. | [optional] 
+**latest_revision** | **int** | The latest rule revision number that is available for the associated rule revision. | [optional] [readonly] 
+**outdated** | **bool** | Indicates if the associated rule revision is up to date or not. | [optional] [readonly] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/TlsPrivateKeyResponse.md` & `fastly-1.3.1/docs/TlsSubscriptionResponse.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# TlsPrivateKeyResponse
+# TlsSubscriptionResponse
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**TlsPrivateKeyResponseData**](TlsPrivateKeyResponseData.md) |  | [optional] 
+**data** | [**TlsSubscriptionResponseData**](TlsSubscriptionResponseData.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/TlsPrivateKeyResponseAttributes.md` & `fastly-1.3.1/docs/TlsPrivateKeyResponseAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsPrivateKeyResponseAttributesAllOf.md` & `fastly-1.3.1/docs/TlsPrivateKeyResponseAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsPrivateKeyResponseData.md` & `fastly-1.3.1/docs/TlsPrivateKeyResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsPrivateKeysApi.md` & `fastly-1.3.1/docs/TlsPrivateKeysApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsPrivateKeysResponse.md` & `fastly-1.3.1/docs/TlsPrivateKeysResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsPrivateKeysResponseAllOf.md` & `fastly-1.3.1/docs/TlsPrivateKeysResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsSubscription.md` & `fastly-1.3.1/docs/TlsSubscription.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsSubscriptionData.md` & `fastly-1.3.1/docs/TlsSubscriptionData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsSubscriptionDataAttributes.md` & `fastly-1.3.1/docs/TlsSubscriptionDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsSubscriptionResponse.md` & `fastly-1.3.1/docs/TlsSubscriptionsResponseAllOf.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# TlsSubscriptionResponse
+# TlsSubscriptionsResponseAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**TlsSubscriptionResponseData**](TlsSubscriptionResponseData.md) |  | [optional] 
+**data** | [**[TlsSubscriptionResponse]**](TlsSubscriptionResponse.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/TlsSubscriptionResponseAttributes.md` & `fastly-1.3.1/docs/TlsSubscriptionResponseAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsSubscriptionResponseAttributesAllOf.md` & `fastly-1.3.1/docs/TlsSubscriptionResponseAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsSubscriptionResponseData.md` & `fastly-1.3.1/docs/TlsSubscriptionResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsSubscriptionResponseDataAllOf.md` & `fastly-1.3.1/docs/TlsSubscriptionResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsSubscriptionsApi.md` & `fastly-1.3.1/docs/TlsSubscriptionsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsSubscriptionsResponse.md` & `fastly-1.3.1/docs/TlsSubscriptionsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TlsSubscriptionsResponseAllOf.md` & `fastly-1.3.1/docs/VersionCreateResponse.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-# TlsSubscriptionsResponseAllOf
+# VersionCreateResponse
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**[TlsSubscriptionResponse]**](TlsSubscriptionResponse.md) |  | [optional] 
+**number** | **int** |  | [optional] [readonly] 
+**service_id** | **str** |  | [optional] [readonly] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/Token.md` & `fastly-1.3.1/docs/Token.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TokenCreatedResponse.md` & `fastly-1.3.1/docs/TokenCreatedResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TokenCreatedResponseAllOf.md` & `fastly-1.3.1/docs/TokenCreatedResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TokenResponse.md` & `fastly-1.3.1/docs/TokenResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TokenResponseAllOf.md` & `fastly-1.3.1/docs/TokenResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/TokensApi.md` & `fastly-1.3.1/docs/TokensApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/UpdateBillingAddressRequest.md` & `fastly-1.3.1/docs/UpdateBillingAddressRequest.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/UpdateBillingAddressRequestData.md` & `fastly-1.3.1/docs/UpdateBillingAddressRequestData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/User.md` & `fastly-1.3.1/docs/User.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/UserApi.md` & `fastly-1.3.1/docs/UserApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/UserResponse.md` & `fastly-1.3.1/docs/UserResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/UserResponseAllOf.md` & `fastly-1.3.1/docs/UserResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ValidatorResult.md` & `fastly-1.3.1/docs/ValidatorResult.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/ValidatorResultMessages.md` & `fastly-1.3.1/docs/ValidatorResultMessages.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Vcl.md` & `fastly-1.3.1/docs/Vcl.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/VclApi.md` & `fastly-1.3.1/docs/VclApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/VclDiff.md` & `fastly-1.3.1/docs/VclDiff.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/VclDiffApi.md` & `fastly-1.3.1/docs/VclDiffApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/VclResponse.md` & `fastly-1.3.1/docs/VclResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/Version.md` & `fastly-1.3.1/docs/Version.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/VersionApi.md` & `fastly-1.3.1/docs/VersionApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/VersionCreateResponse.md` & `fastly-1.3.1/docs/WafRuleRevisionResponseDataAllOf.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# VersionCreateResponse
+# WafRuleRevisionResponseDataAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**number** | **int** |  | [optional] [readonly] 
-**service_id** | **str** |  | [optional] [readonly] 
+**relationships** | [**RelationshipWafRule**](RelationshipWafRule.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/VersionDetail.md` & `fastly-1.3.1/docs/VersionDetail.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/VersionDetailSettings.md` & `fastly-1.3.1/docs/VersionDetailSettings.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/VersionResponse.md` & `fastly-1.3.1/docs/VersionResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/VersionResponseAllOf.md` & `fastly-1.3.1/docs/WafTagsResponseAllOf.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-# VersionResponseAllOf
+# WafTagsResponseAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**service_id** | **str** |  | [optional] [readonly] 
+**data** | [**[WafTagsResponseDataItem]**](WafTagsResponseDataItem.md) |  | [optional] 
+**included** | [**[WafRule]**](WafRule.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/WafActiveRule.md` & `fastly-1.3.1/docs/WafActiveRule.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafActiveRuleCreationResponse.md` & `fastly-1.3.1/docs/WafActiveRuleCreationResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafActiveRuleData.md` & `fastly-1.3.1/docs/WafActiveRuleData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafActiveRuleDataAttributes.md` & `fastly-1.3.1/docs/WafActiveRuleDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafActiveRuleResponse.md` & `fastly-1.3.1/docs/WafActiveRuleResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafActiveRuleResponseData.md` & `fastly-1.3.1/docs/WafActiveRuleResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafActiveRuleResponseDataAllOf.md` & `fastly-1.3.1/docs/WafActiveRuleResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafActiveRuleResponseDataAttributes.md` & `fastly-1.3.1/docs/WafActiveRuleResponseDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafActiveRuleResponseDataAttributesAllOf.md` & `fastly-1.3.1/docs/WafRuleRevisionResponseData.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-# WafActiveRuleResponseDataAttributesAllOf
+# WafRuleRevisionResponseData
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**latest_revision** | **int** | The latest rule revision number that is available for the associated rule revision. | [optional] [readonly] 
-**outdated** | **bool** | Indicates if the associated rule revision is up to date or not. | [optional] [readonly] 
+**type** | [**TypeWafRuleRevision**](TypeWafRuleRevision.md) |  | [optional] 
+**id** | **str** | Alphanumeric string identifying a WAF rule revision. | [optional] [readonly] 
+**attributes** | [**WafRuleRevisionAttributes**](WafRuleRevisionAttributes.md) |  | [optional] 
+**relationships** | [**RelationshipWafRule**](RelationshipWafRule.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/WafActiveRuleResponseDataRelationships.md` & `fastly-1.3.1/docs/WafActiveRuleResponseDataRelationships.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafActiveRulesApi.md` & `fastly-1.3.1/docs/WafActiveRulesApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafActiveRulesResponse.md` & `fastly-1.3.1/docs/WafActiveRulesResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafActiveRulesResponseAllOf.md` & `fastly-1.3.1/docs/WafActiveRulesResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafExclusion.md` & `fastly-1.3.1/docs/WafFirewallVersion.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# WafExclusion
+# WafFirewallVersion
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**WafExclusionData**](WafExclusionData.md) |  | [optional] 
+**data** | [**WafFirewallVersionData**](WafFirewallVersionData.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/WafExclusionDataAttributes.md` & `fastly-1.3.1/docs/WafExclusionDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafExclusionResponse.md` & `fastly-1.3.1/docs/WafTagsResponseDataItem.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-# WafExclusionResponse
+# WafTagsResponseDataItem
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**WafExclusionResponseData**](WafExclusionResponseData.md) |  | [optional] 
+**type** | [**TypeWafTag**](TypeWafTag.md) |  | [optional] 
+**id** | **str** | Alphanumeric string identifying a WAF tag. | [optional] [readonly] 
+**attributes** | [**WafTagAttributes**](WafTagAttributes.md) |  | [optional] 
+**relationships** | [**RelationshipWafRule**](RelationshipWafRule.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/WafExclusionResponseData.md` & `fastly-1.3.1/docs/WafExclusionResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafExclusionResponseDataAllOf.md` & `fastly-1.3.1/docs/WafExclusionResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafExclusionResponseDataAttributes.md` & `fastly-1.3.1/docs/WafExclusionResponseDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafExclusionResponseDataAttributesAllOf.md` & `fastly-1.3.1/docs/WafExclusionResponseDataAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafExclusionResponseDataRelationships.md` & `fastly-1.3.1/docs/WafExclusionResponseDataRelationships.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafExclusionsApi.md` & `fastly-1.3.1/docs/WafExclusionsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafExclusionsResponse.md` & `fastly-1.3.1/docs/WafExclusionsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafExclusionsResponseAllOf.md` & `fastly-1.3.1/docs/WafExclusionsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafFirewall.md` & `fastly-1.3.1/docs/WafFirewallData.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-# WafFirewall
+# WafFirewallData
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**WafFirewallData**](WafFirewallData.md) |  | [optional] 
+**type** | [**TypeWafFirewall**](TypeWafFirewall.md) |  | [optional] 
+**attributes** | [**WafFirewallDataAttributes**](WafFirewallDataAttributes.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/WafFirewallData.md` & `fastly-1.3.1/docs/WafFirewallResponseDataAllOf.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-# WafFirewallData
+# WafFirewallResponseDataAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**type** | [**TypeWafFirewall**](TypeWafFirewall.md) |  | [optional] 
-**attributes** | [**WafFirewallDataAttributes**](WafFirewallDataAttributes.md) |  | [optional] 
+**id** | **str** |  | [optional] [readonly] 
+**attributes** | [**WafFirewallResponseDataAttributes**](WafFirewallResponseDataAttributes.md) |  | [optional] 
+**relationships** | [**RelationshipWafFirewallVersions**](RelationshipWafFirewallVersions.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/WafFirewallDataAttributes.md` & `fastly-1.3.1/docs/WafFirewallDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafFirewallResponse.md` & `fastly-1.3.1/docs/WafFirewallResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafFirewallResponseData.md` & `fastly-1.3.1/docs/WafFirewallResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafFirewallResponseDataAllOf.md` & `fastly-1.3.1/docs/WafFirewallVersionResponseData.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# WafFirewallResponseDataAllOf
+# WafFirewallVersionResponseData
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**id** | **str** |  | [optional] [readonly] 
-**attributes** | [**WafFirewallResponseDataAttributes**](WafFirewallResponseDataAttributes.md) |  | [optional] 
-**relationships** | [**RelationshipWafFirewallVersions**](RelationshipWafFirewallVersions.md) |  | [optional] 
+**type** | [**TypeWafFirewallVersion**](TypeWafFirewallVersion.md) |  | [optional] 
+**attributes** | [**WafFirewallVersionResponseDataAttributes**](WafFirewallVersionResponseDataAttributes.md) |  | [optional] 
+**id** | **str** | Alphanumeric string identifying a Firewall version. | [optional] [readonly] 
+**relationships** | [**RelationshipsForWafFirewallVersion**](RelationshipsForWafFirewallVersion.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/WafFirewallResponseDataAttributes.md` & `fastly-1.3.1/docs/WafFirewallResponseDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafFirewallResponseDataAttributesAllOf.md` & `fastly-1.3.1/docs/WafFirewallResponseDataAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafFirewallVersion.md` & `fastly-1.3.1/docs/WafRule.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-# WafFirewallVersion
+# WafRule
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**WafFirewallVersionData**](WafFirewallVersionData.md) |  | [optional] 
+**type** | [**TypeWafRule**](TypeWafRule.md) |  | [optional] 
+**id** | **str** |  | [optional] [readonly] 
+**attributes** | [**WafRuleAttributes**](WafRuleAttributes.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/WafFirewallVersionData.md` & `fastly-1.3.1/docs/WafFirewallVersionData.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafFirewallVersionDataAttributes.md` & `fastly-1.3.1/docs/WafFirewallVersionDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafFirewallVersionResponse.md` & `fastly-1.3.1/docs/WafFirewallVersionResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafFirewallVersionResponseData.md` & `fastly-1.3.1/docs/WafFirewallVersionResponseDataAllOf.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-# WafFirewallVersionResponseData
+# WafFirewallVersionResponseDataAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**type** | [**TypeWafFirewallVersion**](TypeWafFirewallVersion.md) |  | [optional] 
-**attributes** | [**WafFirewallVersionResponseDataAttributes**](WafFirewallVersionResponseDataAttributes.md) |  | [optional] 
 **id** | **str** | Alphanumeric string identifying a Firewall version. | [optional] [readonly] 
+**attributes** | [**WafFirewallVersionResponseDataAttributes**](WafFirewallVersionResponseDataAttributes.md) |  | [optional] 
 **relationships** | [**RelationshipsForWafFirewallVersion**](RelationshipsForWafFirewallVersion.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/WafFirewallVersionResponseDataAllOf.md` & `fastly-1.3.1/docs/WafTagsResponse.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# WafFirewallVersionResponseDataAllOf
+# WafTagsResponse
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**id** | **str** | Alphanumeric string identifying a Firewall version. | [optional] [readonly] 
-**attributes** | [**WafFirewallVersionResponseDataAttributes**](WafFirewallVersionResponseDataAttributes.md) |  | [optional] 
-**relationships** | [**RelationshipsForWafFirewallVersion**](RelationshipsForWafFirewallVersion.md) |  | [optional] 
+**links** | [**PaginationLinks**](PaginationLinks.md) |  | [optional] 
+**meta** | [**PaginationMeta**](PaginationMeta.md) |  | [optional] 
+**data** | [**[WafTagsResponseDataItem]**](WafTagsResponseDataItem.md) |  | [optional] 
+**included** | [**[WafRule]**](WafRule.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/WafFirewallVersionResponseDataAttributes.md` & `fastly-1.3.1/docs/WafFirewallVersionResponseDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafFirewallVersionResponseDataAttributesAllOf.md` & `fastly-1.3.1/docs/WafFirewallVersionResponseDataAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafFirewallVersionsApi.md` & `fastly-1.3.1/docs/WafFirewallVersionsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafFirewallVersionsResponse.md` & `fastly-1.3.1/docs/WafFirewallVersionsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafFirewallVersionsResponseAllOf.md` & `fastly-1.3.1/docs/WafFirewallVersionsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafFirewallsApi.md` & `fastly-1.3.1/docs/WafFirewallsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafFirewallsResponse.md` & `fastly-1.3.1/docs/WafFirewallsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafFirewallsResponseAllOf.md` & `fastly-1.3.1/docs/WafFirewallsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafRule.md` & `fastly-1.3.1/docs/WafTag.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# WafRule
+# WafTag
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**type** | [**TypeWafRule**](TypeWafRule.md) |  | [optional] 
-**id** | **str** |  | [optional] [readonly] 
-**attributes** | [**WafRuleAttributes**](WafRuleAttributes.md) |  | [optional] 
+**type** | [**TypeWafTag**](TypeWafTag.md) |  | [optional] 
+**id** | **str** | Alphanumeric string identifying a WAF tag. | [optional] [readonly] 
+**attributes** | [**WafTagAttributes**](WafTagAttributes.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/WafRuleAttributes.md` & `fastly-1.3.1/docs/WafRuleAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafRuleResponse.md` & `fastly-1.3.1/docs/WafRuleResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafRuleResponseData.md` & `fastly-1.3.1/docs/WafRulesResponse.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# WafRuleResponseData
+# WafRulesResponse
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**type** | [**TypeWafRule**](TypeWafRule.md) |  | [optional] 
-**id** | **str** |  | [optional] [readonly] 
-**attributes** | [**WafRuleAttributes**](WafRuleAttributes.md) |  | [optional] 
-**relationships** | [**RelationshipsForWafRule**](RelationshipsForWafRule.md) |  | [optional] 
+**links** | [**PaginationLinks**](PaginationLinks.md) |  | [optional] 
+**meta** | [**PaginationMeta**](PaginationMeta.md) |  | [optional] 
+**data** | [**[WafRuleResponseData]**](WafRuleResponseData.md) |  | [optional] 
+**included** | [**IncludedWithWafRule**](IncludedWithWafRule.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/WafRuleResponseDataAllOf.md` & `fastly-1.3.1/docs/WafRuleResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafRuleRevision.md` & `fastly-1.3.1/docs/WafRuleRevision.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafRuleRevisionAttributes.md` & `fastly-1.3.1/docs/WafRuleRevisionAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafRuleRevisionResponse.md` & `fastly-1.3.1/docs/WafRuleRevisionResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafRuleRevisionResponseData.md` & `fastly-1.3.1/docs/WafRuleRevisionsResponseAllOf.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-# WafRuleRevisionResponseData
+# WafRuleRevisionsResponseAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**type** | [**TypeWafRuleRevision**](TypeWafRuleRevision.md) |  | [optional] 
-**id** | **str** | Alphanumeric string identifying a WAF rule revision. | [optional] [readonly] 
-**attributes** | [**WafRuleRevisionAttributes**](WafRuleRevisionAttributes.md) |  | [optional] 
-**relationships** | [**RelationshipWafRule**](RelationshipWafRule.md) |  | [optional] 
+**data** | [**[WafRuleRevisionResponseData]**](WafRuleRevisionResponseData.md) |  | [optional] 
+**included** | [**IncludedWithWafRuleRevision**](IncludedWithWafRuleRevision.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/WafRuleRevisionsApi.md` & `fastly-1.3.1/docs/WafRuleRevisionsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafRuleRevisionsResponse.md` & `fastly-1.3.1/docs/WafRuleRevisionsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafRuleRevisionsResponseAllOf.md` & `fastly-1.3.1/docs/WafRulesResponseAllOf.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# WafRuleRevisionsResponseAllOf
+# WafRulesResponseAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**[WafRuleRevisionResponseData]**](WafRuleRevisionResponseData.md) |  | [optional] 
-**included** | [**IncludedWithWafRuleRevision**](IncludedWithWafRuleRevision.md) |  | [optional] 
+**data** | [**[WafRuleResponseData]**](WafRuleResponseData.md) |  | [optional] 
+**included** | [**IncludedWithWafRule**](IncludedWithWafRule.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-1.3.0/docs/WafRulesApi.md` & `fastly-1.3.1/docs/WafRulesApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WafTagsApi.md` & `fastly-1.3.1/docs/WafTagsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/docs/WsMessageFormat.md` & `fastly-1.3.1/docs/WsMessageFormat.md`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/__init__.py` & `fastly-1.3.1/fastly/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Via the Fastly API you can perform any of the operations that are possible within the management console,  including creating services, domains, and backends, configuring rules or uploading your own application code, as well as account operations such as user administration and billing reports. The API is organized into collections of endpoints that allow manipulation of objects related to Fastly services and accounts. For the most accurate and up-to-date API reference content, visit our [Developer Hub](https://developer.fastly.com/reference/api/)   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Contact: oss@fastly.com
 """
 
 
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 
 # import ApiClient
 from fastly.api_client import ApiClient
 
 # import Configuration
 from fastly.configuration import Configuration
```

### Comparing `fastly-1.3.0/fastly/api_client.py` & `fastly-1.3.1/fastly/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'fastly-py/1.3.0'
+        self.user_agent = 'fastly-py/1.3.1'
 
         # The last observed value of http header Fastly-RateLimit-Remaining
         self.rate_limit_remaining = DEFAULT_RATELIMIT
 
         # The last observed value of http header Fastly-RateLimit-Reset
         self.rate_limit_reset = 0
```

### Comparing `fastly-1.3.0/fastly/configuration.py` & `fastly-1.3.1/fastly/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,15 +442,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 1.3.0".\
+               "SDK Package Version: 1.3.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `fastly-1.3.0/fastly/exceptions.py` & `fastly-1.3.1/fastly/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model_utils.py` & `fastly-1.3.1/fastly/model_utils.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/rest.py` & `fastly-1.3.1/fastly/rest.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/acl_api.py` & `fastly-1.3.1/fastly/api/acl_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/acl_entry_api.py` & `fastly-1.3.1/fastly/api/acl_entry_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/apex_redirect_api.py` & `fastly-1.3.1/fastly/api/apex_redirect_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/backend_api.py` & `fastly-1.3.1/fastly/api/backend_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/billing_address_api.py` & `fastly-1.3.1/fastly/api/billing_address_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/billing_api.py` & `fastly-1.3.1/fastly/api/billing_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/cache_settings_api.py` & `fastly-1.3.1/fastly/api/cache_settings_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/condition_api.py` & `fastly-1.3.1/fastly/api/condition_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/contact_api.py` & `fastly-1.3.1/fastly/api/contact_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/content_api.py` & `fastly-1.3.1/fastly/api/content_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/customer_api.py` & `fastly-1.3.1/fastly/api/customer_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/dictionary_api.py` & `fastly-1.3.1/fastly/api/dictionary_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/dictionary_info_api.py` & `fastly-1.3.1/fastly/api/dictionary_info_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/dictionary_item_api.py` & `fastly-1.3.1/fastly/api/dictionary_item_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/diff_api.py` & `fastly-1.3.1/fastly/api/diff_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/director_api.py` & `fastly-1.3.1/fastly/api/director_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/director_backend_api.py` & `fastly-1.3.1/fastly/api/director_backend_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/domain_api.py` & `fastly-1.3.1/fastly/api/domain_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/domain_ownerships_api.py` & `fastly-1.3.1/fastly/api/domain_ownerships_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/enabled_products_api.py` & `fastly-1.3.1/fastly/api/enabled_products_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/events_api.py` & `fastly-1.3.1/fastly/api/events_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/gzip_api.py` & `fastly-1.3.1/fastly/api/gzip_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/header_api.py` & `fastly-1.3.1/fastly/api/header_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/healthcheck_api.py` & `fastly-1.3.1/fastly/api/healthcheck_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/historical_api.py` & `fastly-1.3.1/fastly/api/historical_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/http3_api.py` & `fastly-1.3.1/fastly/api/http3_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/iam_permissions_api.py` & `fastly-1.3.1/fastly/api/iam_permissions_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/iam_roles_api.py` & `fastly-1.3.1/fastly/api/iam_roles_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/iam_service_groups_api.py` & `fastly-1.3.1/fastly/api/iam_service_groups_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/iam_user_groups_api.py` & `fastly-1.3.1/fastly/api/iam_user_groups_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/invitations_api.py` & `fastly-1.3.1/fastly/api/invitations_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_azureblob_api.py` & `fastly-1.3.1/fastly/api/logging_azureblob_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_bigquery_api.py` & `fastly-1.3.1/fastly/api/logging_bigquery_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_cloudfiles_api.py` & `fastly-1.3.1/fastly/api/logging_cloudfiles_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_datadog_api.py` & `fastly-1.3.1/fastly/api/logging_datadog_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_digitalocean_api.py` & `fastly-1.3.1/fastly/api/logging_digitalocean_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_elasticsearch_api.py` & `fastly-1.3.1/fastly/api/logging_elasticsearch_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_ftp_api.py` & `fastly-1.3.1/fastly/api/logging_ftp_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_gcs_api.py` & `fastly-1.3.1/fastly/api/logging_gcs_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_heroku_api.py` & `fastly-1.3.1/fastly/api/logging_heroku_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_honeycomb_api.py` & `fastly-1.3.1/fastly/api/logging_honeycomb_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_https_api.py` & `fastly-1.3.1/fastly/api/logging_https_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_kafka_api.py` & `fastly-1.3.1/fastly/api/logging_kafka_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_kinesis_api.py` & `fastly-1.3.1/fastly/api/logging_kinesis_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_logentries_api.py` & `fastly-1.3.1/fastly/api/logging_logentries_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_loggly_api.py` & `fastly-1.3.1/fastly/api/logging_loggly_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_logshuttle_api.py` & `fastly-1.3.1/fastly/api/logging_logshuttle_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_newrelic_api.py` & `fastly-1.3.1/fastly/api/logging_newrelic_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_openstack_api.py` & `fastly-1.3.1/fastly/api/logging_openstack_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_papertrail_api.py` & `fastly-1.3.1/fastly/api/logging_papertrail_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_pubsub_api.py` & `fastly-1.3.1/fastly/api/logging_pubsub_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_s3_api.py` & `fastly-1.3.1/fastly/api/logging_s3_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_scalyr_api.py` & `fastly-1.3.1/fastly/api/logging_scalyr_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_sftp_api.py` & `fastly-1.3.1/fastly/api/logging_sftp_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_splunk_api.py` & `fastly-1.3.1/fastly/api/logging_splunk_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_sumologic_api.py` & `fastly-1.3.1/fastly/api/logging_sumologic_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/logging_syslog_api.py` & `fastly-1.3.1/fastly/api/logging_syslog_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/mutual_authentication_api.py` & `fastly-1.3.1/fastly/api/mutual_authentication_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/object_store_api.py` & `fastly-1.3.1/fastly/api/object_store_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/object_store_item_api.py` & `fastly-1.3.1/fastly/api/object_store_item_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,15 @@
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
         self.get_value_for_key_endpoint = _Endpoint(
             settings={
-                'response_type': (file_type,),
+                'response_type': (str,),
                 'auth': [
                     'token'
                 ],
                 'endpoint_path': '/resources/stores/object/{store_id}/keys/{key_name}',
                 'operation_id': 'get_value_for_key',
                 'http_method': 'GET',
                 'servers': None,
@@ -220,15 +220,15 @@
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
         self.set_value_for_key_endpoint = _Endpoint(
             settings={
-                'response_type': (file_type,),
+                'response_type': (str,),
                 'auth': [
                     'token'
                 ],
                 'endpoint_path': '/resources/stores/object/{store_id}/keys/{key_name}',
                 'operation_id': 'set_value_for_key',
                 'http_method': 'PUT',
                 'servers': None,
@@ -278,15 +278,15 @@
                     'append':
                         (bool,),
                     'prepend':
                         (bool,),
                     'background_fetch':
                         (bool,),
                     'body':
-                        (file_type,),
+                        (str,),
                 },
                 'attribute_map': {
                     'store_id': 'store_id',
                     'key_name': 'key_name',
                     'if_generation_match': 'if-generation-match',
                     'time_to_live_sec': 'time_to_live_sec',
                     'metadata': 'metadata',
@@ -531,15 +531,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            file_type
+            str
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -592,15 +592,15 @@
             if_generation_match (int): [optional]
             time_to_live_sec (int): [optional]
             metadata (str): [optional]
             add (bool): [optional]
             append (bool): [optional]
             prepend (bool): [optional]
             background_fetch (bool): [optional]
-            body (file_type): [optional]
+            body (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -621,15 +621,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            file_type
+            str
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
```

### Comparing `fastly-1.3.0/fastly/api/package_api.py` & `fastly-1.3.1/fastly/api/package_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/pool_api.py` & `fastly-1.3.1/fastly/api/pool_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/pop_api.py` & `fastly-1.3.1/fastly/api/pop_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/public_ip_list_api.py` & `fastly-1.3.1/fastly/api/public_ip_list_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/publish_api.py` & `fastly-1.3.1/fastly/api/publish_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/purge_api.py` & `fastly-1.3.1/fastly/api/purge_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/rate_limiter_api.py` & `fastly-1.3.1/fastly/api/rate_limiter_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/realtime_api.py` & `fastly-1.3.1/fastly/api/realtime_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/request_settings_api.py` & `fastly-1.3.1/fastly/api/request_settings_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/resource_api.py` & `fastly-1.3.1/fastly/api/resource_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/response_object_api.py` & `fastly-1.3.1/fastly/api/response_object_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/server_api.py` & `fastly-1.3.1/fastly/api/server_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/service_api.py` & `fastly-1.3.1/fastly/api/service_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/service_authorizations_api.py` & `fastly-1.3.1/fastly/api/service_authorizations_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/settings_api.py` & `fastly-1.3.1/fastly/api/settings_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/snippet_api.py` & `fastly-1.3.1/fastly/api/snippet_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/star_api.py` & `fastly-1.3.1/fastly/api/star_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/stats_api.py` & `fastly-1.3.1/fastly/api/stats_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/tls_activations_api.py` & `fastly-1.3.1/fastly/api/tls_activations_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/tls_bulk_certificates_api.py` & `fastly-1.3.1/fastly/api/tls_bulk_certificates_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/tls_certificates_api.py` & `fastly-1.3.1/fastly/api/tls_certificates_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/tls_configurations_api.py` & `fastly-1.3.1/fastly/api/tls_configurations_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/tls_domains_api.py` & `fastly-1.3.1/fastly/api/tls_domains_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/tls_private_keys_api.py` & `fastly-1.3.1/fastly/api/tls_private_keys_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/tls_subscriptions_api.py` & `fastly-1.3.1/fastly/api/tls_subscriptions_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/tokens_api.py` & `fastly-1.3.1/fastly/api/tokens_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/user_api.py` & `fastly-1.3.1/fastly/api/user_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/vcl_api.py` & `fastly-1.3.1/fastly/api/vcl_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/vcl_diff_api.py` & `fastly-1.3.1/fastly/api/vcl_diff_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/version_api.py` & `fastly-1.3.1/fastly/api/version_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/waf_active_rules_api.py` & `fastly-1.3.1/fastly/api/waf_active_rules_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/waf_exclusions_api.py` & `fastly-1.3.1/fastly/api/waf_exclusions_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/waf_firewall_versions_api.py` & `fastly-1.3.1/fastly/api/waf_firewall_versions_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/waf_firewalls_api.py` & `fastly-1.3.1/fastly/api/waf_firewalls_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/waf_rule_revisions_api.py` & `fastly-1.3.1/fastly/api/waf_rule_revisions_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/waf_rules_api.py` & `fastly-1.3.1/fastly/api/waf_rules_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/api/waf_tags_api.py` & `fastly-1.3.1/fastly/api/waf_tags_api.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/apis/__init__.py` & `fastly-1.3.1/fastly/apis/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,14 @@
 from fastly.api.snippet_api import SnippetApi
 from fastly.api.star_api import StarApi
 from fastly.api.stats_api import StatsApi
 from fastly.api.tls_activations_api import TlsActivationsApi
 from fastly.api.tls_bulk_certificates_api import TlsBulkCertificatesApi
 from fastly.api.tls_certificates_api import TlsCertificatesApi
 from fastly.api.tls_configurations_api import TlsConfigurationsApi
-from fastly.api.tls_csrs_api import TlsCsrsApi
 from fastly.api.tls_domains_api import TlsDomainsApi
 from fastly.api.tls_private_keys_api import TlsPrivateKeysApi
 from fastly.api.tls_subscriptions_api import TlsSubscriptionsApi
 from fastly.api.tokens_api import TokensApi
 from fastly.api.user_api import UserApi
 from fastly.api.vcl_api import VclApi
 from fastly.api.vcl_diff_api import VclDiffApi
```

### Comparing `fastly-1.3.0/fastly/model/acl.py` & `fastly-1.3.1/fastly/model/acl.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/acl_entry.py` & `fastly-1.3.1/fastly/model/acl_entry.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/acl_entry_response.py` & `fastly-1.3.1/fastly/model/acl_entry_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/acl_entry_response_all_of.py` & `fastly-1.3.1/fastly/model/acl_entry_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/acl_response.py` & `fastly-1.3.1/fastly/model/acl_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/acl_response_all_of.py` & `fastly-1.3.1/fastly/model/acl_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/apex_redirect.py` & `fastly-1.3.1/fastly/model/apex_redirect.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/apex_redirect_all_of.py` & `fastly-1.3.1/fastly/model/apex_redirect_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/aws_region.py` & `fastly-1.3.1/fastly/model/aws_region.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/backend.py` & `fastly-1.3.1/fastly/model/backend.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/backend_response.py` & `fastly-1.3.1/fastly/model/backend_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/backend_response_all_of.py` & `fastly-1.3.1/fastly/model/backend_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/billing.py` & `fastly-1.3.1/fastly/model/billing.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/billing_address_attributes.py` & `fastly-1.3.1/fastly/model/billing_address_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/billing_address_request.py` & `fastly-1.3.1/fastly/model/billing_address_request.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/billing_address_request_data.py` & `fastly-1.3.1/fastly/model/billing_address_request_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/billing_address_response.py` & `fastly-1.3.1/fastly/model/billing_address_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/billing_address_response_data.py` & `fastly-1.3.1/fastly/model/billing_address_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/billing_address_verification_error_response.py` & `fastly-1.3.1/fastly/model/billing_address_verification_error_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/billing_address_verification_error_response_errors.py` & `fastly-1.3.1/fastly/model/billing_address_verification_error_response_errors.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/billing_estimate_response.py` & `fastly-1.3.1/fastly/model/billing_estimate_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/billing_estimate_response_all_of.py` & `fastly-1.3.1/fastly/model/billing_estimate_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/billing_estimate_response_all_of_line.py` & `fastly-1.3.1/fastly/model/billing_estimate_response_all_of_line.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/billing_estimate_response_all_of_lines.py` & `fastly-1.3.1/fastly/model/billing_estimate_response_all_of_lines.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/billing_response.py` & `fastly-1.3.1/fastly/model/billing_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/billing_response_all_of.py` & `fastly-1.3.1/fastly/model/billing_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/billing_response_line_item.py` & `fastly-1.3.1/fastly/model/billing_response_line_item.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/billing_response_line_item_all_of.py` & `fastly-1.3.1/fastly/model/billing_response_line_item_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/billing_status.py` & `fastly-1.3.1/fastly/model/billing_status.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/billing_total.py` & `fastly-1.3.1/fastly/model/billing_total.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/billing_total_extras.py` & `fastly-1.3.1/fastly/model/billing_total_extras.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/bulk_update_acl_entries_request.py` & `fastly-1.3.1/fastly/model/bulk_update_acl_entries_request.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/bulk_update_acl_entry.py` & `fastly-1.3.1/fastly/model/bulk_update_acl_entry.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/bulk_update_acl_entry_all_of.py` & `fastly-1.3.1/fastly/model/bulk_update_acl_entry_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/bulk_update_dictionary_item.py` & `fastly-1.3.1/fastly/model/bulk_update_dictionary_item.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/bulk_update_dictionary_item_all_of.py` & `fastly-1.3.1/fastly/model/bulk_update_dictionary_item_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/bulk_update_dictionary_list_request.py` & `fastly-1.3.1/fastly/model/bulk_update_dictionary_list_request.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/bulk_waf_active_rule.py` & `fastly-1.3.1/fastly/model/bulk_waf_active_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/bulk_waf_active_rules.py` & `fastly-1.3.1/fastly/model/bulk_waf_active_rules.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/cache_setting.py` & `fastly-1.3.1/fastly/model/cache_setting.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/cache_setting_response.py` & `fastly-1.3.1/fastly/model/cache_setting_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/condition.py` & `fastly-1.3.1/fastly/model/condition.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/condition_response.py` & `fastly-1.3.1/fastly/model/condition_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/conditions_response.py` & `fastly-1.3.1/fastly/model/conditions_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/contact.py` & `fastly-1.3.1/fastly/model/contact.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/contact_response.py` & `fastly-1.3.1/fastly/model/contact_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/contact_response_all_of.py` & `fastly-1.3.1/fastly/model/contact_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/content.py` & `fastly-1.3.1/fastly/model/content.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/customer.py` & `fastly-1.3.1/fastly/model/customer.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/customer_response.py` & `fastly-1.3.1/fastly/model/customer_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/customer_response_all_of.py` & `fastly-1.3.1/fastly/model/customer_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/dictionary.py` & `fastly-1.3.1/fastly/model/dictionary.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/dictionary_info_response.py` & `fastly-1.3.1/fastly/model/dictionary_info_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/dictionary_item.py` & `fastly-1.3.1/fastly/model/dictionary_item.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/dictionary_item_response.py` & `fastly-1.3.1/fastly/model/dictionary_item_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/dictionary_item_response_all_of.py` & `fastly-1.3.1/fastly/model/dictionary_item_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/dictionary_response.py` & `fastly-1.3.1/fastly/model/dictionary_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/dictionary_response_all_of.py` & `fastly-1.3.1/fastly/model/dictionary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/diff_response.py` & `fastly-1.3.1/fastly/model/diff_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/director.py` & `fastly-1.3.1/fastly/model/director.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/director_backend.py` & `fastly-1.3.1/fastly/model/director_backend.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/director_backend_all_of.py` & `fastly-1.3.1/fastly/model/director_backend_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/director_response.py` & `fastly-1.3.1/fastly/model/director_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/domain.py` & `fastly-1.3.1/fastly/model/domain.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/domain_check_item.py` & `fastly-1.3.1/fastly/model/domain_check_item.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/domain_check_response.py` & `fastly-1.3.1/fastly/model/domain_check_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/domain_check_response_list.py` & `fastly-1.3.1/fastly/model/domain_check_response_list.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/domain_response.py` & `fastly-1.3.1/fastly/model/domain_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/domains_response.py` & `fastly-1.3.1/fastly/model/domains_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/enabled_product_response.py` & `fastly-1.3.1/fastly/model/enabled_product_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/enabled_product_response_links.py` & `fastly-1.3.1/fastly/model/enabled_product_response_links.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/enabled_product_response_product.py` & `fastly-1.3.1/fastly/model/enabled_product_response_product.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/enabled_product_response_service.py` & `fastly-1.3.1/fastly/model/enabled_product_response_service.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/error_response.py` & `fastly-1.3.1/fastly/model/pool_response_all_of.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from fastly.model.error_response_data import ErrorResponseData
-    globals()['ErrorResponseData'] = ErrorResponseData
 
-
-class ErrorResponse(ModelNormal):
+class PoolResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -64,52 +60,51 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'errors': ([ErrorResponseData],),  # noqa: E501
+            'id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'errors': 'errors',  # noqa: E501
+        'id': 'id',  # noqa: E501
     }
 
     read_only_vars = {
+        'id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ErrorResponse - a model defined in OpenAPI
+        """PoolResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +129,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            errors ([ErrorResponseData]): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +178,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ErrorResponse - a model defined in OpenAPI
+        """PoolResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +211,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            errors ([ErrorResponseData]): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/error_response_data.py` & `fastly-1.3.1/fastly/model/relationship_member_waf_firewall.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fastly.model.type_waf_firewall import TypeWafFirewall
+    globals()['TypeWafFirewall'] = TypeWafFirewall
 
-class ErrorResponseData(ModelNormal):
+
+class RelationshipMemberWafFirewall(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -60,52 +64,55 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'title': (str,),  # noqa: E501
-            'detail': (str,),  # noqa: E501
+            'type': (TypeWafFirewall,),  # noqa: E501
+            'id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'title': 'title',  # noqa: E501
-        'detail': 'detail',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'id': 'id',  # noqa: E501
     }
 
     read_only_vars = {
+        'id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ErrorResponseData - a model defined in OpenAPI
+        """RelationshipMemberWafFirewall - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -130,16 +137,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            title (str): [optional]  # noqa: E501
-            detail (str): [optional]  # noqa: E501
+            type (TypeWafFirewall): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -180,15 +187,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ErrorResponseData - a model defined in OpenAPI
+        """RelationshipMemberWafFirewall - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -213,16 +220,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            title (str): [optional]  # noqa: E501
-            detail (str): [optional]  # noqa: E501
+            type (TypeWafFirewall): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/event.py` & `fastly-1.3.1/fastly/model/event.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/event_attributes.py` & `fastly-1.3.1/fastly/model/event_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/event_response.py` & `fastly-1.3.1/fastly/model/event_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/events_response.py` & `fastly-1.3.1/fastly/model/events_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/events_response_all_of.py` & `fastly-1.3.1/fastly/model/events_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/generic_token_error.py` & `fastly-1.3.1/fastly/model/generic_token_error.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/gzip.py` & `fastly-1.3.1/fastly/model/gzip.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/gzip_response.py` & `fastly-1.3.1/fastly/model/gzip_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/header.py` & `fastly-1.3.1/fastly/model/header.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/header_response.py` & `fastly-1.3.1/fastly/model/header_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/healthcheck.py` & `fastly-1.3.1/fastly/model/healthcheck.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/healthcheck_response.py` & `fastly-1.3.1/fastly/model/healthcheck_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/historical.py` & `fastly-1.3.1/fastly/model/historical.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/historical_aggregate_response.py` & `fastly-1.3.1/fastly/model/historical_aggregate_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/historical_aggregate_response_all_of.py` & `fastly-1.3.1/fastly/model/historical_aggregate_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/historical_field_aggregate_response.py` & `fastly-1.3.1/fastly/model/historical_field_aggregate_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/historical_field_aggregate_response_all_of.py` & `fastly-1.3.1/fastly/model/historical_field_aggregate_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/historical_field_response.py` & `fastly-1.3.1/fastly/model/historical_field_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/historical_field_response_all_of.py` & `fastly-1.3.1/fastly/model/historical_field_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/historical_field_results.py` & `fastly-1.3.1/fastly/model/historical_field_results.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/historical_meta.py` & `fastly-1.3.1/fastly/model/historical_meta.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/historical_regions_response.py` & `fastly-1.3.1/fastly/model/historical_regions_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/historical_regions_response_all_of.py` & `fastly-1.3.1/fastly/model/historical_regions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/historical_response.py` & `fastly-1.3.1/fastly/model/historical_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/historical_response_all_of.py` & `fastly-1.3.1/fastly/model/historical_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/historical_results.py` & `fastly-1.3.1/fastly/model/historical_results.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/historical_services.py` & `fastly-1.3.1/fastly/model/historical_services.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/historical_usage_aggregate_response.py` & `fastly-1.3.1/fastly/model/historical_usage_aggregate_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/historical_usage_month_response.py` & `fastly-1.3.1/fastly/model/historical_usage_month_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/historical_usage_month_response_all_of.py` & `fastly-1.3.1/fastly/model/historical_usage_month_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/historical_usage_month_response_all_of_data.py` & `fastly-1.3.1/fastly/model/historical_usage_month_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/historical_usage_results.py` & `fastly-1.3.1/fastly/model/historical_usage_results.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/historical_usage_service_response.py` & `fastly-1.3.1/fastly/model/historical_usage_service_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/historical_usage_service_response_all_of.py` & `fastly-1.3.1/fastly/model/historical_usage_service_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/http3.py` & `fastly-1.3.1/fastly/model/http3.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/http3_all_of.py` & `fastly-1.3.1/fastly/model/http3_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/http_response_format.py` & `fastly-1.3.1/fastly/model/http_response_format.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/http_stream_format.py` & `fastly-1.3.1/fastly/model/http_stream_format.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/iam_permission.py` & `fastly-1.3.1/fastly/model/iam_permission.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/iam_role.py` & `fastly-1.3.1/fastly/model/iam_role.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/iam_role_all_of.py` & `fastly-1.3.1/fastly/model/iam_role_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/iam_service_group.py` & `fastly-1.3.1/fastly/model/iam_service_group.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/iam_service_group_all_of.py` & `fastly-1.3.1/fastly/model/iam_service_group_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/iam_user_group.py` & `fastly-1.3.1/fastly/model/iam_user_group.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/iam_user_group_all_of.py` & `fastly-1.3.1/fastly/model/iam_user_group_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/included_with_waf_active_rule.py` & `fastly-1.3.1/fastly/model/included_with_waf_active_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/included_with_waf_active_rule_item.py` & `fastly-1.3.1/fastly/model/included_with_waf_active_rule_item.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/included_with_waf_exclusion.py` & `fastly-1.3.1/fastly/model/included_with_waf_exclusion.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/included_with_waf_exclusion_item.py` & `fastly-1.3.1/fastly/model/included_with_waf_exclusion_item.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/included_with_waf_firewall.py` & `fastly-1.3.1/fastly/model/included_with_waf_firewall.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/included_with_waf_firewall_version.py` & `fastly-1.3.1/fastly/model/included_with_waf_firewall_version.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/included_with_waf_firewall_version_item.py` & `fastly-1.3.1/fastly/model/included_with_waf_firewall_version_item.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/included_with_waf_rule.py` & `fastly-1.3.1/fastly/model/included_with_waf_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/included_with_waf_rule_item.py` & `fastly-1.3.1/fastly/model/included_with_waf_rule_item.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/included_with_waf_rule_revision.py` & `fastly-1.3.1/fastly/model/included_with_waf_rule_revision.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/inline_object.py` & `fastly-1.3.1/fastly/model/inline_object.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/inline_object1.py` & `fastly-1.3.1/fastly/model/inline_object1.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/inline_response200.py` & `fastly-1.3.1/fastly/model/inline_response200.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/inline_response2001.py` & `fastly-1.3.1/fastly/model/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/inline_response2002.py` & `fastly-1.3.1/fastly/model/inline_response2002.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/inline_response2002_meta.py` & `fastly-1.3.1/fastly/model/inline_response2002_meta.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/inline_response2003.py` & `fastly-1.3.1/fastly/model/inline_response2003.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/inline_response2003_meta.py` & `fastly-1.3.1/fastly/model/inline_response2003_meta.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/invitation.py` & `fastly-1.3.1/fastly/model/invitation.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/invitation_data.py` & `fastly-1.3.1/fastly/model/invitation_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/invitation_data_attributes.py` & `fastly-1.3.1/fastly/model/invitation_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/invitation_response.py` & `fastly-1.3.1/fastly/model/invitation_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/invitation_response_all_of.py` & `fastly-1.3.1/fastly/model/invitation_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/invitation_response_data.py` & `fastly-1.3.1/fastly/model/invitation_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/invitation_response_data_all_of.py` & `fastly-1.3.1/fastly/model/invitation_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/invitations_response.py` & `fastly-1.3.1/fastly/model/invitations_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/invitations_response_all_of.py` & `fastly-1.3.1/fastly/model/invitations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_address_and_port.py` & `fastly-1.3.1/fastly/model/logging_address_and_port.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_azureblob.py` & `fastly-1.3.1/fastly/model/logging_azureblob.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_azureblob_all_of.py` & `fastly-1.3.1/fastly/model/logging_azureblob_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_azureblob_response.py` & `fastly-1.3.1/fastly/model/logging_azureblob_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_bigquery.py` & `fastly-1.3.1/fastly/model/logging_bigquery.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_bigquery_all_of.py` & `fastly-1.3.1/fastly/model/logging_bigquery_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_bigquery_response.py` & `fastly-1.3.1/fastly/model/logging_bigquery_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_cloudfiles.py` & `fastly-1.3.1/fastly/model/logging_cloudfiles.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_cloudfiles_all_of.py` & `fastly-1.3.1/fastly/model/logging_cloudfiles_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_cloudfiles_response.py` & `fastly-1.3.1/fastly/model/logging_cloudfiles_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_common.py` & `fastly-1.3.1/fastly/model/logging_common.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_datadog.py` & `fastly-1.3.1/fastly/model/logging_datadog.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_datadog_all_of.py` & `fastly-1.3.1/fastly/model/logging_datadog_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_datadog_response.py` & `fastly-1.3.1/fastly/model/logging_datadog_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_digitalocean.py` & `fastly-1.3.1/fastly/model/logging_digitalocean.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_digitalocean_all_of.py` & `fastly-1.3.1/fastly/model/logging_digitalocean_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_digitalocean_response.py` & `fastly-1.3.1/fastly/model/logging_digitalocean_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_elasticsearch.py` & `fastly-1.3.1/fastly/model/logging_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_elasticsearch_all_of.py` & `fastly-1.3.1/fastly/model/logging_elasticsearch_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_elasticsearch_response.py` & `fastly-1.3.1/fastly/model/logging_elasticsearch_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_format_version.py` & `fastly-1.3.1/fastly/model/logging_format_version.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_ftp.py` & `fastly-1.3.1/fastly/model/logging_ftp.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_ftp_all_of.py` & `fastly-1.3.1/fastly/model/logging_ftp_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_ftp_response.py` & `fastly-1.3.1/fastly/model/logging_ftp_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_gcs.py` & `fastly-1.3.1/fastly/model/logging_gcs.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_gcs_all_of.py` & `fastly-1.3.1/fastly/model/logging_gcs_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_gcs_common.py` & `fastly-1.3.1/fastly/model/logging_gcs_common.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_gcs_response.py` & `fastly-1.3.1/fastly/model/logging_gcs_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_generic_common.py` & `fastly-1.3.1/fastly/model/logging_generic_common.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_google_pubsub.py` & `fastly-1.3.1/fastly/model/logging_google_pubsub.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_google_pubsub_all_of.py` & `fastly-1.3.1/fastly/model/logging_google_pubsub_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_google_pubsub_response.py` & `fastly-1.3.1/fastly/model/logging_google_pubsub_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_heroku.py` & `fastly-1.3.1/fastly/model/logging_heroku.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_heroku_all_of.py` & `fastly-1.3.1/fastly/model/logging_heroku_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_heroku_response.py` & `fastly-1.3.1/fastly/model/logging_heroku_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_honeycomb.py` & `fastly-1.3.1/fastly/model/logging_honeycomb.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_honeycomb_all_of.py` & `fastly-1.3.1/fastly/model/logging_honeycomb_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_honeycomb_response.py` & `fastly-1.3.1/fastly/model/logging_honeycomb_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_https.py` & `fastly-1.3.1/fastly/model/logging_https.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_https_all_of.py` & `fastly-1.3.1/fastly/model/logging_https_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_https_response.py` & `fastly-1.3.1/fastly/model/logging_https_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_kafka.py` & `fastly-1.3.1/fastly/model/logging_kafka.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_kafka_all_of.py` & `fastly-1.3.1/fastly/model/logging_kafka_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_kafka_response.py` & `fastly-1.3.1/fastly/model/logging_kafka_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_kinesis.py` & `fastly-1.3.1/fastly/model/logging_kinesis.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_kinesis_response.py` & `fastly-1.3.1/fastly/model/logging_kinesis_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_logentries.py` & `fastly-1.3.1/fastly/model/logging_logentries.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_logentries_all_of.py` & `fastly-1.3.1/fastly/model/logging_logentries_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_logentries_response.py` & `fastly-1.3.1/fastly/model/logging_logentries_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_loggly.py` & `fastly-1.3.1/fastly/model/logging_loggly.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_loggly_all_of.py` & `fastly-1.3.1/fastly/model/logging_loggly_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_loggly_response.py` & `fastly-1.3.1/fastly/model/logging_loggly_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_logshuttle.py` & `fastly-1.3.1/fastly/model/logging_logshuttle.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_logshuttle_all_of.py` & `fastly-1.3.1/fastly/model/logging_logshuttle_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_logshuttle_response.py` & `fastly-1.3.1/fastly/model/logging_logshuttle_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_message_type.py` & `fastly-1.3.1/fastly/model/logging_message_type.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_newrelic.py` & `fastly-1.3.1/fastly/model/logging_newrelic.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_newrelic_all_of.py` & `fastly-1.3.1/fastly/model/logging_newrelic_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_newrelic_response.py` & `fastly-1.3.1/fastly/model/logging_newrelic_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_openstack.py` & `fastly-1.3.1/fastly/model/logging_openstack.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_openstack_all_of.py` & `fastly-1.3.1/fastly/model/logging_openstack_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_openstack_response.py` & `fastly-1.3.1/fastly/model/logging_openstack_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_papertrail.py` & `fastly-1.3.1/fastly/model/logging_papertrail.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_papertrail_response.py` & `fastly-1.3.1/fastly/model/logging_papertrail_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_placement.py` & `fastly-1.3.1/fastly/model/logging_placement.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_request_caps_common.py` & `fastly-1.3.1/fastly/model/logging_request_caps_common.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_s3.py` & `fastly-1.3.1/fastly/model/logging_s3.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_s3_all_of.py` & `fastly-1.3.1/fastly/model/logging_s3_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_s3_response.py` & `fastly-1.3.1/fastly/model/logging_s3_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_scalyr.py` & `fastly-1.3.1/fastly/model/logging_scalyr.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_scalyr_all_of.py` & `fastly-1.3.1/fastly/model/logging_scalyr_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_scalyr_response.py` & `fastly-1.3.1/fastly/model/logging_scalyr_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_sftp.py` & `fastly-1.3.1/fastly/model/logging_sftp.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_sftp_all_of.py` & `fastly-1.3.1/fastly/model/logging_sftp_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_sftp_response.py` & `fastly-1.3.1/fastly/model/logging_sftp_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_splunk.py` & `fastly-1.3.1/fastly/model/logging_splunk.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_splunk_all_of.py` & `fastly-1.3.1/fastly/model/logging_splunk_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_splunk_response.py` & `fastly-1.3.1/fastly/model/logging_splunk_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_sumologic.py` & `fastly-1.3.1/fastly/model/logging_sumologic.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_sumologic_all_of.py` & `fastly-1.3.1/fastly/model/logging_sumologic_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_sumologic_response.py` & `fastly-1.3.1/fastly/model/logging_sumologic_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_syslog.py` & `fastly-1.3.1/fastly/model/logging_syslog.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_syslog_all_of.py` & `fastly-1.3.1/fastly/model/logging_syslog_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_syslog_response.py` & `fastly-1.3.1/fastly/model/logging_syslog_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_tls_common.py` & `fastly-1.3.1/fastly/model/logging_tls_common.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/logging_use_tls.py` & `fastly-1.3.1/fastly/model/logging_use_tls.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/mutual_authentication.py` & `fastly-1.3.1/fastly/model/mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/mutual_authentication_data.py` & `fastly-1.3.1/fastly/model/mutual_authentication_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/mutual_authentication_data_attributes.py` & `fastly-1.3.1/fastly/model/mutual_authentication_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/mutual_authentication_response.py` & `fastly-1.3.1/fastly/model/mutual_authentication_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/mutual_authentication_response_attributes.py` & `fastly-1.3.1/fastly/model/mutual_authentication_response_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/mutual_authentication_response_attributes_all_of.py` & `fastly-1.3.1/fastly/model/mutual_authentication_response_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/mutual_authentication_response_data.py` & `fastly-1.3.1/fastly/model/mutual_authentication_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/mutual_authentication_response_data_all_of.py` & `fastly-1.3.1/fastly/model/mutual_authentication_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/mutual_authentications_response.py` & `fastly-1.3.1/fastly/model/mutual_authentications_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/mutual_authentications_response_all_of.py` & `fastly-1.3.1/fastly/model/mutual_authentications_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/number_version.py` & `fastly-1.3.1/fastly/model/number_version.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/package.py` & `fastly-1.3.1/fastly/model/package.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/package_metadata.py` & `fastly-1.3.1/fastly/model/package_metadata.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/package_response.py` & `fastly-1.3.1/fastly/model/package_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/package_response_all_of.py` & `fastly-1.3.1/fastly/model/package_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/pagination.py` & `fastly-1.3.1/fastly/model/pagination.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/pagination_links.py` & `fastly-1.3.1/fastly/model/pagination_links.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/pagination_meta.py` & `fastly-1.3.1/fastly/model/pagination_meta.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/permission.py` & `fastly-1.3.1/fastly/model/permission.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/pool.py` & `fastly-1.3.1/fastly/model/pool.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/pool_all_of.py` & `fastly-1.3.1/fastly/model/pool_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/pool_response.py` & `fastly-1.3.1/fastly/model/pool_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/pool_response_all_of.py` & `fastly-1.3.1/fastly/model/snippet_response_all_of.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 
-class PoolResponseAllOf(ModelNormal):
+class SnippetResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -96,15 +96,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PoolResponseAllOf - a model defined in OpenAPI
+        """SnippetResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -178,15 +178,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """PoolResponseAllOf - a model defined in OpenAPI
+        """SnippetResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `fastly-1.3.0/fastly/model/pop.py` & `fastly-1.3.1/fastly/model/pop.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/pop_coordinates.py` & `fastly-1.3.1/fastly/model/pop_coordinates.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/public_ip_list.py` & `fastly-1.3.1/fastly/model/public_ip_list.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/publish_item.py` & `fastly-1.3.1/fastly/model/publish_item.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/publish_item_formats.py` & `fastly-1.3.1/fastly/model/publish_item_formats.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/publish_request.py` & `fastly-1.3.1/fastly/model/publish_request.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/purge_keys.py` & `fastly-1.3.1/fastly/model/purge_keys.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/purge_keys_response.py` & `fastly-1.3.1/fastly/model/purge_keys_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/purge_response.py` & `fastly-1.3.1/fastly/model/purge_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/rate_limiter.py` & `fastly-1.3.1/fastly/model/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/rate_limiter_response.py` & `fastly-1.3.1/fastly/model/rate_limiter_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/rate_limiter_response1.py` & `fastly-1.3.1/fastly/model/rate_limiter_response1.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/rate_limiter_response_all_of.py` & `fastly-1.3.1/fastly/model/rate_limiter_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/realtime.py` & `fastly-1.3.1/fastly/model/realtime.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/realtime_entry.py` & `fastly-1.3.1/fastly/model/realtime_entry.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/realtime_measurements.py` & `fastly-1.3.1/fastly/model/realtime_measurements.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_common_name.py` & `fastly-1.3.1/fastly/model/relationship_common_name.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_customer.py` & `fastly-1.3.1/fastly/model/relationship_customer.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_customer_customer.py` & `fastly-1.3.1/fastly/model/relationship_customer_customer.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_member_customer.py` & `fastly-1.3.1/fastly/model/relationship_member_customer.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_member_mutual_authentication.py` & `fastly-1.3.1/fastly/model/relationship_member_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_member_service.py` & `fastly-1.3.1/fastly/model/relationship_member_service.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_member_service_invitation.py` & `fastly-1.3.1/fastly/model/relationship_member_service_invitation.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_member_tls_activation.py` & `fastly-1.3.1/fastly/model/relationship_member_tls_activation.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_member_tls_bulk_certificate.py` & `fastly-1.3.1/fastly/model/relationship_member_tls_bulk_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_member_tls_certificate.py` & `fastly-1.3.1/fastly/model/relationship_member_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_member_tls_configuration.py` & `fastly-1.3.1/fastly/model/relationship_member_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_member_tls_dns_record.py` & `fastly-1.3.1/fastly/model/relationship_member_tls_dns_record.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_member_tls_domain.py` & `fastly-1.3.1/fastly/model/relationship_member_tls_domain.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_member_tls_private_key.py` & `fastly-1.3.1/fastly/model/relationship_member_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_member_tls_subscription.py` & `fastly-1.3.1/fastly/model/relationship_member_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_member_waf_active_rule.py` & `fastly-1.3.1/fastly/model/relationship_member_waf_active_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_member_waf_firewall.py` & `fastly-1.3.1/fastly/model/relationship_member_waf_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.type_waf_firewall import TypeWafFirewall
-    globals()['TypeWafFirewall'] = TypeWafFirewall
+    from fastly.model.type_waf_tag import TypeWafTag
+    globals()['TypeWafTag'] = TypeWafTag
 
 
-class RelationshipMemberWafFirewall(ModelNormal):
+class RelationshipMemberWafTag(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -81,15 +81,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'type': (TypeWafFirewall,),  # noqa: E501
+            'type': (TypeWafTag,),  # noqa: E501
             'id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -104,15 +104,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RelationshipMemberWafFirewall - a model defined in OpenAPI
+        """RelationshipMemberWafTag - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,16 +137,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (TypeWafFirewall): [optional]  # noqa: E501
-            id (str): [optional]  # noqa: E501
+            type (TypeWafTag): [optional]  # noqa: E501
+            id (str): Alphanumeric string identifying a WAF tag.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -187,15 +187,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """RelationshipMemberWafFirewall - a model defined in OpenAPI
+        """RelationshipMemberWafTag - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -220,16 +220,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (TypeWafFirewall): [optional]  # noqa: E501
-            id (str): [optional]  # noqa: E501
+            type (TypeWafTag): [optional]  # noqa: E501
+            id (str): Alphanumeric string identifying a WAF tag.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/relationship_member_waf_firewall_version.py` & `fastly-1.3.1/fastly/model/relationship_member_waf_firewall_version.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_member_waf_rule.py` & `fastly-1.3.1/fastly/model/relationship_member_waf_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_member_waf_rule_revision.py` & `fastly-1.3.1/fastly/model/relationship_member_waf_rule_revision.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_member_waf_tag.py` & `fastly-1.3.1/fastly/model/service_authorization_data_relationships_user_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.type_waf_tag import TypeWafTag
-    globals()['TypeWafTag'] = TypeWafTag
+    from fastly.model.type_user import TypeUser
+    globals()['TypeUser'] = TypeUser
 
 
-class RelationshipMemberWafTag(ModelNormal):
+class ServiceAuthorizationDataRelationshipsUserData(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -81,15 +81,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'type': (TypeWafTag,),  # noqa: E501
+            'type': (TypeUser,),  # noqa: E501
             'id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -104,15 +104,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RelationshipMemberWafTag - a model defined in OpenAPI
+        """ServiceAuthorizationDataRelationshipsUserData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,16 +137,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (TypeWafTag): [optional]  # noqa: E501
-            id (str): Alphanumeric string identifying a WAF tag.. [optional]  # noqa: E501
+            type (TypeUser): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -187,15 +187,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """RelationshipMemberWafTag - a model defined in OpenAPI
+        """ServiceAuthorizationDataRelationshipsUserData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -220,16 +220,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (TypeWafTag): [optional]  # noqa: E501
-            id (str): Alphanumeric string identifying a WAF tag.. [optional]  # noqa: E501
+            type (TypeUser): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/relationship_mutual_authentication.py` & `fastly-1.3.1/fastly/model/relationship_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_mutual_authentication_mutual_authentication.py` & `fastly-1.3.1/fastly/model/relationship_mutual_authentication_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_mutual_authentications.py` & `fastly-1.3.1/fastly/model/relationship_mutual_authentications.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_mutual_authentications_mutual_authentications.py` & `fastly-1.3.1/fastly/model/relationship_mutual_authentications_mutual_authentications.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_service.py` & `fastly-1.3.1/fastly/model/relationship_service.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_service_invitations.py` & `fastly-1.3.1/fastly/model/relationship_service_invitations.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_service_invitations_create.py` & `fastly-1.3.1/fastly/model/relationship_service_invitations_create.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_service_invitations_create_service_invitations.py` & `fastly-1.3.1/fastly/model/relationship_service_invitations_create_service_invitations.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_service_invitations_service_invitations.py` & `fastly-1.3.1/fastly/model/relationship_service_invitations_service_invitations.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_services.py` & `fastly-1.3.1/fastly/model/relationship_services.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_services_services.py` & `fastly-1.3.1/fastly/model/relationship_services_services.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_activation.py` & `fastly-1.3.1/fastly/model/relationship_tls_activation.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_activation_tls_activation.py` & `fastly-1.3.1/fastly/model/relationship_tls_activation_tls_activation.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_activations.py` & `fastly-1.3.1/fastly/model/relationship_tls_activations.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_bulk_certificate.py` & `fastly-1.3.1/fastly/model/relationship_tls_bulk_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_bulk_certificate_tls_bulk_certificate.py` & `fastly-1.3.1/fastly/model/relationship_tls_bulk_certificate_tls_bulk_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_bulk_certificates.py` & `fastly-1.3.1/fastly/model/relationship_tls_bulk_certificates.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_certificate.py` & `fastly-1.3.1/fastly/model/relationship_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_certificate_tls_certificate.py` & `fastly-1.3.1/fastly/model/relationship_tls_certificate_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_certificates.py` & `fastly-1.3.1/fastly/model/relationship_tls_certificates.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_certificates_tls_certificates.py` & `fastly-1.3.1/fastly/model/relationship_tls_certificates_tls_certificates.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_configuration.py` & `fastly-1.3.1/fastly/model/relationship_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_configuration_tls_configuration.py` & `fastly-1.3.1/fastly/model/relationship_tls_configuration_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_configurations.py` & `fastly-1.3.1/fastly/model/relationship_tls_configurations.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_configurations_tls_configurations.py` & `fastly-1.3.1/fastly/model/relationship_tls_configurations_tls_configurations.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_dns_record.py` & `fastly-1.3.1/fastly/model/relationship_tls_dns_record.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_dns_record_dns_record.py` & `fastly-1.3.1/fastly/model/relationship_tls_dns_record_dns_record.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_dns_records.py` & `fastly-1.3.1/fastly/model/relationship_tls_dns_records.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_domain.py` & `fastly-1.3.1/fastly/model/relationship_tls_domain.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_domain_tls_domain.py` & `fastly-1.3.1/fastly/model/relationship_tls_domain_tls_domain.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_domains.py` & `fastly-1.3.1/fastly/model/relationship_tls_domains.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_domains_tls_domains.py` & `fastly-1.3.1/fastly/model/relationship_tls_domains_tls_domains.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_private_key.py` & `fastly-1.3.1/fastly/model/relationship_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_private_key_tls_private_key.py` & `fastly-1.3.1/fastly/model/relationship_tls_private_key_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_private_keys.py` & `fastly-1.3.1/fastly/model/relationship_tls_private_keys.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_private_keys_tls_private_keys.py` & `fastly-1.3.1/fastly/model/relationship_tls_private_keys_tls_private_keys.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_subscription.py` & `fastly-1.3.1/fastly/model/relationship_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_subscription_tls_subscription.py` & `fastly-1.3.1/fastly/model/relationship_tls_subscription_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_tls_subscriptions.py` & `fastly-1.3.1/fastly/model/relationship_tls_subscriptions.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_user.py` & `fastly-1.3.1/fastly/model/relationship_user.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_user_user.py` & `fastly-1.3.1/fastly/model/relationship_user_user.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_waf_active_rules.py` & `fastly-1.3.1/fastly/model/relationship_waf_active_rules.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_waf_active_rules_waf_active_rules.py` & `fastly-1.3.1/fastly/model/relationship_waf_active_rules_waf_active_rules.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_waf_firewall.py` & `fastly-1.3.1/fastly/model/relationship_waf_firewall.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_waf_firewall_version.py` & `fastly-1.3.1/fastly/model/relationship_waf_firewall_version.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_waf_firewall_version_waf_firewall_version.py` & `fastly-1.3.1/fastly/model/relationship_waf_firewall_version_waf_firewall_version.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_waf_firewall_versions.py` & `fastly-1.3.1/fastly/model/relationship_waf_firewall_versions.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_waf_firewall_waf_firewall.py` & `fastly-1.3.1/fastly/model/relationship_waf_firewall_waf_firewall.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_waf_rule.py` & `fastly-1.3.1/fastly/model/relationship_waf_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_waf_rule_revision.py` & `fastly-1.3.1/fastly/model/relationship_waf_rule_revision.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_waf_rule_revision_waf_rule_revisions.py` & `fastly-1.3.1/fastly/model/relationship_waf_rule_revision_waf_rule_revisions.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_waf_rule_revisions.py` & `fastly-1.3.1/fastly/model/relationship_waf_rule_revisions.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_waf_rule_waf_rule.py` & `fastly-1.3.1/fastly/model/relationship_waf_rule_waf_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_waf_rules.py` & `fastly-1.3.1/fastly/model/relationship_waf_rules.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_waf_tags.py` & `fastly-1.3.1/fastly/model/relationship_waf_tags.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationship_waf_tags_waf_tags.py` & `fastly-1.3.1/fastly/model/relationship_waf_tags_waf_tags.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationships_for_invitation.py` & `fastly-1.3.1/fastly/model/relationships_for_invitation.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationships_for_mutual_authentication.py` & `fastly-1.3.1/fastly/model/relationships_for_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationships_for_star.py` & `fastly-1.3.1/fastly/model/relationships_for_star.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationships_for_tls_activation.py` & `fastly-1.3.1/fastly/model/relationships_for_tls_activation.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationships_for_tls_bulk_certificate.py` & `fastly-1.3.1/fastly/model/relationships_for_tls_bulk_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationships_for_tls_configuration.py` & `fastly-1.3.1/fastly/model/relationships_for_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationships_for_tls_csr.py` & `fastly-1.3.1/fastly/model/relationships_for_tls_private_key.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,21 +26,23 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.relationship_tls_private_key import RelationshipTlsPrivateKey
-    from fastly.model.relationship_tls_private_key_tls_private_key import RelationshipTlsPrivateKeyTlsPrivateKey
-    globals()['RelationshipTlsPrivateKey'] = RelationshipTlsPrivateKey
-    globals()['RelationshipTlsPrivateKeyTlsPrivateKey'] = RelationshipTlsPrivateKeyTlsPrivateKey
+    from fastly.model.relationship_tls_activation_tls_activation import RelationshipTlsActivationTlsActivation
+    from fastly.model.relationship_tls_activations import RelationshipTlsActivations
+    from fastly.model.relationship_tls_domains_tls_domains import RelationshipTlsDomainsTlsDomains
+    globals()['RelationshipTlsActivationTlsActivation'] = RelationshipTlsActivationTlsActivation
+    globals()['RelationshipTlsActivations'] = RelationshipTlsActivations
+    globals()['RelationshipTlsDomainsTlsDomains'] = RelationshipTlsDomainsTlsDomains
 
 
-class RelationshipsForTlsCsr(ModelComposed):
+class RelationshipsForTlsPrivateKey(ModelComposed):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -83,33 +85,35 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'tls_private_key': (RelationshipTlsPrivateKeyTlsPrivateKey,),  # noqa: E501
+            'tls_activations': (RelationshipTlsActivationTlsActivation,),  # noqa: E501
+            'tls_domains': (RelationshipTlsDomainsTlsDomains,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'tls_private_key': 'tls_private_key',  # noqa: E501
+        'tls_activations': 'tls_activations',  # noqa: E501
+        'tls_domains': 'tls_domains',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RelationshipsForTlsCsr - a model defined in OpenAPI
+        """RelationshipsForTlsPrivateKey - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            tls_private_key (RelationshipTlsPrivateKeyTlsPrivateKey): [optional]  # noqa: E501
+            tls_activations (RelationshipTlsActivationTlsActivation): [optional]  # noqa: E501
+            tls_domains (RelationshipTlsDomainsTlsDomains): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -201,15 +206,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """RelationshipsForTlsCsr - a model defined in OpenAPI
+        """RelationshipsForTlsPrivateKey - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -234,15 +239,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            tls_private_key (RelationshipTlsPrivateKeyTlsPrivateKey): [optional]  # noqa: E501
+            tls_activations (RelationshipTlsActivationTlsActivation): [optional]  # noqa: E501
+            tls_domains (RelationshipTlsDomainsTlsDomains): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -298,14 +304,15 @@
         # level we would get an error because the class level
         # code would be run when this module is imported, and these composed
         # classes don't exist yet because their module has not finished
         # loading
         lazy_import()
         return {
           'anyOf': [
-              RelationshipTlsPrivateKey,
+              RelationshipTlsActivations,
+              bool, date, datetime, dict, float, int, list, str, none_type,
           ],
           'allOf': [
           ],
           'oneOf': [
           ],
         }
```

### Comparing `fastly-1.3.0/fastly/model/relationships_for_tls_domain.py` & `fastly-1.3.1/fastly/model/relationships_for_tls_domain.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationships_for_tls_private_key.py` & `fastly-1.3.1/fastly/model/relationships_for_tls_subscription.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,23 +26,27 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.relationship_tls_activation_tls_activation import RelationshipTlsActivationTlsActivation
-    from fastly.model.relationship_tls_activations import RelationshipTlsActivations
+    from fastly.model.relationship_tls_certificates import RelationshipTlsCertificates
+    from fastly.model.relationship_tls_certificates_tls_certificates import RelationshipTlsCertificatesTlsCertificates
+    from fastly.model.relationship_tls_configuration_tls_configuration import RelationshipTlsConfigurationTlsConfiguration
+    from fastly.model.relationship_tls_domains import RelationshipTlsDomains
     from fastly.model.relationship_tls_domains_tls_domains import RelationshipTlsDomainsTlsDomains
-    globals()['RelationshipTlsActivationTlsActivation'] = RelationshipTlsActivationTlsActivation
-    globals()['RelationshipTlsActivations'] = RelationshipTlsActivations
+    globals()['RelationshipTlsCertificates'] = RelationshipTlsCertificates
+    globals()['RelationshipTlsCertificatesTlsCertificates'] = RelationshipTlsCertificatesTlsCertificates
+    globals()['RelationshipTlsConfigurationTlsConfiguration'] = RelationshipTlsConfigurationTlsConfiguration
+    globals()['RelationshipTlsDomains'] = RelationshipTlsDomains
     globals()['RelationshipTlsDomainsTlsDomains'] = RelationshipTlsDomainsTlsDomains
 
 
-class RelationshipsForTlsPrivateKey(ModelComposed):
+class RelationshipsForTlsSubscription(ModelComposed):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -85,35 +89,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'tls_activations': (RelationshipTlsActivationTlsActivation,),  # noqa: E501
             'tls_domains': (RelationshipTlsDomainsTlsDomains,),  # noqa: E501
+            'tls_certificates': (RelationshipTlsCertificatesTlsCertificates,),  # noqa: E501
+            'tls_configuration': (RelationshipTlsConfigurationTlsConfiguration,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'tls_activations': 'tls_activations',  # noqa: E501
         'tls_domains': 'tls_domains',  # noqa: E501
+        'tls_certificates': 'tls_certificates',  # noqa: E501
+        'tls_configuration': 'tls_configuration',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RelationshipsForTlsPrivateKey - a model defined in OpenAPI
+        """RelationshipsForTlsSubscription - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,16 +144,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            tls_activations (RelationshipTlsActivationTlsActivation): [optional]  # noqa: E501
             tls_domains (RelationshipTlsDomainsTlsDomains): [optional]  # noqa: E501
+            tls_certificates (RelationshipTlsCertificatesTlsCertificates): [optional]  # noqa: E501
+            tls_configuration (RelationshipTlsConfigurationTlsConfiguration): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -206,15 +213,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """RelationshipsForTlsPrivateKey - a model defined in OpenAPI
+        """RelationshipsForTlsSubscription - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -239,16 +246,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            tls_activations (RelationshipTlsActivationTlsActivation): [optional]  # noqa: E501
             tls_domains (RelationshipTlsDomainsTlsDomains): [optional]  # noqa: E501
+            tls_certificates (RelationshipTlsCertificatesTlsCertificates): [optional]  # noqa: E501
+            tls_configuration (RelationshipTlsConfigurationTlsConfiguration): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -304,15 +312,16 @@
         # level we would get an error because the class level
         # code would be run when this module is imported, and these composed
         # classes don't exist yet because their module has not finished
         # loading
         lazy_import()
         return {
           'anyOf': [
-              RelationshipTlsActivations,
+              RelationshipTlsCertificates,
+              RelationshipTlsDomains,
               bool, date, datetime, dict, float, int, list, str, none_type,
           ],
           'allOf': [
           ],
           'oneOf': [
           ],
         }
```

### Comparing `fastly-1.3.0/fastly/model/relationships_for_tls_subscription.py` & `fastly-1.3.1/fastly/model/tls_domains_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,27 +26,27 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.relationship_tls_certificates import RelationshipTlsCertificates
-    from fastly.model.relationship_tls_certificates_tls_certificates import RelationshipTlsCertificatesTlsCertificates
-    from fastly.model.relationship_tls_configuration_tls_configuration import RelationshipTlsConfigurationTlsConfiguration
-    from fastly.model.relationship_tls_domains import RelationshipTlsDomains
-    from fastly.model.relationship_tls_domains_tls_domains import RelationshipTlsDomainsTlsDomains
-    globals()['RelationshipTlsCertificates'] = RelationshipTlsCertificates
-    globals()['RelationshipTlsCertificatesTlsCertificates'] = RelationshipTlsCertificatesTlsCertificates
-    globals()['RelationshipTlsConfigurationTlsConfiguration'] = RelationshipTlsConfigurationTlsConfiguration
-    globals()['RelationshipTlsDomains'] = RelationshipTlsDomains
-    globals()['RelationshipTlsDomainsTlsDomains'] = RelationshipTlsDomainsTlsDomains
+    from fastly.model.pagination import Pagination
+    from fastly.model.pagination_links import PaginationLinks
+    from fastly.model.pagination_meta import PaginationMeta
+    from fastly.model.tls_domain_data import TlsDomainData
+    from fastly.model.tls_domains_response_all_of import TlsDomainsResponseAllOf
+    globals()['Pagination'] = Pagination
+    globals()['PaginationLinks'] = PaginationLinks
+    globals()['PaginationMeta'] = PaginationMeta
+    globals()['TlsDomainData'] = TlsDomainData
+    globals()['TlsDomainsResponseAllOf'] = TlsDomainsResponseAllOf
 
 
-class RelationshipsForTlsSubscription(ModelComposed):
+class TlsDomainsResponse(ModelComposed):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -89,37 +89,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'tls_domains': (RelationshipTlsDomainsTlsDomains,),  # noqa: E501
-            'tls_certificates': (RelationshipTlsCertificatesTlsCertificates,),  # noqa: E501
-            'tls_configuration': (RelationshipTlsConfigurationTlsConfiguration,),  # noqa: E501
+            'links': (PaginationLinks,),  # noqa: E501
+            'meta': (PaginationMeta,),  # noqa: E501
+            'data': ([TlsDomainData],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'tls_domains': 'tls_domains',  # noqa: E501
-        'tls_certificates': 'tls_certificates',  # noqa: E501
-        'tls_configuration': 'tls_configuration',  # noqa: E501
+        'links': 'links',  # noqa: E501
+        'meta': 'meta',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RelationshipsForTlsSubscription - a model defined in OpenAPI
+        """TlsDomainsResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -144,17 +144,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            tls_domains (RelationshipTlsDomainsTlsDomains): [optional]  # noqa: E501
-            tls_certificates (RelationshipTlsCertificatesTlsCertificates): [optional]  # noqa: E501
-            tls_configuration (RelationshipTlsConfigurationTlsConfiguration): [optional]  # noqa: E501
+            links (PaginationLinks): [optional]  # noqa: E501
+            meta (PaginationMeta): [optional]  # noqa: E501
+            data ([TlsDomainData]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -213,15 +213,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """RelationshipsForTlsSubscription - a model defined in OpenAPI
+        """TlsDomainsResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -246,17 +246,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            tls_domains (RelationshipTlsDomainsTlsDomains): [optional]  # noqa: E501
-            tls_certificates (RelationshipTlsCertificatesTlsCertificates): [optional]  # noqa: E501
-            tls_configuration (RelationshipTlsConfigurationTlsConfiguration): [optional]  # noqa: E501
+            links (PaginationLinks): [optional]  # noqa: E501
+            meta (PaginationMeta): [optional]  # noqa: E501
+            data ([TlsDomainData]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -312,16 +312,15 @@
         # level we would get an error because the class level
         # code would be run when this module is imported, and these composed
         # classes don't exist yet because their module has not finished
         # loading
         lazy_import()
         return {
           'anyOf': [
-              RelationshipTlsCertificates,
-              RelationshipTlsDomains,
-              bool, date, datetime, dict, float, int, list, str, none_type,
           ],
           'allOf': [
+              Pagination,
+              TlsDomainsResponseAllOf,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `fastly-1.3.0/fastly/model/relationships_for_waf_active_rule.py` & `fastly-1.3.1/fastly/model/relationships_for_waf_active_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationships_for_waf_exclusion.py` & `fastly-1.3.1/fastly/model/relationships_for_waf_exclusion.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationships_for_waf_firewall_version.py` & `fastly-1.3.1/fastly/model/relationships_for_waf_firewall_version.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/relationships_for_waf_rule.py` & `fastly-1.3.1/fastly/model/relationships_for_waf_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/request_settings.py` & `fastly-1.3.1/fastly/model/request_settings.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/request_settings_response.py` & `fastly-1.3.1/fastly/model/request_settings_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/resource.py` & `fastly-1.3.1/fastly/model/resource.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/resource_response.py` & `fastly-1.3.1/fastly/model/resource_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/resource_response_all_of.py` & `fastly-1.3.1/fastly/model/resource_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/response_object.py` & `fastly-1.3.1/fastly/model/response_object.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/response_object_response.py` & `fastly-1.3.1/fastly/model/response_object_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/results.py` & `fastly-1.3.1/fastly/model/results.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/role_user.py` & `fastly-1.3.1/fastly/model/role_user.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/schemas_contact_response.py` & `fastly-1.3.1/fastly/model/schemas_contact_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/schemas_snippet_response.py` & `fastly-1.3.1/fastly/model/schemas_snippet_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/schemas_user_response.py` & `fastly-1.3.1/fastly/model/schemas_user_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/schemas_vcl_response.py` & `fastly-1.3.1/fastly/model/schemas_vcl_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/schemas_version.py` & `fastly-1.3.1/fastly/model/schemas_version.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/schemas_version_response.py` & `fastly-1.3.1/fastly/model/schemas_version_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/schemas_waf_firewall_version.py` & `fastly-1.3.1/fastly/model/schemas_waf_firewall_version.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/schemas_waf_firewall_version_data.py` & `fastly-1.3.1/fastly/model/schemas_waf_firewall_version_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/server.py` & `fastly-1.3.1/fastly/model/server.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/server_response.py` & `fastly-1.3.1/fastly/model/server_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/server_response_all_of.py` & `fastly-1.3.1/fastly/model/server_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service.py` & `fastly-1.3.1/fastly/model/service.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_authorization.py` & `fastly-1.3.1/fastly/model/service_authorization.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_authorization_data.py` & `fastly-1.3.1/fastly/model/service_authorization_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_authorization_data_attributes.py` & `fastly-1.3.1/fastly/model/service_authorization_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_authorization_data_relationships.py` & `fastly-1.3.1/fastly/model/service_authorization_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_authorization_data_relationships_user.py` & `fastly-1.3.1/fastly/model/service_authorization_data_relationships_user.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_authorization_data_relationships_user_data.py` & `fastly-1.3.1/fastly/model/service_authorization_response_data_all_of.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.type_user import TypeUser
-    globals()['TypeUser'] = TypeUser
+    from fastly.model.timestamps import Timestamps
+    globals()['Timestamps'] = Timestamps
 
 
-class ServiceAuthorizationDataRelationshipsUserData(ModelNormal):
+class ServiceAuthorizationResponseDataAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -81,38 +81,38 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'type': (TypeUser,),  # noqa: E501
             'id': (str,),  # noqa: E501
+            'attributes': (Timestamps,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'type': 'type',  # noqa: E501
         'id': 'id',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
         'id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ServiceAuthorizationDataRelationshipsUserData - a model defined in OpenAPI
+        """ServiceAuthorizationResponseDataAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,16 +137,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (TypeUser): [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
+            attributes (Timestamps): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -187,15 +187,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ServiceAuthorizationDataRelationshipsUserData - a model defined in OpenAPI
+        """ServiceAuthorizationResponseDataAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -220,16 +220,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (TypeUser): [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
+            attributes (Timestamps): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/service_authorization_response.py` & `fastly-1.3.1/fastly/model/service_authorization_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_authorization_response_data.py` & `fastly-1.3.1/fastly/model/service_authorization_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_authorization_response_data_all_of.py` & `fastly-1.3.1/fastly/model/service_invitation_response_all_of_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 def lazy_import():
     from fastly.model.timestamps import Timestamps
     globals()['Timestamps'] = Timestamps
 
 
-class ServiceAuthorizationResponseDataAllOf(ModelNormal):
+class ServiceInvitationResponseAllOfData(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -104,15 +104,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ServiceAuthorizationResponseDataAllOf - a model defined in OpenAPI
+        """ServiceInvitationResponseAllOfData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -187,15 +187,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ServiceAuthorizationResponseDataAllOf - a model defined in OpenAPI
+        """ServiceInvitationResponseAllOfData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `fastly-1.3.0/fastly/model/service_authorizations_response.py` & `fastly-1.3.1/fastly/model/service_authorizations_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_authorizations_response_all_of.py` & `fastly-1.3.1/fastly/model/service_authorizations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_create.py` & `fastly-1.3.1/fastly/model/service_create.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_create_all_of.py` & `fastly-1.3.1/fastly/model/service_create_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_detail.py` & `fastly-1.3.1/fastly/model/service_detail.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_detail_all_of.py` & `fastly-1.3.1/fastly/model/service_detail_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_id_and_version.py` & `fastly-1.3.1/fastly/model/service_id_and_version.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_invitation.py` & `fastly-1.3.1/fastly/model/service_invitation.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_invitation_data.py` & `fastly-1.3.1/fastly/model/service_invitation_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_invitation_data_attributes.py` & `fastly-1.3.1/fastly/model/service_invitation_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_invitation_data_relationships.py` & `fastly-1.3.1/fastly/model/service_invitation_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_invitation_response.py` & `fastly-1.3.1/fastly/model/service_invitation_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_invitation_response_all_of.py` & `fastly-1.3.1/fastly/model/service_invitation_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_invitation_response_all_of_data.py` & `fastly-1.3.1/fastly/model/tls_subscription_response_attributes_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from fastly.model.timestamps import Timestamps
-    globals()['Timestamps'] = Timestamps
 
-
-class ServiceInvitationResponseAllOfData(ModelNormal):
+class TlsSubscriptionResponseAttributesAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -53,66 +49,68 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('state',): {
+            'PENDING': "pending",
+            'PROCESSING': "processing",
+            'ISSUED': "issued",
+            'RENEWING': "renewing",
+            'FAILED': "failed",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'id': (str,),  # noqa: E501
-            'attributes': (Timestamps,),  # noqa: E501
+            'state': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'attributes': 'attributes',  # noqa: E501
+        'state': 'state',  # noqa: E501
     }
 
     read_only_vars = {
-        'id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ServiceInvitationResponseAllOfData - a model defined in OpenAPI
+        """TlsSubscriptionResponseAttributesAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,16 +135,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            attributes (Timestamps): [optional]  # noqa: E501
+            state (str): The current state of your subscription.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -187,15 +184,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ServiceInvitationResponseAllOfData - a model defined in OpenAPI
+        """TlsSubscriptionResponseAttributesAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -220,16 +217,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            attributes (Timestamps): [optional]  # noqa: E501
+            state (str): The current state of your subscription.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/service_list_response.py` & `fastly-1.3.1/fastly/model/service_list_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_list_response_all_of.py` & `fastly-1.3.1/fastly/model/service_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_response.py` & `fastly-1.3.1/fastly/model/service_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_response_all_of.py` & `fastly-1.3.1/fastly/model/service_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_version_detail.py` & `fastly-1.3.1/fastly/model/service_version_detail.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/service_version_detail_or_null.py` & `fastly-1.3.1/fastly/model/service_version_detail_or_null.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/settings.py` & `fastly-1.3.1/fastly/model/settings.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/settings_response.py` & `fastly-1.3.1/fastly/model/settings_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/snippet.py` & `fastly-1.3.1/fastly/model/snippet.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/snippet_response.py` & `fastly-1.3.1/fastly/model/snippet_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/snippet_response_all_of.py` & `fastly-1.3.1/fastly/model/tls_configuration_data_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 
-class SnippetResponseAllOf(ModelNormal):
+class TlsConfigurationDataAttributes(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -75,36 +75,35 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (str,),  # noqa: E501
+            'name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
+        'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
-        'id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SnippetResponseAllOf - a model defined in OpenAPI
+        """TlsConfigurationDataAttributes - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -129,15 +128,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
+            name (str): A custom name for your TLS configuration.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -178,15 +177,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SnippetResponseAllOf - a model defined in OpenAPI
+        """TlsConfigurationDataAttributes - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -211,15 +210,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
+            name (str): A custom name for your TLS configuration.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/star.py` & `fastly-1.3.1/fastly/model/star.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/star_data.py` & `fastly-1.3.1/fastly/model/star_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/star_response.py` & `fastly-1.3.1/fastly/model/star_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/star_response_all_of.py` & `fastly-1.3.1/fastly/model/star_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/stats.py` & `fastly-1.3.1/fastly/model/stats.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/store.py` & `fastly-1.3.1/fastly/model/store.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/store_response.py` & `fastly-1.3.1/fastly/model/store_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/timestamps.py` & `fastly-1.3.1/fastly/model/timestamps.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/timestamps_no_delete.py` & `fastly-1.3.1/fastly/model/timestamps_no_delete.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_activation.py` & `fastly-1.3.1/fastly/model/tls_activation.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_activation_data.py` & `fastly-1.3.1/fastly/model/tls_activation_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_activation_response.py` & `fastly-1.3.1/fastly/model/tls_activation_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_activation_response_data.py` & `fastly-1.3.1/fastly/model/tls_activation_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_activation_response_data_all_of.py` & `fastly-1.3.1/fastly/model/tls_activation_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_activations_response.py` & `fastly-1.3.1/fastly/model/tls_activations_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_activations_response_all_of.py` & `fastly-1.3.1/fastly/model/tls_activations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_bulk_certificate.py` & `fastly-1.3.1/fastly/model/tls_bulk_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_bulk_certificate_data.py` & `fastly-1.3.1/fastly/model/tls_bulk_certificate_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_bulk_certificate_data_attributes.py` & `fastly-1.3.1/fastly/model/tls_bulk_certificate_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_bulk_certificate_response.py` & `fastly-1.3.1/fastly/model/tls_bulk_certificate_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_bulk_certificate_response_attributes.py` & `fastly-1.3.1/fastly/model/tls_bulk_certificate_response_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_bulk_certificate_response_attributes_all_of.py` & `fastly-1.3.1/fastly/model/tls_bulk_certificate_response_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_bulk_certificate_response_data.py` & `fastly-1.3.1/fastly/model/tls_bulk_certificate_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_bulk_certificate_response_data_all_of.py` & `fastly-1.3.1/fastly/model/tls_bulk_certificate_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_bulk_certificates_response.py` & `fastly-1.3.1/fastly/model/tls_bulk_certificates_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_bulk_certificates_response_all_of.py` & `fastly-1.3.1/fastly/model/tls_bulk_certificates_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_certificate.py` & `fastly-1.3.1/fastly/model/tls_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_certificate_data.py` & `fastly-1.3.1/fastly/model/tls_certificate_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_certificate_data_attributes.py` & `fastly-1.3.1/fastly/model/tls_certificate_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_certificate_response.py` & `fastly-1.3.1/fastly/model/tls_certificate_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_certificate_response_attributes.py` & `fastly-1.3.1/fastly/model/tls_certificate_response_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_certificate_response_attributes_all_of.py` & `fastly-1.3.1/fastly/model/tls_certificate_response_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_certificate_response_data.py` & `fastly-1.3.1/fastly/model/tls_certificate_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_certificate_response_data_all_of.py` & `fastly-1.3.1/fastly/model/tls_certificate_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_certificates_response.py` & `fastly-1.3.1/fastly/model/tls_certificates_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_certificates_response_all_of.py` & `fastly-1.3.1/fastly/model/tls_certificates_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_common.py` & `fastly-1.3.1/fastly/model/tls_common.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_configuration.py` & `fastly-1.3.1/fastly/model/tls_configuration.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_configuration_data.py` & `fastly-1.3.1/fastly/model/tls_configuration_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_configuration_data_attributes.py` & `fastly-1.3.1/fastly/model/waf_tag_attributes.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 
-class TlsConfigurationDataAttributes(ModelNormal):
+class WafTagAttributes(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -88,22 +88,23 @@
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
+        'name',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TlsConfigurationDataAttributes - a model defined in OpenAPI
+        """WafTagAttributes - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -128,15 +129,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): A custom name for your TLS configuration.. [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -177,15 +178,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TlsConfigurationDataAttributes - a model defined in OpenAPI
+        """WafTagAttributes - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -210,15 +211,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): A custom name for your TLS configuration.. [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/tls_configuration_response.py` & `fastly-1.3.1/fastly/model/tls_configuration_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_configuration_response_attributes.py` & `fastly-1.3.1/fastly/model/tls_configuration_response_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_configuration_response_attributes_all_of.py` & `fastly-1.3.1/fastly/model/tls_configuration_response_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_configuration_response_data.py` & `fastly-1.3.1/fastly/model/tls_configuration_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_configuration_response_data_all_of.py` & `fastly-1.3.1/fastly/model/tls_configuration_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_configurations_response.py` & `fastly-1.3.1/fastly/model/tls_configurations_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_configurations_response_all_of.py` & `fastly-1.3.1/fastly/model/tls_configurations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_csr.py` & `fastly-1.3.1/fastly/model/waf_firewall.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.tls_csr_data import TlsCsrData
-    globals()['TlsCsrData'] = TlsCsrData
+    from fastly.model.waf_firewall_data import WafFirewallData
+    globals()['WafFirewallData'] = WafFirewallData
 
 
-class TlsCsr(ModelNormal):
+class WafFirewall(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -81,15 +81,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (TlsCsrData,),  # noqa: E501
+            'data': (WafFirewallData,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -101,15 +101,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TlsCsr - a model defined in OpenAPI
+        """WafFirewall - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +134,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (TlsCsrData): [optional]  # noqa: E501
+            data (WafFirewallData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TlsCsr - a model defined in OpenAPI
+        """WafFirewall - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (TlsCsrData): [optional]  # noqa: E501
+            data (WafFirewallData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/tls_csr_data.py` & `fastly-1.3.1/fastly/model/tls_subscription_response_data_all_of.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,23 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.relationships_for_tls_csr import RelationshipsForTlsCsr
-    from fastly.model.tls_csr_data_attributes import TlsCsrDataAttributes
-    from fastly.model.type_tls_csr import TypeTlsCsr
-    globals()['RelationshipsForTlsCsr'] = RelationshipsForTlsCsr
-    globals()['TlsCsrDataAttributes'] = TlsCsrDataAttributes
-    globals()['TypeTlsCsr'] = TypeTlsCsr
+    from fastly.model.tls_subscription_response_attributes import TlsSubscriptionResponseAttributes
+    globals()['TlsSubscriptionResponseAttributes'] = TlsSubscriptionResponseAttributes
 
 
-class TlsCsrData(ModelNormal):
+class TlsSubscriptionResponseDataAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -85,39 +81,38 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'type': (TypeTlsCsr,),  # noqa: E501
-            'attributes': (TlsCsrDataAttributes,),  # noqa: E501
-            'relationships': (RelationshipsForTlsCsr,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'attributes': (TlsSubscriptionResponseAttributes,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'type': 'type',  # noqa: E501
+        'id': 'id',  # noqa: E501
         'attributes': 'attributes',  # noqa: E501
-        'relationships': 'relationships',  # noqa: E501
     }
 
     read_only_vars = {
+        'id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TlsCsrData - a model defined in OpenAPI
+        """TlsSubscriptionResponseDataAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,17 +137,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (TypeTlsCsr): [optional]  # noqa: E501
-            attributes (TlsCsrDataAttributes): [optional]  # noqa: E501
-            relationships (RelationshipsForTlsCsr): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            attributes (TlsSubscriptionResponseAttributes): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -193,15 +187,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TlsCsrData - a model defined in OpenAPI
+        """TlsSubscriptionResponseDataAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,17 +220,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (TypeTlsCsr): [optional]  # noqa: E501
-            attributes (TlsCsrDataAttributes): [optional]  # noqa: E501
-            relationships (RelationshipsForTlsCsr): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            attributes (TlsSubscriptionResponseAttributes): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/tls_csr_data_attributes.py` & `fastly-1.3.1/fastly/model/token_response_all_of.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 
-class TlsCsrDataAttributes(ModelNormal):
+class TokenResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -75,56 +75,50 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'sans': ([str],),  # noqa: E501
-            'common_name': (str,),  # noqa: E501
-            'country': (str,),  # noqa: E501
-            'state': (str,),  # noqa: E501
-            'city': (str,),  # noqa: E501
-            'postal_code': (str,),  # noqa: E501
-            'street_address': (str,),  # noqa: E501
-            'organization': (str,),  # noqa: E501
-            'organizational_unit': (str,),  # noqa: E501
-            'email': (str,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'user_id': (str,),  # noqa: E501
+            'created_at': (str,),  # noqa: E501
+            'last_used_at': (str,),  # noqa: E501
+            'expires_at': (str,),  # noqa: E501
+            'ip': (str,),  # noqa: E501
+            'user_agent': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'sans': 'sans',  # noqa: E501
-        'common_name': 'common_name',  # noqa: E501
-        'country': 'country',  # noqa: E501
-        'state': 'state',  # noqa: E501
-        'city': 'city',  # noqa: E501
-        'postal_code': 'postal_code',  # noqa: E501
-        'street_address': 'street_address',  # noqa: E501
-        'organization': 'organization',  # noqa: E501
-        'organizational_unit': 'organizational_unit',  # noqa: E501
-        'email': 'email',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'user_id': 'user_id',  # noqa: E501
+        'created_at': 'created_at',  # noqa: E501
+        'last_used_at': 'last_used_at',  # noqa: E501
+        'expires_at': 'expires_at',  # noqa: E501
+        'ip': 'ip',  # noqa: E501
+        'user_agent': 'user_agent',  # noqa: E501
     }
 
     read_only_vars = {
+        'id',  # noqa: E501
+        'user_id',  # noqa: E501
+        'last_used_at',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, sans, *args, **kwargs):  # noqa: E501
-        """TlsCsrDataAttributes - a model defined in OpenAPI
-
-        Args:
-            sans ([str]): Subject Altername Names - An array of one or more fully qualified domain names or public IP addresses to be secured by this certificate. Required.
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """TokenResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -149,23 +143,21 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            common_name (str): Common Name (CN) - The fully qualified domain name (FQDN) to be secured by this certificate. The common name should be one of the entries in the SANs parameter.. [optional]  # noqa: E501
-            country (str): Country (C) - The two-letter ISO country code where the organization is located.. [optional]  # noqa: E501
-            state (str): State (S) - The state, province, region, or county where the organization is located. This should not be abbreviated.. [optional]  # noqa: E501
-            city (str): Locality (L) - The locality, city, town, or village where the organization is located.. [optional]  # noqa: E501
-            postal_code (str): Postal Code - The postal code where the organization is located.. [optional]  # noqa: E501
-            street_address (str): Street Address - The street address where the organization is located.. [optional]  # noqa: E501
-            organization (str): Organization (O) - The legal name of the organization, including any suffixes. This should not be abbreviated.. [optional]  # noqa: E501
-            organizational_unit (str): Organizational Unit (OU) - The internal division of the organization managing the certificate.. [optional]  # noqa: E501
-            email (str): Email Address (EMAIL) - The organizational contact for this.. [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            user_id (str): [optional]  # noqa: E501
+            created_at (str): Time-stamp (UTC) of when the token was created.. [optional]  # noqa: E501
+            last_used_at (str): Time-stamp (UTC) of when the token was last used.. [optional]  # noqa: E501
+            expires_at (str): Time-stamp (UTC) of when the token will expire (optional).. [optional]  # noqa: E501
+            ip (str): IP Address of the client that last used the token.. [optional]  # noqa: E501
+            user_agent (str): User-Agent header of the client that last used the token.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -185,15 +177,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.sans = sans
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -206,19 +197,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, sans, *args, **kwargs):  # noqa: E501
-        """TlsCsrDataAttributes - a model defined in OpenAPI
-
-        Args:
-            sans ([str]): Subject Altername Names - An array of one or more fully qualified domain names or public IP addresses to be secured by this certificate. Required.
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """TokenResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -243,23 +231,21 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            common_name (str): Common Name (CN) - The fully qualified domain name (FQDN) to be secured by this certificate. The common name should be one of the entries in the SANs parameter.. [optional]  # noqa: E501
-            country (str): Country (C) - The two-letter ISO country code where the organization is located.. [optional]  # noqa: E501
-            state (str): State (S) - The state, province, region, or county where the organization is located. This should not be abbreviated.. [optional]  # noqa: E501
-            city (str): Locality (L) - The locality, city, town, or village where the organization is located.. [optional]  # noqa: E501
-            postal_code (str): Postal Code - The postal code where the organization is located.. [optional]  # noqa: E501
-            street_address (str): Street Address - The street address where the organization is located.. [optional]  # noqa: E501
-            organization (str): Organization (O) - The legal name of the organization, including any suffixes. This should not be abbreviated.. [optional]  # noqa: E501
-            organizational_unit (str): Organizational Unit (OU) - The internal division of the organization managing the certificate.. [optional]  # noqa: E501
-            email (str): Email Address (EMAIL) - The organizational contact for this.. [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            user_id (str): [optional]  # noqa: E501
+            created_at (str): Time-stamp (UTC) of when the token was created.. [optional]  # noqa: E501
+            last_used_at (str): Time-stamp (UTC) of when the token was last used.. [optional]  # noqa: E501
+            expires_at (str): Time-stamp (UTC) of when the token will expire (optional).. [optional]  # noqa: E501
+            ip (str): IP Address of the client that last used the token.. [optional]  # noqa: E501
+            user_agent (str): User-Agent header of the client that last used the token.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -277,15 +263,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.sans = sans
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `fastly-1.3.0/fastly/model/tls_csr_response.py` & `fastly-1.3.1/fastly/model/waf_exclusion_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.tls_csr_response_data import TlsCsrResponseData
-    globals()['TlsCsrResponseData'] = TlsCsrResponseData
+    from fastly.model.waf_exclusion_response_data import WafExclusionResponseData
+    globals()['WafExclusionResponseData'] = WafExclusionResponseData
 
 
-class TlsCsrResponse(ModelNormal):
+class WafExclusionResponse(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -81,15 +81,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (TlsCsrResponseData,),  # noqa: E501
+            'data': (WafExclusionResponseData,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -101,15 +101,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TlsCsrResponse - a model defined in OpenAPI
+        """WafExclusionResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +134,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (TlsCsrResponseData): [optional]  # noqa: E501
+            data (WafExclusionResponseData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TlsCsrResponse - a model defined in OpenAPI
+        """WafExclusionResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (TlsCsrResponseData): [optional]  # noqa: E501
+            data (WafExclusionResponseData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/tls_csr_response_attributes.py` & `fastly-1.3.1/fastly/model/tls_private_key_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fastly.model.tls_private_key_response_data import TlsPrivateKeyResponseData
+    globals()['TlsPrivateKeyResponseData'] = TlsPrivateKeyResponseData
 
-class TlsCsrResponseAttributes(ModelNormal):
+
+class TlsPrivateKeyResponse(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -60,50 +64,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'content': (str,),  # noqa: E501
+            'data': (TlsPrivateKeyResponseData,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'content': 'content',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TlsCsrResponseAttributes - a model defined in OpenAPI
+        """TlsPrivateKeyResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -128,15 +134,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            content (str): The PEM encoded CSR.. [optional]  # noqa: E501
+            data (TlsPrivateKeyResponseData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -177,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TlsCsrResponseAttributes - a model defined in OpenAPI
+        """TlsPrivateKeyResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -210,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            content (str): The PEM encoded CSR.. [optional]  # noqa: E501
+            data (TlsPrivateKeyResponseData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/tls_csr_response_data.py` & `fastly-1.3.1/fastly/model/token.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,24 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from fastly.model.relationships_for_tls_csr import RelationshipsForTlsCsr
-    from fastly.model.tls_csr_response_attributes import TlsCsrResponseAttributes
-    from fastly.model.type_tls_csr import TypeTlsCsr
-    globals()['RelationshipsForTlsCsr'] = RelationshipsForTlsCsr
-    globals()['TlsCsrResponseAttributes'] = TlsCsrResponseAttributes
-    globals()['TypeTlsCsr'] = TypeTlsCsr
 
-
-class TlsCsrResponseData(ModelNormal):
+class Token(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -57,69 +49,72 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('scope',): {
+            'GLOBAL': "global",
+            'PURGE_SELECT': "purge_select",
+            'PURGE_ALL': "purge_all",
+            'GLOBAL:READ': "global:read",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'id': (str,),  # noqa: E501
-            'type': (TypeTlsCsr,),  # noqa: E501
-            'attributes': (TlsCsrResponseAttributes,),  # noqa: E501
-            'relationships': (RelationshipsForTlsCsr,),  # noqa: E501
+            'services': ([str],),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'scope': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'type': 'type',  # noqa: E501
-        'attributes': 'attributes',  # noqa: E501
-        'relationships': 'relationships',  # noqa: E501
+        'services': 'services',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'scope': 'scope',  # noqa: E501
     }
 
     read_only_vars = {
+        'services',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TlsCsrResponseData - a model defined in OpenAPI
+        """Token - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -144,18 +139,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            type (TypeTlsCsr): [optional]  # noqa: E501
-            attributes (TlsCsrResponseAttributes): [optional]  # noqa: E501
-            relationships (RelationshipsForTlsCsr): [optional]  # noqa: E501
+            services ([str]): List of alphanumeric strings identifying services (optional). If no services are specified, the token will have access to all services on the account. . [optional]  # noqa: E501
+            name (str): Name of the token.. [optional]  # noqa: E501
+            scope (str): Space-delimited list of authorization scope.. [optional] if omitted the server will use the default value of "global"  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -196,15 +190,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TlsCsrResponseData - a model defined in OpenAPI
+        """Token - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -229,18 +223,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            type (TypeTlsCsr): [optional]  # noqa: E501
-            attributes (TlsCsrResponseAttributes): [optional]  # noqa: E501
-            relationships (RelationshipsForTlsCsr): [optional]  # noqa: E501
+            services ([str]): List of alphanumeric strings identifying services (optional). If no services are specified, the token will have access to all services on the account. . [optional]  # noqa: E501
+            name (str): Name of the token.. [optional]  # noqa: E501
+            scope (str): Space-delimited list of authorization scope.. [optional] if omitted the server will use the default value of "global"  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/tls_dns_record.py` & `fastly-1.3.1/fastly/model/tls_dns_record.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_domain_data.py` & `fastly-1.3.1/fastly/model/tls_domain_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_domains_response.py` & `fastly-1.3.1/fastly/model/waf_exclusions_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,27 +26,29 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
+    from fastly.model.included_with_waf_exclusion import IncludedWithWafExclusion
     from fastly.model.pagination import Pagination
     from fastly.model.pagination_links import PaginationLinks
     from fastly.model.pagination_meta import PaginationMeta
-    from fastly.model.tls_domain_data import TlsDomainData
-    from fastly.model.tls_domains_response_all_of import TlsDomainsResponseAllOf
+    from fastly.model.waf_exclusion_response_data import WafExclusionResponseData
+    from fastly.model.waf_exclusions_response_all_of import WafExclusionsResponseAllOf
+    globals()['IncludedWithWafExclusion'] = IncludedWithWafExclusion
     globals()['Pagination'] = Pagination
     globals()['PaginationLinks'] = PaginationLinks
     globals()['PaginationMeta'] = PaginationMeta
-    globals()['TlsDomainData'] = TlsDomainData
-    globals()['TlsDomainsResponseAllOf'] = TlsDomainsResponseAllOf
+    globals()['WafExclusionResponseData'] = WafExclusionResponseData
+    globals()['WafExclusionsResponseAllOf'] = WafExclusionsResponseAllOf
 
 
-class TlsDomainsResponse(ModelComposed):
+class WafExclusionsResponse(ModelComposed):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -91,35 +93,37 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'links': (PaginationLinks,),  # noqa: E501
             'meta': (PaginationMeta,),  # noqa: E501
-            'data': ([TlsDomainData],),  # noqa: E501
+            'data': ([WafExclusionResponseData],),  # noqa: E501
+            'included': (IncludedWithWafExclusion,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'links': 'links',  # noqa: E501
         'meta': 'meta',  # noqa: E501
         'data': 'data',  # noqa: E501
+        'included': 'included',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TlsDomainsResponse - a model defined in OpenAPI
+        """WafExclusionsResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -146,15 +150,16 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             links (PaginationLinks): [optional]  # noqa: E501
             meta (PaginationMeta): [optional]  # noqa: E501
-            data ([TlsDomainData]): [optional]  # noqa: E501
+            data ([WafExclusionResponseData]): [optional]  # noqa: E501
+            included (IncludedWithWafExclusion): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -213,15 +218,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TlsDomainsResponse - a model defined in OpenAPI
+        """WafExclusionsResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -248,15 +253,16 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             links (PaginationLinks): [optional]  # noqa: E501
             meta (PaginationMeta): [optional]  # noqa: E501
-            data ([TlsDomainData]): [optional]  # noqa: E501
+            data ([WafExclusionResponseData]): [optional]  # noqa: E501
+            included (IncludedWithWafExclusion): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -315,12 +321,12 @@
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
               Pagination,
-              TlsDomainsResponseAllOf,
+              WafExclusionsResponseAllOf,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `fastly-1.3.0/fastly/model/tls_domains_response_all_of.py` & `fastly-1.3.1/fastly/model/tls_domains_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_private_key.py` & `fastly-1.3.1/fastly/model/tls_private_key.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_private_key_data.py` & `fastly-1.3.1/fastly/model/tls_private_key_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_private_key_data_attributes.py` & `fastly-1.3.1/fastly/model/tls_private_key_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_private_key_response.py` & `fastly-1.3.1/fastly/model/tls_private_keys_response_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 def lazy_import():
     from fastly.model.tls_private_key_response_data import TlsPrivateKeyResponseData
     globals()['TlsPrivateKeyResponseData'] = TlsPrivateKeyResponseData
 
 
-class TlsPrivateKeyResponse(ModelNormal):
+class TlsPrivateKeysResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -81,15 +81,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (TlsPrivateKeyResponseData,),  # noqa: E501
+            'data': ([TlsPrivateKeyResponseData],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -101,15 +101,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TlsPrivateKeyResponse - a model defined in OpenAPI
+        """TlsPrivateKeysResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +134,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (TlsPrivateKeyResponseData): [optional]  # noqa: E501
+            data ([TlsPrivateKeyResponseData]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TlsPrivateKeyResponse - a model defined in OpenAPI
+        """TlsPrivateKeysResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (TlsPrivateKeyResponseData): [optional]  # noqa: E501
+            data ([TlsPrivateKeyResponseData]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/tls_private_key_response_attributes.py` & `fastly-1.3.1/fastly/model/tls_private_key_response_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_private_key_response_attributes_all_of.py` & `fastly-1.3.1/fastly/model/tls_private_key_response_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_private_key_response_data.py` & `fastly-1.3.1/fastly/model/tls_private_key_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_private_keys_response.py` & `fastly-1.3.1/fastly/model/tls_private_keys_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_private_keys_response_all_of.py` & `fastly-1.3.1/fastly/model/tls_subscription.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.tls_private_key_response_data import TlsPrivateKeyResponseData
-    globals()['TlsPrivateKeyResponseData'] = TlsPrivateKeyResponseData
+    from fastly.model.tls_subscription_data import TlsSubscriptionData
+    globals()['TlsSubscriptionData'] = TlsSubscriptionData
 
 
-class TlsPrivateKeysResponseAllOf(ModelNormal):
+class TlsSubscription(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -81,15 +81,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([TlsPrivateKeyResponseData],),  # noqa: E501
+            'data': (TlsSubscriptionData,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -101,15 +101,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TlsPrivateKeysResponseAllOf - a model defined in OpenAPI
+        """TlsSubscription - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +134,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([TlsPrivateKeyResponseData]): [optional]  # noqa: E501
+            data (TlsSubscriptionData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TlsPrivateKeysResponseAllOf - a model defined in OpenAPI
+        """TlsSubscription - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([TlsPrivateKeyResponseData]): [optional]  # noqa: E501
+            data (TlsSubscriptionData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/tls_subscription.py` & `fastly-1.3.1/fastly/model/tls_subscription_data_attributes.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from fastly.model.tls_subscription_data import TlsSubscriptionData
-    globals()['TlsSubscriptionData'] = TlsSubscriptionData
 
-
-class TlsSubscription(ModelNormal):
+class TlsSubscriptionDataAttributes(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -53,63 +49,65 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('certificate_authority',): {
+            'LETS-ENCRYPT': "lets-encrypt",
+            'GLOBALSIGN': "globalsign",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'data': (TlsSubscriptionData,),  # noqa: E501
+            'certificate_authority': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'certificate_authority': 'certificate_authority',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TlsSubscription - a model defined in OpenAPI
+        """TlsSubscriptionDataAttributes - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +132,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (TlsSubscriptionData): [optional]  # noqa: E501
+            certificate_authority (str): The entity that issues and certifies the TLS certificates for your subscription.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +181,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TlsSubscription - a model defined in OpenAPI
+        """TlsSubscriptionDataAttributes - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +214,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (TlsSubscriptionData): [optional]  # noqa: E501
+            certificate_authority (str): The entity that issues and certifies the TLS certificates for your subscription.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/tls_subscription_data.py` & `fastly-1.3.1/fastly/model/tls_subscription_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_subscription_data_attributes.py` & `fastly-1.3.1/fastly/model/waf_exclusion.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fastly.model.waf_exclusion_data import WafExclusionData
+    globals()['WafExclusionData'] = WafExclusionData
 
-class TlsSubscriptionDataAttributes(ModelNormal):
+
+class WafExclusion(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -49,65 +53,63 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('certificate_authority',): {
-            'LETS-ENCRYPT': "lets-encrypt",
-            'GLOBALSIGN': "globalsign",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'certificate_authority': (str,),  # noqa: E501
+            'data': (WafExclusionData,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'certificate_authority': 'certificate_authority',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TlsSubscriptionDataAttributes - a model defined in OpenAPI
+        """WafExclusion - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -132,15 +134,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            certificate_authority (str): The entity that issues and certifies the TLS certificates for your subscription.. [optional]  # noqa: E501
+            data (WafExclusionData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -181,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TlsSubscriptionDataAttributes - a model defined in OpenAPI
+        """WafExclusion - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -214,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            certificate_authority (str): The entity that issues and certifies the TLS certificates for your subscription.. [optional]  # noqa: E501
+            data (WafExclusionData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/tls_subscription_response.py` & `fastly-1.3.1/fastly/model/tls_subscription_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_subscription_response_attributes.py` & `fastly-1.3.1/fastly/model/tls_subscription_response_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_subscription_response_attributes_all_of.py` & `fastly-1.3.1/fastly/model/version_response_all_of.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 
-class TlsSubscriptionResponseAttributesAllOf(ModelNormal):
+class VersionResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -49,21 +49,14 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('state',): {
-            'PENDING': "pending",
-            'PROCESSING': "processing",
-            'ISSUED': "issued",
-            'RENEWING': "renewing",
-            'FAILED': "failed",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -82,35 +75,36 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'state': (str,),  # noqa: E501
+            'service_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'state': 'state',  # noqa: E501
+        'service_id': 'service_id',  # noqa: E501
     }
 
     read_only_vars = {
+        'service_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TlsSubscriptionResponseAttributesAllOf - a model defined in OpenAPI
+        """VersionResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,15 +129,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            state (str): The current state of your subscription.. [optional]  # noqa: E501
+            service_id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -184,15 +178,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TlsSubscriptionResponseAttributesAllOf - a model defined in OpenAPI
+        """VersionResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -217,15 +211,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            state (str): The current state of your subscription.. [optional]  # noqa: E501
+            service_id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/tls_subscription_response_data.py` & `fastly-1.3.1/fastly/model/tls_subscription_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_subscription_response_data_all_of.py` & `fastly-1.3.1/fastly/model/user_response_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from fastly.model.tls_subscription_response_attributes import TlsSubscriptionResponseAttributes
-    globals()['TlsSubscriptionResponseAttributes'] = TlsSubscriptionResponseAttributes
 
-
-class TlsSubscriptionResponseDataAllOf(ModelNormal):
+class UserResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -64,55 +60,57 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
             'id': (str,),  # noqa: E501
-            'attributes': (TlsSubscriptionResponseAttributes,),  # noqa: E501
+            'email_hash': (str,),  # noqa: E501
+            'customer_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
-        'attributes': 'attributes',  # noqa: E501
+        'email_hash': 'email_hash',  # noqa: E501
+        'customer_id': 'customer_id',  # noqa: E501
     }
 
     read_only_vars = {
         'id',  # noqa: E501
+        'email_hash',  # noqa: E501
+        'customer_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TlsSubscriptionResponseDataAllOf - a model defined in OpenAPI
+        """UserResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,15 +136,16 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): [optional]  # noqa: E501
-            attributes (TlsSubscriptionResponseAttributes): [optional]  # noqa: E501
+            email_hash (str): The alphanumeric string identifying a email login.. [optional]  # noqa: E501
+            customer_id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -187,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TlsSubscriptionResponseDataAllOf - a model defined in OpenAPI
+        """UserResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -221,15 +220,16 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): [optional]  # noqa: E501
-            attributes (TlsSubscriptionResponseAttributes): [optional]  # noqa: E501
+            email_hash (str): The alphanumeric string identifying a email login.. [optional]  # noqa: E501
+            customer_id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/tls_subscriptions_response.py` & `fastly-1.3.1/fastly/model/tls_subscriptions_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/tls_subscriptions_response_all_of.py` & `fastly-1.3.1/fastly/model/tls_subscriptions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/token.py` & `fastly-1.3.1/fastly/model/waf_firewall_data_attributes.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 
-class Token(ModelNormal):
+class WafFirewallDataAttributes(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -49,20 +49,14 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('scope',): {
-            'GLOBAL': "global",
-            'PURGE_SELECT': "purge_select",
-            'PURGE_ALL': "purge_all",
-            'GLOBAL:READ': "global:read",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -81,40 +75,42 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'services': ([str],),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'scope': (str,),  # noqa: E501
+            'disabled': (bool,),  # noqa: E501
+            'prefetch_condition': (str,),  # noqa: E501
+            'response': (str,),  # noqa: E501
+            'service_version_number': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'services': 'services',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'scope': 'scope',  # noqa: E501
+        'disabled': 'disabled',  # noqa: E501
+        'prefetch_condition': 'prefetch_condition',  # noqa: E501
+        'response': 'response',  # noqa: E501
+        'service_version_number': 'service_version_number',  # noqa: E501
     }
 
     read_only_vars = {
-        'services',  # noqa: E501
+        'service_version_number',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Token - a model defined in OpenAPI
+        """WafFirewallDataAttributes - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,17 +135,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            services ([str]): List of alphanumeric strings identifying services (optional). If no services are specified, the token will have access to all services on the account. . [optional]  # noqa: E501
-            name (str): Name of the token.. [optional]  # noqa: E501
-            scope (str): Space-delimited list of authorization scope.. [optional] if omitted the server will use the default value of "global"  # noqa: E501
+            disabled (bool): The status of the firewall.. [optional] if omitted the server will use the default value of False  # noqa: E501
+            prefetch_condition (str): Name of the corresponding condition object.. [optional]  # noqa: E501
+            response (str): Name of the corresponding response object.. [optional]  # noqa: E501
+            service_version_number (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -190,15 +187,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Token - a model defined in OpenAPI
+        """WafFirewallDataAttributes - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -223,17 +220,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            services ([str]): List of alphanumeric strings identifying services (optional). If no services are specified, the token will have access to all services on the account. . [optional]  # noqa: E501
-            name (str): Name of the token.. [optional]  # noqa: E501
-            scope (str): Space-delimited list of authorization scope.. [optional] if omitted the server will use the default value of "global"  # noqa: E501
+            disabled (bool): The status of the firewall.. [optional] if omitted the server will use the default value of False  # noqa: E501
+            prefetch_condition (str): Name of the corresponding condition object.. [optional]  # noqa: E501
+            response (str): Name of the corresponding response object.. [optional]  # noqa: E501
+            service_version_number (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/token_created_response.py` & `fastly-1.3.1/fastly/model/token_created_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/token_created_response_all_of.py` & `fastly-1.3.1/fastly/model/token_created_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/token_response.py` & `fastly-1.3.1/fastly/model/token_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/token_response_all_of.py` & `fastly-1.3.1/fastly/model/vcl_diff.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 
-class TokenResponseAllOf(ModelNormal):
+class VclDiff(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -49,14 +49,19 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('format',): {
+            'TEXT': "text",
+            'HTML': "html",
+            'HTML_SIMPLE': "html_simple",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -75,50 +80,41 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (str,),  # noqa: E501
-            'user_id': (str,),  # noqa: E501
-            'created_at': (str,),  # noqa: E501
-            'last_used_at': (str,),  # noqa: E501
-            'expires_at': (str,),  # noqa: E501
-            'ip': (str,),  # noqa: E501
-            'user_agent': (str,),  # noqa: E501
+            '_from': (int,),  # noqa: E501
+            'to': (int,),  # noqa: E501
+            'format': (str,),  # noqa: E501
+            'diff': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'user_id': 'user_id',  # noqa: E501
-        'created_at': 'created_at',  # noqa: E501
-        'last_used_at': 'last_used_at',  # noqa: E501
-        'expires_at': 'expires_at',  # noqa: E501
-        'ip': 'ip',  # noqa: E501
-        'user_agent': 'user_agent',  # noqa: E501
+        '_from': 'from',  # noqa: E501
+        'to': 'to',  # noqa: E501
+        'format': 'format',  # noqa: E501
+        'diff': 'diff',  # noqa: E501
     }
 
     read_only_vars = {
-        'id',  # noqa: E501
-        'user_id',  # noqa: E501
-        'last_used_at',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TokenResponseAllOf - a model defined in OpenAPI
+        """VclDiff - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,21 +139,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            user_id (str): [optional]  # noqa: E501
-            created_at (str): Time-stamp (UTC) of when the token was created.. [optional]  # noqa: E501
-            last_used_at (str): Time-stamp (UTC) of when the token was last used.. [optional]  # noqa: E501
-            expires_at (str): Time-stamp (UTC) of when the token will expire (optional).. [optional]  # noqa: E501
-            ip (str): IP Address of the client that last used the token.. [optional]  # noqa: E501
-            user_agent (str): User-Agent header of the client that last used the token.. [optional]  # noqa: E501
+            _from (int): The version number of the service to which changes in the generated VCL are being compared.. [optional]  # noqa: E501
+            to (int): The version number of the service from which changes in the generated VCL are being compared.. [optional]  # noqa: E501
+            format (str): The format in which compared VCL changes are being returned in.. [optional]  # noqa: E501
+            diff (str): The differences between two specified versions.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -198,15 +191,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TokenResponseAllOf - a model defined in OpenAPI
+        """VclDiff - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -231,21 +224,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            user_id (str): [optional]  # noqa: E501
-            created_at (str): Time-stamp (UTC) of when the token was created.. [optional]  # noqa: E501
-            last_used_at (str): Time-stamp (UTC) of when the token was last used.. [optional]  # noqa: E501
-            expires_at (str): Time-stamp (UTC) of when the token will expire (optional).. [optional]  # noqa: E501
-            ip (str): IP Address of the client that last used the token.. [optional]  # noqa: E501
-            user_agent (str): User-Agent header of the client that last used the token.. [optional]  # noqa: E501
+            _from (int): The version number of the service to which changes in the generated VCL are being compared.. [optional]  # noqa: E501
+            to (int): The version number of the service from which changes in the generated VCL are being compared.. [optional]  # noqa: E501
+            format (str): The format in which compared VCL changes are being returned in.. [optional]  # noqa: E501
+            diff (str): The differences between two specified versions.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/type_billing_address.py` & `fastly-1.3.1/fastly/model/type_billing_address.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/type_contact.py` & `fastly-1.3.1/fastly/model/type_contact.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/type_customer.py` & `fastly-1.3.1/fastly/model/type_customer.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/type_event.py` & `fastly-1.3.1/fastly/model/type_event.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/type_invitation.py` & `fastly-1.3.1/fastly/model/type_invitation.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/type_mutual_authentication.py` & `fastly-1.3.1/fastly/model/type_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/type_resource.py` & `fastly-1.3.1/fastly/model/type_resource.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/type_service.py` & `fastly-1.3.1/fastly/model/type_service.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/type_service_authorization.py` & `fastly-1.3.1/fastly/model/type_service_authorization.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/type_service_invitation.py` & `fastly-1.3.1/fastly/model/type_service_invitation.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/type_star.py` & `fastly-1.3.1/fastly/model/type_star.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/type_tls_activation.py` & `fastly-1.3.1/fastly/model/type_tls_activation.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/type_tls_bulk_certificate.py` & `fastly-1.3.1/fastly/model/type_tls_bulk_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/type_tls_certificate.py` & `fastly-1.3.1/fastly/model/type_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/type_tls_configuration.py` & `fastly-1.3.1/fastly/model/type_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/type_tls_csr.py` & `fastly-1.3.1/fastly/model/type_tls_dns_record.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 
-class TypeTlsCsr(ModelSimple):
+class TypeTlsDnsRecord(ModelSimple):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -46,15 +46,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'CSR': "csr",
+            'DNS_RECORD': "dns_record",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -93,23 +93,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """TypeTlsCsr - a model defined in OpenAPI
+        """TypeTlsDnsRecord - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): CSR Resource Type. if omitted defaults to "csr", must be one of ["csr", ]  # noqa: E501
+            args[0] (str): Resource type. if omitted defaults to "dns_record", must be one of ["dns_record", ]  # noqa: E501
 
         Keyword Args:
-            value (str): CSR Resource Type. if omitted defaults to "csr", must be one of ["csr", ]  # noqa: E501
+            value (str): Resource type. if omitted defaults to "dns_record", must be one of ["dns_record", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -142,15 +142,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "csr"
+            value = "dns_record"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -179,23 +179,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """TypeTlsCsr - a model defined in OpenAPI
+        """TypeTlsDnsRecord - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): CSR Resource Type. if omitted defaults to "csr", must be one of ["csr", ]  # noqa: E501
+            args[0] (str): Resource type. if omitted defaults to "dns_record", must be one of ["dns_record", ]  # noqa: E501
 
         Keyword Args:
-            value (str): CSR Resource Type. if omitted defaults to "csr", must be one of ["csr", ]  # noqa: E501
+            value (str): Resource type. if omitted defaults to "dns_record", must be one of ["dns_record", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -230,15 +230,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "csr"
+            value = "dns_record"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `fastly-1.3.0/fastly/model/type_tls_dns_record.py` & `fastly-1.3.1/fastly/model/type_waf_active_rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 
-class TypeTlsDnsRecord(ModelSimple):
+class TypeWafActiveRule(ModelSimple):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -46,15 +46,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'DNS_RECORD': "dns_record",
+            'WAF_ACTIVE_RULE': "waf_active_rule",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -93,23 +93,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """TypeTlsDnsRecord - a model defined in OpenAPI
+        """TypeWafActiveRule - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): Resource type. if omitted defaults to "dns_record", must be one of ["dns_record", ]  # noqa: E501
+            args[0] (str): Resource type.. if omitted defaults to "waf_active_rule", must be one of ["waf_active_rule", ]  # noqa: E501
 
         Keyword Args:
-            value (str): Resource type. if omitted defaults to "dns_record", must be one of ["dns_record", ]  # noqa: E501
+            value (str): Resource type.. if omitted defaults to "waf_active_rule", must be one of ["waf_active_rule", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -142,15 +142,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "dns_record"
+            value = "waf_active_rule"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -179,23 +179,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """TypeTlsDnsRecord - a model defined in OpenAPI
+        """TypeWafActiveRule - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): Resource type. if omitted defaults to "dns_record", must be one of ["dns_record", ]  # noqa: E501
+            args[0] (str): Resource type.. if omitted defaults to "waf_active_rule", must be one of ["waf_active_rule", ]  # noqa: E501
 
         Keyword Args:
-            value (str): Resource type. if omitted defaults to "dns_record", must be one of ["dns_record", ]  # noqa: E501
+            value (str): Resource type.. if omitted defaults to "waf_active_rule", must be one of ["waf_active_rule", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -230,15 +230,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "dns_record"
+            value = "waf_active_rule"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `fastly-1.3.0/fastly/model/type_tls_domain.py` & `fastly-1.3.1/fastly/model/type_tls_domain.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/type_tls_private_key.py` & `fastly-1.3.1/fastly/model/type_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/type_tls_subscription.py` & `fastly-1.3.1/fastly/model/type_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/type_user.py` & `fastly-1.3.1/fastly/model/type_user.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/type_waf_active_rule.py` & `fastly-1.3.1/fastly/model/type_waf_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 
-class TypeWafActiveRule(ModelSimple):
+class TypeWafRule(ModelSimple):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -46,15 +46,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'WAF_ACTIVE_RULE': "waf_active_rule",
+            'WAF_RULE': "waf_rule",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -93,23 +93,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """TypeWafActiveRule - a model defined in OpenAPI
+        """TypeWafRule - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): Resource type.. if omitted defaults to "waf_active_rule", must be one of ["waf_active_rule", ]  # noqa: E501
+            args[0] (str): Resource type.. if omitted defaults to "waf_rule", must be one of ["waf_rule", ]  # noqa: E501
 
         Keyword Args:
-            value (str): Resource type.. if omitted defaults to "waf_active_rule", must be one of ["waf_active_rule", ]  # noqa: E501
+            value (str): Resource type.. if omitted defaults to "waf_rule", must be one of ["waf_rule", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -142,15 +142,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "waf_active_rule"
+            value = "waf_rule"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -179,23 +179,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """TypeWafActiveRule - a model defined in OpenAPI
+        """TypeWafRule - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): Resource type.. if omitted defaults to "waf_active_rule", must be one of ["waf_active_rule", ]  # noqa: E501
+            args[0] (str): Resource type.. if omitted defaults to "waf_rule", must be one of ["waf_rule", ]  # noqa: E501
 
         Keyword Args:
-            value (str): Resource type.. if omitted defaults to "waf_active_rule", must be one of ["waf_active_rule", ]  # noqa: E501
+            value (str): Resource type.. if omitted defaults to "waf_rule", must be one of ["waf_rule", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -230,15 +230,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "waf_active_rule"
+            value = "waf_rule"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `fastly-1.3.0/fastly/model/type_waf_exclusion.py` & `fastly-1.3.1/fastly/model/type_waf_exclusion.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/type_waf_firewall.py` & `fastly-1.3.1/fastly/model/type_waf_firewall.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/type_waf_firewall_version.py` & `fastly-1.3.1/fastly/model/type_waf_firewall_version.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/type_waf_rule.py` & `fastly-1.3.1/fastly/model/type_waf_tag.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 
-class TypeWafRule(ModelSimple):
+class TypeWafTag(ModelSimple):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -46,15 +46,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'WAF_RULE': "waf_rule",
+            'WAF_TAG': "waf_tag",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -93,23 +93,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """TypeWafRule - a model defined in OpenAPI
+        """TypeWafTag - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): Resource type.. if omitted defaults to "waf_rule", must be one of ["waf_rule", ]  # noqa: E501
+            args[0] (str): Resource type.. if omitted defaults to "waf_tag", must be one of ["waf_tag", ]  # noqa: E501
 
         Keyword Args:
-            value (str): Resource type.. if omitted defaults to "waf_rule", must be one of ["waf_rule", ]  # noqa: E501
+            value (str): Resource type.. if omitted defaults to "waf_tag", must be one of ["waf_tag", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -142,15 +142,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "waf_rule"
+            value = "waf_tag"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -179,23 +179,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """TypeWafRule - a model defined in OpenAPI
+        """TypeWafTag - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): Resource type.. if omitted defaults to "waf_rule", must be one of ["waf_rule", ]  # noqa: E501
+            args[0] (str): Resource type.. if omitted defaults to "waf_tag", must be one of ["waf_tag", ]  # noqa: E501
 
         Keyword Args:
-            value (str): Resource type.. if omitted defaults to "waf_rule", must be one of ["waf_rule", ]  # noqa: E501
+            value (str): Resource type.. if omitted defaults to "waf_tag", must be one of ["waf_tag", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -230,15 +230,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "waf_rule"
+            value = "waf_tag"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `fastly-1.3.0/fastly/model/type_waf_rule_revision.py` & `fastly-1.3.1/fastly/model/type_waf_rule_revision.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/type_waf_tag.py` & `fastly-1.3.1/fastly/model/waf_rule_revision_or_latest.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,90 +26,84 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 
-class TypeWafTag(ModelSimple):
+class WafRuleRevisionOrLatest(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
       validations (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('value',): {
-            'WAF_TAG': "waf_tag",
-        },
     }
 
     validations = {
     }
 
-    additional_properties_type = None
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'value': (str,),
         }
 
     @cached_property
     def discriminator():
         return None
 
 
-    attribute_map = {}
+    attribute_map = {
+    }
 
-    read_only_vars = set()
+    read_only_vars = {
+    }
 
-    _composed_schemas = None
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
+    _composed_schemas = {}
 
+    @classmethod
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):
-        """TypeWafTag - a model defined in OpenAPI
-
-        Note that value can be passed either in args or in kwargs, but not in both.
-
-        Args:
-            args[0] (str): Resource type.. if omitted defaults to "waf_tag", must be one of ["waf_tag", ]  # noqa: E501
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """WafRuleRevisionOrLatest - a model defined in OpenAPI
 
         Keyword Args:
-            value (str): Resource type.. if omitted defaults to "waf_tag", must be one of ["waf_tag", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -133,30 +127,23 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
-        # required up here when default value is not given
-        _path_to_item = kwargs.pop('_path_to_item', ())
-
-        if 'value' in kwargs:
-            value = kwargs.pop('value')
-        elif args:
-            args = list(args)
-            value = args.pop(0)
-        else:
-            value = "waf_tag"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
+        self = super(OpenApiModel, cls).__new__(cls)
+
         if args:
             raise ApiTypeError(
                 "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
                     args,
                     self.__class__.__name__,
                 ),
                 path_to_item=_path_to_item,
@@ -165,37 +152,39 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-        self.value = value
-        if kwargs:
-            raise ApiTypeError(
-                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
-                    kwargs,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):
-        """TypeWafTag - a model defined in OpenAPI
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
 
-        Note that value can be passed either in args or in kwargs, but not in both.
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
 
-        Args:
-            args[0] (str): Resource type.. if omitted defaults to "waf_tag", must be one of ["waf_tag", ]  # noqa: E501
+    @convert_js_args_to_python_args
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """WafRuleRevisionOrLatest - a model defined in OpenAPI
 
         Keyword Args:
-            value (str): Resource type.. if omitted defaults to "waf_tag", must be one of ["waf_tag", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -219,29 +208,18 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
-        # required up here when default value is not given
-        _path_to_item = kwargs.pop('_path_to_item', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if 'value' in kwargs:
-            value = kwargs.pop('value')
-        elif args:
-            args = list(args)
-            value = args.pop(0)
-        else:
-            value = "waf_tag"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
             raise ApiTypeError(
                 "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
                     args,
@@ -253,19 +231,19 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-        self.value = value
-        if kwargs:
-            raise ApiTypeError(
-                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
-                    kwargs,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
-        return self
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `fastly-1.3.0/fastly/model/update_billing_address_request.py` & `fastly-1.3.1/fastly/model/update_billing_address_request.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/update_billing_address_request_data.py` & `fastly-1.3.1/fastly/model/update_billing_address_request_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/user.py` & `fastly-1.3.1/fastly/model/user.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/user_response.py` & `fastly-1.3.1/fastly/model/user_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/user_response_all_of.py` & `fastly-1.3.1/fastly/model/waf_tag.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,16 +25,22 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fastly.model.type_waf_tag import TypeWafTag
+    from fastly.model.waf_tag_attributes import WafTagAttributes
+    globals()['TypeWafTag'] = TypeWafTag
+    globals()['WafTagAttributes'] = WafTagAttributes
 
-class UserResponseAllOf(ModelNormal):
+
+class WafTag(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -60,57 +66,57 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
+            'type': (TypeWafTag,),  # noqa: E501
             'id': (str,),  # noqa: E501
-            'email_hash': (str,),  # noqa: E501
-            'customer_id': (str,),  # noqa: E501
+            'attributes': (WafTagAttributes,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'type': 'type',  # noqa: E501
         'id': 'id',  # noqa: E501
-        'email_hash': 'email_hash',  # noqa: E501
-        'customer_id': 'customer_id',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
         'id',  # noqa: E501
-        'email_hash',  # noqa: E501
-        'customer_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UserResponseAllOf - a model defined in OpenAPI
+        """WafTag - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,17 +141,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            email_hash (str): The alphanumeric string identifying a email login.. [optional]  # noqa: E501
-            customer_id (str): [optional]  # noqa: E501
+            type (TypeWafTag): [optional]  # noqa: E501
+            id (str): Alphanumeric string identifying a WAF tag.. [optional]  # noqa: E501
+            attributes (WafTagAttributes): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,15 +192,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """UserResponseAllOf - a model defined in OpenAPI
+        """WafTag - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,17 +225,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            email_hash (str): The alphanumeric string identifying a email login.. [optional]  # noqa: E501
-            customer_id (str): [optional]  # noqa: E501
+            type (TypeWafTag): [optional]  # noqa: E501
+            id (str): Alphanumeric string identifying a WAF tag.. [optional]  # noqa: E501
+            attributes (WafTagAttributes): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/validator_result.py` & `fastly-1.3.1/fastly/model/validator_result.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/validator_result_messages.py` & `fastly-1.3.1/fastly/model/validator_result_messages.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/vcl.py` & `fastly-1.3.1/fastly/model/vcl.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/vcl_diff.py` & `fastly-1.3.1/fastly/model/waf_exclusions_response_all_of.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,22 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fastly.model.included_with_waf_exclusion import IncludedWithWafExclusion
+    from fastly.model.waf_exclusion_response_data import WafExclusionResponseData
+    globals()['IncludedWithWafExclusion'] = IncludedWithWafExclusion
+    globals()['WafExclusionResponseData'] = WafExclusionResponseData
 
-class VclDiff(ModelNormal):
+
+class WafExclusionsResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -49,72 +55,65 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('format',): {
-            'TEXT': "text",
-            'HTML': "html",
-            'HTML_SIMPLE': "html_simple",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            '_from': (int,),  # noqa: E501
-            'to': (int,),  # noqa: E501
-            'format': (str,),  # noqa: E501
-            'diff': (str,),  # noqa: E501
+            'data': ([WafExclusionResponseData],),  # noqa: E501
+            'included': (IncludedWithWafExclusion,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        '_from': 'from',  # noqa: E501
-        'to': 'to',  # noqa: E501
-        'format': 'format',  # noqa: E501
-        'diff': 'diff',  # noqa: E501
+        'data': 'data',  # noqa: E501
+        'included': 'included',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """VclDiff - a model defined in OpenAPI
+        """WafExclusionsResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,18 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            _from (int): The version number of the service to which changes in the generated VCL are being compared.. [optional]  # noqa: E501
-            to (int): The version number of the service from which changes in the generated VCL are being compared.. [optional]  # noqa: E501
-            format (str): The format in which compared VCL changes are being returned in.. [optional]  # noqa: E501
-            diff (str): The differences between two specified versions.. [optional]  # noqa: E501
+            data ([WafExclusionResponseData]): [optional]  # noqa: E501
+            included (IncludedWithWafExclusion): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -191,15 +188,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """VclDiff - a model defined in OpenAPI
+        """WafExclusionsResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -224,18 +221,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            _from (int): The version number of the service to which changes in the generated VCL are being compared.. [optional]  # noqa: E501
-            to (int): The version number of the service from which changes in the generated VCL are being compared.. [optional]  # noqa: E501
-            format (str): The format in which compared VCL changes are being returned in.. [optional]  # noqa: E501
-            diff (str): The differences between two specified versions.. [optional]  # noqa: E501
+            data ([WafExclusionResponseData]): [optional]  # noqa: E501
+            included (IncludedWithWafExclusion): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/vcl_response.py` & `fastly-1.3.1/fastly/model/vcl_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/version.py` & `fastly-1.3.1/fastly/model/version.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/version_create_response.py` & `fastly-1.3.1/fastly/model/version_create_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/version_detail.py` & `fastly-1.3.1/fastly/model/version_detail.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/version_detail_settings.py` & `fastly-1.3.1/fastly/model/version_detail_settings.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/version_response.py` & `fastly-1.3.1/fastly/model/version_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/version_response_all_of.py` & `fastly-1.3.1/fastly/model/waf_firewall_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fastly.model.waf_firewall_version_data import WafFirewallVersionData
+    globals()['WafFirewallVersionData'] = WafFirewallVersionData
 
-class VersionResponseAllOf(ModelNormal):
+
+class WafFirewallVersion(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -60,51 +64,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'service_id': (str,),  # noqa: E501
+            'data': (WafFirewallVersionData,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'service_id': 'service_id',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
-        'service_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """VersionResponseAllOf - a model defined in OpenAPI
+        """WafFirewallVersion - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -129,15 +134,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            service_id (str): [optional]  # noqa: E501
+            data (WafFirewallVersionData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -178,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """VersionResponseAllOf - a model defined in OpenAPI
+        """WafFirewallVersion - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -211,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            service_id (str): [optional]  # noqa: E501
+            data (WafFirewallVersionData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/waf_active_rule.py` & `fastly-1.3.1/fastly/model/waf_active_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_active_rule_creation_response.py` & `fastly-1.3.1/fastly/model/waf_active_rule_creation_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_active_rule_data.py` & `fastly-1.3.1/fastly/model/waf_active_rule_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_active_rule_data_attributes.py` & `fastly-1.3.1/fastly/model/waf_active_rule_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_active_rule_response.py` & `fastly-1.3.1/fastly/model/waf_active_rule_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_active_rule_response_data.py` & `fastly-1.3.1/fastly/model/waf_active_rule_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_active_rule_response_data_all_of.py` & `fastly-1.3.1/fastly/model/waf_active_rule_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_active_rule_response_data_attributes.py` & `fastly-1.3.1/fastly/model/waf_active_rule_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_active_rule_response_data_attributes_all_of.py` & `fastly-1.3.1/fastly/model/waf_active_rule_response_data_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_active_rule_response_data_relationships.py` & `fastly-1.3.1/fastly/model/waf_active_rule_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_active_rules_response.py` & `fastly-1.3.1/fastly/model/waf_active_rules_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_active_rules_response_all_of.py` & `fastly-1.3.1/fastly/model/waf_active_rules_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_exclusion.py` & `fastly-1.3.1/fastly/model/waf_tags_response_all_of.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,19 +26,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.waf_exclusion_data import WafExclusionData
-    globals()['WafExclusionData'] = WafExclusionData
+    from fastly.model.waf_rule import WafRule
+    from fastly.model.waf_tags_response_data_item import WafTagsResponseDataItem
+    globals()['WafRule'] = WafRule
+    globals()['WafTagsResponseDataItem'] = WafTagsResponseDataItem
 
 
-class WafExclusion(ModelNormal):
+class WafTagsResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -81,35 +83,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (WafExclusionData,),  # noqa: E501
+            'data': ([WafTagsResponseDataItem],),  # noqa: E501
+            'included': ([WafRule],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'data': 'data',  # noqa: E501
+        'included': 'included',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafExclusion - a model defined in OpenAPI
+        """WafTagsResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (WafExclusionData): [optional]  # noqa: E501
+            data ([WafTagsResponseDataItem]): [optional]  # noqa: E501
+            included ([WafRule]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +188,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafExclusion - a model defined in OpenAPI
+        """WafTagsResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +221,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (WafExclusionData): [optional]  # noqa: E501
+            data ([WafTagsResponseDataItem]): [optional]  # noqa: E501
+            included ([WafRule]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/waf_exclusion_data.py` & `fastly-1.3.1/fastly/model/waf_exclusion_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_exclusion_data_attributes.py` & `fastly-1.3.1/fastly/model/waf_exclusion_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_exclusion_response.py` & `fastly-1.3.1/fastly/model/ws_message_format.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from fastly.model.waf_exclusion_response_data import WafExclusionResponseData
-    globals()['WafExclusionResponseData'] = WafExclusionResponseData
 
-
-class WafExclusionResponse(ModelNormal):
+class WsMessageFormat(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -64,52 +60,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'data': (WafExclusionResponseData,),  # noqa: E501
+            'content': (str,),  # noqa: E501
+            'content_bin': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'content': 'content',  # noqa: E501
+        'content_bin': 'content-bin',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafExclusionResponse - a model defined in OpenAPI
+        """WsMessageFormat - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +130,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (WafExclusionResponseData): [optional]  # noqa: E501
+            content (str): The content of a WebSocket `TEXT` message.. [optional]  # noqa: E501
+            content_bin (str): The base64-encoded content of a WebSocket `BINARY` message.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +180,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafExclusionResponse - a model defined in OpenAPI
+        """WsMessageFormat - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +213,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (WafExclusionResponseData): [optional]  # noqa: E501
+            content (str): The content of a WebSocket `TEXT` message.. [optional]  # noqa: E501
+            content_bin (str): The base64-encoded content of a WebSocket `BINARY` message.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/waf_exclusion_response_data.py` & `fastly-1.3.1/fastly/model/waf_exclusion_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_exclusion_response_data_all_of.py` & `fastly-1.3.1/fastly/model/waf_exclusion_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_exclusion_response_data_attributes.py` & `fastly-1.3.1/fastly/model/waf_exclusion_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_exclusion_response_data_attributes_all_of.py` & `fastly-1.3.1/fastly/model/waf_exclusion_response_data_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_exclusion_response_data_relationships.py` & `fastly-1.3.1/fastly/model/waf_exclusion_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_exclusions_response.py` & `fastly-1.3.1/fastly/model/waf_tags_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,29 +26,29 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.included_with_waf_exclusion import IncludedWithWafExclusion
     from fastly.model.pagination import Pagination
     from fastly.model.pagination_links import PaginationLinks
     from fastly.model.pagination_meta import PaginationMeta
-    from fastly.model.waf_exclusion_response_data import WafExclusionResponseData
-    from fastly.model.waf_exclusions_response_all_of import WafExclusionsResponseAllOf
-    globals()['IncludedWithWafExclusion'] = IncludedWithWafExclusion
+    from fastly.model.waf_rule import WafRule
+    from fastly.model.waf_tags_response_all_of import WafTagsResponseAllOf
+    from fastly.model.waf_tags_response_data_item import WafTagsResponseDataItem
     globals()['Pagination'] = Pagination
     globals()['PaginationLinks'] = PaginationLinks
     globals()['PaginationMeta'] = PaginationMeta
-    globals()['WafExclusionResponseData'] = WafExclusionResponseData
-    globals()['WafExclusionsResponseAllOf'] = WafExclusionsResponseAllOf
+    globals()['WafRule'] = WafRule
+    globals()['WafTagsResponseAllOf'] = WafTagsResponseAllOf
+    globals()['WafTagsResponseDataItem'] = WafTagsResponseDataItem
 
 
-class WafExclusionsResponse(ModelComposed):
+class WafTagsResponse(ModelComposed):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -93,16 +93,16 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'links': (PaginationLinks,),  # noqa: E501
             'meta': (PaginationMeta,),  # noqa: E501
-            'data': ([WafExclusionResponseData],),  # noqa: E501
-            'included': (IncludedWithWafExclusion,),  # noqa: E501
+            'data': ([WafTagsResponseDataItem],),  # noqa: E501
+            'included': ([WafRule],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -115,15 +115,15 @@
 
     read_only_vars = {
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafExclusionsResponse - a model defined in OpenAPI
+        """WafTagsResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -150,16 +150,16 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             links (PaginationLinks): [optional]  # noqa: E501
             meta (PaginationMeta): [optional]  # noqa: E501
-            data ([WafExclusionResponseData]): [optional]  # noqa: E501
-            included (IncludedWithWafExclusion): [optional]  # noqa: E501
+            data ([WafTagsResponseDataItem]): [optional]  # noqa: E501
+            included ([WafRule]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -218,15 +218,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafExclusionsResponse - a model defined in OpenAPI
+        """WafTagsResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -253,16 +253,16 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             links (PaginationLinks): [optional]  # noqa: E501
             meta (PaginationMeta): [optional]  # noqa: E501
-            data ([WafExclusionResponseData]): [optional]  # noqa: E501
-            included (IncludedWithWafExclusion): [optional]  # noqa: E501
+            data ([WafTagsResponseDataItem]): [optional]  # noqa: E501
+            included ([WafRule]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -321,12 +321,12 @@
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
               Pagination,
-              WafExclusionsResponseAllOf,
+              WafTagsResponseAllOf,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `fastly-1.3.0/fastly/model/waf_exclusions_response_all_of.py` & `fastly-1.3.1/fastly/model/waf_firewalls_response_all_of.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.included_with_waf_exclusion import IncludedWithWafExclusion
-    from fastly.model.waf_exclusion_response_data import WafExclusionResponseData
-    globals()['IncludedWithWafExclusion'] = IncludedWithWafExclusion
-    globals()['WafExclusionResponseData'] = WafExclusionResponseData
+    from fastly.model.included_with_waf_firewall import IncludedWithWafFirewall
+    from fastly.model.waf_firewall_response_data import WafFirewallResponseData
+    globals()['IncludedWithWafFirewall'] = IncludedWithWafFirewall
+    globals()['WafFirewallResponseData'] = WafFirewallResponseData
 
 
-class WafExclusionsResponseAllOf(ModelNormal):
+class WafFirewallsResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -83,16 +83,16 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([WafExclusionResponseData],),  # noqa: E501
-            'included': (IncludedWithWafExclusion,),  # noqa: E501
+            'data': ([WafFirewallResponseData],),  # noqa: E501
+            'included': (IncludedWithWafFirewall,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -105,15 +105,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafExclusionsResponseAllOf - a model defined in OpenAPI
+        """WafFirewallsResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,16 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([WafExclusionResponseData]): [optional]  # noqa: E501
-            included (IncludedWithWafExclusion): [optional]  # noqa: E501
+            data ([WafFirewallResponseData]): [optional]  # noqa: E501
+            included (IncludedWithWafFirewall): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -188,15 +188,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafExclusionsResponseAllOf - a model defined in OpenAPI
+        """WafFirewallsResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -221,16 +221,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([WafExclusionResponseData]): [optional]  # noqa: E501
-            included (IncludedWithWafExclusion): [optional]  # noqa: E501
+            data ([WafFirewallResponseData]): [optional]  # noqa: E501
+            included (IncludedWithWafFirewall): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/waf_firewall.py` & `fastly-1.3.1/fastly/model/waf_rule_revision_response_data_all_of.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.waf_firewall_data import WafFirewallData
-    globals()['WafFirewallData'] = WafFirewallData
+    from fastly.model.relationship_waf_rule import RelationshipWafRule
+    globals()['RelationshipWafRule'] = RelationshipWafRule
 
 
-class WafFirewall(ModelNormal):
+class WafRuleRevisionResponseDataAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -81,35 +81,35 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (WafFirewallData,),  # noqa: E501
+            'relationships': (RelationshipWafRule,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'relationships': 'relationships',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafFirewall - a model defined in OpenAPI
+        """WafRuleRevisionResponseDataAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +134,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (WafFirewallData): [optional]  # noqa: E501
+            relationships (RelationshipWafRule): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafFirewall - a model defined in OpenAPI
+        """WafRuleRevisionResponseDataAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (WafFirewallData): [optional]  # noqa: E501
+            relationships (RelationshipWafRule): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/waf_firewall_data.py` & `fastly-1.3.1/fastly/model/waf_firewall_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_firewall_data_attributes.py` & `fastly-1.3.1/fastly/model/waf_firewall_response_data_all_of.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,16 +25,22 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fastly.model.relationship_waf_firewall_versions import RelationshipWafFirewallVersions
+    from fastly.model.waf_firewall_response_data_attributes import WafFirewallResponseDataAttributes
+    globals()['RelationshipWafFirewallVersions'] = RelationshipWafFirewallVersions
+    globals()['WafFirewallResponseDataAttributes'] = WafFirewallResponseDataAttributes
 
-class WafFirewallDataAttributes(ModelNormal):
+
+class WafFirewallResponseDataAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -60,57 +66,57 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'disabled': (bool,),  # noqa: E501
-            'prefetch_condition': (str,),  # noqa: E501
-            'response': (str,),  # noqa: E501
-            'service_version_number': (int,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'attributes': (WafFirewallResponseDataAttributes,),  # noqa: E501
+            'relationships': (RelationshipWafFirewallVersions,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'disabled': 'disabled',  # noqa: E501
-        'prefetch_condition': 'prefetch_condition',  # noqa: E501
-        'response': 'response',  # noqa: E501
-        'service_version_number': 'service_version_number',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
+        'relationships': 'relationships',  # noqa: E501
     }
 
     read_only_vars = {
-        'service_version_number',  # noqa: E501
+        'id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafFirewallDataAttributes - a model defined in OpenAPI
+        """WafFirewallResponseDataAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,18 +141,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            disabled (bool): The status of the firewall.. [optional] if omitted the server will use the default value of False  # noqa: E501
-            prefetch_condition (str): Name of the corresponding condition object.. [optional]  # noqa: E501
-            response (str): Name of the corresponding response object.. [optional]  # noqa: E501
-            service_version_number (int): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            attributes (WafFirewallResponseDataAttributes): [optional]  # noqa: E501
+            relationships (RelationshipWafFirewallVersions): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -187,15 +192,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafFirewallDataAttributes - a model defined in OpenAPI
+        """WafFirewallResponseDataAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -220,18 +225,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            disabled (bool): The status of the firewall.. [optional] if omitted the server will use the default value of False  # noqa: E501
-            prefetch_condition (str): Name of the corresponding condition object.. [optional]  # noqa: E501
-            response (str): Name of the corresponding response object.. [optional]  # noqa: E501
-            service_version_number (int): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            attributes (WafFirewallResponseDataAttributes): [optional]  # noqa: E501
+            relationships (RelationshipWafFirewallVersions): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/waf_firewall_response.py` & `fastly-1.3.1/fastly/model/waf_firewall_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_firewall_response_data.py` & `fastly-1.3.1/fastly/model/waf_firewall_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_firewall_response_data_all_of.py` & `fastly-1.3.1/fastly/model/waf_firewall_version_response_data_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.relationship_waf_firewall_versions import RelationshipWafFirewallVersions
-    from fastly.model.waf_firewall_response_data_attributes import WafFirewallResponseDataAttributes
-    globals()['RelationshipWafFirewallVersions'] = RelationshipWafFirewallVersions
-    globals()['WafFirewallResponseDataAttributes'] = WafFirewallResponseDataAttributes
+    from fastly.model.relationships_for_waf_firewall_version import RelationshipsForWafFirewallVersion
+    from fastly.model.waf_firewall_version_response_data_attributes import WafFirewallVersionResponseDataAttributes
+    globals()['RelationshipsForWafFirewallVersion'] = RelationshipsForWafFirewallVersion
+    globals()['WafFirewallVersionResponseDataAttributes'] = WafFirewallVersionResponseDataAttributes
 
 
-class WafFirewallResponseDataAllOf(ModelNormal):
+class WafFirewallVersionResponseDataAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -84,16 +84,16 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'id': (str,),  # noqa: E501
-            'attributes': (WafFirewallResponseDataAttributes,),  # noqa: E501
-            'relationships': (RelationshipWafFirewallVersions,),  # noqa: E501
+            'attributes': (WafFirewallVersionResponseDataAttributes,),  # noqa: E501
+            'relationships': (RelationshipsForWafFirewallVersion,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -108,15 +108,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafFirewallResponseDataAllOf - a model defined in OpenAPI
+        """WafFirewallVersionResponseDataAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -141,17 +141,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            attributes (WafFirewallResponseDataAttributes): [optional]  # noqa: E501
-            relationships (RelationshipWafFirewallVersions): [optional]  # noqa: E501
+            id (str): Alphanumeric string identifying a Firewall version.. [optional]  # noqa: E501
+            attributes (WafFirewallVersionResponseDataAttributes): [optional]  # noqa: E501
+            relationships (RelationshipsForWafFirewallVersion): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -192,15 +192,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafFirewallResponseDataAllOf - a model defined in OpenAPI
+        """WafFirewallVersionResponseDataAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -225,17 +225,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            attributes (WafFirewallResponseDataAttributes): [optional]  # noqa: E501
-            relationships (RelationshipWafFirewallVersions): [optional]  # noqa: E501
+            id (str): Alphanumeric string identifying a Firewall version.. [optional]  # noqa: E501
+            attributes (WafFirewallVersionResponseDataAttributes): [optional]  # noqa: E501
+            relationships (RelationshipsForWafFirewallVersion): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/waf_firewall_response_data_attributes.py` & `fastly-1.3.1/fastly/model/waf_firewall_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_firewall_response_data_attributes_all_of.py` & `fastly-1.3.1/fastly/model/waf_firewall_response_data_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_firewall_version.py` & `fastly-1.3.1/fastly/model/waf_firewall_version_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,19 +26,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.waf_firewall_version_data import WafFirewallVersionData
-    globals()['WafFirewallVersionData'] = WafFirewallVersionData
+    from fastly.model.type_waf_firewall_version import TypeWafFirewallVersion
+    from fastly.model.waf_firewall_version_data_attributes import WafFirewallVersionDataAttributes
+    globals()['TypeWafFirewallVersion'] = TypeWafFirewallVersion
+    globals()['WafFirewallVersionDataAttributes'] = WafFirewallVersionDataAttributes
 
 
-class WafFirewallVersion(ModelNormal):
+class WafFirewallVersionData(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -81,35 +83,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (WafFirewallVersionData,),  # noqa: E501
+            'type': (TypeWafFirewallVersion,),  # noqa: E501
+            'attributes': (WafFirewallVersionDataAttributes,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafFirewallVersion - a model defined in OpenAPI
+        """WafFirewallVersionData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (WafFirewallVersionData): [optional]  # noqa: E501
+            type (TypeWafFirewallVersion): [optional]  # noqa: E501
+            attributes (WafFirewallVersionDataAttributes): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +188,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafFirewallVersion - a model defined in OpenAPI
+        """WafFirewallVersionData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +221,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (WafFirewallVersionData): [optional]  # noqa: E501
+            type (TypeWafFirewallVersion): [optional]  # noqa: E501
+            attributes (WafFirewallVersionDataAttributes): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/waf_firewall_version_data.py` & `fastly-1.3.1/fastly/model/waf_rule_revision.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.type_waf_firewall_version import TypeWafFirewallVersion
-    from fastly.model.waf_firewall_version_data_attributes import WafFirewallVersionDataAttributes
-    globals()['TypeWafFirewallVersion'] = TypeWafFirewallVersion
-    globals()['WafFirewallVersionDataAttributes'] = WafFirewallVersionDataAttributes
+    from fastly.model.type_waf_rule_revision import TypeWafRuleRevision
+    from fastly.model.waf_rule_revision_attributes import WafRuleRevisionAttributes
+    globals()['TypeWafRuleRevision'] = TypeWafRuleRevision
+    globals()['WafRuleRevisionAttributes'] = WafRuleRevisionAttributes
 
 
-class WafFirewallVersionData(ModelNormal):
+class WafRuleRevision(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -83,37 +83,40 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'type': (TypeWafFirewallVersion,),  # noqa: E501
-            'attributes': (WafFirewallVersionDataAttributes,),  # noqa: E501
+            'type': (TypeWafRuleRevision,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'attributes': (WafRuleRevisionAttributes,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'type': 'type',  # noqa: E501
+        'id': 'id',  # noqa: E501
         'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
+        'id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafFirewallVersionData - a model defined in OpenAPI
+        """WafRuleRevision - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,16 +141,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (TypeWafFirewallVersion): [optional]  # noqa: E501
-            attributes (WafFirewallVersionDataAttributes): [optional]  # noqa: E501
+            type (TypeWafRuleRevision): [optional]  # noqa: E501
+            id (str): Alphanumeric string identifying a WAF rule revision.. [optional]  # noqa: E501
+            attributes (WafRuleRevisionAttributes): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -188,15 +192,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafFirewallVersionData - a model defined in OpenAPI
+        """WafRuleRevision - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -221,16 +225,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (TypeWafFirewallVersion): [optional]  # noqa: E501
-            attributes (WafFirewallVersionDataAttributes): [optional]  # noqa: E501
+            type (TypeWafRuleRevision): [optional]  # noqa: E501
+            id (str): Alphanumeric string identifying a WAF rule revision.. [optional]  # noqa: E501
+            attributes (WafRuleRevisionAttributes): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/waf_firewall_version_data_attributes.py` & `fastly-1.3.1/fastly/model/waf_firewall_version_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_firewall_version_response.py` & `fastly-1.3.1/fastly/model/waf_firewall_version_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_firewall_version_response_data.py` & `fastly-1.3.1/fastly/model/waf_firewall_version_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_firewall_version_response_data_all_of.py` & `fastly-1.3.1/fastly/model/waf_rule_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.relationships_for_waf_firewall_version import RelationshipsForWafFirewallVersion
-    from fastly.model.waf_firewall_version_response_data_attributes import WafFirewallVersionResponseDataAttributes
-    globals()['RelationshipsForWafFirewallVersion'] = RelationshipsForWafFirewallVersion
-    globals()['WafFirewallVersionResponseDataAttributes'] = WafFirewallVersionResponseDataAttributes
+    from fastly.model.included_with_waf_rule import IncludedWithWafRule
+    from fastly.model.waf_rule_response_data import WafRuleResponseData
+    globals()['IncludedWithWafRule'] = IncludedWithWafRule
+    globals()['WafRuleResponseData'] = WafRuleResponseData
 
 
-class WafFirewallVersionResponseDataAllOf(ModelNormal):
+class WafRuleResponse(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -83,40 +83,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'id': (str,),  # noqa: E501
-            'attributes': (WafFirewallVersionResponseDataAttributes,),  # noqa: E501
-            'relationships': (RelationshipsForWafFirewallVersion,),  # noqa: E501
+            'data': (WafRuleResponseData,),  # noqa: E501
+            'included': (IncludedWithWafRule,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'attributes': 'attributes',  # noqa: E501
-        'relationships': 'relationships',  # noqa: E501
+        'data': 'data',  # noqa: E501
+        'included': 'included',  # noqa: E501
     }
 
     read_only_vars = {
-        'id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafFirewallVersionResponseDataAllOf - a model defined in OpenAPI
+        """WafRuleResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -141,17 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): Alphanumeric string identifying a Firewall version.. [optional]  # noqa: E501
-            attributes (WafFirewallVersionResponseDataAttributes): [optional]  # noqa: E501
-            relationships (RelationshipsForWafFirewallVersion): [optional]  # noqa: E501
+            data (WafRuleResponseData): [optional]  # noqa: E501
+            included (IncludedWithWafRule): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -192,15 +188,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafFirewallVersionResponseDataAllOf - a model defined in OpenAPI
+        """WafRuleResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -225,17 +221,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): Alphanumeric string identifying a Firewall version.. [optional]  # noqa: E501
-            attributes (WafFirewallVersionResponseDataAttributes): [optional]  # noqa: E501
-            relationships (RelationshipsForWafFirewallVersion): [optional]  # noqa: E501
+            data (WafRuleResponseData): [optional]  # noqa: E501
+            included (IncludedWithWafRule): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/waf_firewall_version_response_data_attributes.py` & `fastly-1.3.1/fastly/model/waf_firewall_version_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_firewall_version_response_data_attributes_all_of.py` & `fastly-1.3.1/fastly/model/waf_firewall_version_response_data_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_firewall_versions_response.py` & `fastly-1.3.1/fastly/model/waf_firewall_versions_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_firewall_versions_response_all_of.py` & `fastly-1.3.1/fastly/model/waf_firewall_versions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_firewalls_response.py` & `fastly-1.3.1/fastly/model/waf_firewalls_response.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_firewalls_response_all_of.py` & `fastly-1.3.1/fastly/model/waf_rules_response_all_of.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.included_with_waf_firewall import IncludedWithWafFirewall
-    from fastly.model.waf_firewall_response_data import WafFirewallResponseData
-    globals()['IncludedWithWafFirewall'] = IncludedWithWafFirewall
-    globals()['WafFirewallResponseData'] = WafFirewallResponseData
+    from fastly.model.included_with_waf_rule import IncludedWithWafRule
+    from fastly.model.waf_rule_response_data import WafRuleResponseData
+    globals()['IncludedWithWafRule'] = IncludedWithWafRule
+    globals()['WafRuleResponseData'] = WafRuleResponseData
 
 
-class WafFirewallsResponseAllOf(ModelNormal):
+class WafRulesResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -83,16 +83,16 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([WafFirewallResponseData],),  # noqa: E501
-            'included': (IncludedWithWafFirewall,),  # noqa: E501
+            'data': ([WafRuleResponseData],),  # noqa: E501
+            'included': (IncludedWithWafRule,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -105,15 +105,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafFirewallsResponseAllOf - a model defined in OpenAPI
+        """WafRulesResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,16 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([WafFirewallResponseData]): [optional]  # noqa: E501
-            included (IncludedWithWafFirewall): [optional]  # noqa: E501
+            data ([WafRuleResponseData]): [optional]  # noqa: E501
+            included (IncludedWithWafRule): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -188,15 +188,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafFirewallsResponseAllOf - a model defined in OpenAPI
+        """WafRulesResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -221,16 +221,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([WafFirewallResponseData]): [optional]  # noqa: E501
-            included (IncludedWithWafFirewall): [optional]  # noqa: E501
+            data ([WafRuleResponseData]): [optional]  # noqa: E501
+            included (IncludedWithWafRule): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/waf_rule.py` & `fastly-1.3.1/fastly/model/waf_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_rule_attributes.py` & `fastly-1.3.1/fastly/model/waf_rule_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_rule_response.py` & `fastly-1.3.1/fastly/model/waf_rule_revisions_response_all_of.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.included_with_waf_rule import IncludedWithWafRule
-    from fastly.model.waf_rule_response_data import WafRuleResponseData
-    globals()['IncludedWithWafRule'] = IncludedWithWafRule
-    globals()['WafRuleResponseData'] = WafRuleResponseData
+    from fastly.model.included_with_waf_rule_revision import IncludedWithWafRuleRevision
+    from fastly.model.waf_rule_revision_response_data import WafRuleRevisionResponseData
+    globals()['IncludedWithWafRuleRevision'] = IncludedWithWafRuleRevision
+    globals()['WafRuleRevisionResponseData'] = WafRuleRevisionResponseData
 
 
-class WafRuleResponse(ModelNormal):
+class WafRuleRevisionsResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -83,16 +83,16 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (WafRuleResponseData,),  # noqa: E501
-            'included': (IncludedWithWafRule,),  # noqa: E501
+            'data': ([WafRuleRevisionResponseData],),  # noqa: E501
+            'included': (IncludedWithWafRuleRevision,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -105,15 +105,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafRuleResponse - a model defined in OpenAPI
+        """WafRuleRevisionsResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,16 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (WafRuleResponseData): [optional]  # noqa: E501
-            included (IncludedWithWafRule): [optional]  # noqa: E501
+            data ([WafRuleRevisionResponseData]): [optional]  # noqa: E501
+            included (IncludedWithWafRuleRevision): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -188,15 +188,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafRuleResponse - a model defined in OpenAPI
+        """WafRuleRevisionsResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -221,16 +221,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (WafRuleResponseData): [optional]  # noqa: E501
-            included (IncludedWithWafRule): [optional]  # noqa: E501
+            data ([WafRuleRevisionResponseData]): [optional]  # noqa: E501
+            included (IncludedWithWafRuleRevision): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/waf_rule_response_data.py` & `fastly-1.3.1/fastly/model/waf_rule_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_rule_response_data_all_of.py` & `fastly-1.3.1/fastly/model/waf_rule_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_rule_revision.py` & `fastly-1.3.1/fastly/model/waf_rule_revision_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.type_waf_rule_revision import TypeWafRuleRevision
-    from fastly.model.waf_rule_revision_attributes import WafRuleRevisionAttributes
-    globals()['TypeWafRuleRevision'] = TypeWafRuleRevision
-    globals()['WafRuleRevisionAttributes'] = WafRuleRevisionAttributes
+    from fastly.model.included_with_waf_rule_revision import IncludedWithWafRuleRevision
+    from fastly.model.waf_rule_revision_response_data import WafRuleRevisionResponseData
+    globals()['IncludedWithWafRuleRevision'] = IncludedWithWafRuleRevision
+    globals()['WafRuleRevisionResponseData'] = WafRuleRevisionResponseData
 
 
-class WafRuleRevision(ModelNormal):
+class WafRuleRevisionResponse(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -83,40 +83,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'type': (TypeWafRuleRevision,),  # noqa: E501
-            'id': (str,),  # noqa: E501
-            'attributes': (WafRuleRevisionAttributes,),  # noqa: E501
+            'data': (WafRuleRevisionResponseData,),  # noqa: E501
+            'included': (IncludedWithWafRuleRevision,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'type': 'type',  # noqa: E501
-        'id': 'id',  # noqa: E501
-        'attributes': 'attributes',  # noqa: E501
+        'data': 'data',  # noqa: E501
+        'included': 'included',  # noqa: E501
     }
 
     read_only_vars = {
-        'id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafRuleRevision - a model defined in OpenAPI
+        """WafRuleRevisionResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -141,17 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (TypeWafRuleRevision): [optional]  # noqa: E501
-            id (str): Alphanumeric string identifying a WAF rule revision.. [optional]  # noqa: E501
-            attributes (WafRuleRevisionAttributes): [optional]  # noqa: E501
+            data (WafRuleRevisionResponseData): [optional]  # noqa: E501
+            included (IncludedWithWafRuleRevision): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -192,15 +188,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafRuleRevision - a model defined in OpenAPI
+        """WafRuleRevisionResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -225,17 +221,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (TypeWafRuleRevision): [optional]  # noqa: E501
-            id (str): Alphanumeric string identifying a WAF rule revision.. [optional]  # noqa: E501
-            attributes (WafRuleRevisionAttributes): [optional]  # noqa: E501
+            data (WafRuleRevisionResponseData): [optional]  # noqa: E501
+            included (IncludedWithWafRuleRevision): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-1.3.0/fastly/model/waf_rule_revision_attributes.py` & `fastly-1.3.1/fastly/model/waf_rule_revision_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/fastly/model/waf_rule_revision_or_latest.py` & `fastly-1.3.1/fastly/model/waf_rule_revision_response_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,16 +25,28 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fastly.model.relationship_waf_rule import RelationshipWafRule
+    from fastly.model.type_waf_rule_revision import TypeWafRuleRevision
+    from fastly.model.waf_rule_revision import WafRuleRevision
+    from fastly.model.waf_rule_revision_attributes import WafRuleRevisionAttributes
+    from fastly.model.waf_rule_revision_response_data_all_of import WafRuleRevisionResponseDataAllOf
+    globals()['RelationshipWafRule'] = RelationshipWafRule
+    globals()['TypeWafRuleRevision'] = TypeWafRuleRevision
+    globals()['WafRuleRevision'] = WafRuleRevision
+    globals()['WafRuleRevisionAttributes'] = WafRuleRevisionAttributes
+    globals()['WafRuleRevisionResponseDataAllOf'] = WafRuleRevisionResponseDataAllOf
 
-class WafRuleRevisionOrLatest(ModelNormal):
+
+class WafRuleRevisionResponseData(ModelComposed):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -60,48 +72,57 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
+            'type': (TypeWafRuleRevision,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'attributes': (WafRuleRevisionAttributes,),  # noqa: E501
+            'relationships': (RelationshipWafRule,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'type': 'type',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
+        'relationships': 'relationships',  # noqa: E501
     }
 
     read_only_vars = {
+        'id',  # noqa: E501
     }
 
-    _composed_schemas = {}
-
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafRuleRevisionOrLatest - a model defined in OpenAPI
+        """WafRuleRevisionResponseData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -126,14 +147,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            type (TypeWafRuleRevision): [optional]  # noqa: E501
+            id (str): Alphanumeric string identifying a WAF rule revision.. [optional]  # noqa: E501
+            attributes (WafRuleRevisionAttributes): [optional]  # noqa: E501
+            relationships (RelationshipWafRule): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -153,36 +178,54 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        constant_args = {
+            '_check_type': _check_type,
+            '_path_to_item': _path_to_item,
+            '_spec_property_naming': _spec_property_naming,
+            '_configuration': _configuration,
+            '_visited_composed_classes': self._visited_composed_classes,
+        }
+        composed_info = validate_get_composed_info(
+            constant_args, kwargs, self)
+        self._composed_instances = composed_info[0]
+        self._var_name_to_model_instances = composed_info[1]
+        self._additional_properties_model_instances = composed_info[2]
+        discarded_args = composed_info[3]
+
         for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
+            if var_name in discarded_args and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
+                        self._additional_properties_model_instances:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
+
         return self
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
+        '_composed_instances',
+        '_var_name_to_model_instances',
+        '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafRuleRevisionOrLatest - a model defined in OpenAPI
+        """WafRuleRevisionResponseData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -207,14 +250,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            type (TypeWafRuleRevision): [optional]  # noqa: E501
+            id (str): Alphanumeric string identifying a WAF rule revision.. [optional]  # noqa: E501
+            attributes (WafRuleRevisionAttributes): [optional]  # noqa: E501
+            relationships (RelationshipWafRule): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -232,18 +279,53 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        constant_args = {
+            '_check_type': _check_type,
+            '_path_to_item': _path_to_item,
+            '_spec_property_naming': _spec_property_naming,
+            '_configuration': _configuration,
+            '_visited_composed_classes': self._visited_composed_classes,
+        }
+        composed_info = validate_get_composed_info(
+            constant_args, kwargs, self)
+        self._composed_instances = composed_info[0]
+        self._var_name_to_model_instances = composed_info[1]
+        self._additional_properties_model_instances = composed_info[2]
+        discarded_args = composed_info[3]
+
         for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
+            if var_name in discarded_args and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
+                        self._additional_properties_model_instances:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
             if var_name in self.read_only_vars:
                 raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
                                      f"class with read only attributes.")
+
+    @cached_property
+    def _composed_schemas():
+        # we need this here to make our import statements work
+        # we must store _composed_schemas in here so the code is only run
+        # when we invoke this method. If we kept this at the class
+        # level we would get an error because the class level
+        # code would be run when this module is imported, and these composed
+        # classes don't exist yet because their module has not finished
+        # loading
+        lazy_import()
+        return {
+          'anyOf': [
+          ],
+          'allOf': [
+              WafRuleRevision,
+              WafRuleRevisionResponseDataAllOf,
+          ],
+          'oneOf': [
+          ],
+        }
```

### Comparing `fastly-1.3.0/fastly/model/waf_rule_revision_response.py` & `fastly-1.3.1/fastly/model/waf_rule_revisions_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,20 +27,28 @@
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from fastly.model.included_with_waf_rule_revision import IncludedWithWafRuleRevision
+    from fastly.model.pagination import Pagination
+    from fastly.model.pagination_links import PaginationLinks
+    from fastly.model.pagination_meta import PaginationMeta
     from fastly.model.waf_rule_revision_response_data import WafRuleRevisionResponseData
+    from fastly.model.waf_rule_revisions_response_all_of import WafRuleRevisionsResponseAllOf
     globals()['IncludedWithWafRuleRevision'] = IncludedWithWafRuleRevision
+    globals()['Pagination'] = Pagination
+    globals()['PaginationLinks'] = PaginationLinks
+    globals()['PaginationMeta'] = PaginationMeta
     globals()['WafRuleRevisionResponseData'] = WafRuleRevisionResponseData
+    globals()['WafRuleRevisionsResponseAllOf'] = WafRuleRevisionsResponseAllOf
 
 
-class WafRuleRevisionResponse(ModelNormal):
+class WafRuleRevisionsResponse(ModelComposed):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -83,37 +91,39 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (WafRuleRevisionResponseData,),  # noqa: E501
+            'links': (PaginationLinks,),  # noqa: E501
+            'meta': (PaginationMeta,),  # noqa: E501
+            'data': ([WafRuleRevisionResponseData],),  # noqa: E501
             'included': (IncludedWithWafRuleRevision,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'links': 'links',  # noqa: E501
+        'meta': 'meta',  # noqa: E501
         'data': 'data',  # noqa: E501
         'included': 'included',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
-    _composed_schemas = {}
-
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafRuleRevisionResponse - a model defined in OpenAPI
+        """WafRuleRevisionsResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,15 +148,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (WafRuleRevisionResponseData): [optional]  # noqa: E501
+            links (PaginationLinks): [optional]  # noqa: E501
+            meta (PaginationMeta): [optional]  # noqa: E501
+            data ([WafRuleRevisionResponseData]): [optional]  # noqa: E501
             included (IncludedWithWafRuleRevision): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -167,36 +179,54 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        constant_args = {
+            '_check_type': _check_type,
+            '_path_to_item': _path_to_item,
+            '_spec_property_naming': _spec_property_naming,
+            '_configuration': _configuration,
+            '_visited_composed_classes': self._visited_composed_classes,
+        }
+        composed_info = validate_get_composed_info(
+            constant_args, kwargs, self)
+        self._composed_instances = composed_info[0]
+        self._var_name_to_model_instances = composed_info[1]
+        self._additional_properties_model_instances = composed_info[2]
+        discarded_args = composed_info[3]
+
         for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
+            if var_name in discarded_args and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
+                        self._additional_properties_model_instances:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
+
         return self
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
+        '_composed_instances',
+        '_var_name_to_model_instances',
+        '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafRuleRevisionResponse - a model defined in OpenAPI
+        """WafRuleRevisionsResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -221,15 +251,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (WafRuleRevisionResponseData): [optional]  # noqa: E501
+            links (PaginationLinks): [optional]  # noqa: E501
+            meta (PaginationMeta): [optional]  # noqa: E501
+            data ([WafRuleRevisionResponseData]): [optional]  # noqa: E501
             included (IncludedWithWafRuleRevision): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -248,18 +280,53 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        constant_args = {
+            '_check_type': _check_type,
+            '_path_to_item': _path_to_item,
+            '_spec_property_naming': _spec_property_naming,
+            '_configuration': _configuration,
+            '_visited_composed_classes': self._visited_composed_classes,
+        }
+        composed_info = validate_get_composed_info(
+            constant_args, kwargs, self)
+        self._composed_instances = composed_info[0]
+        self._var_name_to_model_instances = composed_info[1]
+        self._additional_properties_model_instances = composed_info[2]
+        discarded_args = composed_info[3]
+
         for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
+            if var_name in discarded_args and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
+                        self._additional_properties_model_instances:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
             if var_name in self.read_only_vars:
                 raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
                                      f"class with read only attributes.")
+
+    @cached_property
+    def _composed_schemas():
+        # we need this here to make our import statements work
+        # we must store _composed_schemas in here so the code is only run
+        # when we invoke this method. If we kept this at the class
+        # level we would get an error because the class level
+        # code would be run when this module is imported, and these composed
+        # classes don't exist yet because their module has not finished
+        # loading
+        lazy_import()
+        return {
+          'anyOf': [
+          ],
+          'allOf': [
+              Pagination,
+              WafRuleRevisionsResponseAllOf,
+          ],
+          'oneOf': [
+          ],
+        }
```

### Comparing `fastly-1.3.0/fastly/model/waf_rule_revision_response_data.py` & `fastly-1.3.1/fastly/model/waf_tags_response_data_item.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,26 +27,26 @@
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from fastly.model.relationship_waf_rule import RelationshipWafRule
-    from fastly.model.type_waf_rule_revision import TypeWafRuleRevision
-    from fastly.model.waf_rule_revision import WafRuleRevision
-    from fastly.model.waf_rule_revision_attributes import WafRuleRevisionAttributes
+    from fastly.model.type_waf_tag import TypeWafTag
     from fastly.model.waf_rule_revision_response_data_all_of import WafRuleRevisionResponseDataAllOf
+    from fastly.model.waf_tag import WafTag
+    from fastly.model.waf_tag_attributes import WafTagAttributes
     globals()['RelationshipWafRule'] = RelationshipWafRule
-    globals()['TypeWafRuleRevision'] = TypeWafRuleRevision
-    globals()['WafRuleRevision'] = WafRuleRevision
-    globals()['WafRuleRevisionAttributes'] = WafRuleRevisionAttributes
+    globals()['TypeWafTag'] = TypeWafTag
     globals()['WafRuleRevisionResponseDataAllOf'] = WafRuleRevisionResponseDataAllOf
+    globals()['WafTag'] = WafTag
+    globals()['WafTagAttributes'] = WafTagAttributes
 
 
-class WafRuleRevisionResponseData(ModelComposed):
+class WafTagsResponseDataItem(ModelComposed):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -89,17 +89,17 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'type': (TypeWafRuleRevision,),  # noqa: E501
+            'type': (TypeWafTag,),  # noqa: E501
             'id': (str,),  # noqa: E501
-            'attributes': (WafRuleRevisionAttributes,),  # noqa: E501
+            'attributes': (WafTagAttributes,),  # noqa: E501
             'relationships': (RelationshipWafRule,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -114,15 +114,15 @@
     read_only_vars = {
         'id',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafRuleRevisionResponseData - a model defined in OpenAPI
+        """WafTagsResponseDataItem - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -147,17 +147,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (TypeWafRuleRevision): [optional]  # noqa: E501
-            id (str): Alphanumeric string identifying a WAF rule revision.. [optional]  # noqa: E501
-            attributes (WafRuleRevisionAttributes): [optional]  # noqa: E501
+            type (TypeWafTag): [optional]  # noqa: E501
+            id (str): Alphanumeric string identifying a WAF tag.. [optional]  # noqa: E501
+            attributes (WafTagAttributes): [optional]  # noqa: E501
             relationships (RelationshipWafRule): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -217,15 +217,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafRuleRevisionResponseData - a model defined in OpenAPI
+        """WafTagsResponseDataItem - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -250,17 +250,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (TypeWafRuleRevision): [optional]  # noqa: E501
-            id (str): Alphanumeric string identifying a WAF rule revision.. [optional]  # noqa: E501
-            attributes (WafRuleRevisionAttributes): [optional]  # noqa: E501
+            type (TypeWafTag): [optional]  # noqa: E501
+            id (str): Alphanumeric string identifying a WAF tag.. [optional]  # noqa: E501
+            attributes (WafTagAttributes): [optional]  # noqa: E501
             relationships (RelationshipWafRule): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -319,13 +319,13 @@
         # classes don't exist yet because their module has not finished
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
-              WafRuleRevision,
               WafRuleRevisionResponseDataAllOf,
+              WafTag,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `fastly-1.3.0/fastly/model/waf_rule_revision_response_data_all_of.py` & `fastly-1.3.1/fastly/model/waf_rules_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,19 +26,29 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.relationship_waf_rule import RelationshipWafRule
-    globals()['RelationshipWafRule'] = RelationshipWafRule
+    from fastly.model.included_with_waf_rule import IncludedWithWafRule
+    from fastly.model.pagination import Pagination
+    from fastly.model.pagination_links import PaginationLinks
+    from fastly.model.pagination_meta import PaginationMeta
+    from fastly.model.waf_rule_response_data import WafRuleResponseData
+    from fastly.model.waf_rules_response_all_of import WafRulesResponseAllOf
+    globals()['IncludedWithWafRule'] = IncludedWithWafRule
+    globals()['Pagination'] = Pagination
+    globals()['PaginationLinks'] = PaginationLinks
+    globals()['PaginationMeta'] = PaginationMeta
+    globals()['WafRuleResponseData'] = WafRuleResponseData
+    globals()['WafRulesResponseAllOf'] = WafRulesResponseAllOf
 
 
-class WafRuleRevisionResponseDataAllOf(ModelNormal):
+class WafRulesResponse(ModelComposed):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -81,35 +91,39 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'relationships': (RelationshipWafRule,),  # noqa: E501
+            'links': (PaginationLinks,),  # noqa: E501
+            'meta': (PaginationMeta,),  # noqa: E501
+            'data': ([WafRuleResponseData],),  # noqa: E501
+            'included': (IncludedWithWafRule,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'relationships': 'relationships',  # noqa: E501
+        'links': 'links',  # noqa: E501
+        'meta': 'meta',  # noqa: E501
+        'data': 'data',  # noqa: E501
+        'included': 'included',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
-    _composed_schemas = {}
-
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafRuleRevisionResponseDataAllOf - a model defined in OpenAPI
+        """WafRulesResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +148,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            relationships (RelationshipWafRule): [optional]  # noqa: E501
+            links (PaginationLinks): [optional]  # noqa: E501
+            meta (PaginationMeta): [optional]  # noqa: E501
+            data ([WafRuleResponseData]): [optional]  # noqa: E501
+            included (IncludedWithWafRule): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -162,36 +179,54 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        constant_args = {
+            '_check_type': _check_type,
+            '_path_to_item': _path_to_item,
+            '_spec_property_naming': _spec_property_naming,
+            '_configuration': _configuration,
+            '_visited_composed_classes': self._visited_composed_classes,
+        }
+        composed_info = validate_get_composed_info(
+            constant_args, kwargs, self)
+        self._composed_instances = composed_info[0]
+        self._var_name_to_model_instances = composed_info[1]
+        self._additional_properties_model_instances = composed_info[2]
+        discarded_args = composed_info[3]
+
         for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
+            if var_name in discarded_args and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
+                        self._additional_properties_model_instances:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
+
         return self
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
+        '_composed_instances',
+        '_var_name_to_model_instances',
+        '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafRuleRevisionResponseDataAllOf - a model defined in OpenAPI
+        """WafRulesResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +251,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            relationships (RelationshipWafRule): [optional]  # noqa: E501
+            links (PaginationLinks): [optional]  # noqa: E501
+            meta (PaginationMeta): [optional]  # noqa: E501
+            data ([WafRuleResponseData]): [optional]  # noqa: E501
+            included (IncludedWithWafRule): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -242,18 +280,53 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        constant_args = {
+            '_check_type': _check_type,
+            '_path_to_item': _path_to_item,
+            '_spec_property_naming': _spec_property_naming,
+            '_configuration': _configuration,
+            '_visited_composed_classes': self._visited_composed_classes,
+        }
+        composed_info = validate_get_composed_info(
+            constant_args, kwargs, self)
+        self._composed_instances = composed_info[0]
+        self._var_name_to_model_instances = composed_info[1]
+        self._additional_properties_model_instances = composed_info[2]
+        discarded_args = composed_info[3]
+
         for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
+            if var_name in discarded_args and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
+                        self._additional_properties_model_instances:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
             if var_name in self.read_only_vars:
                 raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
                                      f"class with read only attributes.")
+
+    @cached_property
+    def _composed_schemas():
+        # we need this here to make our import statements work
+        # we must store _composed_schemas in here so the code is only run
+        # when we invoke this method. If we kept this at the class
+        # level we would get an error because the class level
+        # code would be run when this module is imported, and these composed
+        # classes don't exist yet because their module has not finished
+        # loading
+        lazy_import()
+        return {
+          'anyOf': [
+          ],
+          'allOf': [
+              Pagination,
+              WafRulesResponseAllOf,
+          ],
+          'oneOf': [
+          ],
+        }
```

### Comparing `fastly-1.3.0/fastly/models/__init__.py` & `fastly-1.3.1/fastly/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,16 +78,14 @@
 from fastly.model.domain_check_response_list import DomainCheckResponseList
 from fastly.model.domain_response import DomainResponse
 from fastly.model.domains_response import DomainsResponse
 from fastly.model.enabled_product_response import EnabledProductResponse
 from fastly.model.enabled_product_response_links import EnabledProductResponseLinks
 from fastly.model.enabled_product_response_product import EnabledProductResponseProduct
 from fastly.model.enabled_product_response_service import EnabledProductResponseService
-from fastly.model.error_response import ErrorResponse
-from fastly.model.error_response_data import ErrorResponseData
 from fastly.model.event import Event
 from fastly.model.event_attributes import EventAttributes
 from fastly.model.event_response import EventResponse
 from fastly.model.events_response import EventsResponse
 from fastly.model.events_response_all_of import EventsResponseAllOf
 from fastly.model.generic_token_error import GenericTokenError
 from fastly.model.gzip import Gzip
@@ -360,15 +358,14 @@
 from fastly.model.relationship_waf_tags_waf_tags import RelationshipWafTagsWafTags
 from fastly.model.relationships_for_invitation import RelationshipsForInvitation
 from fastly.model.relationships_for_mutual_authentication import RelationshipsForMutualAuthentication
 from fastly.model.relationships_for_star import RelationshipsForStar
 from fastly.model.relationships_for_tls_activation import RelationshipsForTlsActivation
 from fastly.model.relationships_for_tls_bulk_certificate import RelationshipsForTlsBulkCertificate
 from fastly.model.relationships_for_tls_configuration import RelationshipsForTlsConfiguration
-from fastly.model.relationships_for_tls_csr import RelationshipsForTlsCsr
 from fastly.model.relationships_for_tls_domain import RelationshipsForTlsDomain
 from fastly.model.relationships_for_tls_private_key import RelationshipsForTlsPrivateKey
 from fastly.model.relationships_for_tls_subscription import RelationshipsForTlsSubscription
 from fastly.model.relationships_for_waf_active_rule import RelationshipsForWafActiveRule
 from fastly.model.relationships_for_waf_exclusion import RelationshipsForWafExclusion
 from fastly.model.relationships_for_waf_firewall_version import RelationshipsForWafFirewallVersion
 from fastly.model.relationships_for_waf_rule import RelationshipsForWafRule
@@ -470,20 +467,14 @@
 from fastly.model.tls_configuration_response import TlsConfigurationResponse
 from fastly.model.tls_configuration_response_attributes import TlsConfigurationResponseAttributes
 from fastly.model.tls_configuration_response_attributes_all_of import TlsConfigurationResponseAttributesAllOf
 from fastly.model.tls_configuration_response_data import TlsConfigurationResponseData
 from fastly.model.tls_configuration_response_data_all_of import TlsConfigurationResponseDataAllOf
 from fastly.model.tls_configurations_response import TlsConfigurationsResponse
 from fastly.model.tls_configurations_response_all_of import TlsConfigurationsResponseAllOf
-from fastly.model.tls_csr import TlsCsr
-from fastly.model.tls_csr_data import TlsCsrData
-from fastly.model.tls_csr_data_attributes import TlsCsrDataAttributes
-from fastly.model.tls_csr_response import TlsCsrResponse
-from fastly.model.tls_csr_response_attributes import TlsCsrResponseAttributes
-from fastly.model.tls_csr_response_data import TlsCsrResponseData
 from fastly.model.tls_dns_record import TlsDnsRecord
 from fastly.model.tls_domain_data import TlsDomainData
 from fastly.model.tls_domains_response import TlsDomainsResponse
 from fastly.model.tls_domains_response_all_of import TlsDomainsResponseAllOf
 from fastly.model.tls_private_key import TlsPrivateKey
 from fastly.model.tls_private_key_data import TlsPrivateKeyData
 from fastly.model.tls_private_key_data_attributes import TlsPrivateKeyDataAttributes
@@ -519,15 +510,14 @@
 from fastly.model.type_service_authorization import TypeServiceAuthorization
 from fastly.model.type_service_invitation import TypeServiceInvitation
 from fastly.model.type_star import TypeStar
 from fastly.model.type_tls_activation import TypeTlsActivation
 from fastly.model.type_tls_bulk_certificate import TypeTlsBulkCertificate
 from fastly.model.type_tls_certificate import TypeTlsCertificate
 from fastly.model.type_tls_configuration import TypeTlsConfiguration
-from fastly.model.type_tls_csr import TypeTlsCsr
 from fastly.model.type_tls_dns_record import TypeTlsDnsRecord
 from fastly.model.type_tls_domain import TypeTlsDomain
 from fastly.model.type_tls_private_key import TypeTlsPrivateKey
 from fastly.model.type_tls_subscription import TypeTlsSubscription
 from fastly.model.type_user import TypeUser
 from fastly.model.type_waf_active_rule import TypeWafActiveRule
 from fastly.model.type_waf_exclusion import TypeWafExclusion
```

### Comparing `fastly-1.3.0/.gitignore` & `fastly-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/LICENSE` & `fastly-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastly-1.3.0/README.md` & `fastly-1.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,14 @@
 
 A Python client library for interacting with most facets of the [Fastly API](https://developer.fastly.com/reference/api).
 
 > NOTE: This 1.x release is a new [generated API client](https://dev.to/fastly/better-fastly-api-clients-with-openapi-generator-3lno) for the Fastly API.
 > The previous 0.5.x version is no longer supported, but can be found at https://github.com/fastly/fastly-py/tree/v0.5.x.
 
 
-    > ⚠️ This client library (`1.3.0`)  is an early-access release. Features may change without notice. Use at your own risk.
-
-**We strongly recommend that you do not install alpha and beta releases on live production services.** No official support is provided for such releases. Please try out the library in a test environment, see what breaks without worrying about consequences, and give us [feedback](#issues).
-
-Read about the [Fastly Product Lifecycle](https://docs.fastly.com/products/fastly-product-lifecycle).
-
 
 ## Requirements
 
 Python >=3.6
 
 ## Installation
 
@@ -408,15 +402,14 @@
 *TlsCertificatesApi* | [**delete_tls_cert**](docs/TlsCertificatesApi.md#delete_tls_cert) | **DELETE** /tls/certificates/{tls_certificate_id} | Delete a TLS certificate
 *TlsCertificatesApi* | [**get_tls_cert**](docs/TlsCertificatesApi.md#get_tls_cert) | **GET** /tls/certificates/{tls_certificate_id} | Get a TLS certificate
 *TlsCertificatesApi* | [**list_tls_certs**](docs/TlsCertificatesApi.md#list_tls_certs) | **GET** /tls/certificates | List TLS certificates
 *TlsCertificatesApi* | [**update_tls_cert**](docs/TlsCertificatesApi.md#update_tls_cert) | **PATCH** /tls/certificates/{tls_certificate_id} | Update a TLS certificate
 *TlsConfigurationsApi* | [**get_tls_config**](docs/TlsConfigurationsApi.md#get_tls_config) | **GET** /tls/configurations/{tls_configuration_id} | Get a TLS configuration
 *TlsConfigurationsApi* | [**list_tls_configs**](docs/TlsConfigurationsApi.md#list_tls_configs) | **GET** /tls/configurations | List TLS configurations
 *TlsConfigurationsApi* | [**update_tls_config**](docs/TlsConfigurationsApi.md#update_tls_config) | **PATCH** /tls/configurations/{tls_configuration_id} | Update a TLS configuration
-*TlsCsrsApi* | [**create_csr**](docs/TlsCsrsApi.md#create_csr) | **POST** /tls/certificate_signing_requests | Create CSR
 *TlsDomainsApi* | [**list_tls_domains**](docs/TlsDomainsApi.md#list_tls_domains) | **GET** /tls/domains | List TLS domains
 *TlsPrivateKeysApi* | [**create_tls_key**](docs/TlsPrivateKeysApi.md#create_tls_key) | **POST** /tls/private_keys | Create a TLS private key
 *TlsPrivateKeysApi* | [**delete_tls_key**](docs/TlsPrivateKeysApi.md#delete_tls_key) | **DELETE** /tls/private_keys/{tls_private_key_id} | Delete a TLS private key
 *TlsPrivateKeysApi* | [**get_tls_key**](docs/TlsPrivateKeysApi.md#get_tls_key) | **GET** /tls/private_keys/{tls_private_key_id} | Get a TLS private key
 *TlsPrivateKeysApi* | [**list_tls_keys**](docs/TlsPrivateKeysApi.md#list_tls_keys) | **GET** /tls/private_keys | List TLS private keys
 *TlsSubscriptionsApi* | [**create_globalsign_email_challenge**](docs/TlsSubscriptionsApi.md#create_globalsign_email_challenge) | **POST** /tls/subscriptions/{tls_subscription_id}/authorizations/{tls_authorization_id}/globalsign_email_challenges | Creates a GlobalSign email challenge.
 *TlsSubscriptionsApi* | [**create_tls_sub**](docs/TlsSubscriptionsApi.md#create_tls_sub) | **POST** /tls/subscriptions | Create a TLS subscription
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fastly-1.3.0/pyproject.toml` & `fastly-1.3.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastly"
-version = "1.3.0"
+version = "1.3.1"
 authors = [{ name = "Fastly", email = "oss@fastly.com" }]
 description = "A Python Fastly API client library"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `fastly-1.3.0/PKG-INFO` & `fastly-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastly
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Python Fastly API client library
 Project-URL: Homepage, https://github.com/fastly/fastly-py
 Project-URL: Bug Tracker, https://github.com/fastly/fastly-py/issues
 Author-email: Fastly <oss@fastly.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,20 +16,14 @@
 
 A Python client library for interacting with most facets of the [Fastly API](https://developer.fastly.com/reference/api).
 
 > NOTE: This 1.x release is a new [generated API client](https://dev.to/fastly/better-fastly-api-clients-with-openapi-generator-3lno) for the Fastly API.
 > The previous 0.5.x version is no longer supported, but can be found at https://github.com/fastly/fastly-py/tree/v0.5.x.
 
 
-    > ⚠️ This client library (`1.3.0`)  is an early-access release. Features may change without notice. Use at your own risk.
-
-**We strongly recommend that you do not install alpha and beta releases on live production services.** No official support is provided for such releases. Please try out the library in a test environment, see what breaks without worrying about consequences, and give us [feedback](#issues).
-
-Read about the [Fastly Product Lifecycle](https://docs.fastly.com/products/fastly-product-lifecycle).
-
 
 ## Requirements
 
 Python >=3.6
 
 ## Installation
 
@@ -422,15 +416,14 @@
 *TlsCertificatesApi* | [**delete_tls_cert**](docs/TlsCertificatesApi.md#delete_tls_cert) | **DELETE** /tls/certificates/{tls_certificate_id} | Delete a TLS certificate
 *TlsCertificatesApi* | [**get_tls_cert**](docs/TlsCertificatesApi.md#get_tls_cert) | **GET** /tls/certificates/{tls_certificate_id} | Get a TLS certificate
 *TlsCertificatesApi* | [**list_tls_certs**](docs/TlsCertificatesApi.md#list_tls_certs) | **GET** /tls/certificates | List TLS certificates
 *TlsCertificatesApi* | [**update_tls_cert**](docs/TlsCertificatesApi.md#update_tls_cert) | **PATCH** /tls/certificates/{tls_certificate_id} | Update a TLS certificate
 *TlsConfigurationsApi* | [**get_tls_config**](docs/TlsConfigurationsApi.md#get_tls_config) | **GET** /tls/configurations/{tls_configuration_id} | Get a TLS configuration
 *TlsConfigurationsApi* | [**list_tls_configs**](docs/TlsConfigurationsApi.md#list_tls_configs) | **GET** /tls/configurations | List TLS configurations
 *TlsConfigurationsApi* | [**update_tls_config**](docs/TlsConfigurationsApi.md#update_tls_config) | **PATCH** /tls/configurations/{tls_configuration_id} | Update a TLS configuration
-*TlsCsrsApi* | [**create_csr**](docs/TlsCsrsApi.md#create_csr) | **POST** /tls/certificate_signing_requests | Create CSR
 *TlsDomainsApi* | [**list_tls_domains**](docs/TlsDomainsApi.md#list_tls_domains) | **GET** /tls/domains | List TLS domains
 *TlsPrivateKeysApi* | [**create_tls_key**](docs/TlsPrivateKeysApi.md#create_tls_key) | **POST** /tls/private_keys | Create a TLS private key
 *TlsPrivateKeysApi* | [**delete_tls_key**](docs/TlsPrivateKeysApi.md#delete_tls_key) | **DELETE** /tls/private_keys/{tls_private_key_id} | Delete a TLS private key
 *TlsPrivateKeysApi* | [**get_tls_key**](docs/TlsPrivateKeysApi.md#get_tls_key) | **GET** /tls/private_keys/{tls_private_key_id} | Get a TLS private key
 *TlsPrivateKeysApi* | [**list_tls_keys**](docs/TlsPrivateKeysApi.md#list_tls_keys) | **GET** /tls/private_keys | List TLS private keys
 *TlsSubscriptionsApi* | [**create_globalsign_email_challenge**](docs/TlsSubscriptionsApi.md#create_globalsign_email_challenge) | **POST** /tls/subscriptions/{tls_subscription_id}/authorizations/{tls_authorization_id}/globalsign_email_challenges | Creates a GlobalSign email challenge.
 *TlsSubscriptionsApi* | [**create_tls_sub**](docs/TlsSubscriptionsApi.md#create_tls_sub) | **POST** /tls/subscriptions | Create a TLS subscription
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

