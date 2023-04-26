# Comparing `tmp/databento_dbn-0.4.3-cp39-none-win_amd64.whl.zip` & `tmp/databento_dbn-0.5.0-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 525806 bytes, number of entries: 7
--rw-r--r--  4.6 unx     2968 b- defN 23-Apr-07 04:22 databento_dbn-0.4.3.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Apr-07 04:22 databento_dbn-0.4.3.dist-info/WHEEL
--rw-r--r--  4.6 unx      135 b- defN 23-Apr-07 04:22 databento_dbn/__init__.py
--rw-r--r--  4.6 unx    34378 b- defN 23-Apr-07 04:22 databento_dbn/__init__.pyi
--rw-r--r--  4.6 unx        0 b- defN 23-Apr-07 04:22 databento_dbn/py.typed
--rwxr-xr-x  4.6 unx  1495040 b- defN 23-Apr-07 04:22 databento_dbn/databento_dbn.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      571 b- defN 23-Apr-07 04:22 databento_dbn-0.4.3.dist-info/RECORD
-7 files, 1533188 bytes uncompressed, 524796 bytes compressed:  65.8%
+Zip file size: 548221 bytes, number of entries: 8
+-rw-r--r--  4.6 unx     2966 b- defN 23-Apr-25 21:19 databento_dbn-0.5.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-Apr-25 21:19 databento_dbn-0.5.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     9868 b- defN 23-Apr-25 21:19 databento_dbn-0.5.0.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx      135 b- defN 23-Apr-25 21:19 databento_dbn/__init__.py
+-rw-r--r--  4.6 unx    34694 b- defN 23-Apr-25 21:19 databento_dbn/__init__.pyi
+-rw-r--r--  4.6 unx        0 b- defN 23-Apr-25 21:19 databento_dbn/py.typed
+-rwxr-xr-x  4.6 unx  1567232 b- defN 23-Apr-25 21:19 databento_dbn/databento_dbn.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      679 b- defN 23-Apr-25 21:19 databento_dbn-0.5.0.dist-info/RECORD
+8 files, 1615670 bytes uncompressed, 547033 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
-Filename: databento_dbn-0.4.3.dist-info/METADATA
+Filename: databento_dbn-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: databento_dbn-0.4.3.dist-info/WHEEL
+Filename: databento_dbn-0.5.0.dist-info/WHEEL
+Comment: 
+
+Filename: databento_dbn-0.5.0.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: databento_dbn/__init__.py
 Comment: 
 
 Filename: databento_dbn/__init__.pyi
 Comment: 
 
 Filename: databento_dbn/py.typed
 Comment: 
 
 Filename: databento_dbn/databento_dbn.cp39-win_amd64.pyd
 Comment: 
 
-Filename: databento_dbn-0.4.3.dist-info/RECORD
+Filename: databento_dbn-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## databento_dbn/__init__.pyi

```diff
@@ -1,26 +1,53 @@
-"""Type stubs for databento_dbn"""
-from typing import BinaryIO, Optional, Sequence, SupportsBytes
+"""Type stubs for databento_dbn."""
+from typing import (
+    Any,
+    BinaryIO,
+    Dict,
+    List,
+    Optional,
+    Sequence,
+    SupportsBytes,
+    Tuple,
+    Union,
+)
+
+_DBNRecord = Union[
+    Metadata,
+    MBOMsg,
+    MBP1Msg,
+    MBP10Msg,
+    OHLCVMsg,
+    TradeMsg,
+    InstrumentDefMsg,
+    ImbalanceMsg,
+    ErrorMsg,
+    SymbolMappingMsg,
+    SystemMsg,
+]
 
-class Metadata:
+class Metadata(SupportsBytes):
     """
-    Information about the data contained in a DBN file or stream. DBN requires the
-    Metadata to be included at the start of the encoded data.
+    Information about the data contained in a DBN file or stream. DBN requires
+    the Metadata to be included at the start of the encoded data.
 
     See Also
     ---------
     decode_metadata
     encode_metadata
 
     """
 
+    def __bytes__(self) -> bytes: ...
+    def __eq__(self, other) -> bool: ...
+    def __ne__(self, other) -> bool: ...
     @property
     def version(self) -> int:
         """
-        The DBN schema version number. Newly-encoded DBN files will use [`crate::DBN_VERSION`].
+        The DBN schema version number.
 
         Returns
         -------
         int
 
         """
     @property
@@ -30,37 +57,40 @@
 
         Returns
         -------
         str
 
         """
     @property
-    def schema(self) -> int:
+    def schema(self) -> Optional[str]:
         """
-        The data record schema. Specifies which record type is stored in the Zstd-compressed DBN file.
+        The data record schema. Specifies which record type is stored in the
+        Zstd-compressed DBN file.
 
         Returns
         -------
-        int
+        Optional[str]
 
         """
     @property
     def start(self) -> int:
         """
-        The UNIX nanosecond timestamp of the query start, or the first record if the file was split.
+        The UNIX nanosecond timestamp of the query start, or the first record
+        if the file was split.
 
         Returns
         -------
         int
 
         """
     @property
     def end(self) -> int:
         """
-        The UNIX nanosecond timestamp of the query end, or the last record if the file was split.
+        The UNIX nanosecond timestamp of the query end, or the last record if
+        the file was split.
 
         Returns
         -------
         int
 
         """
     @property
@@ -70,89 +100,123 @@
 
         Returns
         -------
         int
 
         """
     @property
-    def stype_in(self) -> int:
+    def stype_in(self) -> Optional[str]:
         """
         The input symbology type to map from.
 
         Returns
         -------
-        int
+        Optional[str]
 
         """
     @property
-    def stype_out(self) -> int:
+    def stype_out(self) -> str:
         """
         The output symbology type to map to.
 
         Returns
         -------
-        int
+        str
 
         """
     @property
     def ts_out(self) -> bool:
         """
-        `true` if this store contains live data with send timestamps appended to each
-        record.
+        `true` if this store contains live data with send timestamps appended
+        to each record.
 
         Returns
         -------
         bool
 
         """
     @property
-    def symbols(self) -> Sequence[str]:
+    def symbols(self) -> List[str]:
         """
         The original query input symbols from the request.
 
         Returns
         -------
-        Sequence[str]
+        List[str]
 
         """
     @property
-    def partial(self) -> Sequence[str]:
+    def partial(self) -> List[str]:
         """
-        Symbols that did not resolve for _at least one day_ in the query time range.
+        Symbols that did not resolve for at least one day in the query time
+        range.
 
         Returns
         -------
-        str
+        List[str]
 
         """
     @property
-    def not_found(self) -> Sequence[str]:
+    def not_found(self) -> List[str]:
         """
-        Symbols that did not resolve for _any_ day in the query time range.
+        Symbols that did not resolve for any day in the query time range.
 
         Returns
         -------
-        Sequence[str]
+        List[str]
 
         """
     @property
-    def mappings(self) -> Sequence[SymbolMapping]:
+    def mappings(self) -> Dict[str, List[Dict[str, Any]]]:
         """
         Symbol mappings containing a native symbol and its mapping intervals.
 
         Returns
         -------
-        Sequence[SymbolMapping]
+        Dict[str, List[Dict[str, Any]]]:
+
+        """
+    @classmethod
+    def decode(cls, data: bytes) -> "Metadata":
+        """
+        Decodes the given Python `bytes` to `Metadata`. Returns a `Metadata`
+        object with all the DBN metadata attributes.
+
+        Parameters
+        ----------
+        data : bytes
+            The bytes to decode from.
+
+        Returns
+        -------
+        Metadata
+
+        Raises
+        ------
+        ValueError
+            When a Metadata instance cannot be parsed from `data`.
+
+        """
+    def encode(self) -> bytes:
+        """
+        Encodes the Metadata to bytes.
+
+        Returns
+        -------
+        bytes
+
+        Raises
+        ------
+        ValueError
+            When the Metadata object cannot be encoded.
 
         """
 
 class RecordHeader:
-    """
-    DBN Record Header
-    """
+    """DBN Record Header."""
 
     @property
     def length(self) -> int:
         """
         The length of the record.
 
         Returns
@@ -177,40 +241,41 @@
 
         Returns
         -------
         int
 
         """
     @property
-    def product_id(self) -> int:
+    def instrument_id(self) -> int:
         """
-        The numeric product ID assigned to the instrument.
+        The numeric ID assigned to the instrument.
 
         Returns
         -------
         int
 
         """
     @property
     def ts_event(self) -> int:
         """
-        The matching-engine-received timestamp expressed as number of nanoseconds since the UNIX epoch.
+        The matching-engine-received timestamp expressed as number of
+        nanoseconds since the UNIX epoch.
 
         Returns
         -------
         int
 
         """
 
 class Record(SupportsBytes):
-    """
-    Base class for DBN records.
-    """
+    """Base class for DBN records."""
 
     def __bytes__(self) -> bytes: ...
+    def __eq__(self, other) -> bool: ...
+    def __ne__(self, other) -> bool: ...
     @property
     def hd(self) -> RecordHeader:
         """
         The common header.
 
         Returns
         -------
@@ -222,19 +287,58 @@
         Return the size of the record.
 
         Returns
         -------
         int
 
         """
+    @property
+    def rtype(self) -> int:
+        """
+        The record type.
+
+        Returns
+        -------
+        int
+
+        """
+    @property
+    def publisher_id(self) -> int:
+        """
+        The publisher ID assigned by Databento.
+
+        Returns
+        -------
+        int
+
+        """
+    @property
+    def instrument_id(self) -> int:
+        """
+        The numeric ID assigned to the instrument.
+
+        Returns
+        -------
+        int
+
+        """
+    @property
+    def ts_event(self) -> int:
+        """
+        The matching-engine-received timestamp expressed as number of
+        nanoseconds since the UNIX epoch.
+
+        Returns
+        -------
+        int
+
+        """
 
 class _MBOBase:
-    """
-    Base for market-by-order messages.
-    """
+    """Base for market-by-order messages."""
 
     @property
     def order_id(self) -> int:
         """
         The order ID assigned at the venue.
 
         Returns
@@ -282,39 +386,42 @@
         -------
         int
 
         """
     @property
     def action(self) -> str:
         """
-        The event action. Can be `A`dd, `C`ancel, `M`odify, clea`R`, or `T`rade.
+        The event action. Can be `A`dd, `C`ancel, `M`odify, clea`R`, or
+        `T`rade.
 
         Returns
         -------
         str
+
         """
     @property
     def side(self) -> str:
         """
         The order side. Can be `A`sk, `B`id or `N`one.
 
         Returns
         -------
         str
 
         """
     @property
     def ts_recv(self) -> int:
         """
-        The capture-server-received timestamp expressed as number of nanoseconds since
-        the UNIX epoch.
+        The capture-server-received timestamp expressed as number of
+        nanoseconds since the UNIX epoch.
 
         Returns
         -------
         int
+
         """
     @property
     def ts_in_delta(self) -> int:
         """
         The delta of `ts_recv - ts_exchange_send`, max 2 seconds.
 
         Returns
@@ -330,22 +437,18 @@
         Returns
         -------
         int
 
         """
 
 class MBOMsg(Record, _MBOBase):
-    """
-    A market-by-order (MBO) tick message.
-    """
+    """A market-by-order (MBO) tick message."""
 
 class BidAskPair:
-    """
-    A book level.
-    """
+    """A book level."""
 
     @property
     def bid_px(self) -> int:
         """
         The bid price.
 
         Returns
@@ -401,17 +504,15 @@
         Returns
         -------
         int
 
         """
 
 class _MBPBase:
-    """
-    Base for market-by-price messages.
-    """
+    """Base for market-by-price messages."""
 
     @property
     def price(self) -> int:
         """
         The order price expressed as a signed integer where every 1 unit
         corresponds to 1e-9, i.e. 1/1,000,000,000 or 0.000000001.
 
@@ -429,15 +530,16 @@
         -------
         int
 
         """
     @property
     def action(self) -> str:
         """
-        The event action. Can be `A`dd, `C`ancel, `M`odify, clea`R`, or `T`rade.
+        The event action. Can be `A`dd, `C`ancel, `M`odify, clea`R`, or
+        `T`rade.
 
         Returns
         -------
         str
 
         """
     @property
@@ -469,15 +571,16 @@
         -------
         int
 
         """
     @property
     def ts_recv(self) -> int:
         """
-        The capture-server-received timestamp expressed as number of nanoseconds since the UNIX epoch.
+        The capture-server-received timestamp expressed as number of
+        nanoseconds since the UNIX epoch.
 
         Returns
         -------
         int
 
         """
     @property
@@ -499,62 +602,58 @@
         -------
         int
 
         """
 
 class TradeMsg(Record, _MBPBase):
     """
-    Market by price implementation with a book depth of 0. Equivalent to
-    MBP-0. The record of the `Trades` schema.
+    Market by price implementation with a book depth of 0.
+
+    Equivalent to MBP-0. The record of the `Trades` schema.
+
     """
 
 class MBP1Msg(Record, _MBPBase):
-    """
-    Market by price implementation with a known book depth of 1.
-    """
+    """Market by price implementation with a known book depth of 1."""
 
     @property
-    def booklevel(self) -> Sequence[BidAskPair]:
+    def booklevel(self) -> List[BidAskPair]:
         """
         The top of the order book.
 
         Returns
         -------
-        Sequence[BidAskPair]
+        List[BidAskPair]
 
         Notes
         -----
         MBP1Msg contains 1 level of BidAskPair.
 
         """
 
 class MBP10Msg(Record, _MBPBase):
-    """
-    Market by price implementation with a known book depth of 10.
-    """
+    """Market by price implementation with a known book depth of 10."""
 
     @property
-    def booklevel(self) -> Sequence[BidAskPair]:
+    def booklevel(self) -> List[BidAskPair]:
         """
         The top of the order book.
 
         Returns
         -------
-        Sequence[BidAskPair]
+        List[BidAskPair]
 
         Notes
         -----
         MBP10Msg contains 10 levels of BidAskPairs.
 
         """
 
 class OHLCVMsg(Record):
-    """
-    Open, high, low, close, and volume message.
-    """
+    """Open, high, low, close, and volume message."""
 
     @property
     def open(self) -> int:
         """
         The open price for the bar.
 
         Returns
@@ -600,23 +699,21 @@
         Returns
         -------
         int
 
         """
 
 class InstrumentDefMsg(Record):
-    """
-    Definition of an instrument.
-    """
+    """Definition of an instrument."""
 
     @property
     def ts_recv(self) -> int:
         """
-        The capture-server-received timestamp expressed as number of nanoseconds since the
-        UNIX epoch.
+        The capture-server-received timestamp expressed as number of
+        nanoseconds since the UNIX epoch.
 
         Returns
         -------
         int
 
         """
     @property
@@ -629,70 +726,71 @@
         -------
         int
 
         """
     @property
     def display_factor(self) -> int:
         """
-        The multiplier to convert the venue’s display price to the conventional price.
+        The multiplier to convert the venue’s display price to the conventional
+        price.
 
         Returns
         -------
         int
 
         """
     @property
     def expiration(self) -> int:
         """
-        The last eligible trade time expressed as a number of nanoseconds since the
-        UNIX epoch.
+        The last eligible trade time expressed as a number of nanoseconds since
+        the UNIX epoch.
 
         Returns
         -------
         int
 
         """
     @property
     def activation(self) -> int:
         """
-        The time of instrument activation expressed as a number of nanoseconds since the
-        UNIX epoch.
+        The time of instrument activation expressed as a number of nanoseconds
+        since the UNIX epoch.
 
         Returns
         -------
         int
 
         """
     @property
     def high_limit_price(self) -> int:
         """
-        The allowable high limit price for the trading day in units of 1e-9, i.e.
-        1/1,000,000,000 or 0.000000001.
+        The allowable high limit price for the trading day in units of 1e-9,
+        i.e. 1/1,000,000,000 or 0.000000001.
 
         Returns
         -------
         int
 
         """
     @property
     def low_limit_price(self) -> int:
         """
-        The allowable low limit price for the trading day in units of 1e-9, i.e.
-        1/1,000,000,000 or 0.000000001.
+        The allowable low limit price for the trading day in units of 1e-9,
+        i.e. 1/1,000,000,000 or 0.000000001.
 
         Returns
         -------
         int
 
         """
     @property
     def max_price_variation(self) -> int:
         """
-        The differential value for price banding in units of 1e-9, i.e. 1/1,000,000,000
-        or 0.000000001.
+        The differential value for price banding in units of 1e-9, i.e.
+        1/1,000,000,000 or 0.000000001.
 
         Returns
         -------
         int
 
         """
     @property
@@ -704,37 +802,38 @@
         -------
         int
 
         """
     @property
     def unit_of_measure_qty(self) -> int:
         """
-        The contract size for each instrument, in combination with `unit_of_measure`.
+        The contract size for each instrument, in combination with
+        `unit_of_measure`.
 
         Returns
         -------
         int
 
         """
     @property
     def min_price_increment_amount(self) -> int:
         """
-        The value currently under development by the venue. Converted to units of 1e-9, i.e.
-        1/1,000,000,000 or 0.000000001.
+        The value currently under development by the venue. Converted to units
+        of 1e-9, i.e. 1/1,000,000,000 or 0.000000001.
 
         Returns
         -------
         int
 
         """
     @property
     def price_ratio(self) -> int:
         """
-        The value used for price calculation in spread and leg pricing in units of 1e-9,
-        i.e. 1/1,000,000,000 or 0.000000001.
+        The value used for price calculation in spread and leg pricing in units
+        of 1e-9, i.e. 1/1,000,000,000 or 0.000000001.
 
         Returns
         -------
         int
 
         """
     @property
@@ -746,25 +845,26 @@
         -------
         int
 
         """
     @property
     def underlying_id(self) -> int:
         """
-        The `product_id` of the first underlying instrument.
+        The `instrument_id` of the first underlying instrument.
 
         Returns
         -------
         int
 
         """
     @property
     def cleared_volume(self) -> int:
         """
-        The total cleared volume of the instrument traded during the prior trading session.
+        The total cleared volume of the instrument traded during the prior
+        trading session.
 
         Returns
         -------
         int
 
         """
     @property
@@ -826,16 +926,16 @@
         -------
         int
 
         """
     @property
     def min_lot_size_round_lot(self) -> int:
         """
-        The minimum quantity required for a round lot of the instrument. Multiples of
-        this quantity are also round lots.
+        The minimum quantity required for a round lot of the instrument.
+        Multiples of this quantity are also round lots.
 
         Returns
         -------
         int
 
         """
     @property
@@ -847,15 +947,16 @@
         -------
         int
 
         """
     @property
     def open_interest_qty(self) -> int:
         """
-        The total open interest for the market at the close of the prior trading session.
+        The total open interest for the market at the close of the prior
+        trading session.
 
         Returns
         -------
         int
 
         """
     @property
@@ -867,16 +968,16 @@
         -------
         int
 
         """
     @property
     def decay_quantity(self) -> int:
         """
-        The quantity that a contract will decay daily, after `decay_start_date` has
-        been reached.
+        The quantity that a contract will decay daily, after `decay_start_date`
+        has been reached.
 
         Retruns
         -------
         int
 
         """
     @property
@@ -929,15 +1030,16 @@
         -------
         int
 
         """
     @property
     def channel_id(self) -> int:
         """
-        The channel ID assigned by Databento as an incrementing integer starting at zero.
+        The channel ID assigned by Databento as an incrementing integer
+        starting at zero.
 
         Returns
         -------
         int
 
         """
     @property
@@ -967,15 +1069,15 @@
 
         Returns
         -------
         str
 
         """
     @property
-    def symbol(self) -> str:
+    def raw_symbol(self) -> str:
         """
         The instrument name (symbol).
 
         Returns
         -------
         str
 
@@ -1029,15 +1131,16 @@
         -------
         str
 
         """
     @property
     def unit_of_measure(self) -> str:
         """
-        The unit of measure for the instrument’s original contract size, e.g. USD or LBS.
+        The unit of measure for the instrument’s original contract size, e.g.
+        USD or LBS.
 
         Returns
         -------
         str
 
         """
     @property
@@ -1069,16 +1172,16 @@
         -------
         str
 
         """
     @property
     def strike_price(self) -> int:
         """
-        The strike price of the option. Converted to units of 1e-9, i.e. 1/1,000,000,000
-        or 0.000000001.
+        The strike price of the option. Converted to units of 1e-9, i.e.
+        1/1,000,000,000 or 0.000000001.
 
         Returns
         -------
         int
 
         """
     @property
@@ -1110,15 +1213,16 @@
         -------
         int
 
         """
     @property
     def price_display_format(self) -> int:
         """
-        The number of digits to the right of the tick mark, to display fractional prices.
+        The number of digits to the right of the tick mark, to display
+        fractional prices.
 
         Returns
         -------
         int
 
         """
     @property
@@ -1150,15 +1254,16 @@
         -------
         int
 
         """
     @property
     def security_update_action(self) -> str:
         """
-        Indicates if the instrument definition has been added, modified, or deleted.
+        Indicates if the instrument definition has been added, modified, or
+        deleted.
 
         Returns
         -------
         str
 
         """
     @property
@@ -1200,15 +1305,16 @@
         -------
         str
 
         """
     @property
     def contract_multiplier_unit(self) -> int:
         """
-        The type of `contract_multiplier`. Either `1` for hours, or `2` for days.
+        The type of `contract_multiplier`. Either `1` for hours, or `2` for
+        days.
 
         Returns
         -------
         int
 
         """
     @property
@@ -1229,34 +1335,32 @@
         Returns
         -------
         int
 
         """
 
 class ImbalanceMsg(Record):
-    """
-    An auction imbalance message.
-    """
+    """An auction imbalance message."""
 
     @property
     def ts_recv(self) -> int:
         """
-        The capture-server-received timestamp expressed as the number of nanoseconds
-        since the UNIX epoch.
+        The capture-server-received timestamp expressed as the number of
+        nanoseconds since the UNIX epoch.
 
         Returns
         -------
         int
 
         """
     @property
     def ref_price(self) -> int:
         """
-        The price at which the imbalance shares are calculated, where every 1 unit corresponds to
-        1e-9, i.e. 1/1,000,000,000 or 0.000000001.
+        The price at which the imbalance shares are calculated, where every 1
+        unit corresponds to 1e-9, i.e. 1/1,000,000,000 or 0.000000001.
 
         Returns
         -------
         int
 
         """
     @property
@@ -1268,15 +1372,16 @@
         -------
         int
 
         """
     @property
     def cont_book_clr_price(self) -> int:
         """
-        The hypothetical auction-clearing price for both cross and continuous orders.
+        The hypothetical auction-clearing price for both cross and continuous
+        orders.
 
         Returns
         -------
         int
 
         """
     @property
@@ -1378,15 +1483,16 @@
         -------
         str
 
         """
     @property
     def side(self) -> str:
         """
-        The market side of the `total_imbalance_qty`. Can be `A`sk, `B`id, or `N`one.
+        The market side of the `total_imbalance_qty`. Can be `A`sk, `B`id, or
+        `N`one.
 
         Returns
         -------
         str
 
         """
     @property
@@ -1428,42 +1534,40 @@
         -------
         str
 
         """
     @property
     def significant_imbalance(self) -> str:
         """
-        Venue-specific character code. For Nasdaq, contains the raw Price Variation Indicator.
+        Venue-specific character code. For Nasdaq, contains the raw Price
+        Variation Indicator.
 
         Returns
         -------
         str
 
         """
 
 class ErrorMsg(Record):
-    """
-    An error message from the Databento Live Subscription Gateway (LSG).
-    """
+    """An error message from the Databento Live Subscription Gateway (LSG)."""
 
     @property
     def err(self) -> str:
         """
         The error message.
 
         Returns
         -------
         str
 
         """
 
 class SymbolMappingMsg(Record):
-    """
-    A symbol mapping message which maps a symbol of one `SType` to another.
-    """
+    """A symbol mapping message which maps a symbol of one `SType` to
+    another."""
 
     @property
     def stype_in_symbol(self) -> str:
         """
         The input symbol.
 
         Returns
@@ -1480,75 +1584,85 @@
         -------
         str
 
         """
     @property
     def start_ts(self) -> int:
         """
-        The start of the mapping interval expressed as the number of nanoseconds since
-        the UNIX epoch.
+        The start of the mapping interval expressed as the number of
+        nanoseconds since the UNIX epoch.
 
         Returns
         -------
         int
 
         """
     @property
     def end_ts(self) -> int:
         """
-        The end of the mapping interval expressed as the number of nanoseconds since
-        the UNIX epoch.
+        The end of the mapping interval expressed as the number of nanoseconds
+        since the UNIX epoch.
 
         Returns
         -------
         int
 
         """
 
 class SystemMsg(Record):
     """
-    A non-error message from the Databento Live Subscription Gateway (LSG). Also used
-    for heartbeating.
+    A non-error message from the Databento Live Subscription Gateway (LSG).
+
+    Also used for heartbeating.
+
     """
 
     @property
     def msg(self) -> str:
         """
         The message from the Databento Live Subscription Gateway (LSG).
 
         Returns
         -------
         str
 
         """
+    @property
+    def is_heartbeat(self) -> bool:
+        """
+        `true` if this message is a heartbeat, used to indicate the connection with the gateway
+        is still open.
+
+        Returns
+        -------
+        bool
+
+        """
 
 class DbnDecoder:
-    """
-    A class for decoding DBN data to Python objects.
-    """
+    """A class for decoding DBN data to Python objects."""
 
-    @property
     def buffer(self) -> bytes:
         """
-        The internal buffer.
+        Return the internal buffer of the decoder.
 
         Returns
         -------
         bytes
 
         """
     def decode(
         self,
-    ) -> Sequence[Record]:
+    ) -> List[Tuple[_DBNRecord, Optional[int]]]:
         """
         Decode the buffered data into DBN records.
 
         Returns
         -------
-        Sequence[Record]
+        List[Tuple[DBNRecord, Optional[int]]]
 
         Raises
         ------
         ValueError
             When the decoding fails.
 
         See Also
@@ -1570,101 +1684,33 @@
 
         See Also
         --------
         decode
 
         """
 
-def decode_metadata(bytes: bytes) -> Metadata:
-    """
-    Decodes the given Python `bytes` to `Metadata`. Returns a `Metadata` object with
-    all the DBN metadata attributes.
-
-    Parameters
-    ----------
-    bytes
-
-    Raises
-    ------
-    ValueError
-        When the metadata cannot be parsed from `bytes`.
-
-    """
-
-def encode_metadata(
-    dataset: str,
-    schema: str,
-    start: int,
-    stype_in: str,
-    stype_out: str,
-    symbols: Sequence[str],
-    partial: Sequence[str],
-    not_found: Sequence[str],
-    mappings: Sequence[SymbolMapping],
-    end: Optional[int] = None,
-    limit: Optional[int] = None,
-) -> bytes:
-    """
-    Encodes the given metadata into the DBN metadata binary format.
-    Returns Python `bytes`.
-
-    Parameters
-    ----------
-    dataset : str
-       The dataset code.
-    schema : str
-        The data record schema.
-    start : int
-        The UNIX nanosecond timestamp of the query start, or the first record if the file was split.
-    stype_in : str
-        The input symbology type to map from.
-    stype_out: str
-        The output symbology type to map to.
-    symbols : Sequence[str]
-        The original query input symbols from the request.
-    partial : Sequence[str]
-        Symbols that did not resolve for _at least one day_ in the query time range.
-    not_found : Sequence[str]
-        Symbols that did not resolve for _any_ day in the query time range.
-    mappings : Sequence[SymbolMapping]
-        Symbol mappings containing a native symbol and its mapping intervals.
-    end : Optional[int]
-        The UNIX nanosecond timestamp of the query end, or the last record if the file was split.
-    limit : Optional[int]
-        The optional maximum number of records for the query.
-
-    Returns
-    -------
-    bytes
-
-    Raises
-    ------
-    ValueError
-        When any of the arguments cannot be converted to their Rust equivalents.
-        When there's an issue writing the encoded metadata to bytes.
-
-    """
-
 def update_encoded_metadata(
     file: BinaryIO,
     start: int,
     end: Optional[int] = None,
     limit: Optional[int] = None,
 ) -> None:
     """
     Updates existing fields that have already been written to the given file.
 
     Parameters
     ----------
     file : BinaryIO
         The file handle to update.
     start : int
-        The UNIX nanosecond timestamp of the query start, or the first record if the file was split.
+        The UNIX nanosecond timestamp of the query start, or the
+        first record if the file was split.
     end : Optional[int]
-        The UNIX nanosecond timestamp of the query end, or the last record if the file was split.
+        The UNIX nanosecond timestamp of the query end, or the
+        last record if the file was split.
     limit : Optional[int]
         The optional maximum number of records for the query.
 
     Raises
     ------
     ValueError
         When the file update fails.
@@ -1692,23 +1738,25 @@
     compression : str
         The DBN compression format.
     dataset : str
        The dataset code.
     schema : str
         The data record schema.
     start : int
-        The UNIX nanosecond timestamp of the query start, or the first record if the file was split.
+        The UNIX nanosecond timestamp of the query start, or the
+        first record if the file was split.
     stype_in : str
         The input symbology type to map from.
     stype_out : str
         The output symbology type to map to.
     records : Sequence[object]
         A sequence of DBN record objects.
     end : Optional[int]
-        The UNIX nanosecond timestamp of the query end, or the last record if the file was split.
+        The UNIX nanosecond timestamp of the query end, or the
+        last record if the file was split.
 
     Raises
     ------
     ValueError
         When any of the enum arguments cannot be converted to their Rust equivalents.
         When there's an issue writing the encoded to bytes.
         When an expected field is missing from one of the dicts.
```

## Comparing `databento_dbn-0.4.3.dist-info/METADATA` & `databento_dbn-0.5.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: databento-dbn
-Version: 0.4.3
+Version: 0.5.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Summary: Python library written in Rust for working with Databento Binary Encoding (DBN)
+License-File: LICENSE
+Summary: Native Databento bindings based on dbn Rust crate
 Author: Databento <support@databento.com>
 Author-email: Databento <support@databento.com>
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/databento/dbn
 
@@ -43,21 +44,21 @@
 ```
 
 You can write Zstd-compressed DBN files using `write_dbn_file`:
 ```python
 from databento_dbn import write_dbn_file
 
 records = [
-    {"rtype": 160, "publisher_id": 1, "product_id": 1, "ts_event": 647784973705, "order_id": 1,
+    {"rtype": 160, "publisher_id": 1, "instrument_id": 1, "ts_event": 647784973705, "order_id": 1,
      "price": 3723000000000, "size": 1, "flags": 128, "channel_id": 0, "action": ord('C'),
      "side": ord('A'), "ts_recv": 1609160400000704060, "ts_in_delta": 0, "sequence": 1170352}
 ]
 with open("my.dbn.zst", "wb") as out:
     write_dbn_file(file=out, compression="zstd", schema="mbo", dataset="custom",
-                   records=records, stype="product_id")
+                   records=records, stype="instrument_id")
 ```
 Note that the keys in the dictionaries in `records` must match the field names of the schema, or
 the function will raise a `KeyError`.
 
 ## Building
 
 `databento-dbn` is written in Rust, so you'll need to have [Rust installed](https://www.rust-lang.org/)
```

## Comparing `databento_dbn-0.4.3.dist-info/RECORD` & `databento_dbn-0.5.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
-databento_dbn-0.4.3.dist-info/METADATA,sha256=nVZ9HxlzlX5weQKLL93rT3a_VZxpXNiBw7d5k1qTDYc,2968
-databento_dbn-0.4.3.dist-info/WHEEL,sha256=HfbNN9yA0Gn_6VCTRBzbKHMHpOwMN7MCpAKvpT7Uqyk,96
+databento_dbn-0.5.0.dist-info/METADATA,sha256=jbAEx5iu3Gyovt-AXSRX5k4qaRL1RCF0yskhm_rJajs,2966
+databento_dbn-0.5.0.dist-info/WHEEL,sha256=HfbNN9yA0Gn_6VCTRBzbKHMHpOwMN7MCpAKvpT7Uqyk,96
+databento_dbn-0.5.0.dist-info/license_files/LICENSE,sha256=d69bve2VkRS216XupRiyvjZOBPT0qV-eh9mHDCdxPSQ,9868
 databento_dbn/__init__.py,sha256=TeY-_YtACSjQLT3FBRPqxJrcYFf8yu_11WeB5LcyEKo,135
-databento_dbn/__init__.pyi,sha256=ZtJVPy4cXuqDt8V9IIKJRlKji9WcCVT2ZLnVNgbuDFY,34378
+databento_dbn/__init__.pyi,sha256=zCosErocILH-muUw3lo_ITl2XzRPtTRHUPMprtrsqYk,34694
 databento_dbn/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-databento_dbn/databento_dbn.cp39-win_amd64.pyd,sha256=vJESnQosE9k2JD8rcYHojBfx5hY_zwLVFKVqTJIvznU,1495040
-databento_dbn-0.4.3.dist-info/RECORD,,
+databento_dbn/databento_dbn.cp39-win_amd64.pyd,sha256=pUujTUbzzU2pml0AHBTAFwF8VTxcZWN_VkdUXJa4kFc,1567232
+databento_dbn-0.5.0.dist-info/RECORD,,
```

