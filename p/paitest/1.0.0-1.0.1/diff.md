# Comparing `tmp/paitest-1.0.0-py3-none-any.whl.zip` & `tmp/paitest-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 24727 bytes, number of entries: 13
+Zip file size: 25031 bytes, number of entries: 13
 -rw-r--r--  2.0 unx       40 b- defN 80-Jan-01 00:00 paitest/__init__.py
--rw-r--r--  2.0 unx      267 b- defN 80-Jan-01 00:00 paitest/frames/__init__.py
+-rw-r--r--  2.0 unx      342 b- defN 80-Jan-01 00:00 paitest/frames/__init__.py
 -rw-r--r--  2.0 unx     2581 b- defN 80-Jan-01 00:00 paitest/frames/coord.py
--rw-r--r--  2.0 unx      805 b- defN 80-Jan-01 00:00 paitest/frames/coord.pyi
--rw-r--r--  2.0 unx    14188 b- defN 80-Jan-01 00:00 paitest/frames/frame.py
--rw-r--r--  2.0 unx     4706 b- defN 80-Jan-01 00:00 paitest/frames/frame_params.py
+-rw-r--r--  2.0 unx      823 b- defN 80-Jan-01 00:00 paitest/frames/coord.pyi
+-rw-r--r--  2.0 unx    14448 b- defN 80-Jan-01 00:00 paitest/frames/frame.py
+-rw-r--r--  2.0 unx     4707 b- defN 80-Jan-01 00:00 paitest/frames/frame_params.py
 -rw-r--r--  2.0 unx      230 b- defN 80-Jan-01 00:00 paitest/log.py
--rw-r--r--  2.0 unx    18540 b- defN 80-Jan-01 00:00 paitest/paitest.py
--rw-r--r--  2.0 unx     1692 b- defN 80-Jan-01 00:00 paitest/paitest.pyi
--rw-r--r--  2.0 unx    34523 b- defN 80-Jan-01 00:00 paitest-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3437 b- defN 80-Jan-01 00:00 paitest-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 paitest-1.0.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1001 b- defN 16-Jan-01 00:00 paitest-1.0.0.dist-info/RECORD
-13 files, 82098 bytes uncompressed, 23081 bytes compressed:  71.9%
+-rw-r--r--  2.0 unx    19934 b- defN 80-Jan-01 00:00 paitest/paitest.py
+-rw-r--r--  2.0 unx     1786 b- defN 80-Jan-01 00:00 paitest/paitest.pyi
+-rw-r--r--  2.0 unx    34523 b- defN 80-Jan-01 00:00 paitest-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3665 b- defN 80-Jan-01 00:00 paitest-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 paitest-1.0.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1001 b- defN 16-Jan-01 00:00 paitest-1.0.1.dist-info/RECORD
+13 files, 84168 bytes uncompressed, 23385 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: paitest/paitest.py
 Comment: 
 
 Filename: paitest/paitest.pyi
 Comment: 
 
-Filename: paitest-1.0.0.dist-info/LICENSE
+Filename: paitest-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: paitest-1.0.0.dist-info/METADATA
+Filename: paitest-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: paitest-1.0.0.dist-info/WHEEL
+Filename: paitest-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: paitest-1.0.0.dist-info/RECORD
+Filename: paitest-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## paitest/frames/__init__.py

```diff
@@ -1,10 +1,8 @@
-from .frame import (
-    Addr2Coord as Addr2Coord,
-    Coord2Addr as Coord2Addr,
-    FrameGen as FrameGen,
-    Direction as Direction,
-    FrameMask as FrameMask,
-    FrameSubType as FrameSubType,
-    FrameDecoder as FrameDecoder,
-)
 from .coord import Coord as Coord
+from .frame import Addr2Coord as Addr2Coord
+from .frame import Coord2Addr as Coord2Addr
+from .frame import Direction as Direction
+from .frame import FrameDecoder as FrameDecoder
+from .frame import FrameGen as FrameGen
+from .frame import FrameMask as FrameMask
+from .frame import FrameSubType as FrameSubType
```

## paitest/frames/coord.py

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple, Union, Optional
+from typing import Optional, Tuple, Union
 
 
 class Coord:
     """Coordinate class"""
 
     def __init__(
         self, _x: Union[Tuple[int, int], int], _y: Optional[int] = None
```

## paitest/frames/coord.pyi

```diff
@@ -1,8 +1,8 @@
-from typing import overload, Tuple
+from typing import Tuple, overload
 
 class Coord:
     x: int = ...
     y: int = ...
     @overload
     def __init__(self, _x: Tuple[int, int]) -> None: ...
     @overload
@@ -15,11 +15,15 @@
     def __gt__(self, other) -> bool: ...
     def __le__(self, other) -> bool: ...
     def __ge__(self, other) -> bool: ...
     def __str__(self) -> str: ...
 
     __repr__ = __str__
 
+    ...
+
 class CoordOffset(Coord):
     def __init__(self, _x: int, _y: int) -> None: ...
     def __add__(self, other) -> CoordOffset | Coord: ...
     def __sub__(self, other) -> CoordOffset: ...
+
+    ...
```

## paitest/frames/frame.py

```diff
@@ -1,17 +1,16 @@
-from .frame_params import (
-    FrameType as FT,
-    FrameSubType as FST,
-    FrameMask as FM,
-    ConfigFrameMask as CFM,
-)
-from .frame_params import *
-from .coord import Coord
-from typing import List, Tuple, Union, Dict, Optional, Any
 import random
+from typing import Any, Dict, List, Optional, Tuple, Union
+
+from .coord import Coord
+from .frame_params import ConfigFrameMask as CFM
+from .frame_params import FrameMask as FM
+from .frame_params import FrameSubType as FST
+from .frame_params import FrameType as FT
+from .frame_params import *
 
 
 def Addr2Coord(addr: int) -> Coord:
     return Coord(addr >> 5, addr & ((1 << 5) - 1))
 
 
 def Coord2Addr(coord: Coord) -> int:
@@ -113,17 +112,19 @@
 
         param_reg: List[int] = []
 
         if is_random:
             if not is_legal:
                 # Don't care 'tick_wait_start' split in #1 and #2
                 for _ in range(2):
-                    param_reg.append(random.randint(0, FM.GENERAL_PAYLOAD_MASK))
+                    param_reg.append(random.randint(
+                        0, FM.GENERAL_PAYLOAD_MASK))
 
-                param_reg[1] = (param_reg[1] & (~CFM.TEST_CHIP_ADDR_HIGH3_MASK)) | high3
+                param_reg[1] = (param_reg[1] & (
+                    ~CFM.TEST_CHIP_ADDR_HIGH3_MASK)) | high3
                 param_reg.append(low7 << CFM.TEST_CHIP_ADDR_LOW7_OFFSET)
             else:
                 # Do legal geenration
                 pass
         else:
             pass
 
@@ -342,42 +343,52 @@
 
     def _general_info(self) -> None:
         print("General info of frame: 0x%x" % self._frame)
         print("#1  Frame type:         %s" % self._get_subtype())
 
         chip_coord = self._get_chip_coord()
         print(
-            "#2  Chip coordinate:    [0x%02x | 0x%02x]" % (chip_coord.x, chip_coord.y)
+            "#2  Chip coordinate:    [0x%02x | 0x%02x]" % (
+                chip_coord.x, chip_coord.y)
         )
 
         core_coord = self._get_core_coord()
         print(
-            "#3  Core coordinate:    [0x%02x | 0x%02x]" % (core_coord.x, core_coord.y)
+            "#3  Core coordinate:    [0x%02x | 0x%02x]" % (
+                core_coord.x, core_coord.y)
         )
 
         core_star_coord = self._get_core_star_coord()
         print(
             "#4  Core* coordinate:   [0x%02x | 0x%02x]"
             % (core_star_coord.x, core_star_coord.y)
         )
 
     def _config2_info(self) -> None:
         print("Info of parameter registers")
-        print("#1  Weight width:       0x%x" % self._param_reg_dict["weight_width"])
+        print("#1  Weight width:       0x%x" %
+              self._param_reg_dict["weight_width"])
         print("#2  LCN:                0x%x" % self._param_reg_dict["LCN"])
-        print("#3  Input width:        0x%x" % self._param_reg_dict["input_width"])
-        print("#4  Spike width:        0x%x" % self._param_reg_dict["spike_width"])
-        print("#5  Neuron num:         %d" % self._param_reg_dict["neuron_num"])
+        print("#3  Input width:        0x%x" %
+              self._param_reg_dict["input_width"])
+        print("#4  Spike width:        0x%x" %
+              self._param_reg_dict["spike_width"])
+        print("#5  Neuron num:         %d" %
+              self._param_reg_dict["neuron_num"])
         print("#6  Pool max enable:    %d" % self._param_reg_dict["pool_max"])
-        print("#7  Tick wait start:    0x%x" % self._param_reg_dict["tick_wait_start"])
-        print("#8  Tick wait end:      0x%x" % self._param_reg_dict["tick_wait_end"])
+        print("#7  Tick wait start:    0x%x" %
+              self._param_reg_dict["tick_wait_start"])
+        print("#8  Tick wait end:      0x%x" %
+              self._param_reg_dict["tick_wait_end"])
         print("#9  SNN enable:         %d" % self._param_reg_dict["SNN_EN"])
-        print("#10 Target LCN:         0x%x" % self._param_reg_dict["target_LCN"])
+        print("#10 Target LCN:         0x%x" %
+              self._param_reg_dict["target_LCN"])
 
-        test_chip_coord: Coord = self._param_reg_dict["test_chip_coord"]  # type: ignore
+        # type: ignore
+        test_chip_coord: Coord = self._param_reg_dict["test_chip_coord"]
         print(
             "#11 Test chip coord:    [0x%02x | 0x%02x]"
             % (test_chip_coord.x, test_chip_coord.y)
         )
 
     def _test2_info(self) -> None:
         pass
@@ -420,18 +431,20 @@
         ) & CFM.SNN_EN_MASK
         self._param_reg_dict["target_LCN"] = (
             self._frames_group[1] >> CFM.TARGET_LCN_OFFSET
         ) & CFM.TARGET_LCN_MASK
 
         high3 = self._frames_group[1] >> CFM.TEST_CHIP_ADDR_HIGH3_OFFSET
         low7 = self._frames_group[2] >> CFM.TEST_CHIP_ADDR_LOW7_OFFSET
-        self._param_reg_dict["test_chip_coord"] = test_chip_addr_combine(high3, low7)
+        self._param_reg_dict["test_chip_coord"] = test_chip_addr_combine(
+            high3, low7)
 
     def _decode_direction(self) -> Direction:
-        test_chip_coord: Coord = self._param_reg_dict["test_chip_coord"]  # type: ignore
+        # type: ignore
+        test_chip_coord: Coord = self._param_reg_dict["test_chip_coord"]
         offset = test_chip_coord - self._get_chip_coord()
 
         try:
             direction = Direction(offset)
             return direction
         except:
             raise ValueError("Offset is invalid. Check the parameters.")
```

## paitest/frames/frame_params.py

```diff
@@ -1,8 +1,9 @@
-from enum import Flag, Enum, unique
+from enum import Enum, Flag, unique
+
 from .coord import CoordOffset
 
 
 @unique
 class CoreType(Enum):
     CORE_TYPE_OFFLINE = 1
     CORE_TYPE_ONLINE = 0
```

## paitest/paitest.py

```diff
@@ -1,20 +1,15 @@
-from .frames import (
-    Addr2Coord,
-    Coord2Addr,
-    Coord,
-    FrameGen,
-    Direction,
-    FrameMask as FM,
-    FrameSubType as FST,
-)
-from pathlib import Path
-from typing import List, Union, Tuple, Optional
 import random
 import sys
+from pathlib import Path
+from typing import List, Optional, Tuple, Union
+
+from .frames import Addr2Coord, Coord, Coord2Addr, Direction, FrameGen
+from .frames import FrameMask as FM
+from .frames import FrameSubType as FST
 from .log import logger
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 
 
 __all__ = ["paitest"]
@@ -32,33 +27,35 @@
         """
         self._verbose: bool = True
         self._fixed_chip_coord: Coord = Coord(fixed_chip_coord)
         self._masked_core_coord: Coord
         self._fixed_core_star_coord: Coord = Coord(0, 0)
         self._test_chip_coord: Coord
 
-        self._ensure_direction(direction)  # type: ignore
+        self._ensure_direction(direction)
 
     def Get1GroupForNCoresWithNParams(
         self,
         N: int,
         *,
         save_dir: Optional[Union[str, Path]] = None,
         masked_core_coord: Optional[Tuple[int, int]] = None,
+        gen_txt: bool = False,
         verbose: bool = False,
     ) -> Tuple[Tuple[int, ...], ...]:
         """
         Generate 1 group(case) for 'N' random cores coordinates with 'N' different parameters.
 
         - `N`: How many cores coordinates under test.
         - `save_dir`: Where to save the frames files.
         - `masked_core_coord`: to avoid generating the specific core coordinate.
-        - `verbose`: whether to display log.
+        - `gen_txt`: to save frames into text files instead of default binary files.
+        - `verbose`: whether to display the log.
 
-        :return: Three tuples including config, testin & testout tuples. 3*N frames in config & testout tuple and N frames in testin tuple.
+        :return: 3 tuples including config, testin & testout tuples. 3*N frames in config & testout tuple and N frames in testin tuple.
         """
         self._ensure_cores(N)
 
         if save_dir:
             work_dir = self._ensure_dir(save_dir)
         else:
             work_dir = None
@@ -119,37 +116,40 @@
             if verbose:
                 logger.info(
                     "Test in frame  #1/1:  0x%x in group #%d/%d"
                     % (testin_frame, i + 1, N)
                 )
 
         if isinstance(work_dir, Path):
-            self.SaveFrames(work_dir / "config.bin", cf_list, verbose)
-            self.SaveFrames(work_dir / "testin.bin", ti_list, verbose)
-            self.SaveFrames(work_dir / "testout.bin", to_list, verbose)
+            _suffix = ".txt" if gen_txt else ".bin"
+            self.SaveFrames(work_dir / ("config" + _suffix), cf_list, verbose)
+            self.SaveFrames(work_dir / ("testin" + _suffix), ti_list, verbose)
+            self.SaveFrames(work_dir / ("testout" + _suffix), to_list, verbose)
 
         return tuple(cf_list), tuple(ti_list), tuple(to_list)
 
     def Get1GroupForNCoresWith1Param(
         self,
         N: int,
         *,
         save_dir: Optional[Union[str, Path]] = None,
         masked_core_coord: Optional[Tuple[int, int]] = None,
+        gen_txt: bool = False,
         verbose: bool = False,
     ) -> Tuple[Tuple[int, ...], ...]:
         """
         Generate 1 group(case) for 'N' random cores coordinates with the same parameters.
 
         - `N`: How many cores coordinates under test.
         - `save_dir`: Where to save the frames files.
         - `masked_core_coord`: to avoid generating the specific core coordinate.
-        - `verbose`: whether to display log.
+        - `gen_txt`: to save frames into text files instead of default binary files.
+        - `verbose`: whether to display the log.
 
-        :return: Three tuples including config, testin & testout tuples. 3*N frames in config & testout tuple and N frames in testin tuple.
+        :return: 3 tuples including config, testin & testout tuples. 3*N frames in config & testout tuple and N frames in testin tuple.
         """
         self._ensure_cores(N)
 
         if save_dir:
             work_dir = self._ensure_dir(save_dir)
         else:
             work_dir = None
@@ -209,36 +209,40 @@
             if verbose:
                 logger.info(
                     "Test in frame  #1/1:  0x%x in group #%d/%d"
                     % (testin_frame, i + 1, N)
                 )
 
         if isinstance(work_dir, Path):
-            self.SaveFrames(work_dir / "config.bin", cf_list, verbose)
-            self.SaveFrames(work_dir / "testin.bin", ti_list, verbose)
-            self.SaveFrames(work_dir / "testout.bin", to_list, verbose)
+            _suffix = ".txt" if gen_txt else ".bin"
+            self.SaveFrames(work_dir / ("config" + _suffix), cf_list, verbose)
+            self.SaveFrames(work_dir / ("testin" + _suffix), ti_list, verbose)
+            self.SaveFrames(work_dir / ("testout" + _suffix), to_list, verbose)
 
         return tuple(cf_list), tuple(ti_list), tuple(to_list)
 
     def GetNGroupsFor1CoreWithNParams(
         self,
         N: int,
         *,
         save_dir: Optional[Union[str, Path]] = None,
         masked_core_coord: Optional[Tuple[int, int]] = None,
+        gen_txt: bool = False,
         verbose: bool = False,
     ) -> Tuple[Tuple[int, ...], ...]:
         """
         Generate 'N' groups(cases) for 1 random core coordinate with 'N' different parameters.
 
         - `N`: How many test groups(cases) of 1 core will be generated.
         - `save_dir`: Where to save the frames files.
         - `masked_core_coord`: to avoid generating the specific core coordinate.
+        - `gen_txt`: to save frames into text files instead of default binary files.
+        - `verbose`: whether to display the log.
 
-        :return: Three tuples including config, testin & testout tuples. 3*N frames in config & testout tuple and N frames in testin tuple.
+        :return: 3 tuples including config, testin & testout tuples. 3*N frames in config & testout tuple and N frames in testin tuple.
         """
         self._ensure_cores(N)
 
         if save_dir:
             work_dir = self._ensure_dir(save_dir)
         else:
             work_dir = None
@@ -298,17 +302,18 @@
             if verbose:
                 logger.info(
                     "Test in frame  #1/1:  0x%x in group #%d/%d"
                     % (testin_frame, i + 1, N)
                 )
 
         if isinstance(work_dir, Path):
-            self.SaveFrames(work_dir / "config.bin", cf_list, verbose)
-            self.SaveFrames(work_dir / "testin.bin", ti_list, verbose)
-            self.SaveFrames(work_dir / "testout.bin", to_list, verbose)
+            _suffix = ".txt" if gen_txt else ".bin"
+            self.SaveFrames(work_dir / ("config" + _suffix), cf_list, verbose)
+            self.SaveFrames(work_dir / ("testin" + _suffix), ti_list, verbose)
+            self.SaveFrames(work_dir / ("testout" + _suffix), to_list, verbose)
 
         return tuple(cf_list), tuple(ti_list), tuple(to_list)
 
     def ReplaceCoreCoord(
         self,
         frames: Union[int, List[int], Tuple[int, ...]],
         new_core_coord: Optional[Union[Tuple[int, int], Coord]] = None,
@@ -346,30 +351,51 @@
 
     @staticmethod
     def SaveFrames(
         save_path: Union[str, Path],
         frames: Union[int, List[int], Tuple[int, ...]],
         verbose: bool = False,
     ) -> None:
-        """Write frames into specific binary file. Must be '.bin' suffix."""
+        """
+        Write frames into specific binary file. Files with '.bin' suffix is recommended
+
+        Support .txt files as well.
+
+        - gen_txt: Wether to generate txt files.
+        """
 
         _path = Path(save_path)
+        _suffix: str = _path.suffix
 
-        if not _path.suffix == ".bin":
-            raise ValueError(f"Only support .bin file: {_path}")
+        if _suffix != ".bin" and _suffix != ".txt":
+            raise NotImplementedError(
+                f"File with suffix {_suffix} is not supported!")
+
+        if _suffix == ".bin":
+            with open(_path, "wb") as f:
+                if isinstance(frames, int):
+                    f.write(frames.to_bytes(8, "big"))
+                else:
+                    for frame in frames:
+                        f.write(frame.to_bytes(8, "big"))
 
-        with open(_path, "wb") as f:
-            if isinstance(frames, int):
-                f.write(frames.to_bytes(8, "big"))
-            else:
-                for frame in frames:
-                    f.write(frame.to_bytes(8, "big"))
+        else:
+            with open(_path, "w") as f:  # Open with "w"
+                if isinstance(frames, int):
+                    _str64 = bin(frames).split("0b")[1]
+                    _str64 = _str64.zfill(64)
+                    f.write(_str64 + "\n")
+                else:
+                    for frame in frames:
+                        _str64 = bin(frame).split("0b")[1]
+                        _str64 = _str64.zfill(64)
+                        f.write(_str64 + "\n")
 
-            if verbose:
-                logger.info(f"Saved frame(s) into {_path} OK")
+        if verbose:
+            logger.info(f"Saved frame(s) into {_path} OK")
 
     def _Get1CoreCoord(self, masked_coord: Optional[Coord] = None) -> Coord:
         """
         Generate a random core coordinate. Indicate the masked one to avoid generating the same one
         """
         return self._GetNCoresCoord(N=1, masked_coord=masked_coord)[0]
 
@@ -473,21 +499,23 @@
         mask = FM.GENERAL_MASK & (
             ~(FM.GENERAL_CORE_ADDR_MASK << FM.GENERAL_CORE_ADDR_OFFSET)
         )
 
         new_core_addr = Coord2Addr(new_core_coord)
 
         for i, frame in enumerate(frames):
-            frames[i] = (frame & mask) | (new_core_addr << FM.GENERAL_CORE_ADDR_OFFSET)
+            frames[i] = (frame & mask) | (
+                new_core_addr << FM.GENERAL_CORE_ADDR_OFFSET)
 
         return tuple(frames)
 
     def _ReplaceHeader(self, frame: int, header: FST) -> int:
         """Replace the header of a frame with the new one."""
-        mask = FM.GENERAL_MASK & (~(FM.GENERAL_HEADER_MASK << FM.GENERAL_HEADER_OFFSET))
+        mask = FM.GENERAL_MASK & (
+            ~(FM.GENERAL_HEADER_MASK << FM.GENERAL_HEADER_OFFSET))
 
         return (frame & mask) | (header.value << FM.GENERAL_HEADER_OFFSET)
 
     def _ensure_dir(self, user_dir: Union[str, Path]) -> Path:
         _user_dir: Path = Path(user_dir)
 
         if not _user_dir.exists():
@@ -516,10 +544,11 @@
             try:
                 self._direction = Direction[direction.upper()]
             except KeyError:
                 raise KeyError(f"{direction} is an illegal direction!")
 
     def _ensure_coord(self, coord: Coord) -> None:
         if coord >= Coord(0b11100, 0b11100):
-            raise ValueError("Address coordinate must: 0 <= x < 28 or 0 <= y < 28")
+            raise ValueError(
+                "Address coordinate must: 0 <= x < 28 or 0 <= y < 28")
 
         self._masked_core_coord = coord
```

## paitest/paitest.pyi

```diff
@@ -1,12 +1,13 @@
-from typing import Tuple, List, Optional, Union
 import sys
+from typing import List, Optional, Tuple, Union
 
 if sys.version_info >= (3, 8):
     from typing import Literal
+
 from pathlib import Path
 
 class paitest:
     if sys.version_info >= (3, 8):
         def __init__(
             self,
             direction: Literal["EAST", "SOUTH", "WEST", "NORTH"] = "EAST",
@@ -21,30 +22,33 @@
 
     def Get1GroupForNCoresWithNParams(
         self,
         N: int,
         *,
         save_dir: Optional[Union[str, Path]] = None,
         masked_core_coord: Optional[Tuple[int, int]] = None,
+        gen_txt: bool = False,
         verbose: bool = False
     ) -> Tuple[Tuple[int, ...], ...]: ...
     def Get1GroupForNCoresWith1Param(
         self,
         N: int,
         *,
         save_dir: Optional[Union[str, Path]] = None,
         masked_core_coord: Optional[Tuple[int, int]] = None,
+        gen_txt: bool = False,
         verbose: bool = False
     ) -> Tuple[Tuple[int, ...], ...]: ...
     def GetNGroupsFor1CoreWithNParams(
         self,
         N: int,
         *,
         save_dir: Optional[Union[str, Path]] = None,
         masked_core_coord: Optional[Tuple[int, int]] = None,
+        gen_txt: bool = False,
         verbose: bool = False
     ) -> Tuple[Tuple[int, ...], ...]: ...
     def ReplaceCoreCoord(
         self,
         frames: Union[int, List[int], Tuple[int, ...]],
         new_core_coord: Tuple[int, int],
     ) -> int: ...
```

## Comparing `paitest-1.0.0.dist-info/LICENSE` & `paitest-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `paitest-1.0.0.dist-info/METADATA` & `paitest-1.0.1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paitest
-Version: 1.0.0
+Version: 1.0.1
 Summary: Test module for PAICORE 2.0
 Home-page: https://github.com/PAICookers/PAITest
 License: AGPL v3.0
 Keywords: PAICookers,PAITest,PAICORE
 Author: KafCoppelia
 Author-email: k740677208@gmail.com
 Requires-Python: >=3.6,<4.0
@@ -24,15 +24,17 @@
 
 # PAITest
 
 </div>
 
 ## 📦 版本
 
-[v1.0.0](https://github.com/PAICookers/PAITest/releases/tag/v1.0.0)
+[v1.0.1](https://github.com/PAICookers/PAITest/releases/tag/v1.0.1)
+
+✨支持 `.txt` 格式输出
 
 ## 🛠️ 使用生成
 
 配置帧及对应测试输入帧，以实现硬件通路的简单测试，后续将芯片实际测试输出帧与预期结果进行对比即可。
 
 ⚠️ 由于配置帧/测试帧I型需要配合串口配置使用，因此目前仅采用**配置/测试帧II型**方案，且 `CHIP_ADDR` 与 `CORE*_ADDR` 均固定为 `(0, 0)`。
 
@@ -40,54 +42,63 @@
 
    ```python
    from paitest import paitest
 
    # Define the direction of test chip
    PAITestManager = paitest("EAST")
    ```
-2. `Get1GroupForNCoresWithNParams`，产生一组针对 `N` 个核的配置-测试帧，每个核配置不同参数。可以指定单个需要**屏蔽**的核坐标。`verbose=True` 以开启日志显示，默认关闭。
+
+2. `Get1GroupForNCoresWithNParams`，产生一组针对 `N` 个核的配置-测试帧，每个核配置**不同参数**。可以指定单个需要**屏蔽**的核坐标
 
    ```python
    groups = 10             # Generate 10 groups
    save_to_dir="./test"    # Save frames into ./test directory
 
    # Generate configuration frames, testin & testout frames
-   cf, ti, to = PAITestManager.Get1GroupForNCoresWithNParams(groups, save_dir=save_to_dir)
+   cf, ti, to = PAITestManager.Get1GroupForNCoresWithNParams(groups, save_dir=save_to_dir, verbose=True)
 
    # Mask a cord coordinate so that avoid generating the same coordinate.
-   # And enable verbose logging
-   cf, ti, to = PAITestManager.Get1GroupForNCoresWithNParams(groups, 
-       save_dir=save_to_dir, masked_core_coord=(12, 16), verbose=True)
+   cf, ti, to = PAITestManager.Get1GroupForNCoresWithNParams(groups,
+       save_dir=save_to_dir, masked_core_coord=(12, 16), gen_txt=True)
    ```
-3. `Get1GroupForNCoresWith1Param`，产生1组针对 `N` 个核的配置-测试帧，每个核配置相同参数。可以指定单个需要**屏蔽**的核坐标
+
+   ⚠️ 指定 `verbose=True` 以开启日志显示，默认关闭；指定 `gen_txt=True` 以保存至 `.txt`，默认保存至 `.bin`。
+
+3. `Get1GroupForNCoresWith1Param`，产生1组针对 `N` 个核的配置-测试帧，每个核配置**相同参数**。可以指定单个需要**屏蔽**的核坐标
 
    ```python
    # Same as Get1GroupForNCoresWithNParams
    cf, ti, to = PAITestManager.Get1GroupForNCoresWith1Param(10, save_dir="./test")
    ```
-4. `GetNGroupsFor1CoreWithNParams`，产生 `N` 组针对1个核的配置-测试帧，每个核配置不同参数。可以指定单个需要**屏蔽**的核坐标
+
+4. `GetNGroupsFor1CoreWithNParams`，产生 `N` 组针对1个核的配置-测试帧，每个核配置**不同参数**。可以指定单个需要**屏蔽**的核坐标
 
    ```python
    # Same as Get1GroupForNCoresWithNParams
    cf, ti, to = PAITestManager.GetNGroupsFor1CoreWithNParams(1, save_dir="./test")
    ```
-5. `ReplaceCoreCoord`，替换单个或**一组**帧中的 `CORE_ADDR` 为指定坐标。
+
+5. `ReplaceCoreCoord`，替换**单个**或**一组**帧中的 `CORE_ADDR` 为指定坐标
 
    ```python
    # Replaced core coordinate with (9, 9)
    replaced = PAITestManager.ReplaceCoreCoord(original_frames, (9, 9))
    ```
 
    ⚠️ 一组指一组完整的配置帧，包含3帧。对于测试输入帧，即为单帧。
-6. `SaveFrames`，保存帧数据至 `.bin` 文件
+
+6. `SaveFrames`，默认保存帧数据至指定文件，支持 `.bin` 或 `.txt` 格式
 
    ```python
-   # Save into ./test/config.bin
+   # Save into binary files
    PAITestManager.SaveFrames("./test/config.bin", replaced)
+
+   # Or text files
+   PAITestManager.SaveFrames("./test/config.txt", replaced)
    ```
 
 ## 🗓️ TODO
 
-- [X] 上板验证
+- [x] 上板验证
 - [ ] 参数检验
 - [ ] 配置/测试帧III/IV型
```

