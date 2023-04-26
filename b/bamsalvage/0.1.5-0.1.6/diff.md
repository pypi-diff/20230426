# Comparing `tmp/bamsalvage-0.1.5.tar.gz` & `tmp/bamsalvage-0.1.6.tar.gz`

## Comparing `bamsalvage-0.1.5.tar` & `bamsalvage-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bamsalvage-0.1.5/requirements.txt
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 bamsalvage-0.1.5/setup.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bamsalvage-0.1.5/src/bamsalvage/__init__.py
--rwxr-xr-x   0        0        0    24842 2020-02-02 00:00:00.000000 bamsalvage-0.1.5/src/bamsalvage/_bamsalvage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bamsalvage-0.1.5/tests/test_bamsalvage.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 bamsalvage-0.1.5/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bamsalvage-0.1.5/LICENSE
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 bamsalvage-0.1.5/README.md
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 bamsalvage-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 bamsalvage-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0  1943761 2020-02-02 00:00:00.000000 bamsalvage-0.1.6/log.2.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bamsalvage-0.1.6/requirements.txt
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 bamsalvage-0.1.6/setup.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bamsalvage-0.1.6/src/bamsalvage/__init__.py
+-rwxr-xr-x   0        0        0    25964 2020-02-02 00:00:00.000000 bamsalvage-0.1.6/src/bamsalvage/_bamsalvage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bamsalvage-0.1.6/tests/test_bamsalvage.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 bamsalvage-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bamsalvage-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 bamsalvage-0.1.6/README.md
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 bamsalvage-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 bamsalvage-0.1.6/PKG-INFO
```

### Comparing `bamsalvage-0.1.5/setup.py` & `bamsalvage-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `bamsalvage-0.1.5/src/bamsalvage/_bamsalvage.py` & `bamsalvage-0.1.6/src/bamsalvage/_bamsalvage.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import argparse, struct
 import mgzip
 import zlib, logging, json
 import numba
 import numpy as np
 
 def version():
-    return "0.1.5"
+    import bamsalvage
+    return bamsalvage.__version__
 
 # Error handling
 class BAMException(Exception):
     """Exception for BAM decoding
     """
     NO_BAM_FILE = 0
     BLOCK_CORRUPTED = 1
@@ -18,20 +19,22 @@
     INCORRECT_MAGIC_NUMBER = 3
     INCORRECT_GZIP_MAGIC_NUMBER = 4
     BUFFER_TERMINATED = 5
     INCONSISTENT_CHECKSUM = 6
     INCONSISTENT_BLOCK_SIZE = 7
     DECOMPRESSION_FAILURE = 8
     OUT_OF_RANGE_VARIABLES = 9
+    NEGATIVE_DATA_SIZE = 10
     __KIND = ['This is not BAM file', 
               'Block was corrupted', 'Expected buffer size overflow',
               'Incorrect magic number', 'Incorrect GZIP magic number', 
               'Reached the end of file', 'Inconsistent CRC32 checksum',
               'Decompressed buffer size was inconsisted with expected',
-              "Failed to decompress", 'Variables are out of range']
+              "Failed to decompress", 'Variables are out of range',
+              'Negative data size was given']
     def __init__(self, kind:int, message:str=''):
         super(BAMException, self).__init__(message)
         if kind < 0 or kind > len(BAMException.__KIND):
             kind = -1
         self.__kind = kind
     def __str__(self):
         return '{} {}'.format(super().__str__(), BAMException.resolve_error_code(self.__kind))
@@ -62,15 +65,15 @@
         if j + 1 >= l_seq: break
         text[j+1] = bases[b & 15]
         j += 2
 @numba.njit(cache=True)
 def convert_bytes_to_qual(buffer:bytes, start:int, l_seq:int, text:bytearray):
     """Convert byte array into QUAL sequence"""
     for i in range(l_seq):
-        text[i] = min(33 + buffer[start+i], 127)
+        text[i] = min(33 + buffer[start+i], 126)
 
 @numba.njit(cache=True)
 def scan_block_header(buffer:bytes, start:numba.int64)->numba.int64:
     """Scan magic number and signature bytes int data block"""
     # le_I = np.uint32
     # le_i = np.int32
     for i in range(start, len(buffer)-36):
@@ -124,24 +127,23 @@
      CRC32 u32
      ISIZE u32
 
     BBBB I BBH BBH H/BII
 
     Args:
         handler (_io.TextIOWrapper): File handler
-        logger : logging.StreamHandler
+        strict : Check block size and CRC32
 
     Raises:
         BamException: BAM processing error
     Returns:
         _type_: _description_
     """
-    # logger = kwargs.get('logger', None)
-    # read first 18bytes
     current_pos = handler.tell()
+    strict_mode = kwargs.get('strict', False)
     buf = handler.read(18)
     while buf[0] != 31 or buf[1] != 139 or buf[2] != 8 or buf[3] != 4 or buf[12] != 66 or buf[13] != 67:
         offset = False
         for i in range(1, 18):
             if buf[i] == 31:
                 offset = True
                 buf = buf[i:] + handler.read(i)
@@ -156,70 +158,78 @@
     block_size = gzheader[11]
     if xlen >= 6 and block_size > xlen + 19:
         _skip_bytes = xlen - 6
         handler.read(_skip_bytes)
     if len(buf) < xlen:
         raise BAMException(BAMException.BUFFER_TERMINATED, 'cannot load gzipped block AT {} '.format(current_pos))
     compressed_data_size = block_size - xlen - 19
-    return decompress_and_validate(handler, compressed_data_size)
+    return decompress_and_validate(handler, compressed_data_size, strict_mode)
 
     
 def read_next_block(handler, **kwargs):
     """Read BGZF block, block corruption is not assumed.
 
     Args:
         handler (_io.TextIOWrapper): File handler
+        strict (bool) : Check block size and CRC32
 
     Raises:
         BamException: BAM processing error
     Returns:
         _type_: _description_
     """
     # GZIP header, ID1=31, ID2=139
+    strict_mode = kwargs.get('strict', False)
     buf = handler.read(2)
     if len(buf) < 2:
         raise BAMException(BAMException.BUFFER_TERMINATED, 'cannot scan header anymore')
     gzheader = struct.unpack('BB', buf)
     if gzheader[0] != 31 or gzheader[1] != 139:
         raise BAMException(BAMException.INCORRECT_MAGIC_NUMBER)
     buf = handler.read(10)
     values = struct.unpack('<BBIBBH', buf)
     xlen = values[-1]
     buf = handler.read(xlen)
     si1, si2, slen, bsize = struct.unpack('<BBHH', buf[0:6])
     if si1 != 66 or si2 != 67:
         raise BAMException(BAMException.INCORRECT_GZIP_MAGIC_NUMBER, 'SI1={}, SI2={} is different from 66 and 67'.format(si1, si2))
-    return decompress_and_validate(handler, bsize - xlen - 19)
+    return decompress_and_validate(handler, bsize - xlen - 19, strict_mode)
 
-def decompress_and_validate(handler, compressed_data_size):
+def decompress_and_validate(handler, compressed_data_size, strict_mode=False):
     """Read data block and validate BGZF block. Common routine among read_next_block and scan_next_block functions.
 
     Args:
         handler (stream): Stream handler
-        compressed_data_size (_type_): _description_
+        compressed_data_size (int64): Data size
+        strict : Check block size and CRC32
 
     Raises:
         BAMException: Corrupted block detected
 
     Returns:
         byte array : data block
     """
+    if compressed_data_size < 0:
+        raise BAMException(BAMException.NEGATIVE_DATA_SIZE, ' AT {} '.format(handler.tell()))
     current_pos = handler.tell()
     cdata = handler.read(compressed_data_size)
 
     decobj = zlib.decompressobj(-15) # no header
     try:
         decompressed = decobj.decompress(cdata) + decobj.flush()
     except Exception as e:
         raise BAMException(BAMException.DECOMPRESSION_FAILURE, '{} AT {} '.format(str(e), current_pos))
 
     buf = handler.read(8)
     if len(buf) < 8:
         raise BAMException(BAMException.BUFFER_TERMINATED, ' AT {} '.format(current_pos))
     crc32, input_size = struct.unpack('<II', buf)
+    if not strict_mode:
+        if 0 < len(decompressed) <= 65535:
+            return decompressed
     if input_size == len(decompressed):
         crc32_calc = zlib.crc32(decompressed)
         if crc32_calc != crc32:            
             raise BAMException(BAMException.INCONSISTENT_CHECKSUM, 'CRC is {:x} , not {:x} AT {} '.format(crc32_calc, crc32, current_pos))
         return decompressed
     else:
         # sys.stderr.write(f'inconsistent size of decompressed buffer {expected_size} / {len(data)}\n')
@@ -233,19 +243,29 @@
     Args:
         filename_bam (str): BAM filename
         filename_fastq (str): Fastq filename 
 
     Returns:
         dict: information of results
     """
-    logger =kwargs.get('logger', logging.getLogger())
+    verbose = kwargs.get('verbose', False)
+    logger = kwargs.get('logger', None)
+    if logger is None:
+        if verbose:
+            logger = _get_logger('')
+        else:
+            logger = logging.getLogger()
+    if verbose:
+        logger.setLevel(logging.DEBUG)
+#    logger =kwargs.get('logger', logging.getLogger())
     info = {'input':filename_bam, 'output':filename_fastq}
     # force_continuation = kwargs.get('forced', False)
     limit = kwargs.get('limit', 0)
     seek_pos = kwargs.get('fileseek', 0)
+    strict_mode = kwargs.get('strict', False) # check block size and CRC32
 
     fasta_mode = filename_fastq is None or re.search('\\.m?fa(\\.gz)?$', filename_fastq)
 
     if filename_fastq is None:
         # ostr = None
         ostr = sys.stdout
     elif filename_fastq.endswith('.gz'):                                                                                                                                                   
@@ -271,23 +291,23 @@
         n_unaligned_blocks = 0
         
         # read header
         if seek_pos == 0: # read header if the process starts from the top
             file_ptr = 0 # pointer of file for backtracking
             try:
                 n_blocks += 1
-                data = read_next_block(fi)
+                data = read_next_block(fi, strict=strict_mode)
                 if data[0:4] != b'BAM\1':
                     logger.warning('BAM header lost\n')
                     raise Exception('the file is not BAM')
                 l_text = struct.unpack('<I', data[4:8])[0]
                 while l_text + 12 > len(data):
                     logger.info('reading remant header {}/{}\n'.format(len(data), l_text))
                     n_blocks += 1
-                    data += scan_next_block(fi)
+                    data += scan_next_block(fi, strict=strict_mode)
                 text_ = data[8:8+l_text].decode('latin-1')
                 pos = 8 + l_text
                 # load references
                 n_ref = struct.unpack('<I', data[pos:pos+4])[0]
                 logger.info(f'references : {n_ref}')
                 pos += 4
                 for i in range(n_ref):
@@ -298,28 +318,28 @@
                     l_ref = struct.unpack('<I', data[pos:pos+4])[0]
                     references.append((name, l_ref))
                     # logger.info('@SQ\t{}\tLN:{}'.format(name, l_ref))
                     pos += 4
                     if pos > len(data): #
                         # logger.info('extend header block {} / {}'.format(pos, len(data)))
                         n_blocks += 1
-                        data += scan_next_block(fi)
+                        data += scan_next_block(fi, strict=strict_mode)
                 info['references'] = references
             except BAMException as e:
                 if e.kind == BAMException.BUFFER_TERMINATED: # end of file
-                    logger.warning('no header and file terminated')
+                    logger.info('no header and file terminated')
                     return
                 else:
-                    logger.warning(str(e))
+                    logger.info(str(e))
                 tracking_data.append([e.kind, file_ptr])
                 # logger.warning('header was corrupted, skip header blocks {}'.format(str(e)))
                 n_malformed_gzip_blocks += 1
             except Exception as e:
                 tracking_data.append([-2, file_ptr])
-                logger.warning('header was corrupted, skip header blocks')
+                logger.info('header was corrupted, skip header blocks')
                 n_malformed_gzip_blocks += 1
                 raise
 
         # alignment section
         n_seqs = 0
         total_bases = 0
         keep_running = True
@@ -330,19 +350,19 @@
             file_ptr = fi.tell()
             if file_ptr >= filesize: # check position is in the file size
                 tracking_data.append([BAMException.BUFFER_TERMINATED, file_ptr]) # end
                 break
             try:
                 n_blocks += 1
                 if pos == 0:
-                    data = scan_next_block(fi)
+                    data = scan_next_block(fi, strict=strict_mode)
                 else:
-                    data = read_next_block(fi)
+                    data = read_next_block(fi, strict=strict_mode)
             except BAMException as e:
-                logger.warning(str(e))
+                logger.info(str(e))
                 n_malformed_gzip_blocks += 1
                 tracking_data.append([e.kind, file_ptr])
                 pos = 0
                 continue
             except:
                 n_malformed_gzip_blocks += 1
                 tracking_data.append([-2, file_ptr])
@@ -355,15 +375,15 @@
                 if file_ptr >= filesize: # check position is in the file size
                     tracking_data.append([BAMException.BUFFER_TERMINATED, file_ptr])
                     break
                 if pos > 0:
                     data = data[pos:]
                     pos = 0
                 if len(data) < 36: # buffer is empty
-                    sys.stderr.write(f'\033[Kbuffer size below 36 AT {file_ptr}\n')
+                    logger.info(f'\033[Kbuffer size below 36 AT {file_ptr}\n')
                     data = []
                     pos = 0
                     break
                 block_size, refid, mappos, l_read_name, mapq, bai_bin, n_cigar_op, flag, l_seq, next_refid, next_pos, tlen \
                     = struct.unpack('<IiiBBHHHIiii', data[pos:pos + 36])
 
                 # assert variable range
@@ -382,19 +402,19 @@
                 else:
                     # read data block
                     while block_size + ptr_block_start >= len(data):
                         # print(block_size + ptr_block_start, len(data), fi.tell())
                         # logger.info('extending alignment block to {} (current {})'.format(block_size, len(data) - pos))
                         try:
                             n_blocks += 1
-                            data += read_next_block(fi)
+                            data += read_next_block(fi, strict=strict_mode)
                         except BAMException as e:
                             tracking_data.append([e.kind, file_ptr])
                             n_malformed_gzip_blocks += 1
-                            logger.warning('\033[Kfailed to loading : {}'.format(str(e)))
+                            logger.info('\033[Kfailed to loading : {}'.format(str(e)))
                             data = []
                             break
                         except Exception as e:
                             tracking_data.append([-1, file_ptr])
                             raise
                     if len(data) == 0: # skip blocks
                         break
@@ -475,15 +495,15 @@
                         elif atype in ('s', 'S'):
                             pos += count_ * 2
                         elif atype in ('i', 'I', 'f'):
                             pos += count_ * 4
                         while pos > len(data):
                             try:
                                 n_blocks += 1
-                                data += read_next_block(fi)
+                                data += read_next_block(fi, strict=strict_mode)
                                 sys.stderr.write('buffer extended to {} / {}\n'.format(pos, len(data)))
                             except:
                                 tracing_ptr[TRACE_ID_READING] = file_ptr
                                 n_malformed_gzip_blocks += 1
                                 # if not force_continuation:
                                 #     raise
                     else:
@@ -525,14 +545,15 @@
     parser.add_argument('-o','--outdir', default=None)
     parser.add_argument('--seek', default=0, type=int, help='seek position, start from given position by percent(0-100, default 0)')
     parser.add_argument('--verbose', action='store_true')
     parser.add_argument('--mode', choices=['test', 'fasta', 'fasta.gz', 'fastq', 'fastq.gz', 'fa.gz', 'fa', 'fz', 'fq', 'fqz'], default='fastq.gz',
                         help='output mode (test:no output, fq/fastq:fastq fqz/fastq.gz/gzipped fastq, fa/fasta:fasta, fz:gzipped fasta)')
     parser.add_argument('--limit', type=int, default=0)
     parser.add_argument('-V', '--version', action='store_true', help='Show current version')
+    parser.add_argument('--strict', action='store_true', help='Check CRC32')
     parser.add_argument('-p', type=int, default=4, metavar='number', help='Number of threads for gzip compression, this option is ignored if mode is not gzipped output')
     
     args, cmds = parser.parse_known_args()
     if args.version:
         print(version())
         exit()
     if args.input is None:
@@ -557,21 +578,23 @@
         stdout_mode = True
     limit = args.limit
     mode = args.mode
     gzipped = mode in ('fz', 'fastq.gz', 'fqz', 'fasta.gz', 'fa.gz')
     fasta = mode in ('fa', 'fasta', 'fa.gz', 'fz')
 
     logger = _get_logger(os.path.basename(__file__))
-    if args.verbose:
+    verbose = args.verbose
+    if verbose:
         logger.setLevel(10)
     info = {
         'command':sys.argv,
         'input':filenames,
         'files':[],
     }
+    strict_mode = args.strict
     
     if filenames is None:
         raise Exception('no BAM files given')
 
     for filename in filenames:
         if filename.endswith('.bam'):
             title = os.path.basename(filename)[0:-4]
@@ -579,15 +602,15 @@
                 filename_out = None
             elif fasta:
                 filename_out = os.path.join(outdir, title + '.fa')
             else:
                 filename_out = os.path.join(outdir, title + '.fastq')
             if (not stdout_mode) and gzipped:
                 filename_out += '.gz'
-            finfo = retrieve_fastq_from_bam(filename, filename_out, logger=logger, limit=limit, threads=n_threads, fileseek=seek_pos)
+            finfo = retrieve_fastq_from_bam(filename, filename_out, verbose=verbose, limit=limit, threads=n_threads, fileseek=seek_pos, strict=strict_mode)
             # output error log
             tracking_data = finfo.pop('error.log', [])
             if outdir is not None:
                 filename_log = os.path.join(outdir, '.{}.log'.format(os.path.basename(filename)))
                 with open(filename_log, 'w') as fo:
                     fo.write('#filename={}\n'.format(filename))
                     fo.write('#filesize={}\n'.format(os.path.getsize(filename)))
```

### Comparing `bamsalvage-0.1.5/.gitignore` & `bamsalvage-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `bamsalvage-0.1.5/LICENSE` & `bamsalvage-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bamsalvage-0.1.5/README.md` & `bamsalvage-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `bamsalvage-0.1.5/pyproject.toml` & `bamsalvage-0.1.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bamsalvage"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
-  { name="Example Author", email="author@example.com" },
+  { name="Takaho A. Endo", email="takaho.endo@gmail.com"},
 ]
 description = "Sequence salvaging script from corrupted BAM files"
 readme = "README.md"
 licence = "MIT"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `bamsalvage-0.1.5/PKG-INFO` & `bamsalvage-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bamsalvage
-Version: 0.1.5
+Version: 0.1.6
 Summary: Sequence salvaging script from corrupted BAM files
 Project-URL: Homepage, https://pypi.org/project/bamsalvage/
-Author-email: Example Author <author@example.com>
+Author-email: "Takaho A. Endo" <takaho.endo@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: mgzip
 Requires-Dist: numba
```

