# Comparing `tmp/tensorflow_nearest_neighbours-0.0.4-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/tensorflow_nearest_neighbours-0.0.5-cp39-cp39-macosx_13_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 49389 bytes, number of entries: 11
--rw-r--r--  2.0 unx       87 b- defN 23-Apr-21 22:27 tensorflow_nearest_neighbours/__init__.py
--rwxr-xr-x  2.0 unx   120064 b- defN 23-Apr-21 22:33 tensorflow_nearest_neighbours/_nearest_neighbours_op.so
--rw-r--r--  2.0 unx       51 b- defN 23-Apr-21 22:27 tensorflow_nearest_neighbours/python/__init__.py
--rw-r--r--  2.0 unx     2167 b- defN 23-Apr-21 22:27 tensorflow_nearest_neighbours/python/nearest_neighbours.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-21 22:27 test/__init__.py
--rw-r--r--  2.0 unx     2805 b- defN 23-Apr-21 22:27 test/nearest_neighbours_test.py
--rw-r--r--  2.0 unx    11342 b- defN 23-Apr-21 22:33 tensorflow_nearest_neighbours-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     1094 b- defN 23-Apr-21 22:33 tensorflow_nearest_neighbours-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx      103 b- defN 23-Apr-21 22:33 tensorflow_nearest_neighbours-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       35 b- defN 23-Apr-21 22:33 tensorflow_nearest_neighbours-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1084 b- defN 23-Apr-21 22:33 tensorflow_nearest_neighbours-0.0.4.dist-info/RECORD
-11 files, 138832 bytes uncompressed, 47495 bytes compressed:  65.8%
+Zip file size: 34480 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      115 b- defN 23-Apr-25 20:26 tensorflow_nearest_neighbours/__init__.py
+-rw-r--r--  2.0 unx     7896 b- defN 23-Apr-26 00:29 tensorflow_nearest_neighbours/_nearest_neighbours.metallib
+-rwxr-xr-x  2.0 unx    93078 b- defN 23-Apr-26 00:29 tensorflow_nearest_neighbours/_nearest_neighbours_op.so
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-25 20:26 tensorflow_nearest_neighbours/python/__init__.py
+-rw-r--r--  2.0 unx     3512 b- defN 23-Apr-25 20:26 tensorflow_nearest_neighbours/python/nearest_neighbours.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-20 22:13 test/__init__.py
+-rw-r--r--  2.0 unx     4415 b- defN 23-Apr-25 20:43 test/nearest_neighbours_test.py
+-rw-r--r--  2.0 unx    11342 b- defN 23-Apr-26 00:29 tensorflow_nearest_neighbours-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1094 b- defN 23-Apr-26 00:29 tensorflow_nearest_neighbours-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Apr-26 00:29 tensorflow_nearest_neighbours-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       35 b- defN 23-Apr-26 00:29 tensorflow_nearest_neighbours-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1198 b- defN 23-Apr-26 00:29 tensorflow_nearest_neighbours-0.0.5.dist-info/RECORD
+12 files, 122793 bytes uncompressed, 32394 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: tensorflow_nearest_neighbours/__init__.py
 Comment: 
 
+Filename: tensorflow_nearest_neighbours/_nearest_neighbours.metallib
+Comment: 
+
 Filename: tensorflow_nearest_neighbours/_nearest_neighbours_op.so
 Comment: 
 
 Filename: tensorflow_nearest_neighbours/python/__init__.py
 Comment: 
 
 Filename: tensorflow_nearest_neighbours/python/nearest_neighbours.py
@@ -12,23 +15,23 @@
 
 Filename: test/__init__.py
 Comment: 
 
 Filename: test/nearest_neighbours_test.py
 Comment: 
 
-Filename: tensorflow_nearest_neighbours-0.0.4.dist-info/LICENSE
+Filename: tensorflow_nearest_neighbours-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: tensorflow_nearest_neighbours-0.0.4.dist-info/METADATA
+Filename: tensorflow_nearest_neighbours-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: tensorflow_nearest_neighbours-0.0.4.dist-info/WHEEL
+Filename: tensorflow_nearest_neighbours-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: tensorflow_nearest_neighbours-0.0.4.dist-info/top_level.txt
+Filename: tensorflow_nearest_neighbours-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: tensorflow_nearest_neighbours-0.0.4.dist-info/RECORD
+Filename: tensorflow_nearest_neighbours-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tensorflow_nearest_neighbours/__init__.py

```diff
@@ -1 +1 @@
-from tensorflow_nearest_neighbours.python.nearest_neighbours import nearest_neighbours
+from tensorflow_nearest_neighbours.python.nearest_neighbours import nearest_neighbours, nearest_neighbours_indexes
```

## tensorflow_nearest_neighbours/_nearest_neighbours_op.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### strings --all --bytes=8 {}

```diff
@@ -1,813 +1,479 @@
-__gmon_start__
-_ITM_deregisterTMCloneTable
-_ITM_registerTMCloneTable
-__cxa_finalize
-_Unwind_Resume
-_ZN10tensorflow11register_op19OpDefBuilderWrapper5InputEPKc
-_ZN10tensorflow11register_op19OpDefBuilderWrapper6OutputEPKc
-_ZN10tensorflow11register_op19OpDefBuilderWrapperC2EPKc
-_ZN10tensorflow11register_op19OpDefBuilderWrapperclEv
-_ZN10tensorflow12OpDefBuilder10SetShapeFnESt8functionIFN3tsl6StatusEPNS_15shape_inference16InferenceContextEEE
-_ZN10tensorflow12OpDefBuilder5InputENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
-_ZN10tensorflow12OpDefBuilder6OutputENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
-_ZN10tensorflow12OpDefBuilderC1ENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
-_ZN10tensorflow12OpDefBuilderD2Ev
-_ZN10tensorflow15shape_inference16InferenceContext12DimKnownRankENS0_11ShapeHandleEl
-_ZN10tensorflow15shape_inference16InferenceContext3DimENS0_11ShapeHandleEl
-_ZN10tensorflow15shape_inference16InferenceContext8WithRankENS0_11ShapeHandleElPS2_
-_ZN10tensorflow15shape_inference16InferenceContext9MakeShapeESt16initializer_listINS0_19DimensionOrConstantEE
-_ZN10tensorflow5OpDefD1Ev
-_ZN3tsl6StatusD1Ev
-_ZN3tsl8OkStatusEv
-_ZN3tsl8internal15LogMessageFatalC1EPKci
-_ZN3tsl8internal15LogMessageFatalD1Ev
-_ZN3tsl8internal17MakeCheckOpStringIiiEEPNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERKT_RKT0_PKc
-_ZN3tsl8internal21CheckOpMessageBuilder7ForVar2Ev
-_ZN3tsl8internal21CheckOpMessageBuilder9NewStringB5cxx11Ev
-_ZN3tsl8internal21CheckOpMessageBuilderC1EPKc
-_ZN3tsl8internal21CheckOpMessageBuilderD1Ev
-_ZNSolsEi
-_ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm
-_ZNSt8ios_base4InitC1Ev
-_ZNSt8ios_base4InitD1Ev
-_ZSt16__ostream_insertIcSt11char_traitsIcEERSt13basic_ostreamIT_T0_ES6_PKS3_l
-_ZSt19__throw_logic_errorPKc
-_ZSt20__throw_length_errorPKc
-_ZSt24__throw_out_of_range_fmtPKcz
-_ZSt9terminatev
-_ZStlsIN3tsl8internal15LogMessageFatalENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEEENSt9enable_ifIXsr6__and_ISt6__not_ISt19is_lvalue_referenceIT_EESt33__is_convertible_to_basic_ostreamISC_ESt15__is_insertableINSG_14__ostream_typeERKT0_vEEE5valueESI_E4typeEOSC_SL_
-_ZStlsISt11char_traitsIcEERSt13basic_ostreamIcT_ES5_PKc
-_ZTVN10__cxxabiv117__class_type_infoE
-__cxa_atexit
-__cxa_begin_catch
-__gxx_personality_v0
-_ZN10tensorflow14kernel_factory17OpKernelRegistrar12InitInternalEPKNS_9KernelDefESt17basic_string_viewIcSt11char_traitsIcEESt10unique_ptrINS0_15OpKernelFactoryESt14default_deleteISA_EE
-_ZN10tensorflow14kernel_factory17OpKernelRegistrarC2EPKNS_9KernelDefESt17basic_string_viewIcSt11char_traitsIcEEPFPNS_8OpKernelEPNS_20OpKernelConstructionEE
-_ZN10tensorflow15OpKernelContext15allocate_outputEiRKNS_11TensorShapeEPPNS_6TensorE
-_ZN10tensorflow15OpKernelContext21CtxFailureWithWarningEPKciRKN3tsl6StatusE
-_ZN10tensorflow15OpKernelContext5inputESt17basic_string_viewIcSt11char_traitsIcEEPPKNS_6TensorE
-_ZN10tensorflow15register_kernel4NameC1EPKc
-_ZN10tensorflow16KernelDefBuilder5BuildEv
-_ZN10tensorflow16KernelDefBuilder6DeviceEPKc
-_ZN10tensorflow16KernelDefBuilderD2Ev
-_ZN10tensorflow22CheckNotInComputeAsyncEPNS_15OpKernelContextEPKc
-_ZN10tensorflow7functor19NearestNeighboursOpIN5Eigen16ThreadPoolDeviceEfE7ComputeEPNS_15OpKernelContextE
-_ZN10tensorflow7functor19NearestNeighboursOpIN5Eigen16ThreadPoolDeviceEfED0Ev
-_ZN10tensorflow7functor19NearestNeighboursOpIN5Eigen9GpuDeviceEfE7ComputeEPNS_15OpKernelContextE
-_ZN10tensorflow7functor19NearestNeighboursOpIN5Eigen9GpuDeviceEfED0Ev
-_ZN10tensorflow7functor24NearestNeighboursFunctorIN5Eigen16ThreadPoolDeviceEfEclERKS3_NS0_10paramsTypeEPKfS9_Pf
-_ZN10tensorflow7functor24NearestNeighboursFunctorIN5Eigen9GpuDeviceEfEclERKS3_NS0_10paramsTypeEPKfS9_Pf
-_ZN10tensorflow8OpKernel11IsExpensiveEv
-_ZN10tensorflow8OpKernel7AsAsyncEv
-_ZN10tensorflow8OpKernelC2EPNS_20OpKernelConstructionE
-_ZN10tensorflow8OpKernelD2Ev
-_ZN5Eigen15PlainObjectBaseINS_6MatrixIfLin1ELi1ELi0ELin1ELi1EEEE6resizeEll
-_ZN5Eigen15PlainObjectBaseINS_6MatrixIfLin1ELi1ELi0ELin1ELi1EEEEC2INS_5BlockIKNS_3MapIKNS1_IfLin1ELin1ELi1ELin1ELin1EEELi0ENS_6StrideILi0ELi0EEEEELi1ELin1ELb1EEEEERKNS_9DenseBaseIT_EE
-_ZN5Eigen15PlainObjectBaseINS_6MatrixIfLin1ELin1ELi1ELin1ELin1EEEE6resizeEll
-_ZN5Eigen15PlainObjectBaseINS_6MatrixIfLin1ELin1ELi1ELin1ELin1EEEEC2INS_3MapIKS2_Li0ENS_6StrideILi0ELi0EEEEEEERKNS_9DenseBaseIT_EE
-_ZNK10tensorflow15OpKernelContext12eigen_deviceIN5Eigen16ThreadPoolDeviceEEERKT_v
-_ZNK10tensorflow15OpKernelContext12eigen_deviceIN5Eigen9GpuDeviceEEERKT_v
-_ZNK10tensorflow15TensorShapeBaseINS_11TensorShapeEE8dim_sizeEi
-_ZNK10tensorflow6Tensor21CheckTypeAndIsAlignedENS_8DataTypeE
-_ZNK10tensorflow8OpKernel11TraceStringB5cxx11ERKNS_15OpKernelContextEb
-_ZNK10tensorflow8OpKernel12const_tensorEv
-_ZNSt9bad_allocD1Ev
-_ZTIN10tensorflow7functor19NearestNeighboursOpIN5Eigen16ThreadPoolDeviceEfEE
-_ZTIN10tensorflow7functor19NearestNeighboursOpIN5Eigen9GpuDeviceEfEE
-_ZTIN10tensorflow8OpKernelE
-_ZTISt9bad_alloc
-_ZTSN10tensorflow7functor19NearestNeighboursOpIN5Eigen16ThreadPoolDeviceEfEE
-_ZTSN10tensorflow7functor19NearestNeighboursOpIN5Eigen9GpuDeviceEfEE
-_ZTVN10__cxxabiv120__si_class_type_infoE
-_ZTVN10tensorflow14kernel_factory17OpKernelRegistrar18PtrOpKernelFactoryE
-_ZTVN10tensorflow7functor19NearestNeighboursOpIN5Eigen16ThreadPoolDeviceEfEE
-_ZTVN10tensorflow7functor19NearestNeighboursOpIN5Eigen9GpuDeviceEfEE
-_ZTVSt9bad_alloc
-__assert_fail
-__cxa_allocate_exception
-__cxa_throw
-_ZN4dim3C2Ejjj
-_ZN4dim3C1Ejjj
-_ZN5Eigen8internal5all_tC2Ev
-_ZN5Eigen8internal5all_tC1Ev
-_ZN10tensorflow15TensorShapeBaseINS_11TensorShapeEE10kIsPartialE
-_ZN10tensorflow15TensorShapeBaseINS_18PartialTensorShapeEE10kIsPartialE
-_ZN10tensorflow7functor88_GLOBAL__N__60_tmpxft_00000246_00000000_7_nearest_neighbours_kernel_cpp1_ii_c3e05665_59013index_2d_flatEiii
-_ZN10tensorflow7functor88_GLOBAL__N__60_tmpxft_00000246_00000000_7_nearest_neighbours_kernel_cpp1_ii_c3e05665_59013index_3d_flatEiiiii
-__cudaPushCallConfiguration
-_ZN10tensorflow7functor27NearestNeighboursCudaKernelIfEEvPKT_S4_PS2_iii
-__stack_chk_fail
-_ZN10tensorflow7functor24NearestNeighboursFunctorIN5Eigen9GpuDeviceEdEclERKS3_NS0_10paramsTypeEPKdS9_Pd
-_ZN10tensorflow7functor27NearestNeighboursCudaKernelIdEEvPKT_S4_PS2_iii
-__cudaUnregisterFatBinary
-__cudaInitModule
-__cudaPopCallConfiguration
-__cudaRegisterFunction
-__cudaRegisterFatBinary
-__cudaRegisterFatBinaryEnd
-_ZN5Eigen8symbolic10SymbolExprINS_8internal17symbolic_last_tagEEC2Ev
-_ZN5Eigen8symbolic10SymbolExprINS_8internal17symbolic_last_tagEEC1Ev
-_ZNK5Eigen8internal8FixedIntILi1EEclEv
-_ZNK5Eigen8symbolic8BaseExprINS0_10SymbolExprINS_8internal17symbolic_last_tagEEEEplILi1EEENS0_7AddExprIS5_NS0_9ValueExprINS3_8FixedIntIXT_EEEEEEESB_
-_ZN5Eigen8symbolic9ValueExprINS_8internal8FixedIntILi1EEEEC1Ev
-_ZNK5Eigen8symbolic8BaseExprINS0_10SymbolExprINS_8internal17symbolic_last_tagEEEE7derivedEv
-_ZN5Eigen8symbolic7AddExprINS0_10SymbolExprINS_8internal17symbolic_last_tagEEENS0_9ValueExprINS3_8FixedIntILi1EEEEEEC1ERKS5_RKS9_
-cudaLaunchKernel
-_ZN5Eigen8symbolic9ValueExprINS_8internal8FixedIntILi1EEEEC2Ev
-_ZN5Eigen8symbolic7AddExprINS0_10SymbolExprINS_8internal17symbolic_last_tagEEENS0_9ValueExprINS3_8FixedIntILi1EEEEEEC2ERKS5_RKS9_
-libtensorflow_framework.so.2
-libcudart.so.11.0
-libstdc++.so.6
-libm.so.6
-libgcc_s.so.1
-libc.so.6
-GLIBC_2.4
-GLIBC_2.2.5
-GLIBC_2.14
-GLIBCXX_3.4.9
-CXXABI_1.3
-GLIBCXX_3.4
-AWAVATSH
-([A\A^A_
-AWAVATSH
-H[A\A^A_
-AWAVATSH
-H[A\A^A_
-UAWAVAUATSPH
-[A\A]A^A_]
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_
-UAWAVAUATSH
-8[A\A]A^A_]
-UAWAVAUATSH
-D$8H;\$0L
-[A\A]A^A_]
-AWAVATSPI
-AWAVATSPH
-UAWAVAUATSH
-8[A\A]A^A_]
+__stub_helper
+__objc_stubs
+__gcc_except_tab__TEXT
+__cstring
+__objc_methname
+__unwind_info
+__DATA_CONST
+__DATA_CONST
+__mod_init_func
+__DATA_CONST
+__DATA_CONST
+__cfstring
+__DATA_CONST
+__objc_imageinfo__DATA_CONST
+__la_symbol_ptr
+__objc_selrefs
+__objc_classrefs__DATA
+__common
+__LINKEDIT
+tensorflow_nearest_neighbours/_nearest_neighbours_op.so
+/System/Library/Frameworks/Foundation.framework/Versions/C/Foundation
+/System/Library/Frameworks/Metal.framework/Versions/A/Metal
+@rpath/libtensorflow_framework.2.dylib
+/usr/lib/libc++.1.dylib
+/usr/lib/libSystem.B.dylib
+/System/Library/Frameworks/CoreFoundation.framework/Versions/A/CoreFoundation
+/usr/lib/libobjc.A.dylib
 NearestNeighbours
 token_embeddings: float32
 embedding_matrix: float32
 nearest_neighbours: float32
-basic_string::_M_construct null not valid
-vector::_M_range_check: __n (which is %zu) >= this->size() (which is %zu)
-vector::_M_realloc_insert
-/tensorflow_nearest_neighbours/.tox/linux-py39/lib/python3.9/site-packages/tensorflow/include/tensorflow/core/framework/shape_inference.h
+NearestNeighboursIndexes
+nearest_neighbours_indexes: int32
+basic_string
+/Users/artemsereda/Documents/IdeaProjects/tensorflow_nearest_neighbours/.tox/macosx-py39/lib/python3.9/site-packages/tensorflow/include/tensorflow/core/framework/shape_inference.h
 s->rank_ != kUnknownRank
 Check failed: dim.IsSet() 
 Internal error: Got nullptr for Dimension.
 NearestNeighboursOp<CPUDevice, float>
 token_embeddings
 OP_REQUIRES_OK_ASYNC
 tensorflow_nearest_neighbours/cc/kernels/nearest_neighbours_kernel.cc
 embedding_matrix
+MapBase.h
 (dataPtr == 0) || ( rows >= 0 && (RowsAtCompileTime == Dynamic || RowsAtCompileTime == rows) && cols >= 0 && (ColsAtCompileTime == Dynamic || ColsAtCompileTime == cols))
-/tensorflow_nearest_neighbours/.tox/linux-py39/lib/python3.9/site-packages/tensorflow/include/unsupported/Eigen/CXX11/../../../Eigen/src/Core/MapBase.h
-Eigen::MapBase<Eigen::Map<const Eigen::Matrix<float, -1, -1, 1, -1, -1>, 0, Eigen::Stride<0, 0> >, 0>::MapBase(Eigen::MapBase<type-parameter-0-0, 0>::PointerType, Eigen::Index, Eigen::Index) [Derived = Eigen::Map<const Eigen::Matrix<float, -1, -1, 1, -1, -1>, 0, Eigen::Stride<0, 0> >, Level = 0]
-cannot create std::vector larger than max_size()
 (i>=0) && ( ((BlockRows==1) && (BlockCols==XprType::ColsAtCompileTime) && i<xpr.rows()) ||((BlockRows==XprType::RowsAtCompileTime) && (BlockCols==1) && i<xpr.cols()))
-/tensorflow_nearest_neighbours/.tox/linux-py39/lib/python3.9/site-packages/tensorflow/include/unsupported/Eigen/CXX11/../../../Eigen/src/Core/Block.h
-Eigen::Block<const Eigen::Map<const Eigen::Matrix<float, -1, -1, 1, -1, -1>, 0, Eigen::Stride<0, 0> >, 1, -1, true>::Block(XprType &, Eigen::Index) [XprType = const Eigen::Map<const Eigen::Matrix<float, -1, -1, 1, -1, -1>, 0, Eigen::Stride<0, 0> >, BlockRows = 1, BlockCols = -1, InnerPanel = true]
-Eigen::MapBase<Eigen::Block<const Eigen::Map<const Eigen::Matrix<float, -1, -1, 1, -1, -1>, 0, Eigen::Stride<0, 0> >, 1, -1, true>, 0>::MapBase(Eigen::MapBase<type-parameter-0-0, 0>::PointerType, Eigen::Index, Eigen::Index) [Derived = Eigen::Block<const Eigen::Map<const Eigen::Matrix<float, -1, -1, 1, -1, -1>, 0, Eigen::Stride<0, 0> >, 1, -1, true>, Level = 0]
-Eigen::Block<const Eigen::Matrix<float, -1, -1, 1, -1, -1>, 1, -1, true>::Block(XprType &, Eigen::Index) [XprType = const Eigen::Matrix<float, -1, -1, 1, -1, -1>, BlockRows = 1, BlockCols = -1, InnerPanel = true]
-Eigen::MapBase<Eigen::Block<const Eigen::Matrix<float, -1, -1, 1, -1, -1>, 1, -1, true>, 0>::MapBase(Eigen::MapBase<type-parameter-0-0, 0>::PointerType, Eigen::Index, Eigen::Index) [Derived = Eigen::Block<const Eigen::Matrix<float, -1, -1, 1, -1, -1>, 1, -1, true>, Level = 0]
-aLhs.rows() == aRhs.rows() && aLhs.cols() == aRhs.cols()
-/tensorflow_nearest_neighbours/.tox/linux-py39/lib/python3.9/site-packages/tensorflow/include/unsupported/Eigen/CXX11/../../../Eigen/src/Core/CwiseBinaryOp.h
-Eigen::CwiseBinaryOp<Eigen::internal::scalar_difference_op<float, float>, const Eigen::Block<const Eigen::Matrix<float, -1, -1, 1, -1, -1>, 1, -1, true>, const Eigen::Transpose<const Eigen::Matrix<float, -1, 1, 0, -1, 1> > >::CwiseBinaryOp(const Eigen::CwiseBinaryOp::Lhs &, const Eigen::CwiseBinaryOp::Rhs &, const BinaryOp &) [BinaryOp = Eigen::internal::scalar_difference_op<float, float>, Lhs = const Eigen::Block<const Eigen::Matrix<float, -1, -1, 1, -1, -1>, 1, -1, true>, Rhs = const Eigen::Transpose<const Eigen::Matrix<float, -1, 1, 0, -1, 1> >]
 this->rows()>0 && this->cols()>0 && "you are using an empty matrix"
-/tensorflow_nearest_neighbours/.tox/linux-py39/lib/python3.9/site-packages/tensorflow/include/unsupported/Eigen/CXX11/../../../Eigen/src/Core/Redux.h
-typename internal::traits<Derived>::Scalar Eigen::DenseBase<Eigen::CwiseUnaryOp<Eigen::internal::scalar_abs2_op<float>, const Eigen::CwiseBinaryOp<Eigen::internal::scalar_difference_op<float, float>, const Eigen::Block<const Eigen::Matrix<float, -1, -1, 1, -1, -1>, 1, -1, true>, const Eigen::Transpose<const Eigen::Matrix<float, -1, 1, 0, -1, 1> > > > >::redux(const Func &) const [Derived = Eigen::CwiseUnaryOp<Eigen::internal::scalar_abs2_op<float>, const Eigen::CwiseBinaryOp<Eigen::internal::scalar_difference_op<float, float>, const Eigen::Block<const Eigen::Matrix<float, -1, -1, 1, -1, -1>, 1, -1, true>, const Eigen::Transpose<const Eigen::Matrix<float, -1, 1, 0, -1, 1> > > >, BinaryOp = Eigen::internal::scalar_sum_op<float, float>]
-/tensorflow_nearest_neighbours/.tox/linux-py39/lib/python3.9/site-packages/tensorflow/include/unsupported/Eigen/CXX11/../../../Eigen/src/Core/PlainObjectBase.h
+PlainObjectBase.h
 internal::check_implication(RowsAtCompileTime!=Dynamic, rows==RowsAtCompileTime) && internal::check_implication(ColsAtCompileTime!=Dynamic, cols==ColsAtCompileTime) && internal::check_implication(RowsAtCompileTime==Dynamic && MaxRowsAtCompileTime!=Dynamic, rows<=MaxRowsAtCompileTime) && internal::check_implication(ColsAtCompileTime==Dynamic && MaxColsAtCompileTime!=Dynamic, cols<=MaxColsAtCompileTime) && rows>=0 && cols>=0 && "Invalid sizes when resizing a matrix or array."
-void Eigen::PlainObjectBase<Eigen::Matrix<float, -1, 1, 0, -1, 1> >::resize(Eigen::Index, Eigen::Index) [Derived = Eigen::Matrix<float, -1, 1, 0, -1, 1>]
-dst.rows() == dstRows && dst.cols() == dstCols
-/tensorflow_nearest_neighbours/.tox/linux-py39/lib/python3.9/site-packages/tensorflow/include/unsupported/Eigen/CXX11/../../../Eigen/src/Core/AssignEvaluator.h
-void Eigen::internal::resize_if_allowed(DstXprType &, const SrcXprType &, const internal::assign_op<T1, T2> &) [DstXprType = Eigen::Transpose<Eigen::Matrix<float, -1, 1, 0, -1, 1> >, SrcXprType = Eigen::Block<const Eigen::Map<const Eigen::Matrix<float, -1, -1, 1, -1, -1>, 0, Eigen::Stride<0, 0> >, 1, -1, true>, T1 = float, T2 = float]
-void Eigen::PlainObjectBase<Eigen::Matrix<float, -1, -1, 1, -1, -1> >::resize(Eigen::Index, Eigen::Index) [Derived = Eigen::Matrix<float, -1, -1, 1, -1, -1>]
-void Eigen::internal::resize_if_allowed(DstXprType &, const SrcXprType &, const internal::assign_op<T1, T2> &) [DstXprType = Eigen::Matrix<float, -1, -1, 1, -1, -1>, SrcXprType = Eigen::Map<const Eigen::Matrix<float, -1, -1, 1, -1, -1>, 0, Eigen::Stride<0, 0> >, T1 = float, T2 = float]
-NearestNeighboursOp<GPUDevice, float>
+NearestNeighboursIndexesOp<CPUDevice, float>
+_nearest_neighbours.metallib
+Found metallib at: 
+ Error while registering 
+allocation failed: %s
+no stream was found: %s
+nearest_neighbours
+NearestNeighboursOp_Compute_block_invoke
+nearest_neighbours_kernel.mm
+pipeline
+Failed to find metallib
+Compilation error: %s
+NSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEEE
+NSt3__110__function6__baseIFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEEE
+NSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEEE
 N10tensorflow7functor19NearestNeighboursOpIN5Eigen16ThreadPoolDeviceEfEE
-N10tensorflow7functor19NearestNeighboursOpIN5Eigen9GpuDeviceEfEE
-_ZN10tensorflow7functor27NearestNeighboursCudaKernelIdEEvPKT_S4_PS2_iii
-_ZN10tensorflow7functor27NearestNeighboursCudaKernelIfEEvPKT_S4_PS2_iii
-__NV_MODULE_ID
-.shstrtab
-.symtab_shndx
-.nv.info
-.text._ZN10tensorflow7functor27NearestNeighboursCudaKernelIdEEvPKT_S4_PS2_iii
-.nv.info._ZN10tensorflow7functor27NearestNeighboursCudaKernelIdEEvPKT_S4_PS2_iii
-.nv.shared._ZN10tensorflow7functor27NearestNeighboursCudaKernelIdEEvPKT_S4_PS2_iii
-.nv.global.init
-.nv.constant2._ZN10tensorflow7functor27NearestNeighboursCudaKernelIdEEvPKT_S4_PS2_iii
-.nv.constant0._ZN10tensorflow7functor27NearestNeighboursCudaKernelIdEEvPKT_S4_PS2_iii
-.text._ZN10tensorflow7functor27NearestNeighboursCudaKernelIfEEvPKT_S4_PS2_iii
-.nv.info._ZN10tensorflow7functor27NearestNeighboursCudaKernelIfEEvPKT_S4_PS2_iii
-.nv.shared._ZN10tensorflow7functor27NearestNeighboursCudaKernelIfEEvPKT_S4_PS2_iii
-.nv.constant2._ZN10tensorflow7functor27NearestNeighboursCudaKernelIfEEvPKT_S4_PS2_iii
-.nv.constant0._ZN10tensorflow7functor27NearestNeighboursCudaKernelIfEEvPKT_S4_PS2_iii
-.nv.rel.action
-.shstrtab
-.symtab_shndx
-.nv.info
-_ZN10tensorflow7functor27NearestNeighboursCudaKernelIdEEvPKT_S4_PS2_iii
-.text._ZN10tensorflow7functor27NearestNeighboursCudaKernelIdEEvPKT_S4_PS2_iii
-.nv.info._ZN10tensorflow7functor27NearestNeighboursCudaKernelIdEEvPKT_S4_PS2_iii
-.nv.shared._ZN10tensorflow7functor27NearestNeighboursCudaKernelIdEEvPKT_S4_PS2_iii
-.nv.global.init
-_ZZN3tsl15float8_internal11ConvertImplINS0_13float8_e4m3fnENS0_11float8_e5m2ELb0ELb0EvE3runERKS2_E11kNormalized
-.nv.constant2._ZN10tensorflow7functor27NearestNeighboursCudaKernelIdEEvPKT_S4_PS2_iii
-__ocg_const
-$_ZN10tensorflow7functor27NearestNeighboursCudaKernelIdEEvPKT_S4_PS2_iii$__cuda_sm20_dsqrt_rn_f64_mediumpath_v1
-$_ZN10tensorflow7functor27NearestNeighboursCudaKernelIdEEvPKT_S4_PS2_iii$__internal_accurate_pow
-.nv.constant0._ZN10tensorflow7functor27NearestNeighboursCudaKernelIdEEvPKT_S4_PS2_iii
-_ZN10tensorflow7functor27NearestNeighboursCudaKernelIfEEvPKT_S4_PS2_iii
-.text._ZN10tensorflow7functor27NearestNeighboursCudaKernelIfEEvPKT_S4_PS2_iii
-.nv.info._ZN10tensorflow7functor27NearestNeighboursCudaKernelIfEEvPKT_S4_PS2_iii
-.nv.shared._ZN10tensorflow7functor27NearestNeighboursCudaKernelIfEEvPKT_S4_PS2_iii
-.nv.constant2._ZN10tensorflow7functor27NearestNeighboursCudaKernelIfEEvPKT_S4_PS2_iii
-$_ZN10tensorflow7functor27NearestNeighboursCudaKernelIfEEvPKT_S4_PS2_iii$__cuda_sm20_sqrt_rn_f32_slowpath
-$_ZN10tensorflow7functor27NearestNeighboursCudaKernelIfEEvPKT_S4_PS2_iii$__internal_accurate_pow
-.nv.constant0._ZN10tensorflow7functor27NearestNeighboursCudaKernelIfEEvPKT_S4_PS2_iii
-.nv.rel.action
-.version 7.2
-.target sm_52
-.address_size 64.
-func (.param .b64 
-_retval0) __internal_accurate_pow
-.global .align 1 .b8 _ZZN3tsl15float8H
-11ConvertImplINS0_13#
-qe4m3fnE
-q5m2ELb0
-1vE3runERKS2_E11kNormalized[8] = {0, 24, 28, 30, 32, 33, 34, 35};E
-isible .entry _ZN10tensorflow7$
-$tor27NearestNeighboursCudaKernelIfEEvPKT_S4_PS2_iii5
-.reg .pred %p<86>;
-f32 %f<50
-64 %fd<58
-setp.eq.s
-@%p4 bra LBB0_53;
-atemp; 7
-146435072;
-s7483647=
-1062207488#
-call.uni (
-rcvt.rziW
-y0dFFF807
-10716446
-$	;/13%	O/51%	
-8(	*51(	"85
-&r8(	,20)	
-(472	N101,+
-9;	/31;	
-	;	$4,A	(29
-.pragma "nounroll";(
-"	;/16#	P
-107312758
-rcp.approx.ftz.
-ED0F5D241AD3B5A#
-EB0F5FF7D2CAFE2
-F3B20A75488A3FJ
-1745CDE4FAECD
-3C71C7258A578BJ
-_a3F6249
-0dBC46A4CB00B9E7B*
-127219200/
-E62E42FEFA39E
-3C7ABC9E3B3980
--3355443
--15728641Q
-F71547652B82FE
-928AF3FCA213EA$
-5ADE1569CE2BDs
-C71DEE624013s
-A01997C89EB71O
-d3F2A01A014761F
-56C16C1852B7A<
-0f4086232B
-GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.1) 9.4.0
-clang version 10.0.0-4ubuntu1 
-GCC_except_table10
-GCC_except_table11
+N10tensorflow7functor26NearestNeighboursIndexesOpIN5Eigen16ThreadPoolDeviceEfEE
+URLWithString:
+UTF8String
+commitAndWait
+computeCommandEncoder
+currentCommandBuffer
+description
+dispatchThreadgroups:threadsPerThreadgroup:
+endEncoding
+mainBundle
+newComputePipelineStateWithFunction:error:
+newFunctionWithName:
+newLibraryWithURL:error:
+resourcePath
+setBuffer:offset:atIndex:
+setBytes:length:atIndex:
+setComputePipelineState:
+stringByDeletingLastPathComponent
+stringWithUTF8String:
+!hRFSAZAp
+@_OBJC_CLASS_$_NSBundle
+@_OBJC_CLASS_$_NSString
+@__ZN10tensorflow15TensorShapeBaseINS_11TensorShapeEEC2EN4absl12lts_202206234SpanIKxEE
+@__ZNK10tensorflow15TensorShapeBaseINS_11TensorShapeEE8dim_sizeEi
+@__ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb
+@__ZTIN10tensorflow8OpKernelE
+@__ZTVN10tensorflow14kernel_factory17OpKernelRegistrar18PtrOpKernelFactoryE
+@__ZNSt12length_errorD1Ev
+@__ZNSt12out_of_rangeD1Ev
+@__ZNSt20bad_array_new_lengthD1Ev
+@__ZNSt3__14cerrE
+@__ZNSt3__14coutE
+@__ZNSt3__15ctypeIcE2idE
+@__ZNSt9bad_allocD1Ev
+@__ZTISt12length_error
+@__ZTISt12out_of_range
+@__ZTISt20bad_array_new_length
+@__ZTISt9bad_alloc
+@__ZTVN10__cxxabiv117__class_type_infoE
+@__ZTVN10__cxxabiv120__si_class_type_infoE
+@__ZTVSt12length_error
+@__ZTVSt12out_of_range
+@__ZdlPv
+@___gxx_personality_v0
+@__NSConcreteStackBlock
+@___stack_chk_guard
+@dyld_stub_binder
+@_OBJC_CLASS_$_NSURL
+@___CFConstantStringClassReference
+@_objc_msgSend
+@__ZN10tensorflow15TensorShapeBaseINS_11TensorShapeEEC2EN4absl12lts_202206234SpanIKxEE
+@__ZNK10tensorflow15TensorShapeBaseINS_11TensorShapeEE8dim_sizeEi
+@__ZTISt12length_error
+@__ZTISt12out_of_range
+@__ZdlPv
+@_MTLCreateSystemDefaultDevice
+@_TF_AllocateOutput
+@_TF_DeleteStatus
+@_TF_DeleteTensor
+@_TF_Dim
+@_TF_GetCode
+@_TF_GetInput
+@_TF_GetStream
+@_TF_Message
+@_TF_NewKernelBuilder
+@_TF_NewStatus
+@_TF_NumDims
+@_TF_OpKernelContext_Failure
+@_TF_RegisterKernelBuilder
+@_TF_TensorData
+@_TF_TensorType
+@__Block_object_assign
+@__Block_object_dispose
+@__Unwind_Resume
+@__ZN10tensorflow11register_op19OpDefBuilderWrapperclEv
+@__ZN10tensorflow12OpDefBuilder10SetShapeFnENSt3__18functionIFN3tsl6StatusEPNS_15shape_inference16InferenceContextEEEE
+@__ZN10tensorflow12OpDefBuilder5InputENSt3__112basic_stringIcNS1_11char_traitsIcEENS1_9allocatorIcEEEE
+@__ZN10tensorflow12OpDefBuilder6OutputENSt3__112basic_stringIcNS1_11char_traitsIcEENS1_9allocatorIcEEEE
+@__ZN10tensorflow12OpDefBuilderC1ENSt3__112basic_stringIcNS1_11char_traitsIcEENS1_9allocatorIcEEEE
+@__ZN10tensorflow14TensorShapeRep12SlowCopyFromERKS0_
+@__ZN10tensorflow14TensorShapeRep19DestructorOutOfLineEv
+@__ZN10tensorflow14kernel_factory17OpKernelRegistrar12InitInternalEPKNS_9KernelDefENSt3__117basic_string_viewIcNS5_11char_traitsIcEEEENS5_10unique_ptrINS0_15OpKernelFactoryENS5_14default_deleteISB_EEEE
+@__ZN10tensorflow15OpKernelContext15allocate_outputEiRKNS_11TensorShapeEPPNS_6TensorE
+@__ZN10tensorflow15OpKernelContext21CtxFailureWithWarningEPKciRKN3tsl6StatusE
+@__ZN10tensorflow15OpKernelContext5inputENSt3__117basic_string_viewIcNS1_11char_traitsIcEEEEPPKNS_6TensorE
+@__ZN10tensorflow15register_kernel4NameC1EPKc
+@__ZN10tensorflow15shape_inference16InferenceContext8WithRankENS0_11ShapeHandleExPS2_
+@__ZN10tensorflow15shape_inference16InferenceContext9MakeShapeESt16initializer_listINS0_19DimensionOrConstantEE
+@__ZN10tensorflow16KernelDefBuilder5BuildEv
+@__ZN10tensorflow16KernelDefBuilder6DeviceEPKc
+@__ZN10tensorflow16KernelDefBuilderD2Ev
+@__ZN10tensorflow22CheckNotInComputeAsyncEPNS_15OpKernelContextEPKc
+@__ZN10tensorflow5OpDefD1Ev
+@__ZN10tensorflow8OpKernelC2EPNS_20OpKernelConstructionE
+@__ZN10tensorflow8OpKernelD2Ev
+@__ZN3tsl6StatusD1Ev
+@__ZN3tsl8OkStatusEv
+@__ZN3tsl8internal15LogMessageFatalC1EPKci
+@__ZN3tsl8internal15LogMessageFatalD1Ev
+@__ZN3tsl8internal21CheckOpMessageBuilder7ForVar2Ev
+@__ZN3tsl8internal21CheckOpMessageBuilder9NewStringEv
+@__ZN3tsl8internal21CheckOpMessageBuilderC1EPKc
+@__ZN3tsl8internal21CheckOpMessageBuilderD1Ev
+@__ZNK10tensorflow15OpKernelContext12eigen_deviceIN5Eigen16ThreadPoolDeviceEEERKT_v
+@__ZNK10tensorflow6Tensor21CheckTypeAndIsAlignedENS_8DataTypeE
+@__ZNKSt3__14__fs10filesystem28recursive_directory_iterator13__dereferenceEv
+@__ZNKSt3__16locale9use_facetERNS0_2idE
+@__ZNKSt3__18ios_base6getlocEv
+@__ZNSt11logic_errorC2EPKc
+@__ZNSt20bad_array_new_lengthC1Ev
+@__ZNSt3__112basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEE6appendEPKcm
+@__ZNSt3__112basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEE9push_backEc
+@__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEE3putEc
+@__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEE5flushEv
+@__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEE6sentryC1ERS3_
+@__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEE6sentryD1Ev
+@__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEElsEi
+@__ZNSt3__119__shared_weak_count14__release_weakEv
+@__ZNSt3__14__fs10filesystem14__current_pathEPNS_10error_codeE
+@__ZNSt3__14__fs10filesystem28recursive_directory_iterator11__incrementEPNS_10error_codeE
+@__ZNSt3__14__fs10filesystem28recursive_directory_iteratorC1ERKNS1_4pathENS1_17directory_optionsEPNS_10error_codeE
+@__ZNSt3__16localeD1Ev
+@__ZNSt3__18ios_base33__set_badbit_and_consider_rethrowEv
+@__ZNSt3__18ios_base5clearEj
+@__ZNSt9bad_allocC1Ev
+@__ZSt9terminatev
+@___assert_rtn
+@___cxa_allocate_exception
+@___cxa_begin_catch
+@___cxa_end_catch
+@___cxa_free_exception
+@___cxa_throw
+@___stack_chk_fail
+@_dispatch_sync
+@_malloc
+@_memcpy
+@_memmove
+@_memset
+@_objc_autorelease
+@_objc_autoreleasePoolPop
+@_objc_autoreleasePoolPush
+@_printf
+@_strcmp
+@_strlen
+16locate_metal_libRKNSt3__112basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEEE
+8getShapeP9TF_Tensor
+9ends_withRKNSt3__112basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEEES7_
+N22KernelLibrarySingleton
+7libraryE
+9sInstanceE
+gInitPlugin
+__Z16locate_metal_libRKNSt3__112basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEEE
+__Z8getShapeP9TF_Tensor
+__Z9ends_withRKNSt3__112basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEEES7_
+__ZN22KernelLibrarySingleton7libraryE
+__ZN22KernelLibrarySingleton9sInstanceE
+_gInitPlugin
+_MTLCreateSystemDefaultDevice
+_OBJC_CLASS_$_NSBundle
+_OBJC_CLASS_$_NSString
+_OBJC_CLASS_$_NSURL
+_TF_AllocateOutput
+_TF_DeleteStatus
+_TF_DeleteTensor
+_TF_GetCode
+_TF_GetInput
+_TF_GetStream
+_TF_Message
+_TF_NewKernelBuilder
+_TF_NewStatus
+_TF_NumDims
+_TF_OpKernelContext_Failure
+_TF_RegisterKernelBuilder
+_TF_TensorData
+_TF_TensorType
+__Block_object_assign
+__Block_object_dispose
+__NSConcreteStackBlock
+__Unwind_Resume
+__ZN10tensorflow11register_op19OpDefBuilderWrapperclEv
+__ZN10tensorflow12OpDefBuilder10SetShapeFnENSt3__18functionIFN3tsl6StatusEPNS_15shape_inference16InferenceContextEEEE
+__ZN10tensorflow12OpDefBuilder5InputENSt3__112basic_stringIcNS1_11char_traitsIcEENS1_9allocatorIcEEEE
+__ZN10tensorflow12OpDefBuilder6OutputENSt3__112basic_stringIcNS1_11char_traitsIcEENS1_9allocatorIcEEEE
+__ZN10tensorflow12OpDefBuilderC1ENSt3__112basic_stringIcNS1_11char_traitsIcEENS1_9allocatorIcEEEE
+__ZN10tensorflow14TensorShapeRep12SlowCopyFromERKS0_
+__ZN10tensorflow14TensorShapeRep19DestructorOutOfLineEv
+__ZN10tensorflow14kernel_factory17OpKernelRegistrar12InitInternalEPKNS_9KernelDefENSt3__117basic_string_viewIcNS5_11char_traitsIcEEEENS5_10unique_ptrINS0_15OpKernelFactoryENS5_14default_deleteISB_EEEE
+__ZN10tensorflow15OpKernelContext15allocate_outputEiRKNS_11TensorShapeEPPNS_6TensorE
+__ZN10tensorflow15OpKernelContext21CtxFailureWithWarningEPKciRKN3tsl6StatusE
+__ZN10tensorflow15OpKernelContext5inputENSt3__117basic_string_viewIcNS1_11char_traitsIcEEEEPPKNS_6TensorE
+__ZN10tensorflow15TensorShapeBaseINS_11TensorShapeEEC2EN4absl12lts_202206234SpanIKxEE
+__ZN10tensorflow15register_kernel4NameC1EPKc
+__ZN10tensorflow15shape_inference16InferenceContext8WithRankENS0_11ShapeHandleExPS2_
+__ZN10tensorflow15shape_inference16InferenceContext9MakeShapeESt16initializer_listINS0_19DimensionOrConstantEE
+__ZN10tensorflow16KernelDefBuilder5BuildEv
+__ZN10tensorflow16KernelDefBuilder6DeviceEPKc
+__ZN10tensorflow16KernelDefBuilderD2Ev
+__ZN10tensorflow22CheckNotInComputeAsyncEPNS_15OpKernelContextEPKc
+__ZN10tensorflow5OpDefD1Ev
+__ZN10tensorflow8OpKernelC2EPNS_20OpKernelConstructionE
+__ZN10tensorflow8OpKernelD2Ev
+__ZN3tsl6StatusD1Ev
+__ZN3tsl8OkStatusEv
+__ZN3tsl8internal15LogMessageFatalC1EPKci
+__ZN3tsl8internal15LogMessageFatalD1Ev
+__ZN3tsl8internal21CheckOpMessageBuilder7ForVar2Ev
+__ZN3tsl8internal21CheckOpMessageBuilder9NewStringEv
+__ZN3tsl8internal21CheckOpMessageBuilderC1EPKc
+__ZN3tsl8internal21CheckOpMessageBuilderD1Ev
+__ZNK10tensorflow15OpKernelContext12eigen_deviceIN5Eigen16ThreadPoolDeviceEEERKT_v
+__ZNK10tensorflow15TensorShapeBaseINS_11TensorShapeEE8dim_sizeEi
+__ZNK10tensorflow6Tensor21CheckTypeAndIsAlignedENS_8DataTypeE
+__ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb
+__ZNKSt3__14__fs10filesystem28recursive_directory_iterator13__dereferenceEv
+__ZNKSt3__16locale9use_facetERNS0_2idE
+__ZNKSt3__18ios_base6getlocEv
+__ZNSt11logic_errorC2EPKc
+__ZNSt12length_errorD1Ev
+__ZNSt12out_of_rangeD1Ev
+__ZNSt20bad_array_new_lengthC1Ev
+__ZNSt20bad_array_new_lengthD1Ev
+__ZNSt3__112basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEE6appendEPKcm
+__ZNSt3__112basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEE9push_backEc
+__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEE3putEc
+__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEE5flushEv
+__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEE6sentryC1ERS3_
+__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEE6sentryD1Ev
+__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEElsEi
+__ZNSt3__119__shared_weak_count14__release_weakEv
+__ZNSt3__14__fs10filesystem14__current_pathEPNS_10error_codeE
+__ZNSt3__14__fs10filesystem28recursive_directory_iterator11__incrementEPNS_10error_codeE
+__ZNSt3__14__fs10filesystem28recursive_directory_iteratorC1ERKNS1_4pathENS1_17directory_optionsEPNS_10error_codeE
+__ZNSt3__14cerrE
+__ZNSt3__14coutE
+__ZNSt3__15ctypeIcE2idE
+__ZNSt3__16localeD1Ev
+__ZNSt3__18ios_base33__set_badbit_and_consider_rethrowEv
+__ZNSt3__18ios_base5clearEj
+__ZNSt9bad_allocC1Ev
+__ZNSt9bad_allocD1Ev
+__ZSt9terminatev
+__ZTIN10tensorflow8OpKernelE
+__ZTISt12length_error
+__ZTISt12out_of_range
+__ZTISt20bad_array_new_length
+__ZTISt9bad_alloc
+__ZTVN10__cxxabiv117__class_type_infoE
+__ZTVN10__cxxabiv120__si_class_type_infoE
+__ZTVN10tensorflow14kernel_factory17OpKernelRegistrar18PtrOpKernelFactoryE
+__ZTVSt12length_error
+__ZTVSt12out_of_range
+___CFConstantStringClassReference
+___assert_rtn
+___cxa_allocate_exception
+___cxa_begin_catch
+___cxa_end_catch
+___cxa_free_exception
+___cxa_throw
+___gxx_personality_v0
+___stack_chk_fail
+___stack_chk_guard
+_dispatch_sync
+_memmove
+_objc_autorelease
+_objc_autoreleasePoolPop
+_objc_autoreleasePoolPush
+_objc_msgSend
+dyld_stub_binder
+__ZN10tensorflow11register_op19OpDefBuilderWrapper5InputEPKc
+__ZN10tensorflow11register_op19OpDefBuilderWrapper6OutputEPKc
+__ZN10tensorflow11register_op19OpDefBuilderWrapper10SetShapeFnENSt3__18functionIFN3tsl6StatusEPNS_15shape_inference16InferenceContextEEEE
+__ZN10tensorflow11register_op19OpDefBuilderWrapperC2EPKc
+__ZNKSt3__112basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEE20__throw_length_errorB6v15006Ev
+__ZNSt3__120__throw_length_errorB6v15006EPKc
+__ZNSt12length_errorC1B6v15006EPKc
+__ZSt28__throw_bad_array_new_lengthB6v15006v
+___clang_call_terminate
+__ZN10tensorflow12OpDefBuilderD2Ev
+__ZNSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEED1Ev
+__ZNSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEED0Ev
+__ZNKSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEE7__cloneEv
+__ZNKSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEE7__cloneEPNS0_6__baseISB_EE
+__ZNSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEE7destroyEv
+__ZNSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEE18destroy_deallocateEv
+__ZNSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEEclEOSA_
+__ZNKSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEE6targetERKSt9type_info
+__ZNKSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEE11target_typeEv
+__ZN10tensorflow15shape_inference16InferenceContext3DimENS0_11ShapeHandleEx
+__ZNKSt3__16vectorIN10tensorflow15shape_inference11ShapeHandleENS_9allocatorIS3_EEE20__throw_out_of_rangeB6v15006Ev
+__ZNSt3__120__throw_out_of_rangeB6v15006EPKc
+__ZNSt12out_of_rangeC1B6v15006EPKc
+__ZN10tensorflow15shape_inference16InferenceContext12DimKnownRankENS0_11ShapeHandleEx
+__ZNKSt3__16vectorIPN10tensorflow15shape_inference9DimensionENS_9allocatorIS4_EEE20__throw_length_errorB6v15006Ev
+__ZNSt3__124__put_character_sequenceIcNS_11char_traitsIcEEEERNS_13basic_ostreamIT_T0_EES7_PKS4_m
+__ZNSt3__116__pad_and_outputIcNS_11char_traitsIcEEEENS_19ostreambuf_iteratorIT_T0_EES6_PKS4_S8_S8_RNS_8ios_baseES4_
+__ZNSt3__1lsB6v15006IN3tsl8internal15LogMessageFatalENS_12basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEEEvEEOT_SB_RKT0_
+__ZN3tsl8internal17MakeCheckOpStringIiiEEPNSt3__112basic_stringIcNS2_11char_traitsIcEENS2_9allocatorIcEEEERKT_RKT0_PKc
+__ZNSt3__1lsB6v15006IN3tsl8internal15LogMessageFatalEA43_cvEEOT_S6_RKT0_
+__ZNSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEED1Ev
+__ZNSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEED0Ev
+__ZNKSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEE7__cloneEv
+__ZNKSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEE7__cloneEPNS0_6__baseISB_EE
+__ZNSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEE7destroyEv
+__ZNSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEE18destroy_deallocateEv
+__ZNSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEEclEOSA_
+__ZNKSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEE6targetERKSt9type_info
+__ZNKSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEE11target_typeEv
+__GLOBAL__sub_I_nearest_neighbours_op.cc
+__ZN10tensorflow14kernel_factory17OpKernelRegistrarC1EPKNS_9KernelDefENSt3__117basic_string_viewIcNS5_11char_traitsIcEEEEPFPNS_8OpKernelEPNS_20OpKernelConstructionEE
+__ZZNK10tensorflow7functor3$_0clEPKNS_9KernelDefEENUlPNS_20OpKernelConstructionEE_8__invokeES6_
+__ZN10tensorflow7functor26NearestNeighboursIndexesOpIN5Eigen16ThreadPoolDeviceEfED1Ev
+__ZN10tensorflow7functor19NearestNeighboursOpIN5Eigen16ThreadPoolDeviceEfED1Ev
+__ZN10tensorflow7functor26NearestNeighboursIndexesOpIN5Eigen16ThreadPoolDeviceEfED0Ev
+__ZN10tensorflow7functor19NearestNeighboursOpIN5Eigen16ThreadPoolDeviceEfED0Ev
+__ZN10tensorflow7functor19NearestNeighboursOpIN5Eigen16ThreadPoolDeviceEfE7ComputeEPNS_15OpKernelContextE
+__ZNK10tensorflow8OpKernel12const_tensorEv
+__ZN10tensorflow8OpKernel7AsAsyncEv
+__ZN10tensorflow8OpKernel11IsExpensiveEv
+__ZN10tensorflow7functor24NearestNeighboursFunctorIN5Eigen16ThreadPoolDeviceEfEclERKS3_NS0_10paramsTypeEPKfS9_Pf
+__ZNKSt3__16vectorIfNS_9allocatorIfEEE20__throw_length_errorB6v15006Ev
+__ZN10tensorflow14kernel_factory17OpKernelRegistrarC2EPKNS_9KernelDefENSt3__117basic_string_viewIcNS5_11char_traitsIcEEEEPFPNS_8OpKernelEPNS_20OpKernelConstructionEE
+__ZZNK10tensorflow7functor3$_1clEPKNS_9KernelDefEENUlPNS_20OpKernelConstructionEE_8__invokeES6_
+__ZN10tensorflow7functor26NearestNeighboursIndexesOpIN5Eigen16ThreadPoolDeviceEfE7ComputeEPNS_15OpKernelContextE
+__ZN10tensorflow11TensorShapeD1Ev
+__ZN10tensorflow7functor31NearestNeighboursIndexesFunctorIN5Eigen16ThreadPoolDeviceEfEclERKS3_NS0_10paramsTypeEPKfS9_Pi
+_OUTLINED_FUNCTION_0
+__GLOBAL__sub_I_nearest_neighbours_kernel.cc
+__ZNSt3__14__fs10filesystem28recursive_directory_iteratorD1Ev
+__ZNSt3__14endlIcNS_11char_traitsIcEEEERNS_13basic_ostreamIT_T0_EES7_
+__ZNSt3__16vectorIxNS_9allocatorIxEEE8__appendEm
+__ZNKSt3__16vectorIxNS_9allocatorIxEEE20__throw_length_errorB6v15006Ev
+__Z14RegisterKernelIfEvPKc
+__ZL26NearestNeighboursOp_CreateP23TF_OpKernelConstruction
+__ZL27NearestNeighboursOp_ComputePvP18TF_OpKernelContext
+__ZL26NearestNeighboursOp_DeletePv
+____ZL27NearestNeighboursOp_ComputePvP18TF_OpKernelContext_block_invoke
+__ZN22KernelLibrarySingleton11getInstanceEv
+___copy_helper_block_e8_32o
+___destroy_helper_block_e8_32o
+__ZNSt3__112basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEE6appendB6v15006IPKcEENS_9enable_ifIXsr27__is_cpp17_forward_iteratorIT_EE5valueERS5_E4typeESA_SA_
+__ZNSt3__115__quoted_outputB6v15006IcNS_11char_traitsIcEEEERNS_13basic_ostreamIT_T0_EES7_PKS4_S9_S4_S4_
+__GLOBAL__sub_I_nearest_neighbours_kernel.mm
+__ZN10tensorflow11register_op19OpDefBuilderWrapper10SetShapeFnENSt3__18functionIFN3tsl6StatusEPNS_15shape_inference16InferenceContextEEEE.cold.1
+__ZN10tensorflow7functor24NearestNeighboursFunctorIN5Eigen16ThreadPoolDeviceEfEclERKS3_NS0_10paramsTypeEPKfS9_Pf.cold.1
+__ZN10tensorflow7functor24NearestNeighboursFunctorIN5Eigen16ThreadPoolDeviceEfEclERKS3_NS0_10paramsTypeEPKfS9_Pf.cold.2
+__ZN10tensorflow7functor31NearestNeighboursIndexesFunctorIN5Eigen16ThreadPoolDeviceEfEclERKS3_NS0_10paramsTypeEPKfS9_Pi.cold.1
+__ZN10tensorflow7functor31NearestNeighboursIndexesFunctorIN5Eigen16ThreadPoolDeviceEfEclERKS3_NS0_10paramsTypeEPKfS9_Pi.cold.2
+____ZL27NearestNeighboursOp_ComputePvP18TF_OpKernelContext_block_invoke.cold.1
+_objc_msgSend$URLWithString:
+_objc_msgSend$UTF8String
+_objc_msgSend$cString
+_objc_msgSend$commitAndWait
+_objc_msgSend$computeCommandEncoder
+_objc_msgSend$currentCommandBuffer
+_objc_msgSend$description
+_objc_msgSend$device
+_objc_msgSend$dispatchThreadgroups:threadsPerThreadgroup:
+_objc_msgSend$endEncoding
+_objc_msgSend$mainBundle
+_objc_msgSend$newComputePipelineStateWithFunction:error:
+_objc_msgSend$newFunctionWithName:
+_objc_msgSend$newLibraryWithURL:error:
+_objc_msgSend$queue
+_objc_msgSend$resourcePath
+_objc_msgSend$setBuffer:offset:atIndex:
+_objc_msgSend$setBytes:length:atIndex:
+_objc_msgSend$setComputePipelineState:
+_objc_msgSend$stringByDeletingLastPathComponent
+_objc_msgSend$stringWithUTF8String:
+GCC_except_table0
+GCC_except_table1
 GCC_except_table2
 GCC_except_table3
-GCC_except_table4
 GCC_except_table5
-GCC_except_table6
-GCC_except_table9
-_GLOBAL__sub_I_nearest_neighbours_op.cc
-_ZL12register_op0
-_ZN5Eigen12placeholdersL3allE
-_ZN5Eigen12placeholdersL4lastE
-_ZN5Eigen12placeholdersL6lastp1E
-_ZNSt14_Function_base13_Base_managerI3$_0E10_M_managerERSt9_Any_dataRKS3_St18_Manager_operation
-_ZNSt17_Function_handlerIFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEE3$_0E9_M_invokeERKSt9_Any_dataOS5_
-_ZStL8__ioinit
-_ZTI3$_0
-_ZTS3$_0
-GCC_except_table0
-GCC_except_table1
-GCC_except_table12
-GCC_except_table14
-GCC_except_table15
-GCC_except_table7
+GCC_except_table16
+GCC_except_table21
+GCC_except_table23
+GCC_except_table25
+GCC_except_table26
+GCC_except_table28
+GCC_except_table36
+GCC_except_table39
+GCC_except_table4
 GCC_except_table8
-_GLOBAL__sub_I_nearest_neighbours_kernel.cc
-_ZN10tensorflow7functorL17register_kernel_0E
-_ZN10tensorflow7functorL17register_kernel_1E
-_ZZNK10tensorflow7functor3$_0clEPKNS_9KernelDefEENUlPNS_20OpKernelConstructionEE_8__invokeES6_
-_ZZNK10tensorflow7functor3$_1clEPKNS_9KernelDefEENUlPNS_20OpKernelConstructionEE_8__invokeES6_
-crtstuff.c
-deregister_tm_clones
-__do_global_dtors_aux
-completed.8061
-__do_global_dtors_aux_fini_array_entry
-frame_dummy
-__frame_dummy_init_array_entry
-tmpxft_00000246_00000000-6_nearest_neighbours_kernel.cudafe1.cpp
-_ZL22__nv_inited_managed_rt
-_ZL32__nv_fatbinhandle_for_managed_rt
-_ZL37__nv_save_fatbinhandle_for_managed_rtPPv
-_ZN6__pstl9execution2v1L3seqE
-_ZN6__pstl9execution2v1L3parE
-_ZN6__pstl9execution2v1L9par_unseqE
-_ZN6__pstl9execution2v1L5unseqE
-_ZN4absl12lts_2022062313time_internalL19kTicksPerNanosecondE
-_ZN4absl12lts_2022062313time_internalL15kTicksPerSecondE
-_ZN5EigenL7DynamicE
-_ZN5EigenL12DynamicIndexE
-_ZN5EigenL13UndefinedIncrE
-_ZN5EigenL8InfinityE
-_ZN5EigenL8HugeCostE
-_ZN5EigenL11RowMajorBitE
-_ZN5EigenL20EvalBeforeNestingBitE
-_ZN5EigenL22EvalBeforeAssigningBitE
-_ZN5EigenL15PacketAccessBitE
-_ZN5EigenL21ActualPacketAccessBitE
-_ZN5EigenL15LinearAccessBitE
-_ZN5EigenL9LvalueBitE
-_ZN5EigenL15DirectAccessBitE
-_ZN5EigenL10AlignedBitE
-_ZN5EigenL12NestByRefBitE
-_ZN5EigenL26NoPreferredStorageOrderBitE
-_ZN5EigenL19CompressedAccessBitE
-_ZN5EigenL14HereditaryBitsE
-_ZN5Eigen12placeholdersL3endE
-_ZN5EigenL9AutoOrderE
-_ZN5Eigen8internalL18defaultL1CacheSizeE
-_ZN5Eigen8internalL18defaultL2CacheSizeE
-_ZN5Eigen8internalL18defaultL3CacheSizeE
-_ZN9__gnu_cxxL21__default_lock_policyE
-_ZN4absl12lts_2022062313cord_internalL13kFlatOverheadE
-_ZN4absl12lts_2022062313cord_internalL12kMinFlatSizeE
-_ZN4absl12lts_2022062313cord_internalL12kMaxFlatSizeE
-_ZN4absl12lts_2022062313cord_internalL14kMaxFlatLengthE
-_ZN4absl12lts_2022062313cord_internalL14kMinFlatLengthE
-_ZN4absl12lts_2022062313cord_internalL17kMaxLargeFlatSizeE
-_ZN4absl12lts_2022062313cord_internalL19kMaxLargeFlatLengthE
-_ZN4absl12lts_2022062313cord_internalL8kTagBaseE
-_ZN4absl12lts_2022062316numbers_internalL17kFastToBufferSizeE
-_ZN4absl12lts_2022062316numbers_internalL22kSixDigitsToBufferSizeE
-_ZN3tslL9kuint8maxE
-_ZN3tslL10kuint16maxE
-_ZN3tslL10kuint32maxE
-_ZN3tslL10kuint64maxE
-_ZN3tslL8kint8minE
-_ZN3tslL8kint8maxE
-_ZN3tslL9kint16minE
-_ZN3tslL9kint16maxE
-_ZN3tslL9kint32minE
-_ZN3tslL9kint32maxE
-_ZN3tslL9kint64minE
-_ZN3tslL9kint64maxE
-_ZN3tsl4portL13kLittleEndianE
-_ZN10tensorflow4portL13kLittleEndianE
-_ZN10tensorflowL9kuint8maxE
-_ZN10tensorflowL10kuint16maxE
-_ZN10tensorflowL10kuint32maxE
-_ZN10tensorflowL10kuint64maxE
-_ZN10tensorflowL8kint8minE
-_ZN10tensorflowL8kint8maxE
-_ZN10tensorflowL9kint16minE
-_ZN10tensorflowL9kint16maxE
-_ZN10tensorflowL9kint32minE
-_ZN10tensorflowL9kint32maxE
-_ZN10tensorflowL9kint64minE
-_ZN10tensorflowL9kint64maxE
-_ZN3tslL4INFOE
-_ZN3tslL7WARNINGE
-_ZN3tslL5ERRORE
-_ZN3tslL5FATALE
-_ZN3tslL14NUM_SEVERITIESE
-_ZN3tsl4portL15kNUMANoAffinityE
-_ZN6google8protobufL9kint32maxE
-_ZN6google8protobufL9kint32minE
-_ZN6google8protobufL9kint64maxE
-_ZN6google8protobufL9kint64minE
-_ZN6google8protobufL10kuint32maxE
-_ZN6google8protobufL10kuint64maxE
-_ZN6google8protobuf8internalL27kMinHeaderVersionForLibraryE
-_ZN6google8protobuf8internalL26kMinHeaderVersionForProtocE
-_ZN6google8protobufL17kFastToBufferSizeE
-_ZN6google8protobufL19kDoubleToBufferSizeE
-_ZN6google8protobufL18kFloatToBufferSizeE
-_ZN6google8protobufL6UTFmaxE
-_ZN6google8protobuf8internalL29kRepeatedFieldUpperClampLimitE
-_ZN10tensorflow5errorL8Code_MINE
-_ZN10tensorflow5errorL8Code_MAXE
-_ZN10tensorflow5errorL14Code_ARRAYSIZEE
-_ZN10tensorflowL15kIllegalFrameIdE
-_ZN10tensorflowL14kIllegalIterIdE
-_ZN6google8protobuf8internalL21kGlobalEmptyTableSizeE
-_ZN5EigenL15kGpuScratchSizeE
-_ZN5EigenL14default_streamE
-_ZN10tensorflowL12DataType_MINE
-_ZN10tensorflowL12DataType_MAXE
-_ZN10tensorflowL18DataType_ARRAYSIZEE
-_ZN3tsl7stringsL17kFastToBufferSizeE
-_ZN10tensorflowL14FullTypeId_MINE
-_ZN10tensorflowL14FullTypeId_MAXE
-_ZN10tensorflowL20FullTypeId_ARRAYSIZEE
-_ZN6google8protobufL34FieldDescriptorProto_Type_Type_MINE
-_ZN6google8protobufL34FieldDescriptorProto_Type_Type_MAXE
-_ZN6google8protobufL40FieldDescriptorProto_Type_Type_ARRAYSIZEE
-_ZN6google8protobufL36FieldDescriptorProto_Label_Label_MINE
-_ZN6google8protobufL36FieldDescriptorProto_Label_Label_MAXE
-_ZN6google8protobufL42FieldDescriptorProto_Label_Label_ARRAYSIZEE
-_ZN6google8protobufL41FileOptions_OptimizeMode_OptimizeMode_MINE
-_ZN6google8protobufL41FileOptions_OptimizeMode_OptimizeMode_MAXE
-_ZN6google8protobufL47FileOptions_OptimizeMode_OptimizeMode_ARRAYSIZEE
-_ZN6google8protobufL28FieldOptions_CType_CType_MINE
-_ZN6google8protobufL28FieldOptions_CType_CType_MAXE
-_ZN6google8protobufL34FieldOptions_CType_CType_ARRAYSIZEE
-_ZN6google8protobufL30FieldOptions_JSType_JSType_MINE
-_ZN6google8protobufL30FieldOptions_JSType_JSType_MAXE
-_ZN6google8protobufL36FieldOptions_JSType_JSType_ARRAYSIZEE
-_ZN6google8protobufL51MethodOptions_IdempotencyLevel_IdempotencyLevel_MINE
-_ZN6google8protobufL51MethodOptions_IdempotencyLevel_IdempotencyLevel_MAXE
-_ZN6google8protobufL57MethodOptions_IdempotencyLevel_IdempotencyLevel_ARRAYSIZEE
-_ZN6google8protobufL19Field_Kind_Kind_MINE
-_ZN6google8protobufL19Field_Kind_Kind_MAXE
-_ZN6google8protobufL25Field_Kind_Kind_ARRAYSIZEE
-_ZN6google8protobufL33Field_Cardinality_Cardinality_MINE
-_ZN6google8protobufL33Field_Cardinality_Cardinality_MAXE
-_ZN6google8protobufL39Field_Cardinality_Cardinality_ARRAYSIZEE
-_ZN6google8protobufL10Syntax_MINE
-_ZN6google8protobufL10Syntax_MAXE
-_ZN6google8protobufL16Syntax_ARRAYSIZEE
-_ZN10tensorflowL9kAllTypesE
-_ZN10tensorflowL16kRealNumberTypesE
-_ZN10tensorflowL12kNumberTypesE
-_ZN10tensorflowL15kQuantizedTypesE
-_ZN10tensorflowL22kRealAndQuantizedTypesE
-_ZN10tensorflowL22kDataTypesCanUseMemcpyE
-_ZN10tensorflowL19kDataTypeIsFloatingE
-_ZN10tensorflowL18kDataTypeIsComplexE
-_ZN10tensorflowL18kDataTypeIsIntegerE
-_ZN10tensorflowL17kDataTypeIsSignedE
-_ZN10tensorflowL19kDataTypeIsUnsignedE
-_ZN4absl12lts_20220623L21kFixedArrayUseDefaultE
-_ZN10tensorflowL32ApiDef_Visibility_Visibility_MINE
-_ZN10tensorflowL32ApiDef_Visibility_Visibility_MAXE
-_ZN10tensorflowL38ApiDef_Visibility_Visibility_ARRAYSIZEE
-_ZN10tensorflowL32VerifierConfig_Toggle_Toggle_MINE
-_ZN10tensorflowL32VerifierConfig_Toggle_Toggle_MAXE
-_ZN10tensorflowL38VerifierConfig_Toggle_Toggle_ARRAYSIZEE
-_ZN10tensorflowL32RewriterConfig_Toggle_Toggle_MINE
-_ZN10tensorflowL32RewriterConfig_Toggle_Toggle_MAXE
-_ZN10tensorflowL38RewriterConfig_Toggle_Toggle_ARRAYSIZEE
-_ZN10tensorflowL38RewriterConfig_CpuLayout_CpuLayout_MINE
-_ZN10tensorflowL38RewriterConfig_CpuLayout_CpuLayout_MAXE
-_ZN10tensorflowL44RewriterConfig_CpuLayout_CpuLayout_ARRAYSIZEE
-_ZN10tensorflowL54RewriterConfig_NumIterationsType_NumIterationsType_MINE
-_ZN10tensorflowL54RewriterConfig_NumIterationsType_NumIterationsType_MAXE
-_ZN10tensorflowL60RewriterConfig_NumIterationsType_NumIterationsType_ARRAYSIZEE
-_ZN10tensorflowL40RewriterConfig_MemOptType_MemOptType_MINE
-_ZN10tensorflowL40RewriterConfig_MemOptType_MemOptType_MAXE
-_ZN10tensorflowL46RewriterConfig_MemOptType_MemOptType_ARRAYSIZEE
-_ZN10tensorflowL32OptimizerOptions_Level_Level_MINE
-_ZN10tensorflowL32OptimizerOptions_Level_Level_MAXE
-_ZN10tensorflowL38OptimizerOptions_Level_Level_ARRAYSIZEE
-_ZN10tensorflowL50OptimizerOptions_GlobalJitLevel_GlobalJitLevel_MINE
-_ZN10tensorflowL50OptimizerOptions_GlobalJitLevel_GlobalJitLevel_MAXE
-_ZN10tensorflowL56OptimizerOptions_GlobalJitLevel_GlobalJitLevel_ARRAYSIZEE
-_ZN10tensorflowL64ConfigProto_Experimental_MlirBridgeRollout_MlirBridgeRollout_MINE
-_ZN10tensorflowL64ConfigProto_Experimental_MlirBridgeRollout_MlirBridgeRollout_MAXE
-_ZN10tensorflowL70ConfigProto_Experimental_MlirBridgeRollout_MlirBridgeRollout_ARRAYSIZEE
-_ZN10tensorflowL36RunOptions_TraceLevel_TraceLevel_MINE
-_ZN10tensorflowL36RunOptions_TraceLevel_TraceLevel_MAXE
-_ZN10tensorflowL42RunOptions_TraceLevel_TraceLevel_ARRAYSIZEE
-_ZZL22____nv_dummy_param_refPvE5__ref
-_ZL22____nv_dummy_param_refPv
-_ZL15__module_id_str
-_ZL20__cudaFatCubinHandle
-_ZL26__cudaUnregisterBinaryUtilv
-_ZL32__nv_init_managed_rt_with_modulePPv
-fatbinData
-_ZL15__fatDeviceText
-_ZZL85__device_stub__ZN10tensorflow7functor27NearestNeighboursCudaKernelIfEEvPKT_S4_PS2_iiiPKfS0_PfiiiE3__f
-_ZL85__device_stub__ZN10tensorflow7functor27NearestNeighboursCudaKernelIfEEvPKT_S4_PS2_iiiPKfS0_Pfiii
-_Z16cudaLaunchKernelIcE9cudaErrorPKT_4dim3S4_PPvmP11CUstream_st
-_ZN10tensorflow7functorL50__wrapper__device_stub_NearestNeighboursCudaKernelIfEEvRPKT_S5_RPS2_RKiS9_S9_
-_ZZL85__device_stub__ZN10tensorflow7functor27NearestNeighboursCudaKernelIdEEvPKT_S4_PS2_iiiPKdS0_PdiiiE3__f
-_ZL85__device_stub__ZN10tensorflow7functor27NearestNeighboursCudaKernelIdEEvPKT_S4_PS2_iiiPKdS0_Pdiii
-_ZN10tensorflow7functorL50__wrapper__device_stub_NearestNeighboursCudaKernelIdEEvRPKT_S5_RPS2_RKiS9_S9_
-_ZZL31__nv_cudaEntityRegisterCallbackPPvE5__ref
-_ZL31__nv_cudaEntityRegisterCallbackPPv
-_ZL24__sti____cudaRegisterAllv
-_Z41__static_initialization_and_destruction_0ii
-_ZN5EigenL3fixILi1EEE
-_ZSt10is_array_vIcE
-_ZSt12is_trivial_vIcE
-_ZSt20is_standard_layout_vIcE
-_ZSt9is_same_vIccE
-_ZSt10is_array_vIwE
-_ZSt12is_trivial_vIwE
-_ZSt20is_standard_layout_vIwE
-_ZSt9is_same_vIwwE
-_ZSt10is_array_vIDsE
-_ZSt12is_trivial_vIDsE
-_ZSt20is_standard_layout_vIDsE
-_ZSt9is_same_vIDsDsE
-_ZSt10is_array_vIDiE
-_ZSt12is_trivial_vIDiE
-_ZSt20is_standard_layout_vIDiE
-_ZSt9is_same_vIDiDiE
-_ZSt15is_arithmetic_vIfE
-_ZSt33is_trivially_copy_constructible_vISt17basic_string_viewIcSt11char_traitsIcEEE
-_ZSt33is_trivially_move_constructible_vISt17basic_string_viewIcSt11char_traitsIcEEE
-_ZSt23is_copy_constructible_vISt17basic_string_viewIcSt11char_traitsIcEEE
-_ZSt7__and_vIJSt21is_copy_constructibleISt17basic_string_viewIcSt11char_traitsIcEEESt18is_copy_assignableIS4_EEE
-_ZSt23is_move_constructible_vISt17basic_string_viewIcSt11char_traitsIcEEE
-_ZSt7__and_vIJSt21is_move_constructibleISt17basic_string_viewIcSt11char_traitsIcEEESt18is_move_assignableIS4_EEE
-_ZSt27is_trivially_destructible_vISt17basic_string_viewIcSt11char_traitsIcEEE
-_ZSt30is_trivially_copy_assignable_vISt17basic_string_viewIcSt11char_traitsIcEEE
-_ZSt30is_trivially_move_assignable_vISt17basic_string_viewIcSt11char_traitsIcEEE
-_ZSt9is_same_vISt17basic_string_viewIcSt11char_traitsIcEESt9nullopt_tE
-_ZSt9is_same_vISt17basic_string_viewIcSt11char_traitsIcEESt10in_place_tE
-_ZSt14is_reference_vISt17basic_string_viewIcSt11char_traitsIcEEE
-_ZSt18is_constructible_vISt17basic_string_viewIcSt11char_traitsIcEEJEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameISt8optionalISt17basic_string_viewIcSt11char_traitsIcEEES6_EES0_IS1_ISt10in_place_tS6_EESt16is_constructibleIS6_JOS6_EESt14is_convertibleISE_S6_EEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameISt8optionalISt17basic_string_viewIcSt11char_traitsIcEEESt9nullopt_tEES0_IS1_ISt10in_place_tS8_EESt16is_constructibleIS6_JRKS8_EESt14is_convertibleISG_S6_EEE
-_ZSt33is_trivially_copy_constructible_vIlE
-_ZSt33is_trivially_move_constructible_vIlE
-_ZSt23is_copy_constructible_vIlE
-_ZSt7__and_vIJSt21is_copy_constructibleIlESt18is_copy_assignableIlEEE
-_ZSt23is_move_constructible_vIlE
-_ZSt7__and_vIJSt21is_move_constructibleIlESt18is_move_assignableIlEEE
-_ZSt27is_trivially_destructible_vIlE
-_ZSt30is_trivially_copy_assignable_vIlE
-_ZSt30is_trivially_move_assignable_vIlE
-_ZSt9is_same_vIlSt9nullopt_tE
-_ZSt9is_same_vIlSt10in_place_tE
-_ZSt14is_reference_vIlE
-_ZSt18is_constructible_vIlJEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameISt8optionalIlES3_EES0_IS1_ISt10in_place_tS3_EESt16is_constructibleIlJRKS3_EESt14is_convertibleISB_lEEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameISt8optionalIlES3_EES0_IS1_ISt10in_place_tS3_EESt16is_constructibleIlJRKS3_EES0_ISt14is_convertibleISB_lEEEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameIllEESt16is_constructibleIlJRKlEESt14is_convertibleIS6_lES0_ISt5__or_IJS4_IlJRKSt8optionalIlEEES4_IlJRSC_EES4_IlJOSD_EES4_IlJOSC_EES8_ISE_lES8_ISG_lES8_ISI_lES8_ISK_lEEEEEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameIllEESt16is_constructibleIlJRKlEES0_ISt14is_convertibleIS6_lEES0_ISt5__or_IJS4_IlJRKSt8optionalIlEEES4_IlJRSD_EES4_IlJOSE_EES4_IlJOSD_EES8_ISF_lES8_ISH_lES8_ISJ_lES8_ISL_lEEEEEE
-_ZSt7__and_vIJSt16is_constructibleIlJEEEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameISt8optionalIlES3_EES0_IS1_ISt10in_place_tS3_EESt16is_constructibleIlJOS3_EESt14is_convertibleISA_lEEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameISt8optionalIlES3_EES0_IS1_ISt10in_place_tS3_EESt16is_constructibleIlJOS3_EES0_ISt14is_convertibleISA_lEEEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameIllEESt16is_constructibleIlJOlEESt14is_convertibleIS5_lES0_ISt5__or_IJS4_IlJRKSt8optionalIlEEES4_IlJRSB_EES4_IlJOSC_EES4_IlJOSB_EES7_ISD_lES7_ISF_lES7_ISH_lES7_ISJ_lEEEEEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameIllEESt16is_constructibleIlJOlEES0_ISt14is_convertibleIS5_lEES0_ISt5__or_IJS4_IlJRKSt8optionalIlEEES4_IlJRSC_EES4_IlJOSD_EES4_IlJOSC_EES7_ISE_lES7_ISG_lES7_ISI_lES7_ISK_lEEEEEE
-_ZSt33is_trivially_copy_constructible_vIN3tsl14AllocatorStatsEE
-_ZSt33is_trivially_move_constructible_vIN3tsl14AllocatorStatsEE
-_ZSt23is_copy_constructible_vIN3tsl14AllocatorStatsEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameIllEESt16is_constructibleIlJRKlEESt13is_assignableIRllES0_ISt5__or_IJS4_IlJRKSt8optionalIlEEES4_IlJRSD_EES4_IlJOSE_EES4_IlJOSD_EESt14is_convertibleISF_lESN_ISH_lESN_ISJ_lESN_ISL_lEEEES0_ISB_IJS8_IS9_SF_ES8_IS9_SH_ES8_IS9_SJ_ES8_IS9_SL_EEEEEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameISt8optionalIlES3_EES0_ISt6__and_IJSt9is_scalarIlES1_IlS3_EEEESt16is_constructibleIlJRKS3_EESt13is_assignableIRlSE_EEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameIllEESt16is_constructibleIlJlEESt13is_assignableIRllES0_ISt5__or_IJS4_IlJRKSt8optionalIlEEES4_IlJRSB_EES4_IlJOSC_EES4_IlJOSB_EESt14is_convertibleISD_lESL_ISF_lESL_ISH_lESL_ISJ_lEEEES0_IS9_IJS6_IS7_SD_ES6_IS7_SF_ES6_IS7_SH_ES6_IS7_SJ_EEEEEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameISt8optionalIlES3_EES0_ISt6__and_IJSt9is_scalarIlES1_IlS3_EEEESt16is_constructibleIlJS3_EESt13is_assignableIRlS3_EEE
-_ZSt7__and_vIJSt21is_copy_constructibleIN3tsl14AllocatorStatsEESt18is_copy_assignableIS2_EEE
-_ZSt23is_move_constructible_vIN3tsl14AllocatorStatsEE
-_ZSt7__and_vIJSt21is_move_constructibleIN3tsl14AllocatorStatsEESt18is_move_assignableIS2_EEE
-_ZSt27is_trivially_destructible_vIN3tsl14AllocatorStatsEE
-_ZSt30is_trivially_copy_assignable_vIN3tsl14AllocatorStatsEE
-_ZSt30is_trivially_move_assignable_vIN3tsl14AllocatorStatsEE
-_ZSt9is_same_vIN3tsl14AllocatorStatsESt9nullopt_tE
-_ZSt9is_same_vIN3tsl14AllocatorStatsESt10in_place_tE
-_ZSt14is_reference_vIN3tsl14AllocatorStatsEE
-_ZSt18is_constructible_vIN3tsl14AllocatorStatsEJEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameISt8optionalIN3tsl14AllocatorStatsEESt9nullopt_tEES0_IS1_ISt10in_place_tS6_EESt16is_constructibleIS4_JRKS6_EESt14is_convertibleISE_S4_EEE
-_ZSt9is_same_vINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESt4pairIKS5_bEE
-_ZSt9is_same_vIiSt4pairIKiN6google8protobuf8internal12ExtensionSet9ExtensionEEE
-_ZSt9is_same_vIN3tsl6StatusES1_E
-_ZSt9is_same_vIiSt4pairIKiSt8functionIFvvEEEE
-_ZSt9is_same_vIPKN6google8protobuf15FieldDescriptorESt4pairIKS4_St10unique_ptrIKNS1_10TextFormat21FastFieldValuePrinterESt14default_deleteISA_EEEE
-_ZSt9is_same_vIPKN6google8protobuf10DescriptorESt4pairIKS4_St10unique_ptrIKNS1_10TextFormat14MessagePrinterESt14default_deleteISA_EEEE
-_ZSt9is_same_vIPKN6google8protobuf15FieldDescriptorESt4pairIKS4_St6vectorINS1_10TextFormat18ParseLocationRangeESaIS9_EEEE
-_ZSt9is_same_vIPKN6google8protobuf15FieldDescriptorESt4pairIKS4_St6vectorISt10unique_ptrINS1_10TextFormat13ParseInfoTreeESt14default_deleteISA_EESaISD_EEEE
-_ZSt9is_same_vIPKN6google8protobuf15FieldDescriptorESt4pairIKS4_NS1_4util21SimpleFieldComparator9ToleranceEEE
-_ZSt9is_same_vIPKN6google8protobuf15FieldDescriptorESt4pairIKS4_NS1_4util18MessageDifferencer23RepeatedFieldComparisonEEE
-_ZSt9is_same_vIPKN6google8protobuf15FieldDescriptorESt4pairIKS4_PKNS1_4util18MessageDifferencer16MapKeyComparatorEEE
-_ZSt9is_same_vIPKN6google8protobuf15FieldDescriptorES4_E
-_ZSt33is_trivially_copy_constructible_vIN10tensorflow17ManagedStackTraceEE
-_ZSt33is_trivially_move_constructible_vIN10tensorflow17ManagedStackTraceEE
-_ZSt23is_copy_constructible_vIN10tensorflow17ManagedStackTraceEE
-_ZSt7__and_vIJSt21is_copy_constructibleIN10tensorflow17ManagedStackTraceEESt18is_copy_assignableIS2_EEE
-_ZSt23is_move_constructible_vIN10tensorflow17ManagedStackTraceEE
-_ZSt7__and_vIJSt21is_move_constructibleIN10tensorflow17ManagedStackTraceEESt18is_move_assignableIS2_EEE
-_ZSt27is_trivially_destructible_vIN10tensorflow17ManagedStackTraceEE
-_ZSt30is_trivially_copy_assignable_vIN10tensorflow17ManagedStackTraceEE
-_ZSt30is_trivially_move_assignable_vIN10tensorflow17ManagedStackTraceEE
-_ZSt9is_same_vIN10tensorflow17ManagedStackTraceESt9nullopt_tE
-_ZSt9is_same_vIN10tensorflow17ManagedStackTraceESt10in_place_tE
-_ZSt14is_reference_vIN10tensorflow17ManagedStackTraceEE
-_ZSt18is_constructible_vIN10tensorflow17ManagedStackTraceEJEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameIN10tensorflow17ManagedStackTraceES3_EESt16is_constructibleIS3_JRKS3_EESt13is_assignableIRS3_S3_ES0_ISt5__or_IJS6_IS3_JRKSt8optionalIS3_EEES6_IS3_JRSF_EES6_IS3_JOSG_EES6_IS3_JOSF_EESt14is_convertibleISH_S3_ESP_ISJ_S3_ESP_ISL_S3_ESP_ISN_S3_EEEES0_ISD_IJSA_ISB_SH_ESA_ISB_SJ_ESA_ISB_SL_ESA_ISB_SN_EEEEEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameISt8optionalIN10tensorflow17ManagedStackTraceEES5_EES0_ISt6__and_IJSt9is_scalarIS4_ES1_IS4_S5_EEEESt16is_constructibleIS4_JRKS5_EESt13is_assignableIRS4_SG_EEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameISt8optionalIN10tensorflow17ManagedStackTraceEES5_EES0_IS1_ISt10in_place_tS5_EESt16is_constructibleIS4_JRKS5_EESt14is_convertibleISD_S4_EEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameISt8optionalIN10tensorflow17ManagedStackTraceEES5_EES0_IS1_ISt10in_place_tS5_EESt16is_constructibleIS4_JRKS5_EES0_ISt14is_convertibleISD_S4_EEEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameIN10tensorflow17ManagedStackTraceES3_EESt16is_constructibleIS3_JRKS3_EESt14is_convertibleIS8_S3_ES0_ISt5__or_IJS6_IS3_JRKSt8optionalIS3_EEES6_IS3_JRSE_EES6_IS3_JOSF_EES6_IS3_JOSE_EESA_ISG_S3_ESA_ISI_S3_ESA_ISK_S3_ESA_ISM_S3_EEEEEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameIN10tensorflow17ManagedStackTraceES3_EESt16is_constructibleIS3_JRKS3_EES0_ISt14is_convertibleIS8_S3_EES0_ISt5__or_IJS6_IS3_JRKSt8optionalIS3_EEES6_IS3_JRSF_EES6_IS3_JOSG_EES6_IS3_JOSF_EESA_ISH_S3_ESA_ISJ_S3_ESA_ISL_S3_ESA_ISN_S3_EEEEEE
-_ZSt7__and_vIJSt16is_constructibleIN10tensorflow17ManagedStackTraceEJEEEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameISt8optionalIlES3_EES0_IS1_ISt10in_place_tS3_EESt16is_constructibleIlJRS3_EESt14is_convertibleISA_lEEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameISt8optionalIlES3_EES0_IS1_ISt10in_place_tS3_EESt16is_constructibleIlJRS3_EES0_ISt14is_convertibleISA_lEEEE
-_ZSt9is_same_vISt17reference_wrapperIKN6google8protobuf6MapKeyEESt4pairIKS5_PvEE
-_ZSt9is_same_vISt17reference_wrapperIKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEEESt4pairIKS8_PvEE
-_ZSt9is_same_vIjSt4pairIKjPvEE
-_ZSt9is_same_vIiSt4pairIKiPvEE
-_ZSt33is_trivially_copy_constructible_vIN4absl12lts_202206234TimeEE
-_ZSt33is_trivially_move_constructible_vIN4absl12lts_202206234TimeEE
-_ZSt23is_copy_constructible_vIN4absl12lts_202206234TimeEE
-_ZSt7__and_vIJSt21is_copy_constructibleIN4absl12lts_202206234TimeEESt18is_copy_assignableIS3_EEE
-_ZSt23is_move_constructible_vIN4absl12lts_202206234TimeEE
-_ZSt7__and_vIJSt21is_move_constructibleIN4absl12lts_202206234TimeEESt18is_move_assignableIS3_EEE
-_ZSt27is_trivially_destructible_vIN4absl12lts_202206234TimeEE
-_ZSt30is_trivially_copy_assignable_vIN4absl12lts_202206234TimeEE
-_ZSt30is_trivially_move_assignable_vIN4absl12lts_202206234TimeEE
-_ZSt9is_same_vIN4absl12lts_202206234TimeESt9nullopt_tE
-_ZSt9is_same_vIN4absl12lts_202206234TimeESt10in_place_tE
-_ZSt14is_reference_vIN4absl12lts_202206234TimeEE
-_ZSt18is_constructible_vIN4absl12lts_202206234TimeEJEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameISt8optionalIN4absl12lts_202206234TimeEES6_EES0_IS1_ISt10in_place_tS6_EESt16is_constructibleIS5_JRS6_EESt14is_convertibleISD_S5_EEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameIN4absl12lts_202206234TimeES4_EESt16is_constructibleIS4_JRKS4_EESt14is_convertibleIS9_S4_ES0_ISt5__or_IJS7_IS4_JRKSt8optionalIS4_EEES7_IS4_JRSF_EES7_IS4_JOSG_EES7_IS4_JOSF_EESB_ISH_S4_ESB_ISJ_S4_ESB_ISL_S4_ESB_ISN_S4_EEEEEE
-_ZSt7__and_vIJSt6__not_ISt7is_sameIN4absl12lts_202206234TimeES4_EESt16is_constructibleIS4_JOS4_EESt14is_convertibleIS8_S4_ES0_ISt5__or_IJS7_IS4_JRKSt8optionalIS4_EEES7_IS4_JRSE_EES7_IS4_JOSF_EES7_IS4_JOSE_EESA_ISG_S4_ESA_ISI_S4_ESA_ISK_S4_ESA_ISM_S4_EEEEEE
-_ZSt12is_base_of_vIN3tsl15float8_internal11float8_baseINS1_13float8_e4m3fnEEES3_E
-_ZSt12is_base_of_vIN3tsl15float8_internal11float8_baseIdEEdE
-_ZSt12is_base_of_vIN3tsl15float8_internal11float8_baseIfEEfE
-_ZSt12is_base_of_vIN3tsl15float8_internal11float8_baseIN5Eigen8bfloat16EEES4_E
-_ZSt12is_base_of_vIN3tsl15float8_internal11float8_baseIN5Eigen4halfEEES4_E
-_ZSt12is_base_of_vIN3tsl15float8_internal11float8_baseINS1_11float8_e5m2EEES3_E
-_ZSt18is_constructible_vISt17basic_string_viewIcSt11char_traitsIcEEJOS3_EE
-_ZN5Eigen8internalL16is_int_or_enum_vIiEE
-_ZN5Eigen8internalL16is_int_or_enum_vImEE
-_ZSt14is_invocable_vIRKSt4lessIiEJRKiS5_EE
-_ZSt14is_invocable_vIRKSt4lessIPKN6google8protobuf15FieldDescriptorEEJRKS5_SA_EE
-_ZSt22is_nothrow_invocable_vIPFvSt17basic_string_viewIcSt11char_traitsIcEEEJRS3_EE
-_ZSt22is_nothrow_invocable_vIRKZNK4absl12lts_202206234Cord14HashFragmentedINS1_13hash_internal15MixingHashStateEEET_S6_EUlSt17basic_string_viewIcSt11char_traitsIcEEE_JSA_EE
-_GLOBAL__sub_I_tmpxft_00000246_00000000_6_nearest_neighbours_kernel.cudafe1.cpp
-__FRAME_END__
-__TMC_END__
-_GLOBAL_OFFSET_TABLE_
-_DYNAMIC
-__clang_call_terminate
-__GNU_EH_FRAME_HDR
-__dso_handle
-DW.ref.__gxx_personality_v0
-_ZN10tensorflow5OpDefD1Ev
-_ZN5Eigen15PlainObjectBaseINS_6MatrixIfLin1ELi1ELi0ELin1ELi1EEEEC2INS_5BlockIKNS_3MapIKNS1_IfLin1ELin1ELi1ELin1ELin1EEELi0ENS_6StrideILi0ELi0EEEEELi1ELin1ELb1EEEEERKNS_9DenseBaseIT_EE
-_ZNK10tensorflow15TensorShapeBaseINS_11TensorShapeEE8dim_sizeEi
-_ZN4dim3C1Ejjj
-_ZSt19__throw_logic_errorPKc@@GLIBCXX_3.4
-__cxa_begin_catch@@CXXABI_1.3
-memcpy@@GLIBC_2.14
-_ZN5Eigen8symbolic9ValueExprINS_8internal8FixedIntILi1EEEEC1Ev
-_ZNSt9bad_allocD1Ev@@GLIBCXX_3.4
-_ZStlsIN3tsl8internal15LogMessageFatalENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEEENSt9enable_ifIXsr6__and_ISt6__not_ISt19is_lvalue_referenceIT_EESt33__is_convertible_to_basic_ostreamISC_ESt15__is_insertableINSG_14__ostream_typeERKT0_vEEE5valueESI_E4typeEOSC_SL_
-_ITM_deregisterTMCloneTable
-_ZN10tensorflow22CheckNotInComputeAsyncEPNS_15OpKernelContextEPKc
-_Znwm@@GLIBCXX_3.4
-memmove@@GLIBC_2.2.5
-_ZN10tensorflow11register_op19OpDefBuilderWrapperclEv
-__assert_fail@@GLIBC_2.2.5
-free@@GLIBC_2.2.5
-_ZNK10tensorflow8OpKernel11TraceStringB5cxx11ERKNS_15OpKernelContextEb
-_ZN3tsl8internal15LogMessageFatalC1EPKci
-__cxa_finalize@@GLIBC_2.2.5
-_ZNK10tensorflow15OpKernelContext12eigen_deviceIN5Eigen16ThreadPoolDeviceEEERKT_v
-_ZN10tensorflow15OpKernelContext21CtxFailureWithWarningEPKciRKN3tsl6StatusE
-_ZN10tensorflow7functor19NearestNeighboursOpIN5Eigen16ThreadPoolDeviceEfE7ComputeEPNS_15OpKernelContextE
-__cudaPushCallConfiguration
-_ZN3tsl8internal21CheckOpMessageBuilder9NewStringB5cxx11Ev
-_ZN10tensorflow12OpDefBuilder10SetShapeFnESt8functionIFN3tsl6StatusEPNS_15shape_inference16InferenceContextEEE
-_ZN5Eigen8internal5all_tC2Ev
-_ZN10tensorflow12OpDefBuilder5InputENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
-__cudaUnregisterFatBinary
-_ZN10tensorflow7functor88_GLOBAL__N__60_tmpxft_00000246_00000000_7_nearest_neighbours_kernel_cpp1_ii_c3e05665_59013index_2d_flatEiii
-__cudaInitModule
-__cudaRegisterFatBinary
-__stack_chk_fail@@GLIBC_2.4
-_ZN10tensorflow7functor27NearestNeighboursCudaKernelIdEEvPKT_S4_PS2_iii
-memset@@GLIBC_2.2.5
-_ZTSN10tensorflow7functor19NearestNeighboursOpIN5Eigen16ThreadPoolDeviceEfEE
-_ZNSolsEi@@GLIBCXX_3.4
-_ZN10tensorflow7functor88_GLOBAL__N__60_tmpxft_00000246_00000000_7_nearest_neighbours_kernel_cpp1_ii_c3e05665_59013index_3d_flatEiiiii
-_ZN5Eigen8symbolic10SymbolExprINS_8internal17symbolic_last_tagEEC2Ev
-_ZTVN10__cxxabiv117__class_type_infoE@@CXXABI_1.3
-_ZN5Eigen8symbolic9ValueExprINS_8internal8FixedIntILi1EEEEC2Ev
-_ZN10tensorflow7functor24NearestNeighboursFunctorIN5Eigen9GpuDeviceEfEclERKS3_NS0_10paramsTypeEPKfS9_Pf
-_ZN3tsl8internal21CheckOpMessageBuilderD1Ev
-__cxa_allocate_exception@@CXXABI_1.3
-__gmon_start__
-strlen@@GLIBC_2.2.5
-_ZTVSt9bad_alloc@@GLIBCXX_3.4
-_ZN10tensorflow7functor19NearestNeighboursOpIN5Eigen16ThreadPoolDeviceEfED0Ev
-_ZTIN10tensorflow7functor19NearestNeighboursOpIN5Eigen9GpuDeviceEfEE
-_ZN5Eigen8symbolic7AddExprINS0_10SymbolExprINS_8internal17symbolic_last_tagEEENS0_9ValueExprINS3_8FixedIntILi1EEEEEEC1ERKS5_RKS9_
-_ZN10tensorflow7functor24NearestNeighboursFunctorIN5Eigen9GpuDeviceEdEclERKS3_NS0_10paramsTypeEPKdS9_Pd
-_ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm
-_ZN3tsl6StatusD1Ev
-_ZN5Eigen8symbolic7AddExprINS0_10SymbolExprINS_8internal17symbolic_last_tagEEENS0_9ValueExprINS3_8FixedIntILi1EEEEEEC2ERKS5_RKS9_
-_ZN10tensorflow7functor19NearestNeighboursOpIN5Eigen9GpuDeviceEfED0Ev
-_ZN5Eigen15PlainObjectBaseINS_6MatrixIfLin1ELin1ELi1ELin1ELin1EEEEC2INS_3MapIKS2_Li0ENS_6StrideILi0ELi0EEEEEEERKNS_9DenseBaseIT_EE
-_ZdlPv@@GLIBCXX_3.4
-_ZN10tensorflow14kernel_factory17OpKernelRegistrar12InitInternalEPKNS_9KernelDefESt17basic_string_viewIcSt11char_traitsIcEESt10unique_ptrINS0_15OpKernelFactoryESt14default_deleteISA_EE
-_ZTISt9bad_alloc@@GLIBCXX_3.4
-_ZN10tensorflow16KernelDefBuilderD2Ev
-_ZStlsISt11char_traitsIcEERSt13basic_ostreamIcT_ES5_PKc@@GLIBCXX_3.4
-__gxx_personality_v0@@CXXABI_1.3
-_ZN10tensorflow16KernelDefBuilder5BuildEv
-_ZNK5Eigen8symbolic8BaseExprINS0_10SymbolExprINS_8internal17symbolic_last_tagEEEE7derivedEv
-_ZN10tensorflow15register_kernel4NameC1EPKc
-_ZSt20__throw_length_errorPKc@@GLIBCXX_3.4
-_ZN10tensorflow11register_op19OpDefBuilderWrapper5InputEPKc
-__cxa_throw@@CXXABI_1.3
-_ZN10tensorflow15shape_inference16InferenceContext3DimENS0_11ShapeHandleEl
-_ZNK5Eigen8internal8FixedIntILi1EEclEv
-_ZN5Eigen15PlainObjectBaseINS_6MatrixIfLin1ELi1ELi0ELin1ELi1EEEE6resizeEll
-_ZTIN10tensorflow8OpKernelE
-_Unwind_Resume@@GCC_3.0
-_ZN10tensorflow12OpDefBuilderC1ENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
-_ZNSt8ios_base4InitD1Ev@@GLIBCXX_3.4
-_ZNK10tensorflow15OpKernelContext12eigen_deviceIN5Eigen9GpuDeviceEEERKT_v
-_ZN10tensorflow7functor27NearestNeighboursCudaKernelIfEEvPKT_S4_PS2_iii
-_ZN3tsl8internal21CheckOpMessageBuilder7ForVar2Ev
-_ZN10tensorflow7functor19NearestNeighboursOpIN5Eigen9GpuDeviceEfE7ComputeEPNS_15OpKernelContextE
-_ZTVN10tensorflow7functor19NearestNeighboursOpIN5Eigen9GpuDeviceEfEE
-_ZN4dim3C2Ejjj
-_ZN10tensorflow15OpKernelContext5inputESt17basic_string_viewIcSt11char_traitsIcEEPPKNS_6TensorE
-__cudaRegisterFatBinaryEnd
-__cudaPopCallConfiguration
-_ZN3tsl8internal17MakeCheckOpStringIiiEEPNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERKT_RKT0_PKc
-_ZN5Eigen8internal5all_tC1Ev
-_ZN10tensorflow15TensorShapeBaseINS_18PartialTensorShapeEE10kIsPartialE
-_ZSt24__throw_out_of_range_fmtPKcz
-_ZTVN10__cxxabiv120__si_class_type_infoE@@CXXABI_1.3
-_ZN5Eigen15PlainObjectBaseINS_6MatrixIfLin1ELin1ELi1ELin1ELin1EEEE6resizeEll
-_ZN3tsl8internal15LogMessageFatalD1Ev
-_ZN10tensorflow8OpKernel11IsExpensiveEv
-__cxa_atexit@@GLIBC_2.2.5
-_ZN10tensorflow8OpKernel7AsAsyncEv
-_ZN10tensorflow11register_op19OpDefBuilderWrapperC2EPKc
-malloc@@GLIBC_2.2.5
-_ZN10tensorflow16KernelDefBuilder6DeviceEPKc
-_ZN3tsl8OkStatusEv
-cudaLaunchKernel
-_ZNK5Eigen8symbolic8BaseExprINS0_10SymbolExprINS_8internal17symbolic_last_tagEEEEplILi1EEENS0_7AddExprIS5_NS0_9ValueExprINS3_8FixedIntIXT_EEEEEEESB_
-_ZSt16__ostream_insertIcSt11char_traitsIcEERSt13basic_ostreamIT_T0_ES6_PKS3_l@@GLIBCXX_3.4.9
-_ZN10tensorflow12OpDefBuilder6OutputENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
-_ZNSt8ios_base4InitC1Ev@@GLIBCXX_3.4
-_ITM_registerTMCloneTable
-_ZN10tensorflow15shape_inference16InferenceContext8WithRankENS0_11ShapeHandleElPS2_
-_ZNK10tensorflow8OpKernel12const_tensorEv
-_ZN10tensorflow15shape_inference16InferenceContext12DimKnownRankENS0_11ShapeHandleEl
-_ZN3tsl8internal21CheckOpMessageBuilderC1EPKc
-_ZN10tensorflow15OpKernelContext15allocate_outputEiRKNS_11TensorShapeEPPNS_6TensorE
-_ZN10tensorflow8OpKernelC2EPNS_20OpKernelConstructionE
-_ZTVN10tensorflow14kernel_factory17OpKernelRegistrar18PtrOpKernelFactoryE
-_ZN10tensorflow8OpKernelD2Ev
-__cudaRegisterFunction
-_ZSt9terminatev@@GLIBCXX_3.4
-_ZN10tensorflow15TensorShapeBaseINS_11TensorShapeEE10kIsPartialE
-_ZN10tensorflow11register_op19OpDefBuilderWrapper6OutputEPKc
-_ZN5Eigen8symbolic10SymbolExprINS_8internal17symbolic_last_tagEEC1Ev
-_ZNK10tensorflow6Tensor21CheckTypeAndIsAlignedENS_8DataTypeE
-_ZN10tensorflow15shape_inference16InferenceContext9MakeShapeESt16initializer_listINS0_19DimensionOrConstantEE
-_ZTVN10tensorflow7functor19NearestNeighboursOpIN5Eigen16ThreadPoolDeviceEfEE
-_ZN10tensorflow7functor24NearestNeighboursFunctorIN5Eigen16ThreadPoolDeviceEfEclERKS3_NS0_10paramsTypeEPKfS9_Pf
-_ZTSN10tensorflow7functor19NearestNeighboursOpIN5Eigen9GpuDeviceEfEE
-_ZTIN10tensorflow7functor19NearestNeighboursOpIN5Eigen16ThreadPoolDeviceEfEE
-_ZN10tensorflow14kernel_factory17OpKernelRegistrarC2EPKNS_9KernelDefESt17basic_string_viewIcSt11char_traitsIcEEPFPNS_8OpKernelEPNS_20OpKernelConstructionEE
-_ZN10tensorflow12OpDefBuilderD2Ev
-.shstrtab
-.note.gnu.build-id
-.gnu.hash
-.gnu.version
-.gnu.version_r
-.rela.dyn
-.rela.plt
-.plt.got
-__nv_module_id
-.nv_fatbin
-.eh_frame_hdr
-.eh_frame
-.gcc_except_table
-.init_array
-.fini_array
-.data.rel.ro
-.dynamic
-.got.plt
-.nvFatBinSegment
-.comment
+GCC_except_table13
+GCC_except_table14
+GCC_except_table17
+GCC_except_table18
+GCC_except_table19
+GCC_except_table20
+GCC_except_table12
+GCC_except_table22
+__ZTSNSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEEE
+__ZTSNSt3__110__function6__baseIFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEEE
+__ZTS3$_0
+__ZTSNSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEEE
+__ZTS3$_1
+__ZTSN10tensorflow7functor19NearestNeighboursOpIN5Eigen16ThreadPoolDeviceEfEE
+__ZTSN10tensorflow7functor26NearestNeighboursIndexesOpIN5Eigen16ThreadPoolDeviceEfEE
+__ZTVNSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEEE
+__ZTINSt3__110__function6__baseIFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEEE
+__ZTINSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEEE
+__ZTI3$_0
+__ZTVNSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEEE
+__ZTINSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN3tsl6StatusEPN10tensorflow15shape_inference16InferenceContextEEEE
+__ZTI3$_1
+__ZTVN10tensorflow7functor19NearestNeighboursOpIN5Eigen16ThreadPoolDeviceEfEE
+__ZTIN10tensorflow7functor19NearestNeighboursOpIN5Eigen16ThreadPoolDeviceEfEE
+__ZTVN10tensorflow7functor26NearestNeighboursIndexesOpIN5Eigen16ThreadPoolDeviceEfEE
+__ZTIN10tensorflow7functor26NearestNeighboursIndexesOpIN5Eigen16ThreadPoolDeviceEfEE
+___block_descriptor_80_e8_32o_e5_v8
+__dyld_private
+__MergedGlobals
+_nearest_neighbours_op.so
```

## tensorflow_nearest_neighbours/python/__init__.py

```diff
@@ -1,4 +0,0 @@
-00000000: 6672 6f6d 202e 6e65 6172 6573 745f 6e65  from .nearest_ne
-00000010: 6967 6862 6f75 7273 2069 6d70 6f72 7420  ighbours import 
-00000020: 6e65 6172 6573 745f 6e65 6967 6862 6f75  nearest_neighbou
-00000030: 7273 0a                                  rs.
```

## tensorflow_nearest_neighbours/python/nearest_neighbours.py

```diff
@@ -1,55 +1,90 @@
 from __future__ import annotations
 
+from typing import Tuple
 import tensorflow as tf
 from tensorflow.python.framework import load_library
 from tensorflow.python.platform import resource_loader
 from tensorflow.python.types.core import TensorLike
 
 _backend = load_library.load_op_library(
     resource_loader.get_path_to_datafile("../_nearest_neighbours_op.so")
 )
 
-__all__ = ["nearest_neighbours"]
+__all__ = ["nearest_neighbours", "nearest_neighbours_indexes"]
 
 
 def nearest_neighbours(
     token_embeddings: tf.Tensor, embedding_matrix: tf.Tensor
 ) -> tf.Tensor:
     """
     Take batch of token embeddings, and compute nearest neighbours for each token in Embedding Matrix's space.
     The underlying C++ function expects float32 precision.
+    Args:
+        token_embeddings:
+            A batch of token embeddings with shape [batch_size, None, embedding_dimension].
+        embedding_matrix:
+            Embedding matrix of Language Model with shape [vocab_size, embedding_dimension].
 
-    :param token_embeddings: A batch of token embeddings with shape [batch_size, None, embedding_dimension].
-    :param embedding_matrix: Embedding matrix of Language Model with shape [vocab_size, embedding_dimension].
-    :return: token_embeddings, shape = [batch_size, None, embedding_dimension], dtype=tf.float32.
+    Returns:
+        token_embeddings, shape = [batch_size, None, embedding_dimension], dtype=tf.float32.
     """
-    with tf.name_scope("nearest_neighbours"):
-        token_embeddings = as_tensor(token_embeddings)
-        embedding_matrix = as_tensor(embedding_matrix)
-        assert_float32_precision(token_embeddings)
-        assert_float32_precision(embedding_matrix)
-
-        em_rank = tf.rank(embedding_matrix)
-        if em_rank != 2:
-            raise ValueError(f"embedding_matrix must have rank 2, but found {em_rank}")
-
-        og_rank = tf.rank(token_embeddings)
-        if og_rank > 3:
-            raise ValueError(
-                f"token_embeddings can have rank <= 3, but found: {og_rank}"
-            )
-
+    with tf.name_scope("NearestNeighbours"):
+        input_rank, token_embeddings, embedding_matrix = pre_process(token_embeddings, embedding_matrix)
         result = _backend.nearest_neighbours(token_embeddings, embedding_matrix)
-        if og_rank == 3:
-            return result
-        if og_rank == 2:
-            return result[0]
-        if og_rank == 1:
-            return result[0, 0]
+        return post_process(input_rank, result)
+
+
+def nearest_neighbours_indexes(
+    token_embeddings: tf.Tensor, embedding_matrix: tf.Tensor
+) -> tf.Tensor:
+    """
+    Take batch of token embeddings, and find index nearest neighbours for each token in Embedding Matrix's space.
+    The underlying C++ function expects float32 precision.
+    Args:
+        token_embeddings:
+            A batch of token embeddings with shape [batch_size, None, embedding_dimension].
+        embedding_matrix:
+            Embedding matrix of Language Model with shape [vocab_size, embedding_dimension].
+
+    Returns:
+        indexes, shape = [batch_size, None], dtype=tf.int32.
+    """
+    with tf.name_scope("NearestNeighboursIndexes"):
+        input_rank, token_embeddings, embedding_matrix = pre_process(token_embeddings, embedding_matrix)
+        result = _backend.nearest_neighbours_indexes(token_embeddings, embedding_matrix)
+        return post_process(input_rank, result)
+
+
+def pre_process(token_embeddings: tf.Tensor, embedding_matrix: tf.Tensor) -> Tuple[int, tf.Tensor, tf.Tensor]:
+    token_embeddings = as_tensor(token_embeddings)
+    embedding_matrix = as_tensor(embedding_matrix)
+    assert_float32_precision(token_embeddings)
+    assert_float32_precision(embedding_matrix)
+
+    em_rank = tf.rank(embedding_matrix)
+    if em_rank != 2:
+        raise ValueError(f"embedding_matrix must have rank 2, but found {em_rank}")
+
+    input_rank = tf.rank(token_embeddings)
+    if input_rank > 3:
+        raise ValueError(
+            f"token_embeddings can have rank <= 3, but found: {input_rank}"
+        )
+
+    return input_rank, token_embeddings, embedding_matrix
+
+
+def post_process(input_rank: int, result: tf.Tensor) -> tf.Tensor:
+    if input_rank == 3:
+        return result
+    if input_rank == 2:
+        return result[0]
+    if input_rank == 1:
+        return result[0, 0]
 
 
 def as_tensor(x: TensorLike) -> tf.Tensor:
     if isinstance(x, tf.Tensor):
         return x
     else:
         return tf.constant(x)
```

## test/nearest_neighbours_test.py

```diff
@@ -1,89 +1,126 @@
 from __future__ import annotations
 
 import tensorflow as tf
 from tensorflow.python.framework import test_util
 from tensorflow.python.platform import test
 
-from tensorflow_nearest_neighbours import nearest_neighbours
+from tensorflow_nearest_neighbours import nearest_neighbours, nearest_neighbours_indexes
 
 
-@tf.function(reduce_retracing=True)
-def py_nearest_neighbour_single_point(
-    token_embedding: tf.Tensor, embedding_matrix: tf.Tensor
-) -> tf.Tensor:
-    dist = tf.linalg.norm(embedding_matrix - token_embedding, axis=-1)
-    index = tf.argmin(dist)
-    return tf.gather(embedding_matrix, index, axis=0)
-
-
-def py_nearest_neighbours(
-    token_embeddings: tf.Tensor, embedding_matrix: tf.Tensor
-) -> tf.Tensor:
-    return tf.stack(
-        [
-            py_nearest_neighbour_single_point(i, embedding_matrix)
-            for i in token_embeddings
-        ]
-    )
-
-
-def py_nearest_neighbours_batch(
-    token_embeddings_batch: tf.Tensor, embedding_matrix: tf.Tensor
-) -> tf.Tensor:
-    return tf.stack(
-        [py_nearest_neighbours(i, embedding_matrix) for i in token_embeddings_batch]
-    )
+def py_nearest_neighbours(embeddings_batch, embedding_matrix):
+    def token_fn(token_embedding):
+        dist = tf.linalg.norm(embedding_matrix - token_embedding, axis=-1)
+        index = tf.argmin(dist)
+        return tf.gather(embedding_matrix, index, axis=0)
 
+    def sequence_fn(sentence_embeddings: tf.Tensor):
+        return tf.map_fn(token_fn, sentence_embeddings)
 
-class TestOP(test.TestCase):
+    return tf.map_fn(sequence_fn, embeddings_batch)
+
+
+def py_nearest_neighbours_indexes(embeddings_batch, embedding_matrix):
+    def token_fn(token_embedding):
+        dist = tf.linalg.norm(embedding_matrix - token_embedding, axis=-1)
+        index = tf.argmin(dist)
+        return tf.cast(index, dtype=tf.float32)
+
+    def sequence_fn(sentence_embeddings: tf.Tensor):
+        return tf.map_fn(token_fn, sentence_embeddings)
+
+    return tf.cast(tf.map_fn(sequence_fn, embeddings_batch), dtype=tf.int32)
+
+
+class TestNearestNeighbours(test.TestCase):
     def testNoNoiseAdded(self):
         with self.session():
             em = tf.random.uniform(shape=[50, 32])
             x = tf.convert_to_tensor([[em[0], em[0], em[0]], [em[0], em[0], em[0]]])
             expected = x
             result = nearest_neighbours(x, em)
 
-        self.assertAllClose(result, expected)
+        self.assertAllClose(expected, result)
 
     def testSmallEM(self):
         with self.session():
             with test_util.device(False):
                 em = tf.random.uniform(shape=[50, 32])
                 x = tf.random.uniform(shape=[8, 10, 32])
                 result = nearest_neighbours(x, em)
-                expected = py_nearest_neighbours_batch(x, em)
+                expected = py_nearest_neighbours(x, em)
 
-        self.assertAllClose(result, expected)
+        self.assertAllClose(expected, result)
 
     def testBigEM(self):
         with self.session():
             em = tf.random.uniform(shape=[15000, 512])
             x = tf.random.uniform(shape=[8, 10, 512])
             result = nearest_neighbours(x, em)
-            expected = py_nearest_neighbours_batch(x, em)
+            expected = py_nearest_neighbours(x, em)
 
-        self.assertAllClose(result, expected)
+        self.assertAllClose(expected, result)
 
     def testBigBatch(self):
         with self.session():
             em = tf.random.uniform(shape=[1500, 512])
             x = tf.random.uniform(shape=[32, 65, 512])
             result = nearest_neighbours(x, em)
-            expected = py_nearest_neighbours_batch(x, em)
+            expected = py_nearest_neighbours(x, em)
 
-        self.assertAllClose(result, expected)
+        self.assertAllClose(expected, result)
 
     @test_util.run_gpu_only
     def test_on_gpu(self):
         with self.session():
             with test_util.force_gpu():
                 em = tf.random.uniform(shape=[50, 32])
                 x = tf.random.uniform(shape=[8, 10, 32])
                 result = nearest_neighbours(x, em)
-                expected = py_nearest_neighbours_batch(x, em)
+                expected = py_nearest_neighbours(x, em)
+
+        self.assertAllClose(expected, result)
+
+
+class TestNearestNeighboursIndexes(test.TestCase):
+    def testSmallEM(self):
+        with self.session():
+            with test_util.device(False):
+                em = tf.random.uniform(shape=[50, 32])
+                x = tf.random.uniform(shape=[8, 10, 32])
+                result = nearest_neighbours_indexes(x, em)
+                expected = py_nearest_neighbours_indexes(x, em)
+
+        self.assertAllEqual(expected, result)
+
+    def testBigEM(self):
+        with self.session():
+            em = tf.random.uniform(shape=[15000, 512])
+            x = tf.random.uniform(shape=[8, 10, 512])
+            result = nearest_neighbours_indexes(x, em)
+            expected = py_nearest_neighbours_indexes(x, em)
+
+        self.assertAllEqual(expected, result)
+
+    def testBigBatch(self):
+        with self.session():
+            em = tf.random.uniform(shape=[1500, 512])
+            x = tf.random.uniform(shape=[32, 65, 512])
+            result = nearest_neighbours_indexes(x, em)
+            expected = py_nearest_neighbours_indexes(x, em)
+
+        self.assertAllEqual(expected, result)
+
+    @test_util.run_gpu_only
+    def test_on_gpu(self):
+        with self.session():
+            with test_util.force_gpu():
+                em = tf.random.uniform(shape=[50, 32])
+                x = tf.random.uniform(shape=[8, 10, 32])
+                result = nearest_neighbours_indexes(x, em)
+                expected = py_nearest_neighbours_indexes(x, em)
 
-        self.assertAllClose(result, expected)
+        self.assertAllEqual(expected, result)
 
 
 if __name__ == "__main__":
-    test.main()
+    test.main(verbosity=2)
```

## Comparing `tensorflow_nearest_neighbours-0.0.4.dist-info/LICENSE` & `tensorflow_nearest_neighbours-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tensorflow_nearest_neighbours-0.0.4.dist-info/METADATA` & `tensorflow_nearest_neighbours-0.0.5.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorflow-nearest-neighbours
-Version: 0.0.4
+Version: 0.0.5
 Summary: Nearest neighbours word embedding computation.
 Author: Artem Sereda
 Author-email: artem.sereda@campus.tu-berlin.de
 Keywords: tensorflow,custom op
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

