# Comparing `tmp/ekonlpy-1.1.6.tar.gz` & `tmp/ekonlpy-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ekonlpy-1.1.6.tar", max compression
+gzip compressed data, was "ekonlpy-1.1.7.tar", max compression
```

## Comparing `ekonlpy-1.1.6.tar` & `ekonlpy-1.1.7.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1071 2023-04-21 11:38:41.100572 ekonlpy-1.1.6/LICENSE
--rw-r--r--   0        0        0     8562 2023-04-21 11:38:41.100572 ekonlpy-1.1.6/README.md
--rw-r--r--   0        0        0     3580 2023-04-21 11:39:23.547649 ekonlpy-1.1.6/pyproject.toml
--rw-r--r--   0        0        0      271 2023-04-21 11:38:41.204573 ekonlpy-1.1.6/src/ekonlpy/__init__.py
--rw-r--r--   0        0        0       22 2023-04-21 11:39:23.471644 ekonlpy-1.1.6/src/ekonlpy/_version.py
--rw-r--r--   0        0        0       31 2023-04-21 11:38:41.204573 ekonlpy-1.1.6/src/ekonlpy/data/__init__.py
--rw-r--r--   0        0        0      514 2023-04-21 11:38:41.204573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/ADJECTIVES.txt
--rw-r--r--   0        0        0      108 2023-04-21 11:38:41.204573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/ADVERBS.txt
--rw-r--r--   0        0        0     2583 2023-04-21 11:38:41.204573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/COUNTRY.txt
--rw-r--r--   0        0        0       17 2023-04-21 11:38:41.204573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/CURRENCY.txt
--rw-r--r--   0        0        0    47727 2023-04-21 11:38:41.208573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/ECON_PHRASES.txt
--rw-r--r--   0        0        0   475773 2023-04-21 11:38:41.220573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/ECON_TERMS.txt
--rwxr-xr-x   0        0        0    77542 2023-04-21 11:38:41.220573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/ENTITY.txt
--rw-r--r--   0        0        0     9629 2023-04-21 11:38:41.220573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/FOREIGN_TERMS.txt
--rw-r--r--   0        0        0     2077 2023-04-21 11:38:41.220573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/GENERIC.txt
--rw-r--r--   0        0        0    35442 2023-04-21 11:38:41.220573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/INDUSTRY_TERMS.txt
--rw-r--r--   0        0        0    69192 2023-04-21 11:38:41.220573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/INSTITUTION.txt
--rw-r--r--   0        0        0    20594 2023-04-21 11:38:41.220573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/LEMMA.txt
--rw-r--r--   0        0        0     2072 2023-04-21 11:38:41.220573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/NAMES.txt
--rw-r--r--   0        0        0      687 2023-04-21 11:38:41.220573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/NOUNS.txt
--rw-r--r--   0        0        0    10396 2023-04-21 11:38:41.224573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/POLARITY_PHRASES.txt
--rw-r--r--   0        0        0    12378 2023-04-21 11:38:41.224573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/PROPER_NOUNS.txt
--rw-r--r--   0        0        0    14928 2023-04-21 11:38:41.224573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/SECTOR.txt
--rw-r--r--   0        0        0     6456 2023-04-21 11:38:41.224573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/STOPWORDS.txt
--rwxr-xr-x   0        0        0      260 2023-04-21 11:38:41.224573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/STOPWORDS_CUST.txt
--rw-r--r--   0        0        0     5788 2023-04-21 11:38:41.224573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/STOPWORDS_EN.txt
--rwxr-xr-x   0        0        0      598 2023-04-21 11:38:41.224573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/STOPWORDS_KOR.txt
--rw-r--r--   0        0        0    33685 2023-04-21 11:38:41.224573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/SYNONYM.txt
--rw-r--r--   0        0        0      300 2023-04-21 11:38:41.224573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/SYNONYM_MAG.txt
--rw-r--r--   0        0        0     5329 2023-04-21 11:38:41.224573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/SYNONYM_PHRASES.txt
--rw-r--r--   0        0        0    27207 2023-04-21 11:38:41.224573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/SYNONYM_TERMS.txt
--rw-r--r--   0        0        0       87 2023-04-21 11:38:41.224573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/SYNONYM_VA.txt
--rw-r--r--   0        0        0       69 2023-04-21 11:38:41.224573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/UNIT.txt
--rw-r--r--   0        0        0       40 2023-04-21 11:38:41.224573 ekonlpy-1.1.6/src/ekonlpy/data/dictionary/VERBS.txt
--rwxr-xr-x   0        0        0     1677 2023-04-21 11:38:41.224573 ekonlpy-1.1.6/src/ekonlpy/data/lexicon/Currencies.txt
--rwxr-xr-x   0        0        0      724 2023-04-21 11:38:41.224573 ekonlpy-1.1.6/src/ekonlpy/data/lexicon/DatesandNumbers.txt
--rwxr-xr-x   0        0        0     1798 2023-04-21 11:38:41.224573 ekonlpy-1.1.6/src/ekonlpy/data/lexicon/Generic.txt
--rwxr-xr-x   0        0        0     1622 2023-04-21 11:38:41.224573 ekonlpy-1.1.6/src/ekonlpy/data/lexicon/Geographic.txt
--rwxr-xr-x   0        0        0  2903900 2023-04-21 11:38:41.236573 ekonlpy-1.1.6/src/ekonlpy/data/lexicon/HIV-4.csv
--rwxr-xr-x   0        0        0  8373373 2023-04-21 11:38:41.288574 ekonlpy-1.1.6/src/ekonlpy/data/lexicon/LM.csv
--rwxr-xr-x   0        0        0    93474 2023-04-21 11:38:41.288574 ekonlpy-1.1.6/src/ekonlpy/data/lexicon/Names.txt
--rw-r--r--   0        0        0  3047832 2023-04-21 11:38:41.304574 ekonlpy-1.1.6/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_lex.csv
--rw-r--r--   0        0        0  2362210 2023-04-21 11:38:41.320574 ekonlpy-1.1.6/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_mkt.csv
--rwxr-xr-x   0        0        0   778128 2023-04-21 11:38:41.324574 ekonlpy-1.1.6/src/ekonlpy/data/lexicon/kosac/expressive-type.csv
--rwxr-xr-x   0        0        0   661841 2023-04-21 11:38:41.328574 ekonlpy-1.1.6/src/ekonlpy/data/lexicon/kosac/intensity.csv
--rwxr-xr-x   0        0        0   659879 2023-04-21 11:38:41.332574 ekonlpy-1.1.6/src/ekonlpy/data/lexicon/kosac/polarity.csv
--rw-r--r--   0        0        0  3226022 2023-04-21 11:38:41.352574 ekonlpy-1.1.6/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_lex.csv
--rw-r--r--   0        0        0  3832440 2023-04-21 11:38:41.376574 ekonlpy-1.1.6/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt.csv
--rw-r--r--   0        0        0  2735025 2023-04-21 11:38:41.392574 ekonlpy-1.1.6/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n3.csv
--rw-r--r--   0        0        0  3749409 2023-04-21 11:38:41.412575 ekonlpy-1.1.6/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n7.csv
--rw-r--r--   0        0        0  2835691 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/data/lexicon/mpko/mp_polarity_vocab.txt
--rw-r--r--   0        0        0    36419 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/data/lexicon/mpko/mp_polarity_wordset.txt
--rw-r--r--   0        0        0   281858 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/data/model/MPKC.nbc
--rw-r--r--   0        0        0    15644 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/data/tagset.py
--rw-r--r--   0        0        0       33 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/etag/__init__.py
--rw-r--r--   0        0        0     4210 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/etag/_template.py
--rwxr-xr-x   0        0        0       63 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/mecab/__init__.py
--rw-r--r--   0        0        0     5687 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/mecab/_mecab.py
--rw-r--r--   0        0        0     4529 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/mecab/_userdic.py
--rw-r--r--   0        0        0        0 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/py.typed
--rwxr-xr-x   0        0        0      236 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/sentiment/__init__.py
--rwxr-xr-x   0        0        0     4149 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/sentiment/base.py
--rwxr-xr-x   0        0        0     1741 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/sentiment/euko.py
--rwxr-xr-x   0        0        0     1010 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/sentiment/hiv4.py
--rw-r--r--   0        0        0     5936 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/sentiment/kosac.py
--rwxr-xr-x   0        0        0     1054 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/sentiment/lm.py
--rw-r--r--   0        0        0    16118 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/sentiment/mpck.py
--rwxr-xr-x   0        0        0     1840 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/sentiment/mpko.py
--rwxr-xr-x   0        0        0     9268 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/sentiment/utils.py
--rw-r--r--   0        0        0       66 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/tag/__init__.py
--rw-r--r--   0        0        0    10630 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/tag/_mecab.py
--rw-r--r--   0        0        0     2172 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/tag/_postprocess.py
--rwxr-xr-x   0        0        0        0 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/utils/__init__.py
--rw-r--r--   0        0        0     3520 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/utils/dictionary.py
--rw-r--r--   0        0        0     6668 2023-04-21 11:38:41.428575 ekonlpy-1.1.6/src/ekonlpy/utils/io.py
--rw-r--r--   0        0        0     9459 1970-01-01 00:00:00.000000 ekonlpy-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-26 19:28:57.344443 ekonlpy-1.1.7/LICENSE
+-rw-r--r--   0        0        0     8562 2023-04-26 19:28:57.348444 ekonlpy-1.1.7/README.md
+-rw-r--r--   0        0        0     3469 2023-04-26 19:29:37.960735 ekonlpy-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0      271 2023-04-26 19:28:57.444444 ekonlpy-1.1.7/src/ekonlpy/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-26 19:29:37.888735 ekonlpy-1.1.7/src/ekonlpy/_version.py
+-rw-r--r--   0        0        0       31 2023-04-26 19:28:57.444444 ekonlpy-1.1.7/src/ekonlpy/data/__init__.py
+-rw-r--r--   0        0        0      514 2023-04-26 19:28:57.444444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/ADJECTIVES.txt
+-rw-r--r--   0        0        0      108 2023-04-26 19:28:57.444444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/ADVERBS.txt
+-rw-r--r--   0        0        0     2583 2023-04-26 19:28:57.444444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/COUNTRY.txt
+-rw-r--r--   0        0        0       17 2023-04-26 19:28:57.444444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/CURRENCY.txt
+-rw-r--r--   0        0        0    47727 2023-04-26 19:28:57.444444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/ECON_PHRASES.txt
+-rw-r--r--   0        0        0   475773 2023-04-26 19:28:57.452444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/ECON_TERMS.txt
+-rwxr-xr-x   0        0        0    77542 2023-04-26 19:28:57.452444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/ENTITY.txt
+-rw-r--r--   0        0        0     9629 2023-04-26 19:28:57.452444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/FOREIGN_TERMS.txt
+-rw-r--r--   0        0        0     2077 2023-04-26 19:28:57.452444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/GENERIC.txt
+-rw-r--r--   0        0        0    35442 2023-04-26 19:28:57.452444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/INDUSTRY_TERMS.txt
+-rw-r--r--   0        0        0    69192 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/INSTITUTION.txt
+-rw-r--r--   0        0        0    20594 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/LEMMA.txt
+-rw-r--r--   0        0        0     2072 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/NAMES.txt
+-rw-r--r--   0        0        0      687 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/NOUNS.txt
+-rw-r--r--   0        0        0    10396 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/POLARITY_PHRASES.txt
+-rw-r--r--   0        0        0    12378 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/PROPER_NOUNS.txt
+-rw-r--r--   0        0        0    14928 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/SECTOR.txt
+-rw-r--r--   0        0        0     6456 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/STOPWORDS.txt
+-rwxr-xr-x   0        0        0      260 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/STOPWORDS_CUST.txt
+-rw-r--r--   0        0        0     5788 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/STOPWORDS_EN.txt
+-rwxr-xr-x   0        0        0      598 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/STOPWORDS_KOR.txt
+-rw-r--r--   0        0        0    33685 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/SYNONYM.txt
+-rw-r--r--   0        0        0      300 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/SYNONYM_MAG.txt
+-rw-r--r--   0        0        0     5329 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/SYNONYM_PHRASES.txt
+-rw-r--r--   0        0        0    27207 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/SYNONYM_TERMS.txt
+-rw-r--r--   0        0        0       87 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/SYNONYM_VA.txt
+-rw-r--r--   0        0        0       69 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/UNIT.txt
+-rw-r--r--   0        0        0       40 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/VERBS.txt
+-rwxr-xr-x   0        0        0     1677 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/Currencies.txt
+-rwxr-xr-x   0        0        0      724 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/DatesandNumbers.txt
+-rwxr-xr-x   0        0        0     1798 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/Generic.txt
+-rwxr-xr-x   0        0        0     1622 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/Geographic.txt
+-rwxr-xr-x   0        0        0  2903900 2023-04-26 19:28:57.468444 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/HIV-4.csv
+-rwxr-xr-x   0        0        0  8373373 2023-04-26 19:28:57.516445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/LM.csv
+-rwxr-xr-x   0        0        0    93474 2023-04-26 19:28:57.516445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/Names.txt
+-rw-r--r--   0        0        0  3047832 2023-04-26 19:28:57.532445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_lex.csv
+-rw-r--r--   0        0        0  2362210 2023-04-26 19:28:57.544445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_mkt.csv
+-rwxr-xr-x   0        0        0   778128 2023-04-26 19:28:57.548445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/kosac/expressive-type.csv
+-rwxr-xr-x   0        0        0   661841 2023-04-26 19:28:57.552445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/kosac/intensity.csv
+-rwxr-xr-x   0        0        0   659879 2023-04-26 19:28:57.556445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/kosac/polarity.csv
+-rw-r--r--   0        0        0  3226022 2023-04-26 19:28:57.572445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_lex.csv
+-rw-r--r--   0        0        0  3832440 2023-04-26 19:28:57.592445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt.csv
+-rw-r--r--   0        0        0  2735025 2023-04-26 19:28:57.608445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n3.csv
+-rw-r--r--   0        0        0  3749409 2023-04-26 19:28:57.628445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n7.csv
+-rw-r--r--   0        0        0  2835691 2023-04-26 19:28:57.640445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_vocab.txt
+-rw-r--r--   0        0        0    36419 2023-04-26 19:28:57.640445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_wordset.txt
+-rw-r--r--   0        0        0   281858 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/data/model/MPKC.nbc
+-rw-r--r--   0        0        0    15644 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/data/tagset.py
+-rw-r--r--   0        0        0       33 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/etag/__init__.py
+-rw-r--r--   0        0        0     4210 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/etag/_template.py
+-rwxr-xr-x   0        0        0       63 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/mecab/__init__.py
+-rw-r--r--   0        0        0     5687 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/mecab/_mecab.py
+-rw-r--r--   0        0        0     4529 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/mecab/_userdic.py
+-rw-r--r--   0        0        0        0 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/py.typed
+-rwxr-xr-x   0        0        0      236 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/sentiment/__init__.py
+-rwxr-xr-x   0        0        0     4149 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/sentiment/base.py
+-rwxr-xr-x   0        0        0     1741 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/sentiment/euko.py
+-rwxr-xr-x   0        0        0     1010 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/sentiment/hiv4.py
+-rw-r--r--   0        0        0     5936 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/sentiment/kosac.py
+-rwxr-xr-x   0        0        0     1054 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/sentiment/lm.py
+-rw-r--r--   0        0        0    16112 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/sentiment/mpck.py
+-rwxr-xr-x   0        0        0     1840 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/sentiment/mpko.py
+-rwxr-xr-x   0        0        0     9268 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/sentiment/utils.py
+-rw-r--r--   0        0        0       66 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/tag/__init__.py
+-rw-r--r--   0        0        0    10630 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/tag/_mecab.py
+-rw-r--r--   0        0        0     2172 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/tag/_postprocess.py
+-rwxr-xr-x   0        0        0        0 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/utils/__init__.py
+-rw-r--r--   0        0        0     3520 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/utils/dictionary.py
+-rw-r--r--   0        0        0     6668 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/utils/io.py
+-rw-r--r--   0        0        0     9459 1970-01-01 00:00:00.000000 ekonlpy-1.1.7/PKG-INFO
```

### Comparing `ekonlpy-1.1.6/LICENSE` & `ekonlpy-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/README.md` & `ekonlpy-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/pyproject.toml` & `ekonlpy-1.1.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eKoNLPy"
-version = "1.1.6"
+version = "1.1.7"
 description = "A Korean natural language processing toolkit for economic analysis"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "ekonlpy", from = "src" }]
 homepage = "https://ekonlpy.entelecheia.ai/"
 repository = "https://github.com/entelecheia/eKoNLPy"
@@ -19,19 +19,18 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 fugashi = "^1.2.1"
 mecab-ko-dic = "^1.0.0"
 nltk = "^3.8.1"
 scipy = "^1.10.1"
-pandas = "^2.0.0"
+pandas = "^1.5.3"
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
-setuptools-scm = "^7.1.0"
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.0"
 flake8-pyproject = "^1.2.2"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
@@ -134,17 +133,16 @@
 version_variable = "src/ekonlpy/_version.py:__version__"
 version_source = "tag"
 commit_version_number = true                                          # required for version_source = "tag"
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
-pre_commit_command = "make scm-version"
 changelog_file = "CHANGELOG.md"
 upload_to_repository = true
 upload_to_release = true
 build_command = "poetry build --no-cache"
 hvcs = "github"                                                       # hosting version control system, gitlab is also supported
 
 [build-system]
-requires = ["poetry-core>=1.0.0", "setuptools>=45", "setuptools_scm[toml]>=6.2"]
-build-backend = 'setuptools.build_meta'
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/dictionary/ADJECTIVES.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/ADJECTIVES.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/dictionary/COUNTRY.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/COUNTRY.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/dictionary/ECON_PHRASES.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/ECON_PHRASES.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/dictionary/ECON_TERMS.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/ECON_TERMS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/dictionary/ENTITY.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/ENTITY.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/dictionary/FOREIGN_TERMS.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/FOREIGN_TERMS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/dictionary/GENERIC.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/GENERIC.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/dictionary/INDUSTRY_TERMS.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/INDUSTRY_TERMS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/dictionary/INSTITUTION.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/INSTITUTION.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/dictionary/LEMMA.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/LEMMA.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/dictionary/NAMES.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/NAMES.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/dictionary/NOUNS.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/NOUNS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/dictionary/POLARITY_PHRASES.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/POLARITY_PHRASES.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/dictionary/PROPER_NOUNS.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/PROPER_NOUNS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/dictionary/SECTOR.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/SECTOR.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/dictionary/STOPWORDS.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/STOPWORDS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/dictionary/STOPWORDS_EN.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/STOPWORDS_EN.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/dictionary/STOPWORDS_KOR.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/STOPWORDS_KOR.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/dictionary/SYNONYM.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/SYNONYM.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/dictionary/SYNONYM_PHRASES.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/SYNONYM_PHRASES.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/dictionary/SYNONYM_TERMS.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/SYNONYM_TERMS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/lexicon/Currencies.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/Currencies.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/lexicon/DatesandNumbers.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/DatesandNumbers.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/lexicon/Generic.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/Generic.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/lexicon/Geographic.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/Geographic.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/lexicon/HIV-4.csv` & `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/HIV-4.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/lexicon/LM.csv` & `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/LM.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/lexicon/Names.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/Names.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_lex.csv` & `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_lex.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_mkt.csv` & `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_mkt.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/lexicon/kosac/expressive-type.csv` & `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/kosac/expressive-type.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/lexicon/kosac/intensity.csv` & `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/kosac/intensity.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/lexicon/kosac/polarity.csv` & `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/kosac/polarity.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_lex.csv` & `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_lex.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt.csv` & `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n3.csv` & `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n3.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n7.csv` & `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n7.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/lexicon/mpko/mp_polarity_vocab.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_vocab.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/lexicon/mpko/mp_polarity_wordset.txt` & `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_wordset.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/model/MPKC.nbc` & `ekonlpy-1.1.7/src/ekonlpy/data/model/MPKC.nbc`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/data/tagset.py` & `ekonlpy-1.1.7/src/ekonlpy/data/tagset.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/etag/_template.py` & `ekonlpy-1.1.7/src/ekonlpy/etag/_template.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/mecab/_mecab.py` & `ekonlpy-1.1.7/src/ekonlpy/mecab/_mecab.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/mecab/_userdic.py` & `ekonlpy-1.1.7/src/ekonlpy/mecab/_userdic.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/sentiment/base.py` & `ekonlpy-1.1.7/src/ekonlpy/sentiment/base.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/sentiment/euko.py` & `ekonlpy-1.1.7/src/ekonlpy/sentiment/euko.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/sentiment/hiv4.py` & `ekonlpy-1.1.7/src/ekonlpy/sentiment/hiv4.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/sentiment/kosac.py` & `ekonlpy-1.1.7/src/ekonlpy/sentiment/kosac.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/sentiment/lm.py` & `ekonlpy-1.1.7/src/ekonlpy/sentiment/lm.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/sentiment/mpck.py` & `ekonlpy-1.1.7/src/ekonlpy/sentiment/mpck.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import nltk
 import numpy as np
 from nltk.classify import NaiveBayesClassifier
 from nltk.collocations import BigramCollocationFinder, TrigramCollocationFinder
 from nltk.metrics import BigramAssocMeasures, TrigramAssocMeasures
 from nltk.metrics.scores import precision, recall
 from nltk.probability import ConditionalFreqDist, FreqDist
-from scipy.stats.stats import pearsonr, spearmanr
+from scipy.stats import pearsonr, spearmanr
 
 from ..data.tagset import aux_tags
 from ..tag import Mecab
 from ..utils.io import installpath
 from .base import LEXICON_PATH
 
 MODEL_PATH = "%s/data/model" % installpath
```

### Comparing `ekonlpy-1.1.6/src/ekonlpy/sentiment/mpko.py` & `ekonlpy-1.1.7/src/ekonlpy/sentiment/mpko.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/sentiment/utils.py` & `ekonlpy-1.1.7/src/ekonlpy/sentiment/utils.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/tag/_mecab.py` & `ekonlpy-1.1.7/src/ekonlpy/tag/_mecab.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/tag/_postprocess.py` & `ekonlpy-1.1.7/src/ekonlpy/tag/_postprocess.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/utils/dictionary.py` & `ekonlpy-1.1.7/src/ekonlpy/utils/dictionary.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/src/ekonlpy/utils/io.py` & `ekonlpy-1.1.7/src/ekonlpy/utils/io.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.6/PKG-INFO` & `ekonlpy-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ekonlpy
-Version: 1.1.6
+Version: 1.1.7
 Summary: A Korean natural language processing toolkit for economic analysis
 Home-page: https://ekonlpy.entelecheia.ai/
 License: MIT
 Keywords: KoNLPy,Tokenization,Sentiment analysis,Monetary policy
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fugashi (>=1.2.1,<2.0.0)
 Requires-Dist: mecab-ko-dic (>=1.0.0,<2.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
-Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Project-URL: Repository, https://github.com/entelecheia/eKoNLPy
 Description-Content-Type: text/markdown
 
 # eKoNLPy: Korean NLP Python Library for Economic Analysis
 
 [![pypi-image]][pypi-url]
```

