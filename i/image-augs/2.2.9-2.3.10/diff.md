# Comparing `tmp/image_augs-2.2.9.tar.gz` & `tmp/image_augs-2.3.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/image_augs-2.2.9.tar", last modified: Tue Apr 25 07:32:26 2023, max compression
+gzip compressed data, was "dist/image_augs-2.3.10.tar", last modified: Wed Apr 26 13:31:50 2023, max compression
```

## Comparing `image_augs-2.2.9.tar` & `image_augs-2.3.10.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-25 07:32:26.000000 image_augs-2.2.9/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     8486 2023-04-25 07:32:26.000000 image_augs-2.2.9/PKG-INFO
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     7906 2023-04-25 07:14:06.000000 image_augs-2.2.9/README.md
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-25 07:32:26.000000 image_augs-2.2.9/classification/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:53.000000 image_augs-2.2.9/classification/__init__.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     9953 2023-03-29 13:10:42.000000 image_augs-2.2.9/classification/classification_.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    12643 2023-04-21 14:07:26.000000 image_augs-2.2.9/classification/classification_combined.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     2006 2023-03-27 09:44:23.000000 image_augs-2.2.9/classification/logging_util.py
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-25 07:32:26.000000 image_augs-2.2.9/image_augs.egg-info/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     8486 2023-04-25 07:32:26.000000 image_augs-2.2.9/image_augs.egg-info/PKG-INFO
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      723 2023-04-25 07:32:26.000000 image_augs-2.2.9/image_augs.egg-info/SOURCES.txt
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        1 2023-04-25 07:32:26.000000 image_augs-2.2.9/image_augs.egg-info/dependency_links.txt
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      241 2023-04-25 07:32:26.000000 image_augs-2.2.9/image_augs.egg-info/requires.txt
--rw-rw-r--   0 souviks   (1001) souviks   (1001)       49 2023-04-25 07:32:26.000000 image_augs-2.2.9/image_augs.egg-info/top_level.txt
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-25 07:32:26.000000 image_augs-2.2.9/instance_seg/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:39.000000 image_augs-2.2.9/instance_seg/__init__.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    17394 2023-04-25 06:55:24.000000 image_augs-2.2.9/instance_seg/augment_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    23719 2023-04-25 07:05:20.000000 image_augs-2.2.9/instance_seg/json_reader_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     2133 2023-03-29 13:20:57.000000 image_augs-2.2.9/instance_seg/logging_util.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     4364 2023-04-10 10:20:24.000000 image_augs-2.2.9/instance_seg/utils_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      513 2023-03-30 08:41:48.000000 image_augs-2.2.9/instance_seg/yml_writer_poly.py
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-25 07:32:26.000000 image_augs-2.2.9/object_detection_new/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2022-11-01 10:58:34.000000 image_augs-2.2.9/object_detection_new/__init__.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    17537 2023-04-25 07:25:05.000000 image_augs-2.2.9/object_detection_new/augmentation_rect.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     2133 2023-04-23 18:52:17.000000 image_augs-2.2.9/object_detection_new/logging_util.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    23341 2023-04-25 07:27:32.000000 image_augs-2.2.9/object_detection_new/txt_reader_rect.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     4796 2023-04-21 10:28:10.000000 image_augs-2.2.9/object_detection_new/utils_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      510 2023-04-21 12:43:02.000000 image_augs-2.2.9/object_detection_new/yml_writer_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)       38 2023-04-25 07:32:26.000000 image_augs-2.2.9/setup.cfg
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      998 2023-03-29 09:59:13.000000 image_augs-2.2.9/setup.py
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-26 13:31:50.000000 image_augs-2.3.10/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     8487 2023-04-26 13:31:50.000000 image_augs-2.3.10/PKG-INFO
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     7906 2023-04-25 07:14:06.000000 image_augs-2.3.10/README.md
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-26 13:31:50.000000 image_augs-2.3.10/classification/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:53.000000 image_augs-2.3.10/classification/__init__.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     9929 2023-04-26 10:51:29.000000 image_augs-2.3.10/classification/classification_.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    15771 2023-04-26 11:03:13.000000 image_augs-2.3.10/classification/classification_combined.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     2006 2023-03-27 09:44:23.000000 image_augs-2.3.10/classification/logging_util.py
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-26 13:31:50.000000 image_augs-2.3.10/image_augs.egg-info/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     8487 2023-04-26 13:31:50.000000 image_augs-2.3.10/image_augs.egg-info/PKG-INFO
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      723 2023-04-26 13:31:50.000000 image_augs-2.3.10/image_augs.egg-info/SOURCES.txt
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        1 2023-04-26 13:31:50.000000 image_augs-2.3.10/image_augs.egg-info/dependency_links.txt
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      363 2023-04-26 13:31:50.000000 image_augs-2.3.10/image_augs.egg-info/requires.txt
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)       49 2023-04-26 13:31:50.000000 image_augs-2.3.10/image_augs.egg-info/top_level.txt
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-26 13:31:50.000000 image_augs-2.3.10/instance_seg/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:39.000000 image_augs-2.3.10/instance_seg/__init__.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    18793 2023-04-26 13:30:48.000000 image_augs-2.3.10/instance_seg/augment_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    28547 2023-04-26 13:05:10.000000 image_augs-2.3.10/instance_seg/json_reader_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     2133 2023-03-29 13:20:57.000000 image_augs-2.3.10/instance_seg/logging_util.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     4719 2023-04-26 13:22:59.000000 image_augs-2.3.10/instance_seg/utils_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      513 2023-03-30 08:41:48.000000 image_augs-2.3.10/instance_seg/yml_writer_poly.py
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-26 13:31:50.000000 image_augs-2.3.10/object_detection_new/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2022-11-01 10:58:34.000000 image_augs-2.3.10/object_detection_new/__init__.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    18848 2023-04-26 13:09:06.000000 image_augs-2.3.10/object_detection_new/augmentation_rect.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     2133 2023-04-23 18:52:17.000000 image_augs-2.3.10/object_detection_new/logging_util.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    27750 2023-04-26 11:46:09.000000 image_augs-2.3.10/object_detection_new/txt_reader_rect.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     4844 2023-04-26 08:52:52.000000 image_augs-2.3.10/object_detection_new/utils_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      510 2023-04-25 08:31:35.000000 image_augs-2.3.10/object_detection_new/yml_writer_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)       38 2023-04-26 13:31:50.000000 image_augs-2.3.10/setup.cfg
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      998 2023-03-29 09:59:13.000000 image_augs-2.3.10/setup.py
```

### Comparing `image_augs-2.2.9/PKG-INFO` & `image_augs-2.3.10/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image_augs
-Version: 2.2.9
+Version: 2.3.10
 Summary: Image Augs supports Augmentation for Object Detection , Instance Segmentation and classification tasks.
 Author: Souvik Saha
 Author-email: ssouvik.191@gmail.com
 Keywords: machine_learning,development,data_augmentations
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `image_augs-2.2.9/README.md` & `image_augs-2.3.10/README.md`

 * *Files identical despite different names*

### Comparing `image_augs-2.2.9/classification/classification_.py` & `image_augs-2.3.10/classification/classification_.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             transform = A.Compose([A.augmentations.geometric.resize.Resize(self.height,self.width),A.HorizontalFlip(p=1.0),])
             
             augmented_image = transform(image=image)['image']
 
             yield augmented_image 
 
         except Exception as e:
-            logger.warning(f'horizontal flip problem  , desc : {e}')
+            logger.error(f'horizontal flip problem  , desc : {e}')
 
     def blur(self,image):
         '''
         This function will blur images.
         Blur values are selected by random. (3,3) , (5,5)
 
         : param image : accepts cv2.imread() image
@@ -63,15 +63,15 @@
         try:
             image = cv2.resize(image,(self.width,self.height),interpolation=cv2.INTER_CUBIC)
             blurrr = [(3,3),(5,5),(7,7)]
             blurrr = secrets.choice(blurrr)
             yield cv2.GaussianBlur(image ,blurrr,0) 
         
         except Exception as e:
-            logger.warning(f'blur  problem  , desc : {e}')
+            logger.error(f'blur  problem  , desc : {e}')
 
 
     def noise(self,image):
 
         '''
         This function will add noise to the images.
         Noise values are selected by random.
@@ -84,26 +84,26 @@
             image = cv2.resize(image,(self.width,self.height),interpolation=cv2.INTER_CUBIC)
             noise = [0.001,0.002,0.003,0.004]
             noise_1 = secrets.choice(noise)
             noise_img = random_noise(image, mode='s&p',amount=noise_1)
             noise_img = np.array(255*noise_img, dtype = 'uint8')
             yield noise_img 
         except Exception as e:
-            logger.warning(f'noise problem  , desc : {e}')
+            logger.error(f'noise problem  , desc : {e}')
     
     def randomBrightness(self,image):
         try:
             transform = A.Compose([A.augmentations.geometric.resize.Resize(self.height,self.width),
                                 A.augmentations.transforms.RandomBrightnessContrast(brightness_limit=0.2, contrast_limit=0.0, brightness_by_max=True, always_apply=False, p=1)])
         
             augmented_image = transform(image=image)['image']
             yield augmented_image
 
         except Exception as e:
-            logger.warning(f'randomBrightness problem  , desc : {e}')
+            logger.error(f'randomBrightness problem  , desc : {e}')
     
     def randomContrast(self,image):
 
         try:
             image = cv2.resize(image,(self.width,self.height),interpolation=cv2.INTER_CUBIC)
             level = secrets.choice(range(30,55))
             factor = (259 * (level + 255)) / (255 * (259 - level))
@@ -112,15 +112,15 @@
             rgb = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
             im_pil = Image.fromarray(rgb)
             con = im_pil.point(contrast)
             bgr = np.asarray(con)
             contrast_im = cv2.cvtColor(bgr, cv2.COLOR_RGB2BGR)
             yield contrast_im
         except Exception as e:
-            logger.warning(f'randomConrast problem  , desc : {e}')
+            logger.error(f'randomConrast problem  , desc : {e}')
     
     #need to change value
     # def fog(self,image):
     #     transform = A.Compose([A.augmentations.geometric.resize.Resize(self.height,self.width),
     #                            A.augmentations.transforms.RandomFog(fog_coef_lower=0.3, fog_coef_upper=1, alpha_coef=0.08, always_apply=False, p=1)])
 
     #     augmented_image = transform(image=image)['image']
@@ -145,26 +145,26 @@
         try:
             transform = A.Compose([A.augmentations.geometric.resize.Resize(self.height,self.width),
                                     A.augmentations.transforms.RandomShadow (shadow_roi=(0, 0.8, 1, 1), num_shadows_lower=1, num_shadows_upper=2, shadow_dimension=5, always_apply=False, p=1)])
 
             augmented_image = transform(image=image)['image']
             yield augmented_image
         except Exception as e:
-            logger.warning(f'randomShadow problem  , desc : {e}')
+            logger.error(f'randomShadow problem  , desc : {e}')
     
     def sharpen(self,image):
         try:
             transform = A.Compose([A.augmentations.geometric.resize.Resize(self.height,self.width),
                                     A.augmentations.transforms.Sharpen (alpha=(0.1, 0.5), lightness=(0.3, 0.6), always_apply=False, p=1)])
     
             augmented_image = transform(image=image)['image']
             yield augmented_image
 
         except Exception as e:
-            logger.warning(f'sharpen problem  , desc : {e}')
+            logger.error(f'sharpen problem  , desc : {e}')
 
     def hue(self,image):
         '''
         This function will add hue to the images.
         Hue values are selected by random.
 
         : param image : accepts cv2.imread() image
@@ -177,15 +177,15 @@
             hsv = cv2.cvtColor(image, cv2.COLOR_BGR2HSV)
             h,s,v = cv2.split(hsv)
             hnew = np.mod(h + int(hue_choice), 180).astype(np.uint8)
             hsv_new = cv2.merge([hnew,s,v])
             bgr_new = cv2.cvtColor(hsv_new, cv2.COLOR_HSV2BGR)
             yield bgr_new
         except Exception as e:
-            logger.warning(f'HUE problem  , desc : {e}')
+            logger.error(f'HUE problem  , desc : {e}')
     
     def saturation(self,image):
         '''
         This function will add saturation to the images.
         Hue values are selected by random.
 
         : param image : accepts cv2.imread() image
@@ -201,52 +201,52 @@
             converter = ImageEnhance.Color(im_pil)
             img2 = converter.enhance(sat_level)
             saturated_image = np.asarray(img2)
             saturated_image = cv2.cvtColor(saturated_image, cv2.COLOR_RGB2BGR)
             yield saturated_image
 
         except Exception as e:
-            logger.warning(f'saturation problem  , desc : {e}')
+            logger.error(f'saturation problem  , desc : {e}')
 
     def perspective(self,image):
         try:
             image = cv2.resize(image,(self.width,self.height),interpolation=cv2.INTER_CUBIC)
             rows,cols = image.shape[:2]
             pts1 = np.float32([[0,0],[cols-1,0],[0,rows-1],[cols-1,rows-1]])
             pts2 = np.float32(pts1 + np.random.normal(0, 50, size=pts1.shape))
             M = cv2.getPerspectiveTransform(pts1, pts2)
 
 
             transformed_img = cv2.warpPerspective(image, M, (cols,rows))
             yield transformed_img
         except Exception as e:
-            logger.warning(f'Perspective problem  , desc : {e}')
+            logger.error(f'Perspective problem  , desc : {e}')
     
     def zoom(self,image):
 
         try:
             zoom = secrets.choice([0.6,0.7,0.8,0.9,1.2,1.3,1.4])
             transform = A.Compose([A.augmentations.geometric.resize.Resize(self.height,self.width),
                                     A.augmentations.geometric.transforms.Affine(shear=None,p=1.0,scale=zoom)])
         
             augmented_image = transform(image=image)['image']
             yield augmented_image
         except Exception as e:
-            logger.warning(f'zoom problem  , desc : {e}')
+            logger.error(f'zoom problem  , desc : {e}')
     
     def translation(self,image):
         try:
             image = cv2.resize(image,(self.width,self.height),interpolation=cv2.INTER_CUBIC)    
             rows,cols = image.shape[:2]
             dx,dy = np.random.randint(-75,75,2)
             M = np.float32([[1,0,dx],[0,1,dy]])
             translated_img = cv2.warpAffine(image, M, (cols,rows))
             yield translated_img
         except Exception as e:
-            logger.warning(f'translation problem  , desc : {e}')
+            logger.error(f'translation problem  , desc : {e}')
 
 
     @staticmethod
     def visualize(image):
         cv2.imshow('im',image)
         cv2.waitKey(0)
```

### Comparing `image_augs-2.2.9/classification/logging_util.py` & `image_augs-2.3.10/classification/logging_util.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.2.9/image_augs.egg-info/PKG-INFO` & `image_augs-2.3.10/image_augs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-augs
-Version: 2.2.9
+Version: 2.3.10
 Summary: Image Augs supports Augmentation for Object Detection , Instance Segmentation and classification tasks.
 Author: Souvik Saha
 Author-email: ssouvik.191@gmail.com
 Keywords: machine_learning,development,data_augmentations
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `image_augs-2.2.9/image_augs.egg-info/SOURCES.txt` & `image_augs-2.3.10/image_augs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `image_augs-2.2.9/instance_seg/augment_poly.py` & `image_augs-2.3.10/instance_seg/augment_poly.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def __init__(self) -> None:
         
         # self.height = height
         
         console.print('[bold green] [+] Image augmentation module loaded....[bold green]')
         logger.info('Image Augmentation module loaded successfully...')
            
-    def image_rotate(self,image:np.array,polygons:Polygon,H,W,rotation_angle:int=12) -> Tuple[Polygon,np.array]:
+    def image_rotate(self,image:np.array,polygons:Polygon,H,W,rotation_angle:int=16) -> Tuple[Polygon,np.array]:
 
         '''
         Image Rotate will rotate an image and its polygon points to a desired angle
 
         : param image           : accepts cv2.imread() images
         : param polygons        : Polygon points of that image
         : param rotation angle  : desired angle you want to rotate (-angle , angle)
@@ -44,88 +44,91 @@
         : return :
         : new polygon points    : it will return after rotation polygon points
         : aug rotated image     : it will return rotated image
         
         '''
         try:
             aug = iaa.Sequential([iaa.Rotate((-rotation_angle,rotation_angle),fit_output=False),
-                                iaa.SaltAndPepper(p=(0.01,0.06)),
-                                iaa.Multiply((0.2, 1.5), per_channel=1.0,),
+                                iaa.SaltAndPepper(p=(0.01,0.03)),
+                                iaa.Multiply((0.2, 1.1), per_channel=1.0,),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_rotated_image = aug(polygons=polygons,image=image)
+            new_points_polygons = new_points_polygons.remove_out_of_image().clip_out_of_image()
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_rotated_image
         except Exception as e:
-            logger.warning(f'problem: Image rotation    desc : {e}')
+            logger.error(f'problem: Image rotation    desc : {e}')
         
         
-    def image_affine(self,image:np.array,polygons:Polygon,H,W,scale_range:range=(0.5,1.7)) -> Tuple[Polygon,np.array]:
+    def image_affine(self,image:np.array,polygons:Polygon,H,W,scale_range:range=(0.5,1.5)) -> Tuple[Polygon,np.array]:
         try:
             aug = iaa.Sequential([iaa.Affine(scale=scale_range,fit_output=False,),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
+            new_points_polygons = new_points_polygons.remove_out_of_image().clip_out_of_image()
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
         except Exception as e:
-            logger.warning(f'problem: Image affine    desc : {e}')
+            logger.error(f'problem: Image affine    desc : {e}')
 
-    def image_perspective_transform(self,image:np.array,polygons:Polygon,H,W,scale_range:range=(0.10,0.17)) -> Tuple[Polygon,np.array]:
+    def image_perspective_transform(self,image:np.array,polygons:Polygon,H,W,scale_range:range=(0.10,0.12)) -> Tuple[Polygon,np.array]:
         try:
             aug = iaa.Sequential([iaa.PerspectiveTransform(scale=scale_range,fit_output=False),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
+            new_points_polygons = new_points_polygons.remove_out_of_image().clip_out_of_image()
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
 
         except Exception as e:
-            logger.warning(f'problem: Image perspective transform    desc : {e}')
+            logger.error(f'problem: Image perspective transform    desc : {e}')
 
 
     def image_noise(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
             choice = random.choice([0,1])
             if choice == 0:
-                aug = iaa.Sequential([iaa.SaltAndPepper(p=(0.01,0.06)),
+                aug = iaa.Sequential([iaa.SaltAndPepper(p=(0.01,0.05)),
                                 iaa.Resize({"height": H, "width": W})])
             else:
                 # aug = iaa.AdditiveLaplaceNoise(scale=(5,0.1*200), per_channel=True)
-                aug = iaa.Sequential([iaa.SaltAndPepper(p=(0.01,0.06),per_channel=True),
+                aug = iaa.Sequential([iaa.SaltAndPepper(p=(0.01,0.05),per_channel=True),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
 
         except Exception as e:
-            logger.warning(f'problem: Image noise    desc : {e}')
+            logger.error(f'problem: Image noise    desc : {e}')
 
 
     def image_blur(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
             aug = iaa.Sequential([iaa.GaussianBlur(sigma=(1.2, 4.0)),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
         
         except Exception as e:
-            logger.warning(f'problem: Image blur    desc : {e}')
+            logger.error(f'problem: Image blur    desc : {e}')
 
     
     #chnag thissssssss
     def image_hue(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
             # aug = iaa.Multiply((0.5, 1.5), per_channel=0.5)
             aug = iaa.Sequential([iaa.Multiply((0.5, 1.5), per_channel=1.0,),
                                   iaa.WithBrightnessChannels(iaa.Add((-40,40))),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
         except Exception as e:
-            logger.warning(f'problem: Image hue    desc : {e}')
+            logger.error(f'problem: Image hue    desc : {e}')
 
     def image_brightness(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
             ranges = random.choice([0,1])
             if ranges == 0:
                 # aug = iaa.WithBrightnessChannels(iaa.Add((10,40)))
                 aug = iaa.Sequential([iaa.WithBrightnessChannels(iaa.Add((10,50))),
@@ -135,97 +138,99 @@
                 aug = iaa.Sequential([iaa.WithBrightnessChannels(iaa.Add((-50,-10))),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
 
         except Exception as e:
-            logger.warning(f'problem: Image brightness    desc : {e}')
+            logger.error(f'problem: Image brightness    desc : {e}')
 
     def image_change_colorTemperature(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
             # aug =  iaa.ChangeColorTemperature((1100, 10000))
             aug = iaa.Sequential([iaa.ChangeColorTemperature((1100, 6500)),
                                   iaa.GaussianBlur(sigma=(1.2, 2.7)),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
         except Exception as e:
-            logger.warning(f'problem: Image color temp    desc : {e}')
+            logger.error(f'problem: Image color temp    desc : {e}')
 
     def image_removeSaturation(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
             choices = random.choice([0.3,0.4,0.5,0.6,0.7,0.8,0.9])
             aug = iaa.Sequential([iaa.RemoveSaturation(choices),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
 
         except Exception as e:
-            logger.warning(f'problem: Image removeSaturation    desc : {e}')
+            logger.error(f'problem: Image removeSaturation    desc : {e}')
 
     def image_contrast(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
         
             aug = iaa.Sequential([iaa.LinearContrast((0.8, 1.7)),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
 
         except Exception as e:
-            logger.warning(f'problem: Image contrast    desc : {e}')
+            logger.error(f'problem: Image contrast    desc : {e}')
 
     def image_upFlip(self,image:np.array,polygons:Polygon,H,W,flip_percentage:float=1.0) -> Tuple[Polygon,np.array]:
         try:
             # aug =  iaa.Flipud(flip_percentage)
             aug = iaa.Sequential([iaa.Flipud(flip_percentage,),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
         except Exception as e:
-            logger.warning(f'problem: Image uplfip    desc : {e}')
+            logger.error(f'problem: Image uplfip    desc : {e}')
 
     def image_shear(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
             choice = random.choice([0,1])
             if choice == 0:
                 # aug =  iaa.ShearX(shear=(-12,12))
-                aug = iaa.Sequential([iaa.ShearX(shear=(-16,16),fit_output=False),
+                aug = iaa.Sequential([iaa.ShearX(shear=(-18,18),fit_output=False),
                                 iaa.Resize({"height": H, "width": W})])
             else:
                 # aug =  iaa.ShearY(shear=(-12,12))
-                aug = iaa.Sequential([iaa.ShearY(shear=(-16,16),fit_output=False),
+                aug = iaa.Sequential([iaa.ShearX(shear=(-18,18),fit_output=False),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
+            new_points_polygons = new_points_polygons.remove_out_of_image().clip_out_of_image()
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
 
         except Exception as e:
-            logger.warning(f'problem: Image shear    desc : {e}')
+            logger.error(f'problem: Image shear    desc : {e}')
 
     def image_rotate90(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
             choice = random.choice([0,1])
             if choice == 0:
                 # aug =  iaa.Rotate(rotate=90,fit_output=True)
                 aug = iaa.Sequential([iaa.Rotate(rotate=90,fit_output=False),
                                 iaa.Resize({"height": H, "width": W})])
             else:
                 # aug =  iaa.Rotate(rotate=-90,fit_output=True)
                 aug = iaa.Sequential([iaa.Rotate(rotate=-90,fit_output=False),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
+            new_points_polygons = new_points_polygons.remove_out_of_image().clip_out_of_image()
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
         except Exception as e:
-            logger.warning(f'problem: Image rotate90   desc : {e}')
+            logger.error(f'problem: Image rotate90   desc : {e}')
             
 
     # beta mode
     def image_weatherChange(self,image:np.array,polygons:Polygon,H,W,rain_speed:range=(0.09, 0.2)) -> Tuple[Polygon,np.array]:
         try:
             choice = random.choice([0,1,2])
             if choice == 0:
@@ -242,90 +247,93 @@
                                 iaa.Resize({"height": H, "width": W})])
 
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
 
         except Exception as e:
-            logger.warning(f'problem: Image weatherchange    desc : {e}')
+            logger.error(f'problem: Image weatherchange    desc : {e}')
 
     def image_cutOut(self,image:np.array,polygons:Polygon,H,W,number_of_square:int=2,size:float=0.1) -> Tuple[Polygon,np.array]:
         try:
             # aug =  iaa.Cutout(fill_mode="constant", cval=random.choice([128,255]),size=size,nb_iterations=number_of_square)
             aug = iaa.Sequential([iaa.Cutout(fill_mode="constant", cval=random.choice([128,255]),size=size,nb_iterations=number_of_square),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
         except Exception as e:
-            logger.warning(f'problem: Image cutout    desc : {e}')
+            logger.error(f'problem: Image cutout    desc : {e}')
     
     def blur_and_noise(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
             aug = iaa.Sequential([iaa.GaussianBlur(sigma=(0.8, 3.5)),
                                 iaa.Resize({"height": H, "width": W}),
                                 iaa.SaltAndPepper(p=(0.02,0.07))])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
 
         except Exception as e:
-            logger.warning(f'problem: Image blur and noise    desc : {e}')
+            logger.error(f'problem: Image blur and noise    desc : {e}')
     
     def mixed_aug_1(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
-            aug = iaa.Sequential([iaa.Affine(scale=(0.5,1.2),fit_output=False),
+            aug = iaa.Sequential([iaa.Affine(scale=(0.5,1.6),fit_output=False),
                                 iaa.Multiply((0.5, 1.5), per_channel=0.5),
                                 iaa.Resize({"height": H, "width": W})])
             
                                 
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
+            new_points_polygons = new_points_polygons.remove_out_of_image().clip_out_of_image()
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
         except Exception as e:
-            logger.warning(f'problem: Mix aug 1    desc : {e}')
+            logger.error(f'problem: Mix aug 1    desc : {e}')
     
     def mixed_aug_2(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
             choices = random.choice([0.4,0.5,0.6,0.7,0.8])
             # aug = iaa.RemoveSaturation(choices)
-            aug = iaa.Sequential([iaa.Rotate((-10,10),fit_output=False),
+            aug = iaa.Sequential([iaa.Rotate((-13,13),fit_output=False),
                                 iaa.WithBrightnessChannels(iaa.Add((-40,40))),
                                 iaa.RemoveSaturation(choices),
-                                iaa.PerspectiveTransform(scale=(0.08,0.15),fit_output=False),
+                                iaa.PerspectiveTransform(scale=(0.08,0.12),fit_output=False),
                                 iaa.Resize({"height": H, "width": W})])
             
                                 
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
+            new_points_polygons = new_points_polygons.remove_out_of_image().clip_out_of_image()
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
         except Exception as e:
-            logger.warning(f'problem: mix aug 2    desc : {e}')
+            logger.error(f'problem: mix aug 2    desc : {e}')
     
     def mixed_aug_3(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
             choice = random.choice([0,1])
             if choice == 0:
                 aug = iaa.Sequential([iaa.ShearX(shear=(-15,15),fit_output=False),
-                                    iaa.GaussianBlur(sigma=(0.8, 1.6)),
+                                    iaa.GaussianBlur(sigma=(0.8, 2.8)),
                                     iaa.ChangeColorTemperature((1100, 7000)),
                                     iaa.Resize({"height": H, "width":W})])
             
             else:
-                aug = iaa.Sequential([iaa.ShearY(shear=(-10,10),fit_output=False),
+                aug = iaa.Sequential([iaa.ShearY(shear=(-15,15),fit_output=False),
                                     iaa.LinearContrast((0.8, 1.6)),
                                     iaa.Resize({"height": H, "width":W})])
     
                             
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
+            new_points_polygons = new_points_polygons.remove_out_of_image().clip_out_of_image()
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
         
         except Exception as e:
-            logger.warning(f'problem: Mix aug 3    desc : {e}')
+            logger.error(f'problem: Mix aug 3    desc : {e}')
     
     def mixed_aug_4(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
             choice = random.choice([-90,90])
             choices =  random.choice([0,1])
             
             if choices == 0:
@@ -340,19 +348,31 @@
                 aug = iaa.Sequential([iaa.Rotate(rotate=choice,fit_output=False),
                                 iaa.WithBrightnessChannels(iaa.Add((-20,20))),
                                 iaa.SaltAndPepper(p=(0.01,0.06)),
                                 iaa.Resize({"height": H, "width": W})])
             
                                 
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
+            new_points_polygons = new_points_polygons.remove_out_of_image().clip_out_of_image()
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
 
         except Exception as e:
-            logger.warning(f'problem: Mixed aug 4    desc : {e}')
+            logger.error(f'problem: Mixed aug 4    desc : {e}')
+    
+    def image_motionBlur(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
+        try:
+            aug = iaa.Sequential([iaa.MotionBlur(k=15, angle=[-45, 45]),
+                                iaa.Resize({"height": H, "width": W})])
+            new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
+            new_points_polygons = new_points_polygons.polygons
+            yield new_points_polygons , aug_affine_image
+        
+        except Exception as e:
+            logger.error(f'problem: Image motion blur    desc : {e}')
```

### Comparing `image_augs-2.2.9/instance_seg/json_reader_poly.py` & `image_augs-2.3.10/object_detection_new/txt_reader_rect.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from tornado import concurrent
 import cv2
 import uuid
-from imgaug.augmentables.polys import Polygon, PolygonsOnImage
+from imgaug.augmentables.bbs import BoundingBox, BoundingBoxesOnImage
 from rich.console import Console
 from rich.traceback import install
 from rich.progress import track
 
 import json
 import os
 import glob
 import shutil
 from typing import NewType , Union
 
-from instance_seg.augment_poly import *
-from instance_seg import utils_poly
-from instance_seg import yml_writer_poly
-import instance_seg.logging_util as logging_util
+from object_detection_new.augmentation_rect import *
+from object_detection_new import utils_poly
+from object_detection_new import yml_writer_poly
+import object_detection_new.logging_util as logging_util
 
 
 install()
 console = Console()
 logger = logging_util.get_logger(os.path.basename(__file__).split('.')[0])
 keep_aspect_ratio = NewType('keep-aspect-ratio','str')
 keep_original_image_height = NewType('keep_original_image_height','str')
@@ -27,21 +27,22 @@
 
 
 '''
 Code logic starts from here.
 
 '''
 
-class PolygonAugmentation():
-    def __init__(self,aug_save_folder_name:os.path='polygon_augmentation',yolo:bool=True) -> None:
+class RectAugmentation():
+    def __init__(self,aug_save_folder_name:os.path='rect_augmentation') -> None:
         self.aug_save_folder_name = aug_save_folder_name
-        self.augment = ImageAugmentation()
+        self.augment = ImageAugmentationBox()
         self.store_dict:dict = dict()
         self.counter:int = 0
-        self.yolo = yolo
+
+     
 
         '''
         : param aug_save_folder_name : give a path where you want to save your augmentations 
         : param image_resize : Image resizing for augmentations
         '''
         
         
@@ -53,226 +54,339 @@
             os.makedirs(f'{self.aug_save_folder_name}/train/labels')
             console.print(f'[bold blue] [+] {self.aug_save_folder_name}/[bold blue] folder - created..')
         
         if not os.path.exists(f'{self.aug_save_folder_name}/test/images') or not os.path.exists(f'{self.aug_save_folder_name}/test/labels'):
             os.makedirs(f'{self.aug_save_folder_name}/test/images')
             os.makedirs(f'{self.aug_save_folder_name}/test/labels')
             
-        if type(self.yolo) != bool:
-            raise TypeError(f'Expected type for yolo is bool, you provided yolo type as {type(self.yolo)}')  
+       
           
         self.train_images_path = f'{self.aug_save_folder_name}/train/images'
         self.train_labels_path = f'{self.aug_save_folder_name}/train/labels'
         self.test_images_path = f'{self.aug_save_folder_name}/test/images'
         self.test_labels_path = f'{self.aug_save_folder_name}/test/labels'
     
-        logger.info('ImageAugments module loaded...')
+        logger.info('RectAugmentation module loaded...')
+
 
-    def json_converter(self,image:os.path):
+    def txt_converter(self,image:os.path):
         '''
-        Json converter will convert json to polygon acceptable format.
+        txt converter will convert json to polygon acceptable format.
         It will return image and converted json
 
         : param image : require full path of a image 
         
         : return :
         : im_read       : it will return cv2.imread() image.
         : poly on image : it will return json converted polygon points 
         
         
         '''
         try:
+
             # temporary to store the result
-            datas = []
+            new_datas = list()
+  
+       
             # first we are checking the extension endswith .json or not 
             # then we read the image and json file
-            if not image.endswith('.json'):
+            if not image.endswith('.txt'):
                     im_read = cv2.imread(image)
-        
-                    JSON = image.split('.')[0] + '.json'
-                    with open(JSON) as f:
-                        data = json.load(f)
-                        annotations = data['shapes']
-                        for i ,annotation in enumerate(annotations):
+      
+                    image_H , image_W , c = im_read.shape
+                    TEXT = image.split('.')[0] + '.txt'
+                    with open(TEXT) as f:
+                        data = f.readlines()
+                     
+                        for datas in data:
+                            strip_data = datas.rstrip().split()
+                            strip_data = list(map(float,strip_data))
+                            
+                            x1,y1,x2,y2 = utils_poly.convert_to_normal_bbox(strip_data[1:],image_W,image_H)
+                            self.labels= int(strip_data[0])
+
                             #taking uuid
                             ids = uuid.uuid4()
-                            # getting the label
-                            self.labels = annotation['label']
-                            # we are saving the labels in the dict
-                            if self.labels in self.store_dict:
-                                pass
-                            
-                            else:
-                                self.store_dict[self.labels] = self.counter
-                                self.counter += 1
-                            
-                            #getting points from json file
-                            poly_points = annotation['points']
-                            poly_points = [tuple(lst) for lst in poly_points]
-                            # taking this in polygon function and their labels
-                            ids = Polygon(poly_points,self.labels)
-                            datas.append(ids)
+
+                            # taking this in bounding box function and their labels
+                            ids = BoundingBox(x1,y1,x2,y2,self.labels)
+                           
+                            new_datas.append(ids)
+                      
                         # input temp datas and image_shape   
-                        poly_on_image = PolygonsOnImage(datas, shape=im_read.shape)
-                        
-                        del datas
-                    
-                        yield im_read , poly_on_image
+                        rect_on_image = BoundingBoxesOnImage(new_datas, shape=im_read.shape)
+                      
+                        del new_datas
+                  
+                        yield im_read , rect_on_image
 
         except Exception as e:
-            logger.error(f'problem : Json converter  desc : {e}')       
-                   
-                  
-    def Combined_augmentation(self,im_read , poly_on_image, no_track,image_height=640 , image_width:Union[int,keep_aspect_ratio]=640, blur=True , blur_f = 0.5 , rotate=True , rotate_f = 0.5 , noise=True,noise_f=0.5,perspective=True,perspective_f = 0.5,affine=True,affine_f=0.5,
-                              brightness=True,brightness_f=0.5,hue=True,hue_f=0.5,removesaturation=True,removesaturation_f=0.5,contrast=True,contrast_f=0.5,upflip=True,upflip_f=0.5,
-                              shear=True ,shear_f=0.5, rotate90=True,rotate90_f = 0.5,blur_and_noise=True,blur_and_noise_f=0.5,image_cutout = True,image_cutout_f=0.5,
-                              mix_aug=True,mix_aug_f=0.5,temperature_change=True,temperature_change_f=0.5,weather_change=True,weather_change_f=0.5):
-        
+            logger.error(f'problem : Txt converter  desc : {e}')
+
+
+    def Combined_augmentation(self,im_read , rect_on_image, no_track,image_height=640 , image_width:Union[int,keep_aspect_ratio]=640,blur=True , blur_f = 0.5 ,motionBlur=True, motionBlur_f = 0.5, rotate=True , rotate_f = 0.5 , noise=True,noise_f=0.5,perspective=True,perspective_f = 0.5,affine=True,affine_f=0.5,
+                            brightness=True,brightness_f=0.5,hue=True,hue_f=0.5,removesaturation=True,removesaturation_f=0.5,contrast=True,contrast_f=0.5,upflip=True,upflip_f=0.5,
+                            shear=True ,shear_f=0.5, rotate90=True,rotate90_f = 0.5,blur_and_noise=True,blur_and_noise_f=0.5,image_cutout = True,image_cutout_f=0.5,
+                            mix_aug=True,mix_aug_f=0.5,temperature_change=True,temperature_change_f=0.5,weather_change=True,weather_change_f=0.5):
         
-        # combining all the augmentations here
         with concurrent.futures.ThreadPoolExecutor(max_workers=20) as executor:
-            
-            if blur:
-           
-                frac_data  = int(self.split * blur_f)
-                if no_track <= frac_data:
-                    points =  executor.submit(self.augment.image_blur,im_read,poly_on_image,image_height,image_width)
-                    p , im = next(points.result())
-                    utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
-            
             if rotate:
                 frac_data  = int(self.split * rotate_f)
-                if no_track <= frac_data:
-                    points2  = executor.submit(self.augment.image_rotate,im_read,poly_on_image,image_height,image_width) 
-                    p , im = next(points2.result())
-                    utils_poly.create_new_txt(im,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                try:
+                    if no_track <= frac_data:
                 
+                        points2  = executor.submit(self.augment.image_rotate,im_read,rect_on_image,image_height,image_width) 
+                        p , im = next(points2.result())
+                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+                except Exception as e:
+                    logger.warning(f'Image rotation problem : {e}')
+
+            if blur:
+                
+                frac_data  = int(self.split * blur_f)
+                try:
+                    if no_track <= frac_data:
+                
+                        points2  = executor.submit(self.augment.image_blur,im_read,rect_on_image,image_height,image_width) 
+                        p , im = next(points2.result())
+                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+                except:
+                  
+                    logger.warning(f'Image blur problem : {e}')
+
             if noise:
                 frac_data  = int(self.split * noise_f)
-                if no_track <= frac_data:
-                    points3  = executor.submit(self.augment.image_noise,im_read,poly_on_image,image_height,image_width) 
-                    p , im = next(points3.result())
-                    utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                try:
+                    if no_track <= frac_data:
                 
+                        points2  = executor.submit(self.augment.image_noise,im_read,rect_on_image,image_height,image_width) 
+                        p , im = next(points2.result())
+                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+
+                except Exception as e:
+                    logger.warning(f'Image noise problem : {e}')
+
             if perspective:
                 frac_data  = int(self.split * perspective_f)
-                if no_track <= frac_data:
-                    points4  = executor.submit(self.augment.image_perspective_transform,im_read,poly_on_image,image_height,image_width) 
-                    p , im = next(points4.result())
-                    utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                try:
+                    if no_track <= frac_data:
                 
+                        points2  = executor.submit(self.augment.image_perspective_transform,im_read,rect_on_image,image_height,image_width) 
+                        p , im = next(points2.result())
+                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+
+                except Exception as e:
+                    logger.warning(f'Image perpective problem : {e}')
+            
             if affine:
                 frac_data  = int(self.split * affine_f)
-                if no_track <= frac_data:
-                    points5  = executor.submit(self.augment.image_affine,im_read,poly_on_image,image_height,image_width) 
-                    p , im = next(points5.result())
-                    utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                try:
+                    if no_track <= frac_data:
                 
+                        points2  = executor.submit(self.augment.image_affine,im_read,rect_on_image,image_height,image_width) 
+                        p , im = next(points2.result())
+                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+
+                except Exception as e:
+                    logger.warning(f'Image affine problem : {e}')
+
             if brightness:
                 frac_data  = int(self.split * brightness_f)
-                if no_track <= frac_data:
-                    points6  = executor.submit(self.augment.image_brightness,im_read,poly_on_image,image_height,image_width) 
-                    p , im = next(points6.result())
-                    utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
-            
+                try:
+                    if no_track <= frac_data:
+                
+                        points2  = executor.submit(self.augment.image_brightness,im_read,rect_on_image,image_height,image_width) 
+                        p , im = next(points2.result())
+                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+
+                except Exception as e:
+                    logger.warning(f'Image brightness problem : {e}')
+
             if hue:
                 frac_data  = int(self.split * hue_f)
-                if no_track <= frac_data:
-                    points6  = executor.submit(self.augment.image_hue,im_read,poly_on_image,image_height,image_width) 
-                    p , im = next(points6.result())
-                    utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                try:
+                    if no_track <= frac_data:
                 
+                        points2  = executor.submit(self.augment.image_hue,im_read,rect_on_image,image_height,image_width) 
+                        p , im = next(points2.result())
+                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+
+                except Exception as e:
+                    logger.warning(f'Image hue problem : {e}')
+
             if removesaturation:
+
                 frac_data  = int(self.split * removesaturation_f)
-                if no_track <= frac_data:
-                    points7  = executor.submit(self.augment.image_removeSaturation,im_read,poly_on_image,image_height,image_width) 
-                    p , im = next(points7.result())
-                    utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                try:
+                    if no_track <= frac_data:
+                
+                        points2  = executor.submit(self.augment.image_removeSaturation,im_read,rect_on_image,image_height,image_width) 
+                        p , im = next(points2.result())
+                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
                 
+                except Exception as e:
+                    logger.warning(f'Image remove saturation problem : {e}')
+            
             if contrast:
                 frac_data  = int(self.split * contrast_f)
-                if no_track <= frac_data:
-                    points8 = executor.submit(self.augment.image_contrast,im_read,poly_on_image,image_height,image_width) 
-                    p , im = next(points8.result())
-                    utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                try:
+                    if no_track <= frac_data:
                 
+                        points2  = executor.submit(self.augment.image_contrast,im_read,rect_on_image,image_height,image_width) 
+                        p , im = next(points2.result())
+                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+
+                except Exception as e:
+                    logger.warning(f'Image contrast problem : {e}')
+
             if upflip:
                 frac_data  = int(self.split * upflip_f)
-                if no_track <= frac_data:
-                    points9  = executor.submit(self.augment.image_upFlip,im_read,poly_on_image,image_height,image_width) 
-                    p , im = next(points9.result())
-                    utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
-                    
+                try:
+                    if no_track <= frac_data:
+                
+                        points2  = executor.submit(self.augment.image_upFlip,im_read,rect_on_image,image_height,image_width) 
+                        p , im = next(points2.result())
+                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+
+                except Exception as e:
+                    logger.warning(f'Image upflip problem : {e}')
+
             if shear:
                 frac_data  = int(self.split * shear_f)
-                if no_track <= frac_data:
-                    points10  = executor.submit(self.augment.image_shear,im_read,poly_on_image,image_height,image_width) 
-                    p , im = next(points10.result())
-                    utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                try:
+                    if no_track <= frac_data:
                 
+                        points2  = executor.submit(self.augment.image_shear,im_read,rect_on_image,image_height,image_width) 
+                        p , im = next(points2.result())
+                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+
+                except Exception as e:
+                    logger.warning(f'Image shear problem : {e}')
+
             if rotate90:
                 frac_data  = int(self.split * rotate90_f)
-                if no_track <= frac_data:
-                    points11  = executor.submit(self.augment.image_rotate90,im_read,poly_on_image,image_height,image_width) 
-                    p , im = next(points11.result())
-                    utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                try:
+                    if no_track <= frac_data:
                 
+                        points2  = executor.submit(self.augment.image_rotate90,im_read,rect_on_image,image_height,image_width) 
+                        p , im = next(points2.result())
+                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+
+                except Exception as e:
+                    logger.warning(f'Image rotation90 problem : {e}')
+
             if blur_and_noise:
                 frac_data  = int(self.split * blur_and_noise_f)
-                if no_track <= frac_data:
-                    points12  = executor.submit(self.augment.blur_and_noise,im_read,poly_on_image,image_height,image_width) 
-                    p , im = next(points12.result())
-                    utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                try:
+                    if no_track <= frac_data:
                 
+                        points2  = executor.submit(self.augment.blur_and_noise,im_read,rect_on_image,image_height,image_width) 
+                        p , im = next(points2.result())
+                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+
+                except Exception as e:
+                    logger.warning(f'Image blur and noise problem : {e}')
+
             if image_cutout:
                 frac_data  = int(self.split * image_cutout_f)
-                if no_track <= frac_data:
-                    points13  = executor.submit(self.augment.image_cutOut,im_read,poly_on_image,image_height,image_width) 
-                    p , im = next(points13.result())
-                    utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
-            
+                try:
+                    if no_track <= frac_data:
+                
+                        points2  = executor.submit(self.augment.image_cutOut,im_read,rect_on_image,image_height,image_width) 
+                        p , im = next(points2.result())
+                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+
+                except Exception as e:
+                    logger.warning(f'Image cutout problem : {e}')
+
             if mix_aug:
                 frac_data  = int(self.split * mix_aug_f)
                 if no_track <= frac_data:
-                    points14  = executor.submit(self.augment.mixed_aug_1,im_read,poly_on_image,image_height,image_width) 
-                    p , im = next(points14.result())
-                    utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                    try:
+                        points14  = executor.submit(self.augment.mixed_aug_1,im_read,rect_on_image,image_height,image_width) 
+                        p , im = next(points14.result())
+                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
                     
-                    points15  = executor.submit(self.augment.mixed_aug_2,im_read,poly_on_image,image_height,image_width) 
-                    p , im = next(points15.result())
-                    utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                    except Exception as e:
+                        logger.warning(f'Mixaug 1 problem : {e}')
+
                     
-                    points16  = executor.submit(self.augment.mixed_aug_3,im_read,poly_on_image,image_height,image_width) 
-                    p , im = next(points16.result())
-                    utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                    try:
+                        points15  = executor.submit(self.augment.mixed_aug_2,im_read,rect_on_image,image_height,image_width) 
+                        p , im = next(points15.result())
+                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+
+                    except Exception as e:
+                        logger.warning(f'Mixaug 2 problem : {e}')
+
+
+                    try:
+                        points16  = executor.submit(self.augment.mixed_aug_3,im_read,rect_on_image,image_height,image_width) 
+                        p , im = next(points16.result())
+                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+
+                    except Exception as e:
+                        logger.warning(f'Mixaug 3 problem : {e}')
+
                     
-                    points17  = executor.submit(self.augment.mixed_aug_4,im_read,poly_on_image,image_height,image_width) 
-                    p , im = next(points17.result())
-                    utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                    try:
+                        points17  = executor.submit(self.augment.mixed_aug_4,im_read,rect_on_image,image_height,image_width) 
+                        p , im = next(points17.result())
+                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+
+                    except Exception as e:
+                        logger.warning(f'Mixaug 4 problem : {e}')
             
             if temperature_change:
                 frac_data  = int(self.split * temperature_change_f)
-                if no_track <= frac_data:
-                    points18  = executor.submit(self.augment.image_change_colorTemperature,im_read,poly_on_image,image_height,image_width) 
-                    p , im = next(points18.result())
-                    utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                try:
+                    if no_track <= frac_data:
+                
+                        points2  = executor.submit(self.augment.image_change_colorTemperature,im_read,rect_on_image,image_height,image_width) 
+                        p , im = next(points2.result())
+                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+
+                except Exception as e:
+                    logger.warning(f'Image temperature problem : {e}')
+
+            if motionBlur:
+                frac_data  = int(self.split * motionBlur_f)
+                try:
+                    if no_track <= frac_data:
+                        
+                        points20  = executor.submit(self.augment.image_motionBlur,im_read,rect_on_image,image_height,image_width) 
+                        p , im = next(points20.result())
+                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+                        
+                except Exception as e:
+                    logger.warning(f'Image motion_blur problem : {e}')
+
 
             if weather_change:
                 frac_data  = int(self.split * weather_change_f)
-                if no_track <= frac_data:
-                    points2  = executor.submit(self.augment.image_change_colorTemperature,im_read,poly_on_image,image_height,image_width) 
-                    p , im = next(points2.result())
-                    utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                try:
+                    if no_track <= frac_data:
+                        
+                        points20  = executor.submit(self.augment.image_weatherChange,im_read,rect_on_image,image_height,image_width) 
+                        p , im = next(points20.result())
+                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+                        
+                except Exception as e:
+                    logger.warning(f'Image weather chnage problem : {e}')
+
+        
+            
+
+
+            
+
+
 
-                
-             
-  
-               
     
-    def Image_augmentation(self,folder,train_split=1.0,image_height:Union[int,keep_original_image_height]=640 , image_width:Union[int,keep_aspect_ratio,keep_original_image_width]=640,blur=True , blur_f = 0.5 , rotate=True , rotate_f = 0.5 , noise=True,noise_f=0.5,perspective=True,perspective_f = 0.5,affine=True,affine_f=0.5,
+    def Image_augmentation(self,folder,train_split=1.0,image_height:Union[int,keep_original_image_height]=640 , image_width:Union[int,keep_aspect_ratio,keep_original_image_width]=640,blur=True , blur_f = 0.5 , motionBlur=True , motionBlur_f = 0.5 ,  rotate=True , rotate_f = 0.5 , noise=True,noise_f=0.5,perspective=True,perspective_f = 0.5,affine=True,affine_f=0.5,
                             brightness=True,brightness_f=0.5,hue=True,hue_f=0.5,removesaturation=True,removesaturation_f=0.5,contrast=True,contrast_f=0.5,upflip=True,upflip_f=0.5,
                             shear=True ,shear_f=0.5, rotate90=True,rotate90_f = 0.5,blur_and_noise=True,blur_and_noise_f=0.5,image_cutout = True,image_cutout_f=0.5,
                             mix_aug=True,mix_aug_f=0.5,temperature_change=True,temperature_change_f=0.5,weather_change=True,weather_change_f=0.5):
         
         #checking if input folder is a directory or not
         dir_checker = os.path.isdir(folder)
         
@@ -281,30 +395,47 @@
             raise NotADirectoryError(f'Provided Path - {folder} is not a directory...')
        
         # changing other images format to same format '.jpg'
         self.image_format_change(folder=folder)
         
         # getting all json and jpg images
         all_images =  glob.glob(f'{folder}/*jpg')
-        all_json =  glob.glob(f'{folder}/*json')
+        all_txt =  list(map(lambda x : x.split('.')[0] + '.txt',all_images))
+        classes_ = glob.glob(f'{folder}/classes*txt')
+
+   
+  
+        if classes_ != []:
+            with open(classes_[0]) as f:
+                data = f.readlines()
+                for index ,classes_name in enumerate(data):
+                    self.store_dict[index] = classes_name.rstrip()
+                   
+                console.print('[bold green] classes.txt found.. [bold green]')
+        else:
+            shutil.rmtree(self.aug_save_folder_name)
+            raise NotImplementedError('Classes.txt not Found !!')
         
         # checking json and images are same or not and checking their len too
-        if len(all_images) == len(all_json) and len(all_images) >= 1 and len(all_json) >=1:
-            del all_json
+        if classes_ != []:
+            if len(all_images)  == len(all_txt) and len(all_images)  >= 1 and len(all_txt)  >=1:
+                del all_txt
             
-        else:
+            else:
+                shutil.rmtree(self.aug_save_folder_name)
+                raise NotImplementedError(f'Images and Txt are not equal , recheck your annotation folder! Total Images : {len(all_images)}  |  Total txt : {len(all_txt)}')
             
-            raise NotImplementedError(f'Images and Jsons are not equal , recheck your annotation folder! \
-                                       Total Images : {len(all_images)}  |  Total Json : {len(all_json)}')
         # checking train is float or not
         if type(train_split) != float:
+            shutil.rmtree(self.aug_save_folder_name)
             raise TypeError(f'please provide "train split" as "float" , You provided train split as {type(train_split)}')
             
         # checking train split value > 1.0 or not   
         if train_split > 1.0:
+            shutil.rmtree(self.aug_save_folder_name)
             raise ValueError(f'[-] please provide "train split" between "0.5 to 1.0", Your provided train split value is : {train_split}')
 
 
         #checking the types here    
         type_1 = { 
                 'blur_f':blur_f,
                 'noise_f':noise_f,
@@ -318,15 +449,16 @@
                 'affine_f':affine_f,
                 'perspective_f':perspective_f,
                 'upflip_f' : upflip_f,
                 'shear_f' : shear_f,
                 'image_cut_f':image_cutout_f,
                 'mix_aug_f' : mix_aug_f,
                 'temperaure_change_f' : temperature_change_f,
-                'weather_change_f' : weather_change_f
+                'weather_change_f' : weather_change_f,
+                'motionBlur_f' : motionBlur_f
                 
               }
         
         type_2 = { 
                 'blur':blur,
                 'noise':noise,
                 'NB':blur_and_noise,
@@ -339,38 +471,43 @@
                 'affine':affine,
                 'perspective':perspective,
                 'upflip' : upflip,
                 'shear' : shear,
                 'image_cut':image_cutout,
                 'mix_aug' : mix_aug,
                 'temp_change' : temperature_change,
-                'weather_change' : weather_change
+                'weather_change' : weather_change,
+                'motionBlur' : motionBlur
                 
               }
 
         # checking the types 
         for types , val in type_1.items():
             if type(val) != float:
+                shutil.rmtree(self.aug_save_folder_name)
                 raise TypeError(f' [-] please provide "{types}" as  "float" , You provided "{types}" as {type(val)}')
              
                 
             if val > 1.0:
+                shutil.rmtree(self.aug_save_folder_name)
                 raise ValueError(f'[-] please provide "{types}" value  between "0.1 to 1.0" , Your provided "{types}" value is : "{val}"')
         
         for typess , vals in type_2.items():
 
             if type(vals) != bool:
+                shutil.rmtree(self.aug_save_folder_name)
                 raise TypeError(f'Please provide "{typess}" as bool , you provided "{typess}" as "{vals}"')
         
 
        
         if (type(image_height) , image_width) == (int,'keep_aspect_ratio') or (type(image_height),type(image_width)) == (int,int) or (image_height , image_width) == ('keep_original_image_height','keep_original_image_width'):
             pass
 
         else:
+            shutil.rmtree(self.aug_save_folder_name)
             raise ValueError('You provided a wrong image height and width combination, right combinations are - \n (image height , image width) = (int ,int) \n (image height , image width) = (int , "keep_aspect_ratio") \n (image height , image width) = ("keep_original_image_height","keep_original_image_width") ')
         
         if image_width == 'keep_aspect_ratio' and type(image_height) == int :
             image_width_N = 'keep-aspect-ratio'
             image_height_N = image_height
         
 
@@ -392,64 +529,63 @@
         if train_split == 1.0:
                     shutil.rmtree(f'{self.aug_save_folder_name}/test')
         
         # if c value less than equal to train split then we will add those images in training data and rest will go for test data            
         for c ,images in enumerate(track(all_images,description='Image Augmentation..',total=len(all_images[:self.split]))):
 
             if c+1 <= self.split:
+
                 
-                poly = list(self.json_converter(images))
+                try:
+                    poly = list(self.txt_converter(images))
+            
+                    #if we want to keep original image height and width -->
+                    if image_height == 'keep_original_image_height' and image_width == 'keep_original_image_width':
+                        image_height_N , image_width_N , channel = poly[0][0].shape
+                    
+                    # print(poly)
 
-                #if we want to keep original image height and width -->
-                if image_height == 'keep_original_image_height' and image_width == 'keep_original_image_width':
-                    image_height_N , image_width_N , _ = poly[0][0].shape
-
-                self.Combined_augmentation(poly[0][0],poly[0][1],c+1,image_height_N,image_width_N,blur=blur , blur_f = blur_f , rotate=rotate , rotate_f = rotate_f , noise=noise,noise_f=noise_f,perspective=perspective,perspective_f = perspective_f,affine=affine,affine_f=affine_f,
-                              brightness=brightness,brightness_f=brightness_f,hue=hue,hue_f=hue_f,removesaturation=removesaturation,removesaturation_f=removesaturation_f,contrast=contrast,contrast_f=contrast_f,upflip=upflip,upflip_f=upflip_f,
-                              shear= shear ,shear_f=shear_f, rotate90=rotate90,rotate90_f = rotate90_f,blur_and_noise=blur_and_noise,blur_and_noise_f=blur_and_noise_f,image_cutout = image_cutout,image_cutout_f=image_cutout_f,
-                              mix_aug=mix_aug,mix_aug_f=mix_aug_f,temperature_change=temperature_change,temperature_change_f=temperature_change_f,weather_change=weather_change,weather_change_f=weather_change_f)
+                    self.Combined_augmentation(poly[0][0],poly[0][1],c+1,image_height_N,image_width_N,blur=blur , blur_f = blur_f , rotate=rotate , rotate_f = rotate_f , noise=noise,noise_f=noise_f,perspective=perspective,perspective_f = perspective_f,affine=affine,affine_f=affine_f,
+                                brightness=brightness,brightness_f=brightness_f,hue=hue,hue_f=hue_f,removesaturation=removesaturation,removesaturation_f=removesaturation_f,contrast=contrast,contrast_f=contrast_f,upflip=upflip,upflip_f=upflip_f,
+                                shear= shear ,shear_f=shear_f, rotate90=rotate90,rotate90_f = rotate90_f,blur_and_noise=blur_and_noise,blur_and_noise_f=blur_and_noise_f,image_cutout = image_cutout,image_cutout_f=image_cutout_f,
+                                mix_aug=mix_aug,mix_aug_f=mix_aug_f,temperature_change=temperature_change,temperature_change_f=temperature_change_f,weather_change=weather_change,weather_change_f=weather_change_f,motionBlur=motionBlur,motionBlur_f=motionBlur_f)
+                
+                except Exception as e:
+                    console.print('[bold yellow] WARNING [bold yellow] : There is some problem with data , skipping this...')
+                    logger.error(f'combined augmentation problem : {e}')
                 
                 
                 
             elif c+1 > self.split:
-                # print(images)
+               
+                try:
                 
-                poly = list(self.json_converter(f'{images}'))
-                utils_poly.create_new_txt(poly[0][0] ,self.labels,poly[0][1],self.test_images_path,self.test_labels_path,self.store_dict,yolo=self.yolo)
+                    poly = list(self.txt_converter(f'{images}'))
+
+                    utils_poly.create_new_txt(poly[0][0] ,poly[0][1],self.test_images_path,self.test_labels_path)
+
+                except Exception as e:
+                    console.print('[bold yellow] WARNING [bold yellow] : There is some problem with data , skipping this...')
+                    logger.error(f'Test data  problem : {e}')
                    
-        console.print(f'[bold dim cyan] Labels name : [/bold dim cyan] [bold magenta] {list(self.store_dict.keys())} [bold magenta]')
-        yml_writer_poly.yaml_writer(len(self.store_dict.keys()),list(self.store_dict.keys()),self.aug_save_folder_name)      
-      
+        console.print(f'[bold dim cyan] Labels name : [/bold dim cyan] [bold magenta] {list(self.store_dict.values())} [bold magenta]')
+
+        yml_writer_poly.yaml_writer(len(self.store_dict.keys()),list(self.store_dict.values()),self.aug_save_folder_name)   
+
+        with open(f'{self.aug_save_folder_name}/classes.txt','w') as f:
+            f.write('\n'.join(list(self.store_dict.values()))) 
       
       
       
     @staticmethod
     def image_format_change(folder):
         for im in os.listdir(folder):
-            if im.endswith('.json'):
+            if im.endswith('.txt'):
                 continue
             elif im.endswith('.jpg'):
                 continue
             else:
                 
                 im_name = im.split('.')[0]
                 ims = cv2.imread(f'{folder}/{im}')
                 cv2.imwrite(f'{folder}/{im_name}.jpg',ims)
-                os.remove(f'{folder}/{im}')
-                      
-
-         
-
-
-    
-
-
-
-
-
-
-
-
-
-
-  
-        
+                os.remove(f'{folder}/{im}')
```

### Comparing `image_augs-2.2.9/instance_seg/logging_util.py` & `image_augs-2.3.10/instance_seg/logging_util.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.2.9/instance_seg/utils_poly.py` & `image_augs-2.3.10/instance_seg/utils_poly.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,20 +38,26 @@
                     x , y = list(ps)
                     normalize_X = x/new_width
                     normalize_Y = y/new_height
 
                     
                     new_name += f'{normalize_X} {normalize_Y}'
                     new_name += ' '
+                
+                if new_name != '':
+                    if type(image) == str:
+                        image = cv2.imread(image)
 
+                    cv2.imwrite(f'{train_path_images}/{save_name}.jpg',image)
+                 
                
-                with open(txt_path,'a+') as f:
+                    with open(txt_path,'a+') as f:
                     
-                    f.write(new_name)
-                    f.write('\n')
+                        f.write(new_name)
+                        f.write('\n')
                     
                         
                 del new_name
             
         except Exception as e:
             logger.warning(f'problem : create new json  desc : {e}')
 
@@ -68,28 +74,30 @@
                 label = dict[labels]
                 new_name = str(label) + ' '
                 points = []
 
                 for ps in p: 
 
                     points.append(list(ps))
+                
+                if points != []:
 
-                sh_dict={"label": labels,"points":points , "group_id": None, "shape_type": "polygon", "flags": {}}
-                annot_dict["shapes"].append(sh_dict)
-                annot_dict["imagePath"] = f'{save_name}.jpg'
-                img_data = labelme.LabelFile.load_image_file(f'{train_path_images}/{save_name}.jpg')
-                img_data = base64.b64encode(img_data).decode('utf-8')
-                height , width , _ = image.shape
-                annot_dict["imageData"]=img_data
-                annot_dict["imageHeight"]=height
-                annot_dict["imageWidth"]=width
-                json_file=f'{train_path_labels}/{save_name}.json'
-                            
-                with open(json_file, 'w', encoding='utf-8') as f:
-                    json.dump(annot_dict, f, ensure_ascii=False, indent=4,cls=NumpyEncoder)
+                    sh_dict={"label": labels,"points":points , "group_id": None, "shape_type": "polygon", "flags": {}}
+                    annot_dict["shapes"].append(sh_dict)
+                    annot_dict["imagePath"] = f'{save_name}.jpg'
+                    img_data = labelme.LabelFile.load_image_file(f'{train_path_images}/{save_name}.jpg')
+                    img_data = base64.b64encode(img_data).decode('utf-8')
+                    height , width , _ = image.shape
+                    annot_dict["imageData"]=img_data
+                    annot_dict["imageHeight"]=height
+                    annot_dict["imageWidth"]=width
+                    json_file=f'{train_path_labels}/{save_name}.json'
+                                
+                    with open(json_file, 'w', encoding='utf-8') as f:
+                        json.dump(annot_dict, f, ensure_ascii=False, indent=4,cls=NumpyEncoder)
                 
             
         except Exception as e:
             logger.warning(f'problem : create new text  desc : {e}')
```

### Comparing `image_augs-2.2.9/instance_seg/yml_writer_poly.py` & `image_augs-2.3.10/instance_seg/yml_writer_poly.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.2.9/object_detection_new/augmentation_rect.py` & `image_augs-2.3.10/object_detection_new/augmentation_rect.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import imgaug.augmenters as iaa
+import imgaug as ia
 from rich.console import Console
 import numpy as np
 from imgaug.augmentables.bbs import BoundingBox, BoundingBoxesOnImage
 
 import os
-import warnings
 import random
 from typing import Tuple
 import secrets
 
 import instance_seg.logging_util as logging_util
 
-warnings.filterwarnings('ignore')
+
 
 
 
 console  = Console()
 logger = logging_util.get_logger(os.path.basename(__file__).split('.')[0])
 
 
@@ -28,15 +28,17 @@
     def __init__(self) -> None:
         
         # self.height = height
         
         console.print('[bold green] [+] Image augmentation Box module loaded....[bold green]')
         logger.info('Image Augmentation Box module loaded successfully...')
 
-    def image_rotate(self,image:np.array,bbox:BoundingBoxesOnImage,H,W,rotation_angle:int=13) -> Tuple[BoundingBoxesOnImage,np.array]:
+   
+
+    def image_rotate(self,image:np.array,bbox:BoundingBoxesOnImage,H,W,rotation_angle:int=16) -> Tuple[BoundingBoxesOnImage,np.array]:
 
         '''
         Image Rotate will rotate an image and its polygon points to a desired angle
 
         : param image                   : accepts cv2.imread() images
         : param boundingBoxesOnImage    : BoundingBox points of that image
         : param rotation angle          : desired angle you want to rotate (-angle , angle)
@@ -45,87 +47,101 @@
         : new polygon points    : it will return after rotation polygon points
         : aug rotated image     : it will return rotated image
         
         '''
         try:
            
             aug = iaa.Sequential([iaa.Rotate((-rotation_angle,rotation_angle),fit_output=False),
-                                iaa.SaltAndPepper(p=(0.01,0.06)),
-                                iaa.Multiply((0.2, 1.5), per_channel=1.0,),
+                                iaa.SaltAndPepper(p=(0.01,0.03)),
+                                iaa.Multiply((0.2, 1.1), per_channel=1.0,),
                                 iaa.Resize({"height": H, "width": W})])
             aug_rotated_image, new_points_bbox  = aug(image=image,bounding_boxes=bbox)
+            new_points_bbox = new_points_bbox.remove_out_of_image().clip_out_of_image()
             new_points_bbox = new_points_bbox.bounding_boxes
             
             yield new_points_bbox , aug_rotated_image
         except Exception as e:
-            logger.warning(f'problem: Image rotation    desc : {e}')
+            logger.error(f'problem: Image rotation    desc : {e}')
 
     
-    def image_affine(self,image:np.array,bbox:BoundingBoxesOnImage,H,W,scale_range:range=(0.5,1.7)) -> Tuple[BoundingBoxesOnImage,np.array]:
+    def image_affine(self,image:np.array,bbox:BoundingBoxesOnImage,H,W,scale_range:range=(0.5,1.6)) -> Tuple[BoundingBoxesOnImage,np.array]:
         try:
             aug = iaa.Sequential([iaa.Affine(scale=scale_range,fit_output=False,),
                                 iaa.Resize({"height": H, "width": W})])
             aug_affine_image , new_points_bbox  = aug(image=image,bounding_boxes=bbox)
+            new_points_bbox = new_points_bbox.remove_out_of_image().clip_out_of_image()
             new_points_bbox = new_points_bbox.bounding_boxes
             yield new_points_bbox , aug_affine_image
         except Exception as e:
-            logger.warning(f'problem: Image affine    desc : {e}')
+            logger.error(f'problem: Image affine    desc : {e}')
 
 
 
-    def image_perspective_transform(self,image:np.array,bbox:BoundingBox,H,W,scale_range:range=(0.10,0.17)) -> Tuple[BoundingBoxesOnImage,np.array]:
+    def image_perspective_transform(self,image:np.array,bbox:BoundingBox,H,W,scale_range:range=(0.10,0.12)) -> Tuple[BoundingBoxesOnImage,np.array]:
         try:
             aug = iaa.Sequential([iaa.PerspectiveTransform(scale=scale_range,fit_output=False,),
                                 iaa.Resize({"height": H, "width": W})])
             aug_affine_image,new_points_bbox = aug(image=image,bounding_boxes=bbox)
+            new_points_bbox = new_points_bbox.remove_out_of_image().clip_out_of_image()
             new_points_bbox = new_points_bbox.bounding_boxes
             yield new_points_bbox , aug_affine_image
 
         except Exception as e:
-            logger.warning(f'problem: Image perspective transform    desc : {e}')
+            logger.error(f'problem: Image perspective transform    desc : {e}')
 
     def image_noise(self,image:np.array,bbox:BoundingBox,H,W) -> Tuple[BoundingBoxesOnImage,np.array]:
         try:
             choice = random.choice([0,1])
             if choice == 0:
-                aug = iaa.Sequential([iaa.SaltAndPepper(p=(0.01,0.06)),
+                aug = iaa.Sequential([iaa.SaltAndPepper(p=(0.01,0.05)),
                                 iaa.Resize({"height": H, "width": W})])
             else:
                 # aug = iaa.AdditiveLaplaceNoise(scale=(5,0.1*200), per_channel=True)
                 aug = iaa.Sequential([iaa.SaltAndPepper(p=(0.01,0.06),per_channel=True),
                                 iaa.Resize({"height": H, "width": W})])
             aug_affine_image,new_points_bbox = aug(image=image,bounding_boxes=bbox)
             new_points_bbox = new_points_bbox.bounding_boxes
             yield new_points_bbox , aug_affine_image
 
         except Exception as e:
-            logger.warning(f'problem: Image noise    desc : {e}')
+            logger.error(f'problem: Image noise    desc : {e}')
 
     def image_blur(self,image:np.array,bbox:BoundingBox,H,W) -> Tuple[BoundingBoxesOnImage,np.array]:
         try:
             aug = iaa.Sequential([iaa.GaussianBlur(sigma=(1.2, 4.0)),
                                 iaa.Resize({"height": H, "width": W})])
             aug_affine_image, new_points_bbox = aug(image=image,bounding_boxes=bbox)
             new_points_bbox = new_points_bbox.bounding_boxes
             yield new_points_bbox , aug_affine_image
         
         except Exception as e:
-            logger.warning(f'problem: Image blur    desc : {e}')
+            logger.error(f'problem: Image blur    desc : {e}')
+
+    def image_motionBlur(self,image:np.array,bbox:BoundingBox,H,W) -> Tuple[BoundingBoxesOnImage,np.array]:
+        try:
+            aug = iaa.Sequential([iaa.MotionBlur(k=15, angle=[-45, 45]),
+                                iaa.Resize({"height": H, "width": W})])
+            aug_affine_image, new_points_bbox = aug(image=image,bounding_boxes=bbox)
+            new_points_bbox = new_points_bbox.bounding_boxes
+            yield new_points_bbox , aug_affine_image
+        
+        except Exception as e:
+            logger.error(f'problem: Image motion blur    desc : {e}')
 
     def image_hue(self,image:np.array,bbox:BoundingBox,H,W) -> Tuple[BoundingBoxesOnImage,np.array]:
         try:
             # aug = iaa.Multiply((0.5, 1.5), per_channel=0.5)
             aug = iaa.Sequential([iaa.Multiply((0.5, 1.5), per_channel=1.0,),
                                 iaa.WithBrightnessChannels(iaa.Add((-40,40))),
                                 iaa.Resize({"height": H, "width": W})])
             aug_affine_image, new_points_bbox = aug(image=image,bounding_boxes=bbox)
             new_points_bbox = new_points_bbox.bounding_boxes
             yield new_points_bbox , aug_affine_image
         except Exception as e:
-            logger.warning(f'problem: Image hue    desc : {e}')
+            logger.error(f'problem: Image hue    desc : {e}')
 
     def image_brightness(self,image:np.array,bbox:BoundingBox,H,W) -> Tuple[BoundingBoxesOnImage,np.array]:
         try:
             ranges = random.choice([0,1])
             if ranges == 0:
        
                 aug = iaa.Sequential([iaa.WithBrightnessChannels(iaa.Add((10,50))),
@@ -135,86 +151,87 @@
                 aug = iaa.Sequential([iaa.WithBrightnessChannels(iaa.Add((-50,-10))),
                                 iaa.Resize({"height": H, "width": W})])
             aug_affine_image, new_points_bbox = aug(image=image,bounding_boxes=bbox)
             new_points_bbox = new_points_bbox.bounding_boxes
             yield new_points_bbox , aug_affine_image
 
         except Exception as e:
-            logger.warning(f'problem: Image brightness    desc : {e}')
+            logger.error(f'problem: Image brightness    desc : {e}')
 
     
     def image_change_colorTemperature(self,image:np.array,bbox:BoundingBox,H,W) -> Tuple[BoundingBoxesOnImage,np.array]:
         try:
             # aug =  iaa.ChangeColorTemperature((1100, 10000))
             aug = iaa.Sequential([iaa.ChangeColorTemperature((1100, 6500)),
-                                  iaa.GaussianBlur(sigma=(1.2, 2.7)),
+                                  iaa.GaussianBlur(sigma=(1.2, 2.3)),
                                 iaa.Resize({"height": H, "width": W})])
             
             aug_affine_image, new_points_bbox = aug(image=image,bounding_boxes=bbox)
             new_points_bbox = new_points_bbox.bounding_boxes
             yield new_points_bbox , aug_affine_image
         except Exception as e:
-            logger.warning(f'problem: Image color temp    desc : {e}')
+            logger.error(f'problem: Image color temp    desc : {e}')
 
     
     def image_removeSaturation(self,image:np.array,bbox:BoundingBox,H,W) -> Tuple[BoundingBoxesOnImage,np.array]:
         try:
             choices = random.choice([0.3,0.4,0.5,0.6,0.7,0.8,0.9])
             aug = iaa.Sequential([iaa.RemoveSaturation(choices),
                                 iaa.Resize({"height": H, "width": W})])
             aug_affine_image, new_points_bbox = aug(image=image,bounding_boxes=bbox)
             new_points_bbox = new_points_bbox.bounding_boxes
             yield new_points_bbox , aug_affine_image
 
         except Exception as e:
-            logger.warning(f'problem: Image removeSaturation    desc : {e}')
+            logger.error(f'problem: Image removeSaturation    desc : {e}')
 
     
     def image_contrast(self,image:np.array,bbox:BoundingBox,H,W) -> Tuple[BoundingBoxesOnImage,np.array]:
         try:
         
             aug = iaa.Sequential([iaa.LinearContrast((0.8, 1.7)),
                                 iaa.Resize({"height": H, "width": W})])
             aug_affine_image, new_points_bbox = aug(image=image,bounding_boxes=bbox)
             new_points_bbox = new_points_bbox.bounding_boxes
             yield new_points_bbox , aug_affine_image
 
         except Exception as e:
-            logger.warning(f'problem: Image contrast    desc : {e}')
+            logger.error(f'problem: Image contrast    desc : {e}')
 
 
     def image_upFlip(self,image:np.array,bbox:BoundingBox,H,W,flip_percentage:float=1.0) -> Tuple[BoundingBoxesOnImage,np.array]:
         try:
             # aug =  iaa.Flipud(flip_percentage)
             aug = iaa.Sequential([iaa.Flipud(flip_percentage,),
                                 iaa.Resize({"height": H, "width": W})])
             aug_affine_image, new_points_bbox = aug(image=image,bounding_boxes=bbox)
             new_points_bbox = new_points_bbox.bounding_boxes
             yield new_points_bbox , aug_affine_image
         except Exception as e:
-            logger.warning(f'problem: Image uplfip    desc : {e}')
+            logger.error(f'problem: Image uplfip    desc : {e}')
 
     def image_shear(self,image:np.array,bbox:BoundingBox,H,W) -> Tuple[BoundingBoxesOnImage,np.array]:
         try:
             choice = random.choice([0,1])
             if choice == 0:
                 # aug =  iaa.ShearX(shear=(-12,12))
-                aug = iaa.Sequential([iaa.ShearX(shear=(-16,16),fit_output=False),
+                aug = iaa.Sequential([iaa.ShearX(shear=(-18,18),fit_output=False),
                                 iaa.Resize({"height": H, "width": W})])
             else:
                 # aug =  iaa.ShearY(shear=(-12,12))
-                aug = iaa.Sequential([iaa.ShearY(shear=(-16,16),fit_output=False),
+                aug = iaa.Sequential([iaa.ShearY(shear=(-18,18),fit_output=False),
                                 iaa.Resize({"height": H, "width": W})])
                 
             aug_affine_image, new_points_bbox = aug(image=image,bounding_boxes=bbox)
+            new_points_bbox = new_points_bbox.remove_out_of_image().clip_out_of_image()
             new_points_bbox = new_points_bbox.bounding_boxes
             yield new_points_bbox , aug_affine_image
 
         except Exception as e:
-            logger.warning(f'problem: Image shear    desc : {e}')
+            logger.error(f'problem: Image shear    desc : {e}')
     
 
     def image_rotate90(self,image:np.array,bbox:BoundingBox,H,W) -> Tuple[BoundingBoxesOnImage,np.array]:
         try:
             choice = random.choice([0,1])
             if choice == 0:
                 # aug =  iaa.Rotate(rotate=90,fit_output=True)
@@ -222,18 +239,19 @@
                                 iaa.Resize({"height": H, "width": W})])
             else:
                 # aug =  iaa.Rotate(rotate=-90,fit_output=True)
                 aug = iaa.Sequential([iaa.Rotate(rotate=-90,fit_output=False),
                                 iaa.Resize({"height": H, "width": W})])
                 
             aug_affine_image, new_points_bbox = aug(image=image,bounding_boxes=bbox)
+            new_points_bbox = new_points_bbox.remove_out_of_image().clip_out_of_image()
             new_points_bbox = new_points_bbox.bounding_boxes
             yield new_points_bbox , aug_affine_image
         except Exception as e:
-            logger.warning(f'problem: Image rotate90   desc : {e}')
+            logger.error(f'problem: Image rotate90   desc : {e}')
     #beta
     def image_weatherChange(self,image:np.array,bbox:BoundingBox,H,W,rain_speed:range=((0.09, 0.2))) -> Tuple[BoundingBoxesOnImage,np.array]:
         try:
             choice = secrets.choice([0,1,2])
         
             if choice == 0:
      
@@ -249,94 +267,98 @@
                                 iaa.Resize({"height": H, "width": W})])
 
             aug_affine_image, new_points_bbox = aug(image=image,bounding_boxes=bbox)
             new_points_bbox = new_points_bbox.bounding_boxes
             yield new_points_bbox , aug_affine_image
 
         except Exception as e:
-            logger.warning(f'problem: Image weatherchange    desc : {e}')
+            logger.error(f'problem: Image weatherchange    desc : {e}')
     
     def image_cutOut(self,image:np.array,bbox:BoundingBox,H,W,number_of_square:int=2,size:float=0.1) -> Tuple[BoundingBoxesOnImage,np.array]:
         try:
             # aug =  iaa.Cutout(fill_mode="constant", cval=random.choice([128,255]),size=size,nb_iterations=number_of_square)
             aug = iaa.Sequential([iaa.Cutout(fill_mode="constant", cval=random.choice([128,255]),size=size,nb_iterations=number_of_square),
                                 iaa.Resize({"height": H, "width": W})])
             aug_affine_image, new_points_bbox = aug(image=image,bounding_boxes=bbox)
+
             new_points_bbox = new_points_bbox.bounding_boxes
             yield new_points_bbox , aug_affine_image
         except Exception as e:
-            logger.warning(f'problem: Image cutout    desc : {e}')
+            logger.error(f'problem: Image cutout    desc : {e}')
 
     def blur_and_noise(self,image:np.array,bbox:BoundingBox,H,W) -> Tuple[BoundingBoxesOnImage,np.array]:
         try:
             aug = iaa.Sequential([iaa.GaussianBlur(sigma=(0.8, 3.5)),
                                 iaa.Resize({"height": H, "width": W}),
                                 iaa.SaltAndPepper(p=(0.02,0.07))])
             
             aug_affine_image, new_points_bbox = aug(image=image,bounding_boxes=bbox)
             new_points_bbox = new_points_bbox.bounding_boxes
             yield new_points_bbox , aug_affine_image
 
         except Exception as e:
-            logger.warning(f'problem: Image blur and noise    desc : {e}')
+            logger.error(f'problem: Image blur and noise    desc : {e}')
 
     
     def mixed_aug_1(self,image:np.array,bbox:BoundingBox,H,W) -> Tuple[BoundingBoxesOnImage,np.array]:
         try:
             aug = iaa.Sequential([iaa.Affine(scale=(0.5,1.6),fit_output=False),
                                 iaa.Multiply((0.5, 1.5), per_channel=0.5),
                                 iaa.Resize({"height": H, "width": W})])
             
                                 
             aug_affine_image, new_points_bbox = aug(image=image,bounding_boxes=bbox)
+            new_points_bbox = new_points_bbox.remove_out_of_image().clip_out_of_image()
             new_points_bbox = new_points_bbox.bounding_boxes
             yield new_points_bbox , aug_affine_image
 
         except Exception as e:
-            logger.warning(f'problem: Mix aug 1    desc : {e}')
+            logger.error(f'problem: Mix aug 1    desc : {e}')
 
 
     def mixed_aug_2(self,image:np.array,bbox:BoundingBox,H,W) -> Tuple[BoundingBoxesOnImage,np.array]:
         try:
             choices = random.choice([0.4,0.5,0.6,0.7,0.8])
             # aug = iaa.RemoveSaturation(choices)
-            aug = iaa.Sequential([iaa.Rotate((-10,10),fit_output=False),
+            aug = iaa.Sequential([iaa.Rotate((-13,13),fit_output=False),
                                 iaa.WithBrightnessChannels(iaa.Add((-40,40))),
                                 iaa.RemoveSaturation(choices),
-                                iaa.PerspectiveTransform(scale=(0.08,0.15),fit_output=False),
+                                iaa.PerspectiveTransform(scale=(0.08,0.12),fit_output=False),
                                 iaa.Resize({"height": H, "width": W})])
             
                                 
             aug_affine_image, new_points_bbox = aug(image=image,bounding_boxes=bbox)
+            new_points_bbox = new_points_bbox.remove_out_of_image().clip_out_of_image()
             new_points_bbox = new_points_bbox.bounding_boxes
             yield new_points_bbox , aug_affine_image
         except Exception as e:
-            logger.warning(f'problem: mix aug 2    desc : {e}')
+            logger.error(f'problem: mix aug 2    desc : {e}')
 
     def mixed_aug_3(self,image:np.array,bbox:BoundingBox,H,W) -> Tuple[BoundingBoxesOnImage,np.array]:
         try:
             choice = random.choice([0,1])
             if choice == 0:
                 aug = iaa.Sequential([iaa.ShearX(shear=(-15,15),fit_output=False),
-                                    iaa.GaussianBlur(sigma=(0.8, 4.0)),
+                                    iaa.GaussianBlur(sigma=(0.8, 2.8)),
                                     iaa.ChangeColorTemperature((1100, 7000)),
                                     iaa.Resize({"height": H, "width":W})])
             
             else:
                 aug = iaa.Sequential([iaa.ShearY(shear=(-15,15),fit_output=False),
                                     iaa.LinearContrast((0.8, 1.6)),
                                     iaa.Resize({"height": H, "width":W})])
     
                             
             aug_affine_image, new_points_bbox = aug(image=image,bounding_boxes=bbox)
+            new_points_bbox = new_points_bbox.remove_out_of_image().clip_out_of_image()
             new_points_bbox = new_points_bbox.bounding_boxes
             yield new_points_bbox , aug_affine_image
         
         except Exception as e:
-            logger.warning(f'problem: Mix aug 3    desc : {e}')
+            logger.error(f'problem: Mix aug 3    desc : {e}')
 
     def mixed_aug_4(self,image:np.array,bbox:BoundingBox,H,W) -> Tuple[BoundingBoxesOnImage,np.array]:
         try:
             choice = random.choice([-90,90])
             choices =  random.choice([0,1])
             
             if choices == 0:
@@ -351,12 +373,15 @@
                 aug = iaa.Sequential([iaa.Rotate(rotate=choice,fit_output=False),
                                 iaa.WithBrightnessChannels(iaa.Add((-20,20))),
                                 iaa.SaltAndPepper(p=(0.01,0.06)),
                                 iaa.Resize({"height": H, "width": W})])
             
                                 
             aug_affine_image, new_points_bbox = aug(image=image,bounding_boxes=bbox)
+            new_points_bbox = new_points_bbox.remove_out_of_image().clip_out_of_image()
             new_points_bbox = new_points_bbox.bounding_boxes
             yield new_points_bbox , aug_affine_image
 
+    
+
         except Exception as e:
-            logger.warning(f'problem: Mixed aug 4    desc : {e}')
+            logger.error(f'problem: Mixed aug 4    desc : {e}')
```

### Comparing `image_augs-2.2.9/object_detection_new/logging_util.py` & `image_augs-2.3.10/object_detection_new/logging_util.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.2.9/object_detection_new/txt_reader_rect.py` & `image_augs-2.3.10/instance_seg/json_reader_poly.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from tornado import concurrent
 import cv2
 import uuid
-from imgaug.augmentables.bbs import BoundingBox, BoundingBoxesOnImage
+from imgaug.augmentables.polys import Polygon, PolygonsOnImage
 from rich.console import Console
 from rich.traceback import install
 from rich.progress import track
 
 import json
 import os
 import glob
 import shutil
 from typing import NewType , Union
 
-from object_detection_new.augmentation_rect import *
-from object_detection_new import utils_poly
-from object_detection_new import yml_writer_poly
+from instance_seg.augment_poly import *
+from instance_seg import utils_poly
+from instance_seg import yml_writer_poly
 import instance_seg.logging_util as logging_util
 
 
 install()
 console = Console()
 logger = logging_util.get_logger(os.path.basename(__file__).split('.')[0])
 keep_aspect_ratio = NewType('keep-aspect-ratio','str')
@@ -27,22 +27,21 @@
 
 
 '''
 Code logic starts from here.
 
 '''
 
-class RectAugmentation():
-    def __init__(self,aug_save_folder_name:os.path='rect_augmentation') -> None:
+class PolygonAugmentation():
+    def __init__(self,aug_save_folder_name:os.path='polygon_augmentation',yolo:bool=True) -> None:
         self.aug_save_folder_name = aug_save_folder_name
-        self.augment = ImageAugmentationBox()
+        self.augment = ImageAugmentation()
         self.store_dict:dict = dict()
         self.counter:int = 0
-
-     
+        self.yolo = yolo
 
         '''
         : param aug_save_folder_name : give a path where you want to save your augmentations 
         : param image_resize : Image resizing for augmentations
         '''
         
         
@@ -54,283 +53,331 @@
             os.makedirs(f'{self.aug_save_folder_name}/train/labels')
             console.print(f'[bold blue] [+] {self.aug_save_folder_name}/[bold blue] folder - created..')
         
         if not os.path.exists(f'{self.aug_save_folder_name}/test/images') or not os.path.exists(f'{self.aug_save_folder_name}/test/labels'):
             os.makedirs(f'{self.aug_save_folder_name}/test/images')
             os.makedirs(f'{self.aug_save_folder_name}/test/labels')
             
-       
+        if type(self.yolo) != bool:
+            raise TypeError(f'Expected type for yolo is bool, you provided yolo type as {type(self.yolo)}')  
           
         self.train_images_path = f'{self.aug_save_folder_name}/train/images'
         self.train_labels_path = f'{self.aug_save_folder_name}/train/labels'
         self.test_images_path = f'{self.aug_save_folder_name}/test/images'
         self.test_labels_path = f'{self.aug_save_folder_name}/test/labels'
     
-        logger.info('RectAugmentation module loaded...')
+        logger.info('ImageAugments module loaded...')
 
-
-    def txt_converter(self,image:os.path):
+    def json_converter(self,image:os.path):
         '''
-        txt converter will convert json to polygon acceptable format.
+        Json converter will convert json to polygon acceptable format.
         It will return image and converted json
 
         : param image : require full path of a image 
         
         : return :
         : im_read       : it will return cv2.imread() image.
         : poly on image : it will return json converted polygon points 
         
         
         '''
         try:
-
             # temporary to store the result
-            new_datas = list()
-  
-       
+            datas = []
             # first we are checking the extension endswith .json or not 
             # then we read the image and json file
-            if not image.endswith('.txt'):
+            if not image.endswith('.json'):
                     im_read = cv2.imread(image)
-      
-                    image_H , image_W , c = im_read.shape
-                    TEXT = image.split('.')[0] + '.txt'
-                    with open(TEXT) as f:
-                        data = f.readlines()
-                     
-                        for datas in data:
-                            strip_data = datas.rstrip().split()
-                            strip_data = list(map(float,strip_data))
-                            
-                            x1,y1,x2,y2 = utils_poly.convert_to_normal_bbox(strip_data[1:],image_W,image_H)
-                            self.labels= int(strip_data[0])
-
+        
+                    JSON = image.split('.')[0] + '.json'
+                    with open(JSON) as f:
+                        data = json.load(f)
+                        annotations = data['shapes']
+                        for i ,annotation in enumerate(annotations):
                             #taking uuid
                             ids = uuid.uuid4()
-
-                            # taking this in bounding box function and their labels
-                            ids = BoundingBox(x1,y1,x2,y2,self.labels)
-                           
-                            new_datas.append(ids)
-                      
+                            # getting the label
+                            self.labels = annotation['label']
+                            # we are saving the labels in the dict
+                            if self.labels in self.store_dict:
+                                pass
+                            
+                            else:
+                                self.store_dict[self.labels] = self.counter
+                                self.counter += 1
+                            
+                            #getting points from json file
+                            poly_points = annotation['points']
+                            poly_points = [tuple(lst) for lst in poly_points]
+                            # taking this in polygon function and their labels
+                            ids = Polygon(poly_points,self.labels)
+                            datas.append(ids)
                         # input temp datas and image_shape   
-                        rect_on_image = BoundingBoxesOnImage(new_datas, shape=im_read.shape)
-                      
-                        del new_datas
-                  
-                        yield im_read , rect_on_image
+                        poly_on_image = PolygonsOnImage(datas, shape=im_read.shape)
+                        
+                        del datas
+                    
+                        yield im_read , poly_on_image
 
         except Exception as e:
-            logger.error(f'problem : Json converter  desc : {e}')
-
-
-    def Combined_augmentation(self,im_read , rect_on_image, no_track,image_height=640 , image_width:Union[int,keep_aspect_ratio]=640,blur=True , blur_f = 0.5 , rotate=True , rotate_f = 0.5 , noise=True,noise_f=0.5,perspective=True,perspective_f = 0.5,affine=True,affine_f=0.5,
-                            brightness=True,brightness_f=0.5,hue=True,hue_f=0.5,removesaturation=True,removesaturation_f=0.5,contrast=True,contrast_f=0.5,upflip=True,upflip_f=0.5,
-                            shear=True ,shear_f=0.5, rotate90=True,rotate90_f = 0.5,blur_and_noise=True,blur_and_noise_f=0.5,image_cutout = True,image_cutout_f=0.5,
-                            mix_aug=True,mix_aug_f=0.5,temperature_change=True,temperature_change_f=0.5,weather_change=True,weather_change_f=0.5):
+            logger.error(f'problem : Json converter  desc : {e}')       
+                   
+                  
+    def Combined_augmentation(self,im_read , poly_on_image, no_track,image_height=640 , image_width:Union[int,keep_aspect_ratio]=640, blur=True , blur_f = 0.5 , motionBlur = True , motion_blur_f = 0.5, rotate=True , rotate_f = 0.5 , noise=True,noise_f=0.5,perspective=True,perspective_f = 0.5,affine=True,affine_f=0.5,
+                              brightness=True,brightness_f=0.5,hue=True,hue_f=0.5,removesaturation=True,removesaturation_f=0.5,contrast=True,contrast_f=0.5,upflip=True,upflip_f=0.5,
+                              shear=True ,shear_f=0.5, rotate90=True,rotate90_f = 0.5,blur_and_noise=True,blur_and_noise_f=0.5,image_cutout = True,image_cutout_f=0.5,
+                              mix_aug=True,mix_aug_f=0.5,temperature_change=True,temperature_change_f=0.5,weather_change=True,weather_change_f=0.5):
+        
         
+        # combining all the augmentations here
         with concurrent.futures.ThreadPoolExecutor(max_workers=20) as executor:
+            
+            if blur:
+           
+                frac_data  = int(self.split * blur_f)
+                if no_track <= frac_data:
+                    try:
+                        points =  executor.submit(self.augment.image_blur,im_read,poly_on_image,image_height,image_width)
+                        p , im = next(points.result())
+                        utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+
+                    except Exception as e:
+                        logger.warning(f'Blur problem : {e} ')
+            
             if rotate:
                 frac_data  = int(self.split * rotate_f)
                 if no_track <= frac_data:
-            
-                    points2  = executor.submit(self.augment.image_rotate,im_read,rect_on_image,image_height,image_width) 
-                    p , im = next(points2.result())
-                    utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
-
-            if blur:
-                try:
-                    frac_data  = int(self.split * blur_f)
-                    if no_track <= frac_data:
-                
-                        points2  = executor.submit(self.augment.image_blur,im_read,rect_on_image,image_height,image_width) 
+                    try:
+                        points2  = executor.submit(self.augment.image_rotate,im_read,poly_on_image,image_height,image_width) 
                         p , im = next(points2.result())
-                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
-                except:
-                    pass
-
+                        utils_poly.create_new_txt(im,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                    except Exception as e:
+                        logger.warning(f'ROTATION problem : {e} ')
+                
             if noise:
                 frac_data  = int(self.split * noise_f)
                 if no_track <= frac_data:
-            
-                    points2  = executor.submit(self.augment.image_noise,im_read,rect_on_image,image_height,image_width) 
-                    p , im = next(points2.result())
-                    utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
-
+                    try:
+                        points3  = executor.submit(self.augment.image_noise,im_read,poly_on_image,image_height,image_width) 
+                        p , im = next(points3.result())
+                        utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                    except Exception as e:
+                        logger.warning(f'Noise problem : {e} ')
+                
             if perspective:
                 frac_data  = int(self.split * perspective_f)
                 if no_track <= frac_data:
-            
-                    points2  = executor.submit(self.augment.image_perspective_transform,im_read,rect_on_image,image_height,image_width) 
-                    p , im = next(points2.result())
-                    utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
-            
+                    try:
+                        points4  = executor.submit(self.augment.image_perspective_transform,im_read,poly_on_image,image_height,image_width) 
+                        p , im = next(points4.result())
+                        utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                    except Exception as e:
+                        logger.warning(f'Perspective problem : {e} ')
+                
             if affine:
                 frac_data  = int(self.split * affine_f)
                 if no_track <= frac_data:
-            
-                    points2  = executor.submit(self.augment.image_affine,im_read,rect_on_image,image_height,image_width) 
-                    p , im = next(points2.result())
-                    utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
-            
+                    try:
+                        points5  = executor.submit(self.augment.image_affine,im_read,poly_on_image,image_height,image_width) 
+                        p , im = next(points5.result())
+                        utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                    except Exception as e:
+                        logger.warning(f'Affine problem : {e} ')
+                
             if brightness:
                 frac_data  = int(self.split * brightness_f)
                 if no_track <= frac_data:
-            
-                    points2  = executor.submit(self.augment.image_brightness,im_read,rect_on_image,image_height,image_width) 
-                    p , im = next(points2.result())
-                    utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+                    try:
+                        points6  = executor.submit(self.augment.image_brightness,im_read,poly_on_image,image_height,image_width) 
+                        p , im = next(points6.result())
+                        utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
 
+                    except Exception as e:
+                        logger.warning(f'Brightness problem : {e} ')
+            
             if hue:
                 frac_data  = int(self.split * hue_f)
                 if no_track <= frac_data:
-            
-                    points2  = executor.submit(self.augment.image_hue,im_read,rect_on_image,image_height,image_width) 
-                    p , im = next(points2.result())
-                    utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
-
+                    try:
+                        points6  = executor.submit(self.augment.image_hue,im_read,poly_on_image,image_height,image_width) 
+                        p , im = next(points6.result())
+                        utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                    except Exception as e:
+                        logger.warning(f'hue problem : {e} ')
+                
             if removesaturation:
                 frac_data  = int(self.split * removesaturation_f)
                 if no_track <= frac_data:
-            
-                    points2  = executor.submit(self.augment.image_removeSaturation,im_read,rect_on_image,image_height,image_width) 
-                    p , im = next(points2.result())
-                    utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
-            
+                    try:
+                        points7  = executor.submit(self.augment.image_removeSaturation,im_read,poly_on_image,image_height,image_width) 
+                        p , im = next(points7.result())
+                        utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                    except Exception as e:
+                        logger.warning(f'remove saturation problem : {e} ')
+                
             if contrast:
                 frac_data  = int(self.split * contrast_f)
                 if no_track <= frac_data:
-            
-                    points2  = executor.submit(self.augment.image_contrast,im_read,rect_on_image,image_height,image_width) 
-                    p , im = next(points2.result())
-                    utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
-
+                    try:
+                        points8 = executor.submit(self.augment.image_contrast,im_read,poly_on_image,image_height,image_width) 
+                        p , im = next(points8.result())
+                        utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                    except Exception as e:
+                        logger.warning(f'Contrast problem : {e} ')
+                
             if upflip:
                 frac_data  = int(self.split * upflip_f)
                 if no_track <= frac_data:
-            
-                    points2  = executor.submit(self.augment.image_upFlip,im_read,rect_on_image,image_height,image_width) 
-                    p , im = next(points2.result())
-                    utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
-
+                    try:
+                        points9  = executor.submit(self.augment.image_upFlip,im_read,poly_on_image,image_height,image_width) 
+                        p , im = next(points9.result())
+                        utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                    except Exception as e:
+                        logger.warning(f'upflip problem : {e} ')
+                    
             if shear:
                 frac_data  = int(self.split * shear_f)
                 if no_track <= frac_data:
-            
-                    points2  = executor.submit(self.augment.image_shear,im_read,rect_on_image,image_height,image_width) 
-                    p , im = next(points2.result())
-                    utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+                    try:
+                        points10  = executor.submit(self.augment.image_shear,im_read,poly_on_image,image_height,image_width) 
+                        p , im = next(points10.result())
+                        utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
 
+                    except Exception as e:
+                        logger.warning(f'shear problem : {e} ')
+                
             if rotate90:
                 frac_data  = int(self.split * rotate90_f)
                 if no_track <= frac_data:
-            
-                    points2  = executor.submit(self.augment.image_rotate90,im_read,rect_on_image,image_height,image_width) 
-                    p , im = next(points2.result())
-                    utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
-
+                    try:
+                        points11  = executor.submit(self.augment.image_rotate90,im_read,poly_on_image,image_height,image_width) 
+                        p , im = next(points11.result())
+                        utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                    except Exception as e:
+                        logger.warning(f'rotate90 problem : {e} ')
+                
             if blur_and_noise:
                 frac_data  = int(self.split * blur_and_noise_f)
                 if no_track <= frac_data:
-            
-                    points2  = executor.submit(self.augment.blur_and_noise,im_read,rect_on_image,image_height,image_width) 
-                    p , im = next(points2.result())
-                    utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
-
+                    try:
+                        points12  = executor.submit(self.augment.blur_and_noise,im_read,poly_on_image,image_height,image_width) 
+                        p , im = next(points12.result())
+                        utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                    except Exception as e:
+                        logger.warning(f'Blur and noise problem : {e} ')
+                
             if image_cutout:
                 frac_data  = int(self.split * image_cutout_f)
                 if no_track <= frac_data:
+                    try:
+                        points13  = executor.submit(self.augment.image_cutOut,im_read,poly_on_image,image_height,image_width) 
+                        p , im = next(points13.result())
+                        utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                    except Exception as e:
+                        logger.warning(f'ImageCut problem : {e} ')
             
-                    points2  = executor.submit(self.augment.image_cutOut,im_read,rect_on_image,image_height,image_width) 
-                    p , im = next(points2.result())
-                    utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
-
             if mix_aug:
                 frac_data  = int(self.split * mix_aug_f)
                 if no_track <= frac_data:
-                    points14  = executor.submit(self.augment.mixed_aug_1,im_read,rect_on_image,image_height,image_width) 
-                    p , im = next(points14.result())
-                    utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+                    try:
+                        points14  = executor.submit(self.augment.mixed_aug_1,im_read,poly_on_image,image_height,image_width) 
+                        p , im = next(points14.result())
+                        utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                    
+                    except Exception as e:
+                        logger.warning(f'Mixaug1 problem : {e} ')
+                    
+                    try: 
+                        points15  = executor.submit(self.augment.mixed_aug_2,im_read,poly_on_image,image_height,image_width) 
+                        p , im = next(points15.result())
+                        utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                    except Exception as e:
+                        logger.warning(f'Mixaug 2 problem : {e} ')
+
+                    try:
+
+                        points16  = executor.submit(self.augment.mixed_aug_3,im_read,poly_on_image,image_height,image_width) 
+                        p , im = next(points16.result())
+                        utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
                     
-                    points15  = executor.submit(self.augment.mixed_aug_2,im_read,rect_on_image,image_height,image_width) 
-                    p , im = next(points15.result())
-                    utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+                    except Exception as e:
+                        logger.warning(f'MixAug 3 problem : {e} ')
                     
-                    points16  = executor.submit(self.augment.mixed_aug_3,im_read,rect_on_image,image_height,image_width) 
-                    p , im = next(points16.result())
-                    utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+                    try:
+                        points17  = executor.submit(self.augment.mixed_aug_4,im_read,poly_on_image,image_height,image_width) 
+                        p , im = next(points17.result())
+                        utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
                     
-                    points17  = executor.submit(self.augment.mixed_aug_4,im_read,rect_on_image,image_height,image_width) 
-                    p , im = next(points17.result())
-                    utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+                    except Exception as e:
+                        logger.warning(f'Mixaug 4 problem : {e} ')
             
             if temperature_change:
                 frac_data  = int(self.split * temperature_change_f)
                 if no_track <= frac_data:
-            
-                    points2  = executor.submit(self.augment.image_change_colorTemperature,im_read,rect_on_image,image_height,image_width) 
-                    p , im = next(points2.result())
-                    utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+                    try:
+                        points18  = executor.submit(self.augment.image_change_colorTemperature,im_read,poly_on_image,image_height,image_width) 
+                        p , im = next(points18.result())
+                        utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                    except Exception as e:
+                        logger.warning(f'Temperature change problem : {e} ')
 
             if weather_change:
                 frac_data  = int(self.split * weather_change_f)
                 if no_track <= frac_data:
-                    points20  = executor.submit(self.augment.image_weatherChange,im_read,rect_on_image,image_height,image_width) 
-                    p , im = next(points20.result())
-                    utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
-
-        
-            
-
-
-            
+                    try:
+                        points2  = executor.submit(self.augment.image_change_colorTemperature,im_read,poly_on_image,image_height,image_width) 
+                        p , im = next(points2.result())
+                        utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+                    
+                    except Exception as e:
+                        logger.warning(f'weather change problem : {e} ')
 
+            if motionBlur:
+                frac_data  = int(self.split * motion_blur_f)
+                if no_track <= frac_data:
+                    try:
+                        points2  = executor.submit(self.augment.image_motionBlur,im_read,poly_on_image,image_height,image_width) 
+                        p , im = next(points2.result())
+                        utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
 
+                    except Exception as e:
+                        logger.warning(f'MotionBlur problem : {e} ')
 
+                
+             
+  
+               
     
     def Image_augmentation(self,folder,train_split=1.0,image_height:Union[int,keep_original_image_height]=640 , image_width:Union[int,keep_aspect_ratio,keep_original_image_width]=640,blur=True , blur_f = 0.5 , rotate=True , rotate_f = 0.5 , noise=True,noise_f=0.5,perspective=True,perspective_f = 0.5,affine=True,affine_f=0.5,
                             brightness=True,brightness_f=0.5,hue=True,hue_f=0.5,removesaturation=True,removesaturation_f=0.5,contrast=True,contrast_f=0.5,upflip=True,upflip_f=0.5,
                             shear=True ,shear_f=0.5, rotate90=True,rotate90_f = 0.5,blur_and_noise=True,blur_and_noise_f=0.5,image_cutout = True,image_cutout_f=0.5,
-                            mix_aug=True,mix_aug_f=0.5,temperature_change=True,temperature_change_f=0.5,weather_change=True,weather_change_f=0.5):
+                            mix_aug=True,mix_aug_f=0.5,temperature_change=True,temperature_change_f=0.5,weather_change=True,weather_change_f=0.5,motionBlur=True,motionBlur_f=0.5):
         
         #checking if input folder is a directory or not
         dir_checker = os.path.isdir(folder)
         
         if dir_checker != True:
             shutil.rmtree(self.aug_save_folder_name)
             raise NotADirectoryError(f'Provided Path - {folder} is not a directory...')
        
         # changing other images format to same format '.jpg'
         self.image_format_change(folder=folder)
         
         # getting all json and jpg images
         all_images =  glob.glob(f'{folder}/*jpg')
-        all_txt =  glob.glob(f'{folder}/*txt')
-        classes_ = glob.glob(f'{folder}/classes*txt')
-
-        
-
-        if classes_ != []:
-            with open(classes_[0]) as f:
-                data = f.readlines()
-                for index ,classes_name in enumerate(data):
-                    self.store_dict[index] = classes_name.rstrip()
-                    
-                console.print('[bold green] classes.txt found.. [bold green]')
-        else:
-            raise NotImplementedError('Classes.txt not Found !!')
+        all_json =  glob.glob(f'{folder}/*json')
         
         # checking json and images are same or not and checking their len too
-        if classes_ != []:
-            if len(all_images)  == len(all_txt) -1 and len(all_images)  >= 1 and len(all_txt) -1 >=1:
-                del all_txt
+        if len(all_images) == len(all_json) and len(all_images) >= 1 and len(all_json) >=1:
+            del all_json
             
-            else:
-                shutil.rmtree(self.aug_save_folder_name)
-                raise NotImplementedError(f'Images and Txt are not equal , recheck your annotation folder! Total Images : {len(all_images)}  |  Total txt : {len(all_txt)-1}')
+        else:
+            shutil.rmtree(self.aug_save_folder_name)
+            raise NotImplementedError(f'Images and Jsons are not equal , recheck your annotation folder! \
+                                       Total Images : {len(all_images)}  |  Total Json : {len(all_json)}')
         # checking train is float or not
         if type(train_split) != float:
             shutil.rmtree(self.aug_save_folder_name)
             raise TypeError(f'please provide "train split" as "float" , You provided train split as {type(train_split)}')
             
         # checking train split value > 1.0 or not   
         if train_split > 1.0:
@@ -352,15 +399,16 @@
                 'affine_f':affine_f,
                 'perspective_f':perspective_f,
                 'upflip_f' : upflip_f,
                 'shear_f' : shear_f,
                 'image_cut_f':image_cutout_f,
                 'mix_aug_f' : mix_aug_f,
                 'temperaure_change_f' : temperature_change_f,
-                'weather_change_f' : weather_change_f
+                'weather_change_f' : weather_change_f,
+                'motionBlur_f' : motionBlur_f
                 
               }
         
         type_2 = { 
                 'blur':blur,
                 'noise':noise,
                 'NB':blur_and_noise,
@@ -373,15 +421,16 @@
                 'affine':affine,
                 'perspective':perspective,
                 'upflip' : upflip,
                 'shear' : shear,
                 'image_cut':image_cutout,
                 'mix_aug' : mix_aug,
                 'temp_change' : temperature_change,
-                'weather_change' : weather_change
+                'weather_change' : weather_change,
+                'motionBlur' : motionBlur
                 
               }
 
         # checking the types 
         for types , val in type_1.items():
             if type(val) != float:
                 shutil.rmtree(self.aug_save_folder_name)
@@ -424,60 +473,82 @@
         self.len_total_images = len(all_images)
         # spliting into training set
         self.split = int(self.len_total_images * train_split)
         
         console.print(f'[bold cyan] [+] Total images : {self.len_total_images}   |   Train Split : {self.split} images   |    Test split : {self.len_total_images-self.split} images [bold cyan]')
         
         if train_split == 1.0:
+                    shutil.rmtree(self.aug_save_folder_name)
                     shutil.rmtree(f'{self.aug_save_folder_name}/test')
         
         # if c value less than equal to train split then we will add those images in training data and rest will go for test data            
         for c ,images in enumerate(track(all_images,description='Image Augmentation..',total=len(all_images[:self.split]))):
 
             if c+1 <= self.split:
 
+                try:
                 
-              
-                poly = list(self.txt_converter(images))
-          
-                #if we want to keep original image height and width -->
-                if image_height == 'keep_original_image_height' and image_width == 'keep_original_image_width':
-                    image_height_N , image_width_N , channel = poly[0][0].shape
-                
-                # print(poly)
-
-                self.Combined_augmentation(poly[0][0],poly[0][1],c+1,image_height_N,image_width_N,blur=blur , blur_f = blur_f , rotate=rotate , rotate_f = rotate_f , noise=noise,noise_f=noise_f,perspective=perspective,perspective_f = perspective_f,affine=affine,affine_f=affine_f,
-                              brightness=brightness,brightness_f=brightness_f,hue=hue,hue_f=hue_f,removesaturation=removesaturation,removesaturation_f=removesaturation_f,contrast=contrast,contrast_f=contrast_f,upflip=upflip,upflip_f=upflip_f,
-                              shear= shear ,shear_f=shear_f, rotate90=rotate90,rotate90_f = rotate90_f,blur_and_noise=blur_and_noise,blur_and_noise_f=blur_and_noise_f,image_cutout = image_cutout,image_cutout_f=image_cutout_f,
-                              mix_aug=mix_aug,mix_aug_f=mix_aug_f,temperature_change=temperature_change,temperature_change_f=temperature_change_f,weather_change=weather_change,weather_change_f=weather_change_f)
-                
+                    poly = list(self.json_converter(images))
+
+                    #if we want to keep original image height and width -->
+                    if image_height == 'keep_original_image_height' and image_width == 'keep_original_image_width':
+                        image_height_N , image_width_N , _ = poly[0][0].shape
+
+                    self.Combined_augmentation(poly[0][0],poly[0][1],c+1,image_height_N,image_width_N,blur=blur , blur_f = blur_f , rotate=rotate , rotate_f = rotate_f , noise=noise,noise_f=noise_f,perspective=perspective,perspective_f = perspective_f,affine=affine,affine_f=affine_f,
+                                brightness=brightness,brightness_f=brightness_f,hue=hue,hue_f=hue_f,removesaturation=removesaturation,removesaturation_f=removesaturation_f,contrast=contrast,contrast_f=contrast_f,upflip=upflip,upflip_f=upflip_f,
+                                shear= shear ,shear_f=shear_f, rotate90=rotate90,rotate90_f = rotate90_f,blur_and_noise=blur_and_noise,blur_and_noise_f=blur_and_noise_f,image_cutout = image_cutout,image_cutout_f=image_cutout_f,
+                                mix_aug=mix_aug,mix_aug_f=mix_aug_f,temperature_change=temperature_change,temperature_change_f=temperature_change_f,weather_change=weather_change,weather_change_f=weather_change_f,motionBlur=motionBlur,motion_blur_f=motionBlur_f)
+                
+                except Exception as e:
+                    console.print('[bold yellow] WARNING [bold yellow] : There is some problem with data , skipping this...')
+                    logger.error(f'combined augmentation problem : {e}')
                 
                 
             elif c+1 > self.split:
-                # print(images)
-                
-                poly = list(self.txt_converter(f'{images}'))
+              
+                try:
+                    
+                    poly = list(self.json_converter(f'{images}'))
+                    utils_poly.create_new_txt(poly[0][0] ,self.labels,poly[0][1],self.test_images_path,self.test_labels_path,self.store_dict,yolo=self.yolo)
 
-                utils_poly.create_new_txt(poly[0][0] ,poly[0][1],self.test_images_path,self.test_labels_path)
+                except Exception as e:
+                    console.print('[bold yellow] WARNING [bold yellow] : There is some problem with data , skipping this...')
+                    logger.error(f'combined augmentation problem : {e}')
+                
                    
-        console.print(f'[bold dim cyan] Labels name : [/bold dim cyan] [bold magenta] {list(self.store_dict.values())} [bold magenta]')
-
-        yml_writer_poly.yaml_writer(len(self.store_dict.keys()),list(self.store_dict.values()),self.aug_save_folder_name)   
-
-        with open(f'{self.aug_save_folder_name}/classes.txt','w') as f:
-            f.write('\n'.join(list(self.store_dict.values()))) 
+        console.print(f'[bold dim cyan] Labels name : [/bold dim cyan] [bold magenta] {list(self.store_dict.keys())} [bold magenta]')
+        yml_writer_poly.yaml_writer(len(self.store_dict.keys()),list(self.store_dict.keys()),self.aug_save_folder_name)      
+      
       
       
       
     @staticmethod
     def image_format_change(folder):
         for im in os.listdir(folder):
-            if im.endswith('.txt'):
+            if im.endswith('.json'):
                 continue
             elif im.endswith('.jpg'):
                 continue
             else:
                 
                 im_name = im.split('.')[0]
                 ims = cv2.imread(f'{folder}/{im}')
                 cv2.imwrite(f'{folder}/{im_name}.jpg',ims)
-                os.remove(f'{folder}/{im}')
+                os.remove(f'{folder}/{im}')
+                      
+
+         
+
+
+    
+
+
+
+
+
+
+
+
+
+
+  
+
```

### Comparing `image_augs-2.2.9/object_detection_new/utils_poly.py` & `image_augs-2.3.10/object_detection_new/utils_poly.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 import uuid
 import cv2
 import os
-import labelme
+
 from numpyencoder import NumpyEncoder
 
-import base64
-import json
+
 
 import instance_seg.logging_util as logging_util
 
 logger = logging_util.get_logger(os.path.basename(__file__).split('.')[0])
 
 def create_new_txt(image ,points,train_path_images , train_path_labels):
 
    
 
     try:
             save_name = uuid.uuid4()
             
-            if type(image) == str:
-                image = cv2.imread(image)
-
-            cv2.imwrite(f'{train_path_images}/{save_name}.jpg',image)
+            
             txt_path=f'{train_path_labels}/{save_name}.txt'
             
             new_height , new_width , c = image.shape
         
             for p in points: 
                 
                 labels = p.label 
@@ -33,22 +29,29 @@
                 
                 new_name = str(labels) + ' '
 
                 x1norm , y1norm , x2norm , y2norm = convert_to_yolo_bbox([new_x1,new_y1,new_x2,new_y2],new_width,new_height)
                 new_name += f'{x1norm} {y1norm} {x2norm} {y2norm}'
                 new_name += ' '
 
-               
-                with open(txt_path,'a+') as f:
+                if new_name != '':
+
+                    if type(image) == str:
+                        image = cv2.imread(image)
+
+                    cv2.imwrite(f'{train_path_images}/{save_name}.jpg',image)
+
+                    with open(txt_path,'a+') as f:
                     
-                    f.write(new_name)
-                    f.write('\n')
+                        f.write(new_name)
+                        f.write('\n')
                     
                         
-                del new_name
+                    del new_name
+            
             
     except Exception as e:
             logger.warning(f'problem : create new json  desc : {e}')
 
 
 def convert_to_normal_bbox(yolo_bbox, image_width, image_height):
     """
```

### Comparing `image_augs-2.2.9/setup.py` & `image_augs-2.3.10/setup.py`

 * *Files identical despite different names*

