# Comparing `tmp/minimizers-0.1.1.tar.gz` & `tmp/minimizers-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/minimizers-0.1.1.tar", last modified: Tue Apr 25 15:25:45 2023, max compression
+gzip compressed data, was "dist/minimizers-0.1.2.tar", last modified: Wed Apr 26 03:48:57 2023, max compression
```

## Comparing `minimizers-0.1.1.tar` & `minimizers-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-04-25 15:25:45.000000 minimizers-0.1.1/
--rw-r--r--   0 fabio      (501) staff       (20)     1068 2023-04-21 17:31:15.000000 minimizers-0.1.1/LICENSE
--rw-r--r--   0 fabio      (501) staff       (20)     2848 2023-04-25 15:25:45.000000 minimizers-0.1.1/PKG-INFO
--rw-r--r--   0 fabio      (501) staff       (20)     1654 2023-04-21 23:00:33.000000 minimizers-0.1.1/README.md
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-04-25 15:25:45.000000 minimizers-0.1.1/minimizers/
--rw-r--r--   0 fabio      (501) staff       (20)        0 2023-04-21 17:32:54.000000 minimizers-0.1.1/minimizers/__init__.py
--rw-r--r--   0 fabio      (501) staff       (20)     7393 2023-04-25 15:23:57.000000 minimizers-0.1.1/minimizers/minimizers.py
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-04-25 15:25:45.000000 minimizers-0.1.1/minimizers.egg-info/
--rw-r--r--   0 fabio      (501) staff       (20)     2848 2023-04-25 15:25:44.000000 minimizers-0.1.1/minimizers.egg-info/PKG-INFO
--rw-r--r--   0 fabio      (501) staff       (20)      313 2023-04-25 15:25:44.000000 minimizers-0.1.1/minimizers.egg-info/SOURCES.txt
--rw-r--r--   0 fabio      (501) staff       (20)        1 2023-04-25 15:25:44.000000 minimizers-0.1.1/minimizers.egg-info/dependency_links.txt
--rw-r--r--   0 fabio      (501) staff       (20)       59 2023-04-25 15:25:44.000000 minimizers-0.1.1/minimizers.egg-info/entry_points.txt
--rw-r--r--   0 fabio      (501) staff       (20)        1 2023-04-25 15:25:44.000000 minimizers-0.1.1/minimizers.egg-info/not-zip-safe
--rw-r--r--   0 fabio      (501) staff       (20)       10 2023-04-25 15:25:44.000000 minimizers-0.1.1/minimizers.egg-info/requires.txt
--rw-r--r--   0 fabio      (501) staff       (20)       11 2023-04-25 15:25:44.000000 minimizers-0.1.1/minimizers.egg-info/top_level.txt
--rw-r--r--   0 fabio      (501) staff       (20)       38 2023-04-25 15:25:45.000000 minimizers-0.1.1/setup.cfg
--rw-r--r--   0 fabio      (501) staff       (20)     1602 2023-04-21 22:57:21.000000 minimizers-0.1.1/setup.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-04-26 03:48:57.000000 minimizers-0.1.2/
+-rw-r--r--   0 fabio      (501) staff       (20)     1068 2023-04-21 17:31:15.000000 minimizers-0.1.2/LICENSE
+-rw-r--r--   0 fabio      (501) staff       (20)     3797 2023-04-26 03:48:57.000000 minimizers-0.1.2/PKG-INFO
+-rw-r--r--   0 fabio      (501) staff       (20)     2475 2023-04-26 03:47:44.000000 minimizers-0.1.2/README.md
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-04-26 03:48:57.000000 minimizers-0.1.2/minimizers/
+-rw-r--r--   0 fabio      (501) staff       (20)        0 2023-04-21 17:32:54.000000 minimizers-0.1.2/minimizers/__init__.py
+-rw-r--r--   0 fabio      (501) staff       (20)    10882 2023-04-26 02:27:00.000000 minimizers-0.1.2/minimizers/minimizers.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-04-26 03:48:57.000000 minimizers-0.1.2/minimizers.egg-info/
+-rw-r--r--   0 fabio      (501) staff       (20)     3797 2023-04-26 03:48:56.000000 minimizers-0.1.2/minimizers.egg-info/PKG-INFO
+-rw-r--r--   0 fabio      (501) staff       (20)      313 2023-04-26 03:48:56.000000 minimizers-0.1.2/minimizers.egg-info/SOURCES.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        1 2023-04-26 03:48:56.000000 minimizers-0.1.2/minimizers.egg-info/dependency_links.txt
+-rw-r--r--   0 fabio      (501) staff       (20)       59 2023-04-26 03:48:56.000000 minimizers-0.1.2/minimizers.egg-info/entry_points.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        1 2023-04-26 03:48:56.000000 minimizers-0.1.2/minimizers.egg-info/not-zip-safe
+-rw-r--r--   0 fabio      (501) staff       (20)       10 2023-04-26 03:48:56.000000 minimizers-0.1.2/minimizers.egg-info/requires.txt
+-rw-r--r--   0 fabio      (501) staff       (20)       11 2023-04-26 03:48:56.000000 minimizers-0.1.2/minimizers.egg-info/top_level.txt
+-rw-r--r--   0 fabio      (501) staff       (20)       38 2023-04-26 03:48:57.000000 minimizers-0.1.2/setup.cfg
+-rw-r--r--   0 fabio      (501) staff       (20)     1602 2023-04-21 22:57:21.000000 minimizers-0.1.2/setup.py
```

### Comparing `minimizers-0.1.1/LICENSE` & `minimizers-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `minimizers-0.1.1/minimizers/minimizers.py` & `minimizers-0.1.2/minimizers/minimizers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 #!/usr/bin/env python3
 """
 Extract the set of minimizers from a sequence file
 """
 
 __author__ = "Fabio Cumbo (fabio.cumbo@gmail.com)"
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __date__ = "Apr 25, 2023"
 
 import argparse as ap
 import errno
 import gzip
 import multiprocessing as mp
 import os
 import time
+from collections import Counter
+from collections.abc import Callable
 from functools import partial
-from typing import Dict, Set
+from typing import Dict, Optional, Set, Union
 
 from Bio import SeqIO
 
 TOOL_ID = "minimizers"
 
 
 def read_params():
@@ -61,34 +63,56 @@
         dest="output_type",
         choices=["list", "fasta"],
         help="The output can be formatted as a list of kmers or as a fasta file"
     )
     p.add_argument(
         "-s",
         "--size",
-        type=int,
+        type=number(int, minv=4),
         required=True,
         dest="size",
         help="Length of the minimizers",
     )
     p.add_argument(
         "-w",
         "--window",
-        type=int,
+        type=number(int, minv=5),
         required=True,
         dest="window",
         help=(
             "Size of the sliding window. "
             "It must be greater than the minimizer size"
         ),
     )
     p.add_argument(
+        "--report-counts",
+        action="store_true",
+        default=False,
+        dest="report_counts",
+        help=(
+            "Report the frequencies of the minimizers. "
+            "This is compatible with \"--output-type list\" only"
+        )
+    )
+    p.add_argument(
+        "--top-perc",
+        type=number(float, minv=1.0, maxv=100.0),
+        dest="top_perc",
+        help="Report the top percentage of minimizers based on their frequency",
+    )
+    p.add_argument(
+        "--top-num",
+        type=number(int, minv=1),
+        dest="top_num",
+        help="Report the top number of minimizers based on their frequency",
+    )
+    p.add_argument(
         "-n",
         "--nproc",
-        type=int,
+        type=number(int, minv=1, maxv=os.cpu_count()),
         default=1,
         dest="nproc",
         help="Make it parallel",
     )
     p.add_argument(
         "--verbose",
         action="store_true",
@@ -101,14 +125,45 @@
         action="version",
         version='"{}" version {} ({})'.format(TOOL_ID, __version__, __date__),
         help='Print the "{}" version and exit'.format(TOOL_ID),
     )
     return p.parse_args()
 
 
+def number(
+    typev: type,
+    minv: Optional[Union[int, float]] = None,
+    maxv: Optional[Union[int, float]] = None,
+) -> Callable:
+    """
+    Take full control of input numeric types by defining custom intervals
+    """
+
+    def type_func(value: Union[int, float]) -> Union[int, float]:
+        """
+        Test data type and ranges on the input value
+        """
+
+        try:
+            value = typev(value)
+
+            if minv and value < minv:
+                raise ap.ArgumentTypeError("Minimum value is {}".format(minv))
+
+            if maxv and value > maxv:
+                raise ap.ArgumentTypeError("Maximum value is {}".format(maxv))
+
+            return value
+
+        except Exception as e:
+            raise ap.ArgumentTypeError("Input value must be {}".format(typev)).with_traceback(e.__traceback__)
+
+    return type_func
+
+
 def openrt(filepath: str, mode: str = "r"):
     """
     Wrapper around "open" and "gzip.open"
 
     :param filepath:    File path
     :param mode:        Read (r - default) or Write mode (w)
     :return:            A buffer
@@ -133,25 +188,25 @@
     """
     Get the set of minimizers for the input sequence
 
     :param sequence_id:         Input sequence ID
     :param sequence_content:    The actual sequence
     :param kmer_size:           Size of the minimizers
     :param window_size:         Size of the sliding window
-    :return:                    A dictionary with just the set of minimizers indexed by the sequence ID
+    :return:                    A dictionary with just the set of minimizers and their frequencies indexed by the sequence ID
     """
 
     # Extract kmers
     kmers = [sequence_content[i:i + kmer_size] for i in range(0, len(sequence_content) - kmer_size + 1, 1)]
 
     # Define windows
     windows = [kmers[i:i + window_size] for i in range(0, len(kmers) - window_size + 1, 1)]
 
-    # Get minimizers
-    minimizers = set([min(window) for window in windows])
+    # Get minimizers and their frequencies
+    minimizers = Counter([min(window) for window in windows])
 
     return {sequence_id: minimizers}
 
 
 def get_minimizers_parallel(
     sequences: Dict[str, str],
     kmer_size: int = 4,
@@ -161,15 +216,15 @@
     """
     Process the input sequences in parallel and retrieve their set of minimizers
 
     :param sequences:   A dictionary with the input sequences indexed by the sequence IDs
     :param kmer_size:   Size of the minimizers
     :param window_size: Size of the sliding window
     :param nproc:       Number of parallel processes
-    :return:            A dictionary with the set of minimizers indexed by the sequence IDs
+    :return:            A dictionary with the set of minimizers and their frequencies indexed by the sequence IDs
     """
 
     minimizers = dict()
 
     get_minimizers_partial = partial(
         get_minimizers,
         kmer_size=kmer_size,
@@ -184,15 +239,15 @@
                 callback=minimizers.update,
             )
             for sequence_id in sequences
         ]
 
         for job in jobs:
             job.wait()
-    
+
     return minimizers
 
 
 def main() -> None:
     args = read_params()
 
     if not os.path.isfile(args.input):
@@ -202,14 +257,17 @@
         raise Exception("The output file already exists!")
 
     outfolder = os.path.dirname(args.output)
 
     if not os.path.isdir(outfolder):
         raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), outfolder)
 
+    if args.output_type == "fasta" and args.report_counts:
+        raise ValueError("\"--report-counts\" is not compatible with \"--output-type fasta\"")
+
     t0 = time.time()
 
     if args.verbose:
         print("Loading input file: {}".format(args.input))
 
     sequences = load_input(args.input)
 
@@ -223,46 +281,92 @@
         sequences,
         kmer_size=args.size,
         window_size=args.window,
         nproc=args.nproc,
     )
 
     if args.aggregate:
-        minimizers = set().union(*minimizers.values())
+        merged = None
+        
+        for record in minimizers:
+            if not merged:
+                merged = minimizers[record]
+            
+            else:
+                merged.update(minimizers[record])
+
+        minimizers = merged
 
         if args.verbose:
             print("The input file contains {} minimizers".format(len(minimizers)))
 
     if args.verbose:
         print("Dumping results to {}".format(args.output))
-    
+
     with open(args.output, "w+") as output:
-        if isinstance(minimizers, set):
+        if isinstance(minimizers, Counter):
+            sorted_minimizers = minimizers.keys()
+
+            if args.top_num or args.top_perc:
+                sorted_minimizers = sorted(sorted_minimizers, key=lambda mini: minimizers[mini], reverse=True)
+
+            mini_counter = 0
+
             if args.output_type == "fasta":
                 output.write(">{}\n".format(os.path.basename(args.input)))
 
-            for mini in minimizers:
+            for mini in sorted_minimizers:
                 output.write(
-                    "{}{}\n".format(
+                    "{}{}{}\n".format(
                         "N" if args.output_type == "fasta" else "",
-                        mini
+                        mini,
+                        "\t{}".format(minimizers[mini]) if args.output_type == "list" and args.report_counts else ""
                     )
                 )
-        
+
+                mini_counter += 1
+
+                if args.top_num and mini_counter >= args.top_num:
+                    break
+
+                elif args.top_perc and (mini_counter / len(minimizers) * 100.0) >= args.top_perc:
+                    break
+
         else:
             for record in minimizers:
+                sorted_minimizers = minimizers[record].keys()
+
+                if args.top_num or args.top_perc:
+                    sorted_minimizers = sorted(sorted_minimizers, key=lambda mini: minimizers[record][mini], reverse=True)
+
+                mini_counter = 0
+
                 if args.output_type == "fasta":
                     output.write(">{}\n".format(record))
 
-                for mini in minimizers[record]:
+                for mini in sorted_minimizers:
                     if args.output_type == "fasta":
                         output.write("N{}\n".format(mini))
 
                     else:
-                        output.write("{}\t{}\n".format(record, mini))
+                        output.write(
+                            "{}\t{}{}\n".format(
+                                record,
+                                mini,
+                                "\t{}".format(minimizers[record][mini]) if args.report_counts else ""
+                            )
+                        )
+
+                    mini_counter += 1
+
+                    if args.top_num and mini_counter >= args.top_num:
+                        break
+
+                    elif args.top_perc and (mini_counter / len(minimizers) * 100.0) >= args.top_perc:
+                        break
 
     t1 = time.time()
 
     if args.verbose:
         print("Total elapsed time {}s".format(int(t1 - t0)))
```

### Comparing `minimizers-0.1.1/setup.py` & `minimizers-0.1.2/setup.py`

 * *Files identical despite different names*

