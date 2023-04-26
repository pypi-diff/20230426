# Comparing `tmp/fastkde-1.0.8.tar.gz` & `tmp/fastkde-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fastkde-1.0.8.tar", last modified: Tue Apr 19 23:29:27 2016, max compression
+gzip compressed data, was "dist/fastkde-1.0.9.tar", last modified: Fri Aug  5 01:17:35 2016, max compression
```

## Comparing `fastkde-1.0.8.tar` & `fastkde-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 taobrien   (501) staff       (20)        0 2016-04-19 23:29:27.000000 fastkde-1.0.8/
--rw-r--r--   0 taobrien   (501) staff       (20)     3805 2016-01-11 22:08:49.000000 fastkde-1.0.8/LICENSE.txt
--rw-r--r--   0 taobrien   (501) staff       (20)    11058 2016-04-19 23:29:27.000000 fastkde-1.0.8/PKG-INFO
--rw-r--r--   0 taobrien   (501) staff       (20)     8758 2016-04-19 16:30:38.000000 fastkde-1.0.8/README
--rw-r--r--   0 taobrien   (501) staff       (20)        6 2016-04-19 23:28:14.000000 fastkde-1.0.8/REVISION
--rw-r--r--   0 taobrien   (501) staff       (20)    70947 2016-01-11 22:08:49.000000 fastkde-1.0.8/conditional_demo.png
-drwxr-xr-x   0 taobrien   (501) staff       (20)        0 2016-04-19 23:29:27.000000 fastkde-1.0.8/fastkde/
--rw-r--r--   0 taobrien   (501) staff       (20)        0 2016-01-11 22:08:49.000000 fastkde-1.0.8/fastkde/__init__.py
--rw-r--r--   0 taobrien   (501) staff       (20)     9630 2016-04-19 15:02:23.000000 fastkde-1.0.8/fastkde/empiricalCharacteristicFunction.py
--rw-r--r--   0 taobrien   (501) staff       (20)    54348 2016-04-19 15:02:23.000000 fastkde-1.0.8/fastkde/fastKDE.py
--rw-r--r--   0 taobrien   (501) staff       (20)    11826 2016-01-11 22:08:49.000000 fastkde-1.0.8/fastkde/floodFillSearch.pyx
--rw-r--r--   0 taobrien   (501) staff       (20)    19185 2016-04-19 23:27:05.000000 fastkde-1.0.8/fastkde/nufft.pyx
--rw-r--r--   0 taobrien   (501) staff       (20)       36 2016-04-19 15:43:46.000000 fastkde-1.0.8/requirements.txt
--rw-r--r--   0 taobrien   (501) staff       (20)       37 2016-04-19 16:32:55.000000 fastkde-1.0.8/setup.cfg
--rw-r--r--   0 taobrien   (501) staff       (20)     1670 2016-04-19 16:33:03.000000 fastkde-1.0.8/setup.py
+drwxr-xr-x   0 taobrien   (501) wheel        (0)        0 2016-08-05 01:17:35.000000 fastkde-1.0.9/
+-rw-r--r--   0 taobrien   (501) wheel        (0)    70947 2016-08-05 00:53:11.000000 fastkde-1.0.9/conditional_demo.png
+drwxr-xr-x   0 taobrien   (501) wheel        (0)        0 2016-08-05 01:17:35.000000 fastkde-1.0.9/fastkde/
+-rw-r--r--   0 taobrien   (501) wheel        (0)        0 2016-08-05 01:04:24.000000 fastkde-1.0.9/fastkde/__init__.py
+-rw-r--r--   0 taobrien   (501) wheel        (0)     9630 2016-08-05 01:04:24.000000 fastkde-1.0.9/fastkde/empiricalCharacteristicFunction.py
+-rw-r--r--   0 taobrien   (501) wheel        (0)    55265 2016-08-05 01:07:24.000000 fastkde-1.0.9/fastkde/fastKDE.py
+-rw-r--r--   0 taobrien   (501) wheel        (0)    12133 2016-08-05 01:04:24.000000 fastkde-1.0.9/fastkde/floodFillSearch.pyx
+-rw-r--r--   0 taobrien   (501) wheel        (0)    19185 2016-08-05 01:04:24.000000 fastkde-1.0.9/fastkde/nufft.pyx
+-rw-r--r--   0 taobrien   (501) wheel        (0)     3805 2016-08-05 01:04:24.000000 fastkde-1.0.9/LICENSE.txt
+-rw-r--r--   0 taobrien   (501) wheel        (0)    11058 2016-08-05 01:17:35.000000 fastkde-1.0.9/PKG-INFO
+-rw-r--r--   0 taobrien   (501) wheel        (0)     8758 2016-08-05 01:04:24.000000 fastkde-1.0.9/README
+-rw-r--r--   0 taobrien   (501) wheel        (0)       36 2016-08-05 01:04:24.000000 fastkde-1.0.9/requirements.txt
+-rw-r--r--   0 taobrien   (501) wheel        (0)        6 2016-08-05 01:08:26.000000 fastkde-1.0.9/REVISION
+-rw-r--r--   0 taobrien   (501) wheel        (0)       37 2016-08-05 01:04:24.000000 fastkde-1.0.9/setup.cfg
+-rw-r--r--   0 taobrien   (501) wheel        (0)     1670 2016-08-05 01:04:24.000000 fastkde-1.0.9/setup.py
```

### Comparing `fastkde-1.0.8/LICENSE.txt` & `fastkde-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastkde-1.0.8/PKG-INFO` & `fastkde-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: fastkde
-Version: 1.0.8
+Version: 1.0.9
 Summary: Tools for fast and robust univariate and multivariate kernel density estimation
 Home-page: https://bitbucket.org/lbl-cascade/fastkde
 Author: Travis A. O'Brien
 Author-email: TAOBrien@lbl.gov
 License: UNKNOWN
-Download-URL: https://bitbucket.org/lbl-cascade/fastkde/get/v1.0.8.tar.gz
+Download-URL: https://bitbucket.org/lbl-cascade/fastkde/get/v1.0.9.tar.gz
 Description: fastKDE
         =======
         
         Software Overview
         -----------------
         
         fastKDE calculates a kernel density estimate of arbitrarily dimensioned
```

### Comparing `fastkde-1.0.8/README` & `fastkde-1.0.9/README`

 * *Files identical despite different names*

### Comparing `fastkde-1.0.8/conditional_demo.png` & `fastkde-1.0.9/conditional_demo.png`

 * *Files identical despite different names*

### Comparing `fastkde-1.0.8/fastkde/empiricalCharacteristicFunction.py` & `fastkde-1.0.9/fastkde/empiricalCharacteristicFunction.py`

 * *Files identical despite different names*

### Comparing `fastkde-1.0.8/fastkde/fastKDE.py` & `fastkde-1.0.9/fastkde/fastKDE.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,17 @@
                 ecfPrecision = 1, \
                 doSaveTransformedKernel = False, \
                 doFFT = True, \
                 doSaveMarginals = True, \
                 beVerbose = False, \
                 fracContiguousHyperVolumes = 1, \
                 numContiguousHyperVolumes = None, \
-                positiveShift = False, \
+                positiveShift = True, \
                 countThreshold = None, \
+                axisExpansionFactor = 1.0, \
               ):
     """ 
 
     Estimates the density function of a given dataset using the self-consistent
     method of Bernacchia and Pigolotti (2011, J. R. Statistic Soc. B.).  Prior
     to estimating the PDF, the data are standardized to have a mean of 0 and a
     variance of 1.  
@@ -116,14 +117,19 @@
 
       positiveShift     : translate the PDF vertically such that the estimate is positive or
                           0 everywhere
 
       countThreshold    : this argument does nothing; it has been deprecated.  It is kept as an argument for backward
                           compatibility.
 
+      axisExpansionFactor : sets the amount by which the KDE grid will be expanded relative to the original min-max
+                            spread for each variable: 1.0 means a 100% (2x) expansion in the range.  Such an expansion
+                            is necessary to avoid kernel power from one end of the grid leaking into the opposite end
+                            due to the perioidicity of the Fourier transform.
+
     Returns: a fastKDE object
 
     """
 
     def vprint(msg):
         """Only print if beVerbose is True"""
         if beVerbose:
@@ -227,17 +233,18 @@
         vprint("Data stats:")
         vprint("\tminima: {}".format(self.xMin))
         vprint("\tmaxima: {}".format(self.xMax))
 
         #Get the grid mid-points
         midPoint = 0.5*(self.xMax + self.xMin)
 
-        #inflate the range by 5% to ensure that the data all fit within the range
-        self.xMin += 0.05*(self.xMin-midPoint)
-        self.xMax += 0.05*(self.xMax-midPoint)
+        #inflate the range by axisExpansionFactor to ensure that KDE power doesn't leak through
+        #the periodic axis boundary
+        self.xMin += axisExpansionFactor*(self.xMin-midPoint)
+        self.xMax += axisExpansionFactor*(self.xMax-midPoint)
 
         if numPoints is None:
             #Calculate the number of standard deviations there
             # are in the data range
             dataRange = self.xMax - self.xMin
             numSigma = dataRange/std(data,axis=1)
             
@@ -402,22 +409,27 @@
 
     if contiguousInds == []:
         raise RuntimeError("No ECF values found above the ECF threshold.  max(ecfSq) = {}, ecfThresh = {}".format(amax(ecfSq),ecfThresh))
 
     #Sort them by distance from the center
     sortedInds = flood.sortByDistanceFromCenter(contiguousInds,shape(ecfSq))
 
+    #Convert the fraction of hypervolumes to a number if needbe
     numVolumes = len(sortedInds)
     if self.fracContiguousHyperVolumes >= 1:
         numVolumesToUse = int(self.fracContiguousHyperVolumes)
     else:
         numVolumesToUse = int(self.fracContiguousHyperVolumes*numVolumes)
     if numVolumesToUse < 1:
         numVolumesToUse = 1
 
+    #Check that we don't exceed the number of provided volumes
+    if numVolumesToUse > numVolumes:
+        numVolumesToUse = numVolumes
+
     #Initialize the filtered value list
     iCalcPhi = self.numVariables*[array([],dtype='int')]
 
     #Pull out fracContiguousHyperVolumes of contiguous hyper volumes, in order of distance from
     #the origin
     for i in range(numVolumesToUse):
         for n in range(self.numVariables):
@@ -505,15 +517,17 @@
             #normalized
             try:
                 delta = newton(normFunc,a,maxiter=10000)
             except:
                 delta = 0.0
 
             #Check if the positive shift method failed
-            if not isfinite(delta):
+            if not isfinite(delta) or delta < 0 or delta >= amax(self.pdf):
+                if self.beVerbose:
+                    print 'positiveShift algorithm failure: defaulting to no shift'
                 delta = 0.0
 
             #If a shift is provided, do the shift
             if delta != 0.0:
                 #Shift the PDF
                 self.pdf -= delta
                 #And set the negative values to 0
```

### Comparing `fastkde-1.0.8/fastkde/floodFillSearch.pyx` & `fastkde-1.0.9/fastkde/floodFillSearch.pyx`

 * *Files 12% similar despite different names*

```diff
@@ -1,304 +1,304 @@
-import numpy as np
-cimport numpy as np
-cimport cython
-
-cdef inline int ravel_shift(   tuple indices, \
-                                int arrayRank, \
-                                np.int_t [:] arrayShape, \
-                                int dimension,  \
-                                int amount,     \
-                                int dimensionWraps):
-    """Return the raveled index of a shifted version of indices, where a
-    specific dimension has been shifted by a certain amount.  If wrapping is
-    not flagged and the shift is out of bounds, returns -1"""
-
-
-    cdef int runningProduct
-    cdef int n
-    cdef int i
-    cdef int np
-    cdef int thisIndex
-
-    runningProduct = 1
-    i = 0
-
-    #Loop over dimensions, starting at the rightmost dimension
-    for n in xrange(arrayRank,0,-1):
-        #Calculate the running product of dimension sizes
-        if( n != arrayRank):
-            runningProduct *= arrayShape[n]
-
-        #Set the current index
-        thisIndex = indices[n-1]
-
-        np = n-1
-        if(np == dimension):
-            #If this is the shifting dimension,
-            #increment it
-            thisIndex += amount
-
-            #Check if we need to deal with a
-            #wrap around dimension
-            if(dimensionWraps):
-                if(thisIndex < 0):
-                    thisIndex += arrayShape[np]
-                if(thisIndex >= arrayShape[np]):
-                    thisIndex -= arrayShape[np]
-
-            #Check if the current index is out of bounds;
-            #return -1 if so
-            if(thisIndex < 0 or thisIndex >= arrayShape[np]):
-                i = -1
-                break
-
-        #increment the counter
-        i += runningProduct*thisIndex
-
-    #Check whether the index is within the memory bounds of the array
-    #return the -1 flag if not
-    runningProduct *= arrayShape[0]
-    if(i >= runningProduct or i < 0):
-        i = -1
-
-    return i
-
-@cython.boundscheck(False)
-cdef tuple findNeighbors(   int raveledStartIndex, \
-                            np.float_t searchThreshold, \
-                            np.int_t [:] arrayShape, \
-                            int arrayRank, \
-                            list dimensionWraps, \
-                            np.float_t [:] inputArray, \
-                            np.int_t [:] isNotSearched, \
-                   ):
-    """Does a flood fill algorithim on inputArray in the vicinity of
-    raveledStartIndex to find contiguous areas where raveledStartIndex > searchThreshold 
-    
-        input:
-        ------
-            raveledStartIndex   :   (integer) the index of inputArray.ravel() at which to start
-
-            searchThreshold :   The threshold for defining fill regions
-                                (inputArray > searchThreshold)
-
-        output:
-        -------
-            A list of N-d array indices.
-    
-    """
-
-    
-    cdef list itemsToSearch #Running item search list
-    cdef list contiguousIndices #A list of indices
-    cdef int r #Current array dimension
-    cdef int testIndexLeft # A test index
-    cdef int testIndexRight # A test index
-    cdef tuple contiguousArray #A tuple of contiguous indices
-    cdef np.ndarray contiguousIndexArray #An array of contiguous indices
-    cdef int testInd #The raveled index of the test point
-
-    cdef tuple itemTuple #The tuple index of the current search item
-
-    cdef int shiftAmount
-
-    #Initialize the contiguous index list
-    contiguousIndices = []
-
-    #Initialize the search list
-    itemsToSearch = [raveledStartIndex]
-
-    while itemsToSearch != []:
-
-        #Get the index of the current item
-        itemTuple = np.unravel_index(itemsToSearch[0],arrayShape)
-
-        for r in xrange(arrayRank):
-            #Shift the current coordinate to the right by 1 in the r dimension
-            shiftAmount = 1
-            testIndexRight = ravel_shift( \
-                                        itemTuple, \
-                                        arrayRank, \
-                                        arrayShape, \
-                                        r, \
-                                        shiftAmount,
-                                        dimensionWraps[r])
-
-            #Check that this coordinate is still within bounds
-            if(testIndexRight >= 0):
-                #Check if this index satisfies the search condition
-                if(inputArray[testIndexRight] > searchThreshold and \
-                        isNotSearched[testIndexRight] == 1):
-                    #Append it to the search list if so
-                    itemsToSearch.append(testIndexRight)
-                    #Flags that this cell has been searched
-                    isNotSearched[testIndexRight] = 0
-
-
-            #Shift the current coordinate to the right by 1 in the r dimension
-            shiftAmount = -1
-            testIndexLeft = ravel_shift( \
-                                        itemTuple, \
-                                        arrayRank, \
-                                        arrayShape, \
-                                        r, \
-                                        shiftAmount,
-                                        dimensionWraps[r])
-
-            #Check that this coordinate is still within bounds
-            if(testIndexLeft > 0):
-                #Check if this index satisfies the search condition
-                if(inputArray[testIndexLeft] > searchThreshold and \
-                        isNotSearched[testIndexLeft] == 1 ):
-                    #Append it to the search list if so
-                    itemsToSearch.append(testIndexLeft)
-                    #Flags that this cell has been searched
-                    isNotSearched[testIndexLeft] = 0
-
- 
-
-        #Flag that this index has been searched
-        #isNotSearched[tuple(itemsToSearch[0])] = 0
-        #Now that the neighbors of the first item in the list have been tested,
-        #remove it from the list and put it in the list of contiguous values
-        contiguousIndices.append(itemsToSearch.pop(0))
-
-    #Return the list of contiguous indices (converted to index tuples)
-    return np.unravel_index(contiguousIndices,arrayShape)
-
-cpdef list floodFillSearch( \
-                np.ndarray inputArray, \
-                np.float_t searchThreshold = 0.0, \
-                wrapDimensions = None):
-    """Given an N-dimensional array, find contiguous areas of the array
-    satisfiying a given condition and return a list of contiguous indices
-    for each contiguous area.
-        
-        input:
-        ------
-
-            inputArray      :   (array-like) an array from which to search
-                                contiguous areas
-
-            searchThreshold :   The threshold for defining fill regions
-                                (inputArray > searchThreshold)
-
-            wrapDimensions :    A list of dimensions in which searching
-                                should have a wraparound condition
-
-        output:
-        -------
-
-            An unordered list, where each item corresponds to a unique
-            contiguous area for which inputArray > searchThreshold, and
-            where the contents of each item are a list of array indicies
-            that access the elements of the array for a given contiguous
-            area.
-
-    """
-    cdef np.ndarray[np.int_t,ndim=1] arrayShape
-    cdef int arrayRank
-    cdef int numArrayElements
-    cdef list dimensionWraps
-    cdef list contiguousAreas
-
-    cdef tuple contiguousArray 
-
-    #Determine the rank of inputArray
-    try:
-        arrayShape = np.array(np.shape(inputArray))
-        arrayRank = len(arrayShape)
-        numArrayElements = np.prod(arrayShape)
-    except BaseException as e:
-        raise ValueError,"inputArray does not appear to be array like.  Error was: {}".format(e)
-
-    #Set the dimension wrapping array
-    dimensionWraps = arrayRank*[False]
-    if wrapDimensions is not None:
-        try:
-            dimensionWraps[list(wrapDimensions)] = True
-        except BaseException as e:
-            raise ValueError,"wrapDimensions must be a list of valid dimensions for inputArray. Original error was: {}".format(e)
-
-    #Set an array of the same size indicating which elements have been set
-    cdef np.ndarray isNotSearched
-    isNotSearched = np.ones(arrayShape,dtype = 'int')
-
-    #Set the raveled input array
-    cdef np.float_t [:] raveledInputArray = inputArray.ravel()
-    #And ravel the search inidcator array
-    cdef np.int_t [:] raveledIsNotSearched = isNotSearched.ravel()
-    
-    #Set the search list to null
-    contiguousAreas = []
-
-    cdef int i
-    #Loop over the array
-    for i in xrange(numArrayElements):
-        #print "{}/{}".format(i,numArrayElements)
-        #Check if the current element meets the search condition
-        if raveledInputArray[i] >= searchThreshold and raveledIsNotSearched[i]:
-            #Flag that this cell has been searched
-            raveledIsNotSearched[i] = 0
-
-            #If it does, use a flood fill search to find the contiguous area surrouinding
-            #the element for which the search condition is satisified. At very least, the index
-            #of this element is appended to contiguousAreas
-            contiguousAreas.append(\
-                                    findNeighbors(  i,  \
-                                                    searchThreshold,    \
-                                                    arrayShape,         \
-                                                    arrayRank,          \
-                                                    dimensionWraps,     \
-                                                    raveledInputArray,         \
-                                                    raveledIsNotSearched      ))
-
-        else:
-            #Flag that this cell has been searched
-            raveledIsNotSearched[i] = 0
-                                    
-
-
-    #Set the list of contiguous area indices
-    return contiguousAreas
-
-def sortByDistanceFromCenter(inds,varShape):
-    """Takes sets of indicies [e.g., from floodFillSearchC.floodFillSearch()] and sorts them by distance from the center of the array from which the indices were taken.
-    
-        input:
-        ------
-        
-            inds     :  a list of tuples of numpy ndarrays (of type integer and
-                        rank 1), where each tuple item contains a vector of
-                        indices for each index of an array.  Each list item
-                        should conform to the output of the numpy where()
-                        function.  It is assumed that each set of indices
-                        represents a contiguous portion of an array.
-                       
-            varShape : the shape of the variable from which inds originate
-            
-        returns:
-        --------
-
-             A sorted version of inds, where the items are sorted by the
-             distance of the contiguous area relative to the center of the
-             array whose shape is varShape.  The first item is the closest to
-             the center of the array.
-             
-    """
-    #Get the center index
-    center = np.around(np.array(varShape)/2)
-    
-    #Transform the indices to be center-relative
-    centeredInds = [ tuple([ aind - cind] for aind,cind in zip(indTuples,center)) for indTuples in inds ]
-    
-    #Calculate center-of-mass ffor each contiguous array
-    centersOfMass = [ np.array([np.average(aind) for aind in indTuples]) for indTuples in centeredInds]
-    
-    #Calculate the distance from the origin of each center of mass
-    distances = [ np.sqrt(sum(indices**2)) for indices in centersOfMass]
-    
-    #Determine the sorting indices that will sort inds by distance from the center
-    isort = list(np.argsort(distances))
-    
-    #Return the sorted index array
-    return [inds[i] for i in isort]
+import numpy as np
+cimport numpy as np
+cimport cython
+
+cdef inline int ravel_shift(   tuple indices, \
+                                int arrayRank, \
+                                np.intp_t [:] arrayShape, \
+                                int dimension,  \
+                                int amount,     \
+                                int dimensionWraps):
+    """Return the raveled index of a shifted version of indices, where a
+    specific dimension has been shifted by a certain amount.  If wrapping is
+    not flagged and the shift is out of bounds, returns -1"""
+
+
+    cdef int runningProduct
+    cdef int n
+    cdef int i
+    cdef int np
+    cdef int thisIndex
+
+    runningProduct = 1
+    i = 0
+
+    #Loop over dimensions, starting at the rightmost dimension
+    for n in xrange(arrayRank,0,-1):
+        #Calculate the running product of dimension sizes
+        if( n != arrayRank):
+            runningProduct *= arrayShape[n]
+
+        #Set the current index
+        thisIndex = indices[n-1]
+
+        np = n-1
+        if(np == dimension):
+            #If this is the shifting dimension,
+            #increment it
+            thisIndex += amount
+
+            #Check if we need to deal with a
+            #wrap around dimension
+            if(dimensionWraps):
+                if(thisIndex < 0):
+                    thisIndex += arrayShape[np]
+                if(thisIndex >= arrayShape[np]):
+                    thisIndex -= arrayShape[np]
+
+            #Check if the current index is out of bounds;
+            #return -1 if so
+            if(thisIndex < 0 or thisIndex >= arrayShape[np]):
+                i = -1
+                break
+
+        #increment the counter
+        i += runningProduct*thisIndex
+
+    #Check whether the index is within the memory bounds of the array
+    #return the -1 flag if not
+    runningProduct *= arrayShape[0]
+    if(i >= runningProduct or i < 0):
+        i = -1
+
+    return i
+
+@cython.boundscheck(False)
+cdef tuple findNeighbors(   int raveledStartIndex, \
+                            np.float_t searchThreshold, \
+                            np.intp_t [:] arrayShape, \
+                            int arrayRank, \
+                            list dimensionWraps, \
+                            np.float_t [:] inputArray, \
+                            np.int_t [:] isNotSearched, \
+                   ):
+    """Does a flood fill algorithim on inputArray in the vicinity of
+    raveledStartIndex to find contiguous areas where raveledStartIndex > searchThreshold 
+    
+        input:
+        ------
+            raveledStartIndex   :   (integer) the index of inputArray.ravel() at which to start
+
+            searchThreshold :   The threshold for defining fill regions
+                                (inputArray > searchThreshold)
+
+        output:
+        -------
+            A list of N-d array indices.
+    
+    """
+
+    
+    cdef list itemsToSearch #Running item search list
+    cdef list contiguousIndices #A list of indices
+    cdef int r #Current array dimension
+    cdef int testIndexLeft # A test index
+    cdef int testIndexRight # A test index
+    cdef tuple contiguousArray #A tuple of contiguous indices
+    cdef np.ndarray contiguousIndexArray #An array of contiguous indices
+    cdef int testInd #The raveled index of the test point
+
+    cdef tuple itemTuple #The tuple index of the current search item
+
+    cdef int shiftAmount
+
+    #Initialize the contiguous index list
+    contiguousIndices = []
+
+    #Initialize the search list
+    itemsToSearch = [raveledStartIndex]
+
+    while itemsToSearch != []:
+
+        #Get the index of the current item
+        itemTuple = np.unravel_index(itemsToSearch[0],arrayShape)
+
+        for r in xrange(arrayRank):
+            #Shift the current coordinate to the right by 1 in the r dimension
+            shiftAmount = 1
+            testIndexRight = ravel_shift( \
+                                        itemTuple, \
+                                        arrayRank, \
+                                        arrayShape, \
+                                        r, \
+                                        shiftAmount,
+                                        dimensionWraps[r])
+
+            #Check that this coordinate is still within bounds
+            if(testIndexRight >= 0):
+                #Check if this index satisfies the search condition
+                if(inputArray[testIndexRight] > searchThreshold and \
+                        isNotSearched[testIndexRight] == 1):
+                    #Append it to the search list if so
+                    itemsToSearch.append(testIndexRight)
+                    #Flags that this cell has been searched
+                    isNotSearched[testIndexRight] = 0
+
+
+            #Shift the current coordinate to the right by 1 in the r dimension
+            shiftAmount = -1
+            testIndexLeft = ravel_shift( \
+                                        itemTuple, \
+                                        arrayRank, \
+                                        arrayShape, \
+                                        r, \
+                                        shiftAmount,
+                                        dimensionWraps[r])
+
+            #Check that this coordinate is still within bounds
+            if(testIndexLeft > 0):
+                #Check if this index satisfies the search condition
+                if(inputArray[testIndexLeft] > searchThreshold and \
+                        isNotSearched[testIndexLeft] == 1 ):
+                    #Append it to the search list if so
+                    itemsToSearch.append(testIndexLeft)
+                    #Flags that this cell has been searched
+                    isNotSearched[testIndexLeft] = 0
+
+ 
+
+        #Flag that this index has been searched
+        #isNotSearched[tuple(itemsToSearch[0])] = 0
+        #Now that the neighbors of the first item in the list have been tested,
+        #remove it from the list and put it in the list of contiguous values
+        contiguousIndices.append(itemsToSearch.pop(0))
+
+    #Return the list of contiguous indices (converted to index tuples)
+    return np.unravel_index(contiguousIndices,arrayShape)
+
+cpdef list floodFillSearch( \
+                np.ndarray inputArray, \
+                np.float_t searchThreshold = 0.0, \
+                wrapDimensions = None):
+    """Given an N-dimensional array, find contiguous areas of the array
+    satisfiying a given condition and return a list of contiguous indices
+    for each contiguous area.
+        
+        input:
+        ------
+
+            inputArray      :   (array-like) an array from which to search
+                                contiguous areas
+
+            searchThreshold :   The threshold for defining fill regions
+                                (inputArray > searchThreshold)
+
+            wrapDimensions :    A list of dimensions in which searching
+                                should have a wraparound condition
+
+        output:
+        -------
+
+            An unordered list, where each item corresponds to a unique
+            contiguous area for which inputArray > searchThreshold, and
+            where the contents of each item are a list of array indicies
+            that access the elements of the array for a given contiguous
+            area.
+
+    """
+    cdef np.ndarray[np.intp_t,ndim=1] arrayShape
+    cdef int arrayRank
+    cdef int numArrayElements
+    cdef list dimensionWraps
+    cdef list contiguousAreas
+
+    cdef tuple contiguousArray 
+
+    #Determine the rank of inputArray
+    try:
+        arrayShape = np.array(np.shape(inputArray))
+        arrayRank = len(arrayShape)
+        numArrayElements = np.prod(arrayShape)
+    except BaseException as e:
+        raise ValueError,"inputArray does not appear to be array like.  Error was: {}".format(e)
+
+    #Set the dimension wrapping array
+    dimensionWraps = arrayRank*[False]
+    if wrapDimensions is not None:
+        try:
+            dimensionWraps[list(wrapDimensions)] = True
+        except BaseException as e:
+            raise ValueError,"wrapDimensions must be a list of valid dimensions for inputArray. Original error was: {}".format(e)
+
+    #Set an array of the same size indicating which elements have been set
+    cdef np.ndarray isNotSearched
+    isNotSearched = np.ones(arrayShape,dtype = 'int')
+
+    #Set the raveled input array
+    cdef np.float_t [:] raveledInputArray = inputArray.ravel()
+    #And ravel the search inidcator array
+    cdef np.int_t [:] raveledIsNotSearched = isNotSearched.ravel()
+    
+    #Set the search list to null
+    contiguousAreas = []
+
+    cdef int i
+    #Loop over the array
+    for i in xrange(numArrayElements):
+        #print "{}/{}".format(i,numArrayElements)
+        #Check if the current element meets the search condition
+        if raveledInputArray[i] >= searchThreshold and raveledIsNotSearched[i]:
+            #Flag that this cell has been searched
+            raveledIsNotSearched[i] = 0
+
+            #If it does, use a flood fill search to find the contiguous area surrouinding
+            #the element for which the search condition is satisified. At very least, the index
+            #of this element is appended to contiguousAreas
+            contiguousAreas.append(\
+                                    findNeighbors(  i,  \
+                                                    searchThreshold,    \
+                                                    arrayShape,         \
+                                                    arrayRank,          \
+                                                    dimensionWraps,     \
+                                                    raveledInputArray,         \
+                                                    raveledIsNotSearched      ))
+
+        else:
+            #Flag that this cell has been searched
+            raveledIsNotSearched[i] = 0
+                                    
+
+
+    #Set the list of contiguous area indices
+    return contiguousAreas
+
+def sortByDistanceFromCenter(inds,varShape):
+    """Takes sets of indicies [e.g., from floodFillSearchC.floodFillSearch()] and sorts them by distance from the center of the array from which the indices were taken.
+    
+        input:
+        ------
+        
+            inds     :  a list of tuples of numpy ndarrays (of type integer and
+                        rank 1), where each tuple item contains a vector of
+                        indices for each index of an array.  Each list item
+                        should conform to the output of the numpy where()
+                        function.  It is assumed that each set of indices
+                        represents a contiguous portion of an array.
+                       
+            varShape : the shape of the variable from which inds originate
+            
+        returns:
+        --------
+
+             A sorted version of inds, where the items are sorted by the
+             distance of the contiguous area relative to the center of the
+             array whose shape is varShape.  The first item is the closest to
+             the center of the array.
+             
+    """
+    #Get the center index
+    center = np.around(np.array(varShape)/2)
+    
+    #Transform the indices to be center-relative
+    centeredInds = [ tuple([ aind - cind] for aind,cind in zip(indTuples,center)) for indTuples in inds ]
+    
+    #Calculate center-of-mass ffor each contiguous array
+    centersOfMass = [ np.array([np.average(aind) for aind in indTuples]) for indTuples in centeredInds]
+    
+    #Calculate the distance from the origin of each center of mass
+    distances = [ np.sqrt(sum(indices**2)) for indices in centersOfMass]
+    
+    #Determine the sorting indices that will sort inds by distance from the center
+    isort = list(np.argsort(distances))
+    
+    #Return the sorted index array
+    return [inds[i] for i in isort]
```

### Comparing `fastkde-1.0.8/fastkde/nufft.pyx` & `fastkde-1.0.9/fastkde/nufft.pyx`

 * *Files identical despite different names*

### Comparing `fastkde-1.0.8/setup.py` & `fastkde-1.0.9/setup.py`

 * *Files identical despite different names*

