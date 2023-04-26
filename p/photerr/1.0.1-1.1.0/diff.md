# Comparing `tmp/photerr-1.0.1.tar.gz` & `tmp/photerr-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photerr-1.0.1.tar", max compression
+gzip compressed data, was "photerr-1.1.0.tar", max compression
```

## Comparing `photerr-1.0.1.tar` & `photerr-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1079 2022-11-04 23:14:11.797407 photerr-1.0.1/LICENSE
--rw-r--r--   0        0        0    10224 2022-11-04 23:14:11.797407 photerr-1.0.1/README.md
--rw-r--r--   0        0        0      337 2022-11-04 23:14:11.797407 photerr-1.0.1/photerr/__init__.py
--rw-r--r--   0        0        0     1362 2022-11-04 23:14:11.797407 photerr-1.0.1/photerr/euclid.py
--rw-r--r--   0        0        0     2218 2022-11-04 23:14:11.797407 photerr-1.0.1/photerr/lsst.py
--rw-r--r--   0        0        0    16410 2022-11-04 23:14:11.797407 photerr-1.0.1/photerr/model.py
--rw-r--r--   0        0        0    18571 2022-11-04 23:14:11.797407 photerr-1.0.1/photerr/params.py
--rw-r--r--   0        0        0     1424 2022-11-04 23:14:11.797407 photerr-1.0.1/photerr/roman.py
--rw-r--r--   0        0        0     1312 2022-11-04 23:14:11.801407 photerr-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    11201 1970-01-01 00:00:00.000000 photerr-1.0.1/setup.py
--rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 photerr-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-04-26 05:38:04.335104 photerr-1.1.0/LICENSE
+-rw-r--r--   0        0        0    11784 2023-04-26 05:38:04.335104 photerr-1.1.0/README.md
+-rw-r--r--   0        0        0      337 2023-04-26 05:38:04.335104 photerr-1.1.0/photerr/__init__.py
+-rw-r--r--   0        0        0     1362 2023-04-26 05:38:04.335104 photerr-1.1.0/photerr/euclid.py
+-rw-r--r--   0        0        0     2218 2023-04-26 05:38:04.335104 photerr-1.1.0/photerr/lsst.py
+-rw-r--r--   0        0        0    18351 2023-04-26 05:38:04.335104 photerr-1.1.0/photerr/model.py
+-rw-r--r--   0        0        0    19273 2023-04-26 05:38:04.335104 photerr-1.1.0/photerr/params.py
+-rw-r--r--   0        0        0     1424 2023-04-26 05:38:04.335104 photerr-1.1.0/photerr/roman.py
+-rw-r--r--   0        0        0     1312 2023-04-26 05:38:04.339104 photerr-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    12414 1970-01-01 00:00:00.000000 photerr-1.1.0/PKG-INFO
```

### Comparing `photerr-1.0.1/LICENSE` & `photerr-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `photerr-1.0.1/README.md` & `photerr-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -32,14 +32,21 @@
 ```
 
 The error model expects an input catalog in the form of a pandas DataFrame with true magnitudes, and it returns another DataFrame containing observed magnitudes and photometric errors.
 Any extraneous columns in the DataFrame (e.g. a redshift column), remain in the new DataFrame - their presence does not effect the error model.
 
 *If compatibility with Astropy Tables, Ordered Dictionaries, etc., would be useful to you, let me know!*
 
+You can also calculate limiting magnitudes:
+
+```python
+errModel.getLimitingMags() # coadded point-source 5-sigma limits
+errModel.getLimitingMags(nSigma=1, coadded=False) # single-image point-source 1-sigma limits
+```
+
 # Tweaking the error model
 
 There are many parameters you can tweak to fine tune the error model.
 To see all available parameters, you can either call help on the error model's `params` object,
 
 ```python
 help(errModel.params)
@@ -98,14 +105,32 @@
 Remember that `sigLim` also sets the detection threshold, so in effect, any galaxy magnitudes beyond the detection threshold will be set equal to the detection threshold.
 
 One other option is provided by the `absFlux` parameter.
 If `absFlux=True`, then the absolute value of all fluxes are taken before converting back to magnitudes.
 If combined with `sigLim=0`, this means every galaxy will have an observed flux in every band.
 This is useful if you do not want to worry about non-detections, but it results in a non-Gaussian error distribution for low-SNR sources.
 
+### Errors for extended sources
+
+PhotErr can be used to calculate errors for extended sources as well.
+You just have to pass `extendedType="auto"` or `extendedType="gaap"` to the constructor (see explanation below for the differences in these models).
+PhotErr will then look for columns in the input DataFrame that correspond to the semi-major and -minor axes of the objects, corresponding to half-light radii in arcseconds.
+By default, it looks for these in columns titled "major" and "minor", but you can change the names of these columns using the `majorCol` and `minorCol` keywords.
+
+You can also calculate limiting magnitudes for apertures of a given size by passing the `aperture` keyword to `errModel.getLimitingMags()`
+
+### Scaling the errors
+
+If you want to scale up or scale down the errors in any band(s), you can use the keyword `scale`. 
+For example, `LsstErrorModel(scale={"u": 2, "y": 2})` will have all the same properties of the default error model, except the errors in the `u` and `y` bands will be doubled.
+This allows you to answer questions like "what happens to my science if the `u` band errors are doubled."
+
+Note this only scales the band-specific error.
+The band-independent systematic error floor, `sigmaSys` is still the same, and so at high-SNR, near the systematic floor, the errors won't scale as you expect.
+
 ### *Other error models*
 
 In addition to `LsstErrorModel`, which comes with the LSST defaults, PhotErr includes `EuclidErrorModel` and `RomanErrorModel`, which come with the Euclid and Roman defaults, respectively.
 Each of these models also have corresponding parameter objects: `EuclidErrorParams` and `RomanErrorParams`.
 
 You can also start with the base error model, `ErrorModel`, which is not defaulted for any specific survey.
 To instantiate `ErrorModel`, there are several required arguments that you must supply.
```

### Comparing `photerr-1.0.1/photerr/euclid.py` & `photerr-1.1.0/photerr/euclid.py`

 * *Files identical despite different names*

### Comparing `photerr-1.0.1/photerr/lsst.py` & `photerr-1.1.0/photerr/lsst.py`

 * *Files identical despite different names*

### Comparing `photerr-1.0.1/photerr/model.py` & `photerr-1.1.0/photerr/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,17 +52,14 @@
 
         # make a list of the bands
         self._bands = [band for band in self._params.nVisYr.keys()]
 
         # calculate all of the 5-sigma limiting magnitudes
         self._calculate_m5()
 
-        # calculate the limits for sigLim
-        self._sigLim = self.getLimitingMags(self._params.sigLim, coadded=True)
-
     @property
     def params(self) -> ErrorParams:
         """The error model parameters in an ErrorParams objet."""  # noqa: D401
         return self._params
 
     def _calculate_m5(self) -> None:
         """Calculate the single-visit 5-sigma limiting magnitudes.
@@ -147,31 +144,31 @@
 
         # convert min/max aperture diameter to Gaussian sigma
         aMin_sig = self.params.aMin / 2.355
         aMax_sig = self.params.aMax / 2.355
 
         # convert galaxy half-light radii to Gaussian sigmas
         # this conversion factor comes from half-IQR -> sigma
-        majors /= 0.6745
-        minors /= 0.6745
+        majors = majors / 0.6745
+        minors = minors / 0.6745
 
         # calculate the area of the psf in each band
         A_psf = np.pi * psf_sig**2
 
         # calculate the area of the galaxy aperture in each band
         a_ap = np.sqrt(psf_sig[None, :] ** 2 + majors[:, None] ** 2 + aMin_sig**2)
         a_ap[a_ap > aMax_sig] = aMax_sig
         b_ap = np.sqrt(psf_sig[None, :] ** 2 + minors[:, None] ** 2 + aMin_sig**2)
         b_ap[b_ap > aMax_sig] = aMax_sig
         A_ap = np.pi * a_ap * b_ap
 
         # return their ratio
         return A_ap / A_psf
 
-    def _get_NSR(
+    def _get_nsr_from_mags(
         self, mags: np.ndarray, majors: np.ndarray, minors: np.ndarray, bands: list
     ) -> np.ndarray:
         """Calculate the noise-to-signal ratio.
 
         Uses Eqs 4 and 5 from Ivezic 2019.
         If using extended errors, also rescales with square root of area ratio.
 
@@ -185,22 +182,24 @@
             The semi-minor axes of the galaxies in arcseconds
         bands : list
             The list of bands the galaxy is observed in
 
         Returns
         -------
         np.ndarray
-            The ratio of aperture size to PSF size for each band and galaxy.
+            The noise-to-signal ratio of each galaxy
         """
         # get the 5-sigma limiting magnitudes for these bands
         m5 = np.array([self._all_m5[band] for band in bands])
         # and the values for gamma
         gamma = np.array([self.params.gamma[band] for band in bands])
         # and the number of visits per year
         nVisYr = np.array([self.params.nVisYr[band] for band in bands])
+        # and the scales
+        scale = np.array([self.params.scale[band] for band in bands])
 
         # calculate x as defined in the paper
         x = 10 ** (0.4 * (mags - m5))
 
         # calculate the NSR for a single visit
         with np.errstate(invalid="ignore"):
             nsrRandSingleExp = np.sqrt((0.04 - gamma) * x + gamma * x**2)
@@ -214,32 +213,116 @@
             A_ratio = self._get_area_ratio_auto(majors, minors, bands)
         elif self.params.extendedType == "gaap":
             A_ratio = self._get_area_ratio_gaap(majors, minors, bands)
         else:
             A_ratio = 1  # type: ignore
         nsrRand *= np.sqrt(A_ratio)
 
+        # rescale the NSR
+        nsrRand *= scale
+
         # get the irreducible system NSR
         if self.params.highSNR:
             nsrSys = self.params.sigmaSys
         else:
             nsrSys = 10 ** (self.params.sigmaSys / 2.5) - 1
 
         # calculate the total NSR
         nsr = np.sqrt(nsrRand**2 + nsrSys**2)
 
         return nsr
 
+    def _get_mags_from_nsr(
+        self,
+        nsr: np.ndarray,
+        majors: np.ndarray,
+        minors: np.ndarray,
+        bands: list,
+        coadded: bool = True,
+    ) -> np.ndarray:
+        """Calculate magnitudes that correspond to the given NSRs.
+
+        Essentially inverts self._get_nsr_from_mags().
+
+        Parameters
+        ----------
+        nsr : np.ndarray
+            The noise-to-signal ratios of the galaxies
+        majors : np.ndarray
+            The semi-major axes of the galaxies in arcseconds
+        minors : np.ndarray
+            The semi-minor axes of the galaxies in arcseconds
+        bands : list
+            The list of bands the galaxy is observed in
+        coadded : bool; default=True
+            If True, assumes NSR is after coaddition.
+
+        Returns
+        -------
+        np.ndarray
+            The magnitude corresponding to the NSR for each galaxy
+        """
+        # get the 5-sigma limiting magnitudes for these bands
+        m5 = np.array([self._all_m5[band] for band in bands])
+        # and the values for gamma
+        gamma = np.array([self.params.gamma[band] for band in bands])
+        # and the number of visits per year
+        nVisYr = np.array([self.params.nVisYr[band] for band in bands])
+        # and the scales
+        scale = np.array([self.params.scale[band] for band in bands])
+
+        # get the irreducible system NSR
+        if self.params.highSNR:
+            nsrSys = self.params.sigmaSys
+        else:
+            nsrSys = 10 ** (self.params.sigmaSys / 2.5) - 1
+
+        # calculate the random NSR
+        nsrRand = np.sqrt(nsr**2 - nsrSys**2)
+
+        # rescale the NSR
+        nsrRand /= scale
+
+        # rescale according to the area ratio
+        if majors is not None and minors is not None:
+            if self.params.extendedType == "auto":
+                A_ratio = self._get_area_ratio_auto(majors, minors, bands)
+            elif self.params.extendedType == "gaap":
+                A_ratio = self._get_area_ratio_gaap(majors, minors, bands)
+            else:
+                A_ratio = 1  # type: ignore
+            nsrRand = nsrRand / np.sqrt(A_ratio)
+
+        # get the number of exposures
+        if coadded:
+            nStackedObs = nVisYr * self.params.nYrObs
+        else:
+            nStackedObs = 1  # type: ignore
+
+        # calculate the NSR for a single image
+        nsrRandSingleExp = nsrRand * np.sqrt(nStackedObs)
+
+        # calculate the value of x that corresponds to this NSR
+        # this is just the quadratic equation applied to Eq 5 from Ivezic 2019
+        x = (
+            (gamma - 0.04)
+            + np.sqrt((gamma - 0.04) ** 2 + 4 * gamma * nsrRandSingleExp**2)
+        ) / (2 * gamma)
+
+        # convert x to magnitudes
+        mags = m5 + 2.5 * np.log10(x)
+
+        return mags
+
     def _get_obs_and_errs(
         self,
         mags: np.ndarray,
         majors: np.ndarray,
         minors: np.ndarray,
         bands: list,
-        sigLim: np.ndarray,
         rng: np.random.Generator,
     ) -> Tuple[np.ndarray, np.ndarray]:
         """Calculate the noise-to-signal ratio.
 
         Uses Eqs 4 and 5 from Ivezic 2019.
         If using extended errors, also rescales with square root of area ratio.
 
@@ -249,64 +332,64 @@
             The magnitudes of the galaxies
         majors : np.ndarray
             The semi-major axes of the galaxies in arcseconds
         minors : np.ndarray
             The semi-minor axes of the galaxies in arcseconds
         bands : list
             The list of bands the galaxy is observed in
-        sigLim : np.ndarray
-            The n-sigma limits for non-detection
         rng : np.random.Generator
             A numpy random number generator
 
         Returns
         -------
         np.ndarray
             The ratio of aperture size to PSF size for each band and galaxy.
         """
         # get the NSR for all galaxies
-        nsr = self._get_NSR(mags, majors, minors, bands)
+        nsr = self._get_nsr_from_mags(mags, majors, minors, bands)
 
         if self.params.highSNR:
             # in the high SNR approximation, mag err ~ nsr, and we can model
             # errors as Gaussian in magnitude space
 
             # calculate observed magnitudes
             obsMags = rng.normal(loc=mags, scale=nsr)
 
-            # if ndMode == sigLim, then clip all magnitudes at the n-sigma limit
-            if self.params.ndMode == "sigLim":
-                obsMags = np.clip(obsMags, None, sigLim)
-
-            # if decorrelate, then we calculate new errors using the observed mags
-            if self.params.decorrelate:
-                nsr = self._get_NSR(obsMags, majors, minors, bands)
-
-            obsMagErrs = nsr
-
         else:
             # in the more accurate error model, we acknowledge err != nsr,
             # and we model errors as Gaussian in flux space
 
             # calculate observed magnitudes
             fluxes = 10 ** (mags / -2.5)
             obsFluxes = fluxes * (1 + rng.normal(scale=nsr))
             if self.params.absFlux:
                 obsFluxes = np.abs(obsFluxes)
             with np.errstate(divide="ignore"):
                 obsMags = -2.5 * np.log10(np.clip(obsFluxes, 0, None))
 
-            # if ndMode == sigLim, then clip all magnitudes at the n-sigma limit
-            if self.params.ndMode == "sigLim":
-                obsMags = np.clip(obsMags, None, sigLim)
-
-            # if decorrelate, then we calculate new errors using the observed mags
-            if self.params.decorrelate:
-                nsr = self._get_NSR(obsMags, majors, minors, bands)
+        # if decorrelate, then we calculate new errors using the observed mags
+        if self.params.decorrelate:
+            nsr = self._get_nsr_from_mags(obsMags, majors, minors, bands)
+
+        # if ndMode == sigLim, then clip at the n-sigma limit
+        if self.params.ndMode == "sigLim":
+            # determine the nsr limit
+            with np.errstate(divide="ignore"):
+                nsrLim = np.divide(1, self.params.sigLim)
+
+            # calculate limiting magnitudes for each galaxy
+            magLim = self._get_mags_from_nsr(nsrLim, majors, minors, bands)
+
+            # clip mags and nsr's at this limit
+            nsr = np.clip(nsr, 0, nsrLim)
+            obsMags = np.clip(obsMags, None, magLim)
 
+        if self.params.highSNR:
+            obsMagErrs = nsr
+        else:
             obsMagErrs = 2.5 * np.log10(1 + nsr)
 
         return obsMags, obsMagErrs
 
     def __call__(
         self, catalog: pd.DataFrame, random_state: Union[np.random.Generator, int]
     ) -> pd.DataFrame:
@@ -332,36 +415,38 @@
             rng = np.random.default_rng(random_state)
         else:
             raise TypeError("random_state must be a numpy random generator or an int.")
 
         # get the bands we will calculate errors for
         bands = [band for band in catalog.columns if band in self._bands]
 
-        # calculate the n-sigma limits
-        sigLim = np.array([self._sigLim[band] for band in bands])
-
         # get the numpy array of magnitudes
         mags = catalog[bands].to_numpy()
 
         # get the semi-major and semi-minor axes
         if self.params.extendedType == "auto" or self.params.extendedType == "gaap":
             majors = catalog[self.params.majorCol].to_numpy()
             minors = catalog[self.params.minorCol].to_numpy()
         else:
             majors = None
             minors = None
 
         # get observed magnitudes and errors
-        obsMags, obsMagErrs = self._get_obs_and_errs(
-            mags, majors, minors, bands, sigLim, rng
-        )
+        obsMags, obsMagErrs = self._get_obs_and_errs(mags, majors, minors, bands, rng)
 
         # flag all non-detections with the ndFlag
         if self.params.ndMode == "flag":
-            idx = (~np.isfinite(obsMags)) | (obsMags > sigLim)
+            # calculate SNR
+            if self.params.highSNR:
+                snr = 1 / obsMagErrs
+            else:
+                snr = 1 / (10 ** (obsMagErrs / 2.5) - 1)
+
+            # flag non-finite mags and where SNR is below sigLim
+            idx = (~np.isfinite(obsMags)) | (snr < self.params.sigLim)
             obsMags[idx] = self.params.ndFlag
             obsMagErrs[idx] = self.params.ndFlag
 
         # save the observations in a DataFrame
         errDf = pd.DataFrame(
             obsMagErrs, columns=[f"{band}_err" for band in bands], index=catalog.index
         )
@@ -378,72 +463,48 @@
             columns = catalog.columns.tolist()
             for band in bands:
                 columns.insert(columns.index(band) + 1, f"{band}_err")
             obsCatalog = obsCatalog[columns]
 
         return obsCatalog
 
-    def getLimitingMags(self, nSigma: float = 5, coadded: bool = True) -> dict:
-        """Return the limiting magnitudes for point sources in all bands.
-
-        This method essentially reverse engineers the _get_NSR method so that we
-        calculate what magnitude results in NSR = 1/nSigma.
-        (NSR is noise-to-signal ratio; NSR = 1/SNR)
+    def getLimitingMags(
+        self, nSigma: float = 5, coadded: bool = True, aperture: float = 0
+    ) -> dict:
+        """Return the limiting magnitudes in all bands.
 
         Parameters
         ----------
         nSigma : float; default=5
             Sets which limiting magnitude to return. E.g. nSigma=1 returns the 1-sigma
             limiting magnitude. In other words, nSigma is equal to the signal-to-noise
             ratio (SNR) of the limiting magnitudes.
         coadded : bool; default=True
             If True, returns the limiting magnitudes for a coadded image. If False,
             returns the limiting magnitudes for a single visit.
+        aperture : float, default=0
+            Radius of circular aperture in arcseconds. If zero, limiting magnitudes
+            are for point sources. If greater than zero, limiting magnitudes are
+            for objects of that size. Increasing the aperture decreases the
+            signal-to-noise ratio. This only has an impact if extendedType != "point.
 
         Returns
         -------
         dict
             The dictionary of limiting magnitudes
         """
-        bands = self._bands
-
-        # if nSigma is zero, return infinite magnitude limits
-        if np.isclose(0, nSigma):
-            return {band: np.inf for band in bands}
-
-        # get the 5-sigma limiting magnitudes for these bands
-        m5 = np.array([self._all_m5[band] for band in bands])
-        # and the values for gamma
-        gamma = np.array([self.params.gamma[band] for band in bands])
-        # and the number of visits per year
-        nVisYr = np.array([self.params.nVisYr[band] for band in bands])
-
-        # get the number of exposures
-        if coadded:
-            nStackedObs = nVisYr * self.params.nYrObs
-        else:
-            nStackedObs = 1  # type: ignore
-
-        # get the irreducible system error
-        if self.params.highSNR:
-            nsrSys = self.params.sigmaSys
-        else:
-            nsrSys = 10 ** (self.params.sigmaSys / 2.5) - 1
-
-        # calculate the random NSR that a single exposure must have
-        nsrRandSingleExp = np.sqrt((1 / nSigma**2 - nsrSys**2) * nStackedObs)
-
-        # calculate the value of x that corresponds to this NSR
-        # this is just the quadratic equation applied to Eq 5 from Ivezic 2019
-        x = (
-            (gamma - 0.04)
-            + np.sqrt((gamma - 0.04) ** 2 + 4 * gamma * nsrRandSingleExp**2)
-        ) / (2 * gamma)
-
-        # convert x to a limiting magnitude
-        limiting_mags = m5 + 2.5 * np.log10(x)
-
         # return as a dictionary
-        return dict(zip(bands, limiting_mags))
+        return dict(
+            zip(
+                self._bands,
+                self._get_mags_from_nsr(
+                    1 / nSigma,  # type: ignore
+                    np.array([aperture]),
+                    np.array([aperture]),
+                    self._bands,
+                    coadded,
+                ).flatten(),
+            )
+        )
 
     def __repr__(self) -> str:  # pragma: no cover
         return "Photometric error model with parameters:\n\n" + str(self.params)
```

### Comparing `photerr-1.0.1/photerr/params.py` & `photerr-1.1.0/photerr/params.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,14 +79,19 @@
         that in this case, the returned photometric errors are calculated from the true
         magnitudes, and thus provide a deterministic link back to the true magnitudes!
     highSNR : bool; default=False
         Whether to use the high SNR approximations given in Ivezic 2019. If False,
         then Eq. 5 from that paper is used to calculate (N/S)^2 in flux, and errors
         are Gaussian in flux space. If True, Eq. 5 is used to calculate the Gaussian
         variance in magnitude space.
+    scale : dict; default=dict()
+        A dictionary that rescales the error for the given bands. For example, if
+        scale = {"u": 2}, then all the errors for the u band are doubled. This allows
+        you to answer questions like "what happens to my science if the u band errors
+        are doubled."
     errLoc: str; default="after"
         Where to place the error columns in the output table. If "after", then the
         error columns will be placed immediately after the corresponding magnitude
         columns. If "end", then all of the error columns will be placed at the end
         of the table. If "alone", then the errors will be returned by themselves.
     renameDict : dict; optional
         A dictionary used to rename the bands in the parameters above that are
@@ -159,14 +164,15 @@
     "extendedType": [False, [str], ["point", "auto", "gaap"], None],
     "aMin": [False, [int, float], [], False],
     "aMax": [False, [int, float], [], False],
     "majorCol": [False, [str], [], None],
     "minorCol": [False, [str], [], None],
     "decorrelate": [False, [bool], [], None],
     "highSNR": [False, [bool], [], None],
+    "scale": [True, [int, float], [], None],
     "errLoc": [False, [str], ["after", "end", "alone"], None],
 }
 
 
 @dataclass
 class ErrorParams:
     """Parameters for the photometric error models."""
@@ -197,18 +203,19 @@
     aMin: float = 0.7
     aMax: float = 2.0
     majorCol: str = "major"
     minorCol: str = "minor"
 
     decorrelate: bool = True
     highSNR: bool = False
+    scale: Dict[str, float] = field(default_factory=lambda: {})
+
     errLoc: str = "after"
 
     renameDict: InitVar[Dict[str, str]] = None
-
     validate: InitVar[bool] = True
 
     def __post_init__(
         self, renameDict: Union[Dict[str, str], None], validate: bool
     ) -> None:
         """Rename bands and remove duplicate parameters."""
         # if renameDict was provided, rename the bands
@@ -239,37 +246,39 @@
         """Remove unnecessary info from all of the dictionaries.
 
         This means that any bands explicitly listed in m5 will have their corresponding
         info removed from Cm, msky, theta, and km.
 
         Additionally, we will remove any band from all dictionaries that don't have
         an entry in all of nVisYr, gamma, and (m5 OR Cm + msky + theta + km).
+
+        Finally, we will set scale=1 for all bands for which the scale isn't
+        explicitly set.
         """
         # keep a running set of all the bands we will calculate errors for
         all_bands = set(self.nVisYr.keys()).intersection(self.gamma.keys())
 
         # remove the m5 bands from all other parameter dictionaries, and remove
         # bands from all_bands for which we don't have m5 data for
-        ignore_dicts = ["m5", "nVisYr", "gamma"]
+        ignore_dicts = ["m5", "nVisYr", "gamma", "scale"]
         for key, param in self.__dict__.items():
             # get the parameters that are dictionaries
             if isinstance(param, dict) and key not in ignore_dicts:
                 if key != "theta":
                     # remove bands that we have explicit m5's for
                     self.__dict__[key] = {
                         band: val for band, val in param.items() if band not in self.m5
                     }
 
                 # update the running list of bands that we have sufficient m5 data for
                 all_bands = all_bands.intersection(
                     set(param.keys()).union(set(self.m5.keys()))
                 )
 
-        # finally, remove all of the data for bands that we will not be
-        # calculating errors for
+        # remove all data for bands we will not be calculating errors for
         for key, param in self.__dict__.items():
             if isinstance(param, dict):
                 self.__dict__[key] = {
                     band: val for band, val in param.items() if band in all_bands
                 }
 
         # if there are no bands left, raise an error
@@ -279,14 +288,20 @@
                 "parameters (i.e. nVisYr, gamma, m5, Cm, msky, theta, or km) such "
                 "that there was not enough info to calculate errors for any of the "
                 "photometric bands. Remember that for each band, you must have an "
                 "entry in nVisYr and gamma, plus either an entry in m5 or an entry "
                 "in all of Cm, msky, theta, and km."
             )
 
+        # finally, fill out the rest of the scale dictionary
+        self.scale = {
+            band: float(self.scale[band]) if band in self.scale else 1.0
+            for band in self.nVisYr
+        }
+
     def rename_bands(self, renameDict: Dict[str, str]) -> None:
         """Rename the bands used in the error model.
 
         This method might be useful if you want to use the default parameters for an
         error model, but have given your bands different names.
 
         Parameters
```

### Comparing `photerr-1.0.1/photerr/roman.py` & `photerr-1.1.0/photerr/roman.py`

 * *Files identical despite different names*

### Comparing `photerr-1.0.1/pyproject.toml` & `photerr-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "photerr"
-version = "1.0.1"
+version = "1.1.0"
 description = "Photometric error model for astronomical imaging surveys"
 authors = ["John Franklin Crenshaw <jfcrenshaw@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/jfcrenshaw/photerr"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
```

### Comparing `photerr-1.0.1/setup.py` & `photerr-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,233 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: photerr
+Version: 1.1.0
+Summary: Photometric error model for astronomical imaging surveys
+Home-page: https://github.com/jfcrenshaw/photerr
+Author: John Franklin Crenshaw
+Author-email: jfcrenshaw@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: numpy (>=1.23.2,<2.0.0)
+Requires-Dist: pandas (>=1.4.3,<2.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['photerr']
+<div align="center">
 
-package_data = \
-{'': ['*']}
+[![build](https://github.com/jfcrenshaw/photerr/actions/workflows/main.yml/badge.svg)](https://github.com/jfcrenshaw/photerr/actions/workflows/main.yml)
+[![Codecov](https://img.shields.io/codecov/c/github/jfcrenshaw/photerr?label=codecov&logo=codecov)](https://app.codecov.io/gh/jfcrenshaw/photerr)
+[![PyPI](https://img.shields.io/pypi/v/photerr?color=blue&label=PyPI)](https://pypi.org/project/photerr/)
 
-install_requires = \
-['numpy>=1.23.2,<2.0.0', 'pandas>=1.4.3,<2.0.0']
-
-setup_kwargs = {
-    'name': 'photerr',
-    'version': '1.0.1',
-    'description': 'Photometric error model for astronomical imaging surveys',
-    'long_description': '<div align="center">\n\n[![build](https://github.com/jfcrenshaw/photerr/actions/workflows/main.yml/badge.svg)](https://github.com/jfcrenshaw/photerr/actions/workflows/main.yml)\n[![Codecov](https://img.shields.io/codecov/c/github/jfcrenshaw/photerr?label=codecov&logo=codecov)](https://app.codecov.io/gh/jfcrenshaw/photerr)\n[![PyPI](https://img.shields.io/pypi/v/photerr?color=blue&label=PyPI)](https://pypi.org/project/photerr/)\n\n</div>\n\n# PhotErr\n\nPhotErr is a photometric error model for astronomical imaging surveys.\nIt implements a generalization of the high-SNR point-source error model from [Ivezic (2019)](https://arxiv.org/abs/0805.2366) that is more accurate in the low SNR regime and includes errors for extended sources, using the models from [van den Busch (2020)](http://arxiv.org/abs/2007.01846) and [Kuijken (2019)](https://arxiv.org/abs/1902.11265).\n\nPhotErr currently includes photometric error models for the Vera C. Rubin Observatory Legacy Survey of Space and Time (LSST), as well as the Euclid and Nancy Grace Roman space telescopes.\n\n# Getting started\n\nPhotErr is available on PyPI and can be installed with pip:\n\n```bash\npip install photerr\n```\n\nNote that PhotErr requires Python >= 3.8.\n\nOnce installed, you can import the error models. For example, to use the default LSST error model,\n\n```python\nfrom photerr import LsstErrorModel\nerrModel = LsstErrorModel()\ncatalog_with_errors = errModel(catalog, random_state=42)\n```\n\nThe error model expects an input catalog in the form of a pandas DataFrame with true magnitudes, and it returns another DataFrame containing observed magnitudes and photometric errors.\nAny extraneous columns in the DataFrame (e.g. a redshift column), remain in the new DataFrame - their presence does not effect the error model.\n\n*If compatibility with Astropy Tables, Ordered Dictionaries, etc., would be useful to you, let me know!*\n\n# Tweaking the error model\n\nThere are many parameters you can tweak to fine tune the error model.\nTo see all available parameters, you can either call help on the error model\'s `params` object,\n\n```python\nhelp(errModel.params)\n```\n\nor look at the docstring of the corresponding parameters object,\n\n```python\nfrom photerr import LsstErrorParams\nhelp(LsstErrorParams)\n```\n\nAll model parameters can be overridden using keyword arguments to the error model constructor.\nBelow, we explain a few of the more commonly tweaked parameters.\n\n### *Changing the observing duration*\n\nThe example above uses the default settings for the LSST model, which includes 10 years of observing time.\nIf instead you want to calculate errors for LSST year 1, you can pass the `nYrObs` argument to the constructor:\n\n```python\nerrModel = LsstErrorModel(nYrObs=1)\n```\n\n### *Changing the band names*\n\nAnother parameter you might want to tweak is the name of the bands.\nBy default, the `LsstErrorModel` assumes that the LSST bands are named `u`, `g`, etc.\nIf instead, the bands in your catalog are named `lsst_u`, `lsst_g`, etc., then you can instantiate the error model with a rename dictionary:\n\n```python\nerrModel = LsstErrorModel(renameDict={"u": "lsst_u", "g": "lsst_g", ...})\n```\n\nThis tells `LsstErrorModel` to use all of the default parameters, but just change the names it gave to all of the bands.\nIf you are changing other dictionary-parameters at the same time (e.g. `nVisYr`, which sets the number of visits in each band per year), you can supply those parameters using *either* the new or old naming scheme!\n\n### *Directly setting limiting magnitudes*\n\nBy default, PhotErr tries to use the provided information to calculate limiting magnitudes for you.\nIf you would like to directly supply your own $5\\sigma$ limits, you can do so using the `m5` parameter.\nNote that PhotErr assumes these are single-visit limiting magnitudes.\nIf you want to supply coadded depths, you should also set `nYrObs=1` and `nVisYr={u: 1, g: 1, ...}`, so that the calculated coadded depths are equal to those you provided.\n\n### *Handling non-detections*\n\nThe other big thing you may want to change is how the error model identifies and handles non-detections.\n\nThe error model has a parameter named `sigLim`, which sets the limit for non-detections.\nBy default, `sigLim=0`, which means that only negative fluxes count as non-detections, however if you set `sigLim=1`, then any magnitudes beyond the 1-sigma limit in each band will count as a non-detection.\nYou can set `sigLim` to any non-negative float.\n\nThe `ndMode` parameter tells the error model how to handle the non-detections.\nBy default, `ndMode="flag"`, which means that the model will flag non-detections with the value set by `ndFlag`, which defaults to `np.inf`.\nHowever, you can also set `ndMode="sigLim"`, in which case the model will set all non-detections to the n-sigma limits set by the `sigLim` parameter described in the previous paragraph.\nRemember that `sigLim` also sets the detection threshold, so in effect, any galaxy magnitudes beyond the detection threshold will be set equal to the detection threshold.\n\nOne other option is provided by the `absFlux` parameter.\nIf `absFlux=True`, then the absolute value of all fluxes are taken before converting back to magnitudes.\nIf combined with `sigLim=0`, this means every galaxy will have an observed flux in every band.\nThis is useful if you do not want to worry about non-detections, but it results in a non-Gaussian error distribution for low-SNR sources.\n\n### *Other error models*\n\nIn addition to `LsstErrorModel`, which comes with the LSST defaults, PhotErr includes `EuclidErrorModel` and `RomanErrorModel`, which come with the Euclid and Roman defaults, respectively.\nEach of these models also have corresponding parameter objects: `EuclidErrorParams` and `RomanErrorParams`.\n\nYou can also start with the base error model, `ErrorModel`, which is not defaulted for any specific survey.\nTo instantiate `ErrorModel`, there are several required arguments that you must supply.\nTo see a list and explanation of these arguments, see the docstring for `ErrorParams`.\n\n# Explanation of the error model\n\n### *The point source model*\n\nTo derive the [Ivezic (2019)](https://arxiv.org/abs/0805.2366) error model, we start with the noise-to-signal ratio (NSR) for an object with photon count $C$ and background noise $N_0$ (which depends on seeing, read-out noise, etc.):\n\n$$\nNSR^2 = \\frac{N_0^2 + C}{C^2}.\n$$\n\nIf we define $C = C_5$ when $NSR = 1/5$, then we can solve for $N_0$ and write\n\n$$\nNSR^2 = \\frac{1}{C_5} \\left( \\frac{C_5}{C} \\right) + \\left[ \\left( \\frac{1}{5} \\right)^2 - \\frac{1}{C_5} \\right] \\left( \\frac{C_5}{C} \\right)^2.\n$$\n\nDefining $x = \\frac{C_5}{C} = 10 ^{(m - m_5) / 2.5}$ and $\\gamma = \\left( \\frac{1}{5} \\right)^2 - \\frac{1}{C_5}$, we have\n\n$$\nNSR^2 = (0.04 - \\gamma) x + \\gamma x^2 ~~ (\\text{mag}^2).\n$$\n\nIn the high signal-to-noise ratio (SNR) limit, $NSR \\ll 1$, and we can approximate\n\n$$\n\\sigma_\\text{rand} = 2.5 \\log_{10}\\left( 1 + NSR \\right) \\approx NSR.\n$$\n\nThis approximation yields Equation 5 from [Ivezic (2019)](https://arxiv.org/abs/0805.2366).\nIn PhotErr, we do not make this approximation so that the error model generalizes to the low SNR regime.\nIn addition, while the high-SNR model assumes photometric errors are Gaussian in magnitude space, we model errors as Gaussian in flux space.\nHowever, both of these high-SNR approximations can be restored with the keyword `highSNR=True`.\n\nThe LSST error model uses the parameters from [Ivezic (2019)](https://arxiv.org/abs/0805.2366).\nThe Euclid and Roman error models follow [Graham (2020)](https://arxiv.org/abs/2004.07885) in setting $\\gamma = 0.04$, which is nearly identical to the values for Rubin (which are all $\\sim 0.039$).\n\nIn addition to the random photometric error above, we include a system error of $\\sigma_\\text{sys} = 0.005$ which is added in quadrature to random error. Note that the system error can be changed using the keyword `sigmaSys`.\n\nAfter adding photometric errors to the catalog, PhotErr recalculates the photometric error from the "observed" magnitudes.\nThis is so that the reported photometric errors do not provide a deterministic link back to the true magnitudes.\nThis behavior can be disabled by setting `decorrelate=False`.\n\n### *The extended source model*\n\nThe [Ivezic (2019)](https://arxiv.org/abs/0805.2366) model calculates errors for point sources.\nTo model errors for extended sources, we use Equation 5 from [van den Busch (2020)](http://arxiv.org/abs/2007.01846):\n\n$$\nNSR_\\text{ext} \\propto\nNSR_\\text{pt} \\sqrt{\\frac{A_\\text{ap}}{A_\\text{psf}}},\n$$\n\nwhere $A_\\text{ap}$ is the area of the source aperture, and $A_\\text{psf}$ is the area of the PSF.\nWe set the proportionality constant to unity, so that when $A_\\text{ap} \\to A_\\text{psf}$, we recover the error for a point source.\n\nWe include two different models for calculating the aperture area. The "auto" method from [van den Busch (2020)](http://arxiv.org/abs/2007.01846) calculates the semi-major and -minor axes of the aperture ( $a_\\text{ap}$ and $b_\\text{ap}$) from the semi-major and -minor axes of the galaxy ( $a_\\text{gal}$ and $b_\\text{gal}$, corresponding to half-light radii):\n\n$$\na_\\text{ap} = \\sqrt{\\sigma_\\text{psf}^2 + (2.5 a_\\text{gal})^2},\n\\quad\nb_\\text{ap} = \\sqrt{\\sigma_\\text{psf}^2 + (2.5 b_\\text{gal})^2},\n$$\n\nwhere $\\sigma\\_\\text{psf} = \\text{FWHM}\\_\\text{psf} / 2.355$ is the PSF standard deviation.\nThe formula for the area of an ellipse is then used to calculate the aperture area: $A_\\text{ap} = \\pi a_\\text{ap} b_\\text{ap}$.\n\nThe "gaap" method for extended sources ([Kuijken 2019](https://arxiv.org/abs/1902.11265)) is nearly identical, except that it adds a minimum aperture diameter in quadrature when calculating $a_\\text{ap}$ and $b_\\text{ap}$, and then clips aperture diameters above a certain maximum.\n\nCalculating errors for extended sources requires columns in the galaxy catalog corresponding to the semi-major and -minor axes of the galaxies (with the length scale corresponding to the half-light radius).\nYou can set the names of these columns using the keywords `majorCol` and `minorCol`.\n\n# Authors\n\n[John Franklin Crenshaw](https://jfcrenshaw.github.io) \\\n[Ziang Yan](https://yanzastro.github.io)\n\n[*Contributors guide*](CONTRIBUTING.md)\n',
-    'author': 'John Franklin Crenshaw',
-    'author_email': 'jfcrenshaw@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/jfcrenshaw/photerr',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+</div>
 
+# PhotErr
+
+PhotErr is a photometric error model for astronomical imaging surveys.
+It implements a generalization of the high-SNR point-source error model from [Ivezic (2019)](https://arxiv.org/abs/0805.2366) that is more accurate in the low SNR regime and includes errors for extended sources, using the models from [van den Busch (2020)](http://arxiv.org/abs/2007.01846) and [Kuijken (2019)](https://arxiv.org/abs/1902.11265).
+
+PhotErr currently includes photometric error models for the Vera C. Rubin Observatory Legacy Survey of Space and Time (LSST), as well as the Euclid and Nancy Grace Roman space telescopes.
+
+# Getting started
+
+PhotErr is available on PyPI and can be installed with pip:
+
+```bash
+pip install photerr
+```
+
+Note that PhotErr requires Python >= 3.8.
+
+Once installed, you can import the error models. For example, to use the default LSST error model,
+
+```python
+from photerr import LsstErrorModel
+errModel = LsstErrorModel()
+catalog_with_errors = errModel(catalog, random_state=42)
+```
+
+The error model expects an input catalog in the form of a pandas DataFrame with true magnitudes, and it returns another DataFrame containing observed magnitudes and photometric errors.
+Any extraneous columns in the DataFrame (e.g. a redshift column), remain in the new DataFrame - their presence does not effect the error model.
+
+*If compatibility with Astropy Tables, Ordered Dictionaries, etc., would be useful to you, let me know!*
+
+You can also calculate limiting magnitudes:
+
+```python
+errModel.getLimitingMags() # coadded point-source 5-sigma limits
+errModel.getLimitingMags(nSigma=1, coadded=False) # single-image point-source 1-sigma limits
+```
+
+# Tweaking the error model
+
+There are many parameters you can tweak to fine tune the error model.
+To see all available parameters, you can either call help on the error model's `params` object,
+
+```python
+help(errModel.params)
+```
+
+or look at the docstring of the corresponding parameters object,
+
+```python
+from photerr import LsstErrorParams
+help(LsstErrorParams)
+```
+
+All model parameters can be overridden using keyword arguments to the error model constructor.
+Below, we explain a few of the more commonly tweaked parameters.
+
+### *Changing the observing duration*
+
+The example above uses the default settings for the LSST model, which includes 10 years of observing time.
+If instead you want to calculate errors for LSST year 1, you can pass the `nYrObs` argument to the constructor:
+
+```python
+errModel = LsstErrorModel(nYrObs=1)
+```
+
+### *Changing the band names*
+
+Another parameter you might want to tweak is the name of the bands.
+By default, the `LsstErrorModel` assumes that the LSST bands are named `u`, `g`, etc.
+If instead, the bands in your catalog are named `lsst_u`, `lsst_g`, etc., then you can instantiate the error model with a rename dictionary:
+
+```python
+errModel = LsstErrorModel(renameDict={"u": "lsst_u", "g": "lsst_g", ...})
+```
+
+This tells `LsstErrorModel` to use all of the default parameters, but just change the names it gave to all of the bands.
+If you are changing other dictionary-parameters at the same time (e.g. `nVisYr`, which sets the number of visits in each band per year), you can supply those parameters using *either* the new or old naming scheme!
+
+### *Directly setting limiting magnitudes*
+
+By default, PhotErr tries to use the provided information to calculate limiting magnitudes for you.
+If you would like to directly supply your own $5\sigma$ limits, you can do so using the `m5` parameter.
+Note that PhotErr assumes these are single-visit limiting magnitudes.
+If you want to supply coadded depths, you should also set `nYrObs=1` and `nVisYr={u: 1, g: 1, ...}`, so that the calculated coadded depths are equal to those you provided.
+
+### *Handling non-detections*
+
+The other big thing you may want to change is how the error model identifies and handles non-detections.
+
+The error model has a parameter named `sigLim`, which sets the limit for non-detections.
+By default, `sigLim=0`, which means that only negative fluxes count as non-detections, however if you set `sigLim=1`, then any magnitudes beyond the 1-sigma limit in each band will count as a non-detection.
+You can set `sigLim` to any non-negative float.
+
+The `ndMode` parameter tells the error model how to handle the non-detections.
+By default, `ndMode="flag"`, which means that the model will flag non-detections with the value set by `ndFlag`, which defaults to `np.inf`.
+However, you can also set `ndMode="sigLim"`, in which case the model will set all non-detections to the n-sigma limits set by the `sigLim` parameter described in the previous paragraph.
+Remember that `sigLim` also sets the detection threshold, so in effect, any galaxy magnitudes beyond the detection threshold will be set equal to the detection threshold.
+
+One other option is provided by the `absFlux` parameter.
+If `absFlux=True`, then the absolute value of all fluxes are taken before converting back to magnitudes.
+If combined with `sigLim=0`, this means every galaxy will have an observed flux in every band.
+This is useful if you do not want to worry about non-detections, but it results in a non-Gaussian error distribution for low-SNR sources.
+
+### Errors for extended sources
+
+PhotErr can be used to calculate errors for extended sources as well.
+You just have to pass `extendedType="auto"` or `extendedType="gaap"` to the constructor (see explanation below for the differences in these models).
+PhotErr will then look for columns in the input DataFrame that correspond to the semi-major and -minor axes of the objects, corresponding to half-light radii in arcseconds.
+By default, it looks for these in columns titled "major" and "minor", but you can change the names of these columns using the `majorCol` and `minorCol` keywords.
+
+You can also calculate limiting magnitudes for apertures of a given size by passing the `aperture` keyword to `errModel.getLimitingMags()`
+
+### Scaling the errors
+
+If you want to scale up or scale down the errors in any band(s), you can use the keyword `scale`. 
+For example, `LsstErrorModel(scale={"u": 2, "y": 2})` will have all the same properties of the default error model, except the errors in the `u` and `y` bands will be doubled.
+This allows you to answer questions like "what happens to my science if the `u` band errors are doubled."
+
+Note this only scales the band-specific error.
+The band-independent systematic error floor, `sigmaSys` is still the same, and so at high-SNR, near the systematic floor, the errors won't scale as you expect.
+
+### *Other error models*
+
+In addition to `LsstErrorModel`, which comes with the LSST defaults, PhotErr includes `EuclidErrorModel` and `RomanErrorModel`, which come with the Euclid and Roman defaults, respectively.
+Each of these models also have corresponding parameter objects: `EuclidErrorParams` and `RomanErrorParams`.
+
+You can also start with the base error model, `ErrorModel`, which is not defaulted for any specific survey.
+To instantiate `ErrorModel`, there are several required arguments that you must supply.
+To see a list and explanation of these arguments, see the docstring for `ErrorParams`.
+
+# Explanation of the error model
+
+### *The point source model*
+
+To derive the [Ivezic (2019)](https://arxiv.org/abs/0805.2366) error model, we start with the noise-to-signal ratio (NSR) for an object with photon count $C$ and background noise $N_0$ (which depends on seeing, read-out noise, etc.):
+
+$$
+NSR^2 = \frac{N_0^2 + C}{C^2}.
+$$
+
+If we define $C = C_5$ when $NSR = 1/5$, then we can solve for $N_0$ and write
+
+$$
+NSR^2 = \frac{1}{C_5} \left( \frac{C_5}{C} \right) + \left[ \left( \frac{1}{5} \right)^2 - \frac{1}{C_5} \right] \left( \frac{C_5}{C} \right)^2.
+$$
+
+Defining $x = \frac{C_5}{C} = 10 ^{(m - m_5) / 2.5}$ and $\gamma = \left( \frac{1}{5} \right)^2 - \frac{1}{C_5}$, we have
+
+$$
+NSR^2 = (0.04 - \gamma) x + \gamma x^2 ~~ (\text{mag}^2).
+$$
+
+In the high signal-to-noise ratio (SNR) limit, $NSR \ll 1$, and we can approximate
+
+$$
+\sigma_\text{rand} = 2.5 \log_{10}\left( 1 + NSR \right) \approx NSR.
+$$
+
+This approximation yields Equation 5 from [Ivezic (2019)](https://arxiv.org/abs/0805.2366).
+In PhotErr, we do not make this approximation so that the error model generalizes to the low SNR regime.
+In addition, while the high-SNR model assumes photometric errors are Gaussian in magnitude space, we model errors as Gaussian in flux space.
+However, both of these high-SNR approximations can be restored with the keyword `highSNR=True`.
+
+The LSST error model uses the parameters from [Ivezic (2019)](https://arxiv.org/abs/0805.2366).
+The Euclid and Roman error models follow [Graham (2020)](https://arxiv.org/abs/2004.07885) in setting $\gamma = 0.04$, which is nearly identical to the values for Rubin (which are all $\sim 0.039$).
+
+In addition to the random photometric error above, we include a system error of $\sigma_\text{sys} = 0.005$ which is added in quadrature to random error. Note that the system error can be changed using the keyword `sigmaSys`.
+
+After adding photometric errors to the catalog, PhotErr recalculates the photometric error from the "observed" magnitudes.
+This is so that the reported photometric errors do not provide a deterministic link back to the true magnitudes.
+This behavior can be disabled by setting `decorrelate=False`.
+
+### *The extended source model*
+
+The [Ivezic (2019)](https://arxiv.org/abs/0805.2366) model calculates errors for point sources.
+To model errors for extended sources, we use Equation 5 from [van den Busch (2020)](http://arxiv.org/abs/2007.01846):
+
+$$
+NSR_\text{ext} \propto
+NSR_\text{pt} \sqrt{\frac{A_\text{ap}}{A_\text{psf}}},
+$$
+
+where $A_\text{ap}$ is the area of the source aperture, and $A_\text{psf}$ is the area of the PSF.
+We set the proportionality constant to unity, so that when $A_\text{ap} \to A_\text{psf}$, we recover the error for a point source.
+
+We include two different models for calculating the aperture area. The "auto" method from [van den Busch (2020)](http://arxiv.org/abs/2007.01846) calculates the semi-major and -minor axes of the aperture ( $a_\text{ap}$ and $b_\text{ap}$) from the semi-major and -minor axes of the galaxy ( $a_\text{gal}$ and $b_\text{gal}$, corresponding to half-light radii):
+
+$$
+a_\text{ap} = \sqrt{\sigma_\text{psf}^2 + (2.5 a_\text{gal})^2},
+\quad
+b_\text{ap} = \sqrt{\sigma_\text{psf}^2 + (2.5 b_\text{gal})^2},
+$$
+
+where $\sigma\_\text{psf} = \text{FWHM}\_\text{psf} / 2.355$ is the PSF standard deviation.
+The formula for the area of an ellipse is then used to calculate the aperture area: $A_\text{ap} = \pi a_\text{ap} b_\text{ap}$.
+
+The "gaap" method for extended sources ([Kuijken 2019](https://arxiv.org/abs/1902.11265)) is nearly identical, except that it adds a minimum aperture diameter in quadrature when calculating $a_\text{ap}$ and $b_\text{ap}$, and then clips aperture diameters above a certain maximum.
+
+Calculating errors for extended sources requires columns in the galaxy catalog corresponding to the semi-major and -minor axes of the galaxies (with the length scale corresponding to the half-light radius).
+You can set the names of these columns using the keywords `majorCol` and `minorCol`.
+
+# Authors
+
+[John Franklin Crenshaw](https://jfcrenshaw.github.io) \
+[Ziang Yan](https://yanzastro.github.io)
+
+[*Contributors guide*](CONTRIBUTING.md)
 
-setup(**setup_kwargs)
```

