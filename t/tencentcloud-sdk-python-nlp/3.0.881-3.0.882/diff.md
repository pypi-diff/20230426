# Comparing `tmp/tencentcloud-sdk-python-nlp-3.0.881.tar.gz` & `tmp/tencentcloud-sdk-python-nlp-3.0.882.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-nlp-3.0.881.tar", last modified: Tue Apr 25 00:46:11 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-nlp-3.0.882.tar", last modified: Wed Apr 26 03:39:36 2023, max compression
```

## Comparing `tencentcloud-sdk-python-nlp-3.0.881.tar` & `tencentcloud-sdk-python-nlp-3.0.882.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:46:11.000000 tencentcloud-sdk-python-nlp-3.0.881/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-25 00:46:11.000000 tencentcloud-sdk-python-nlp-3.0.881/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:46:11.000000 tencentcloud-sdk-python-nlp-3.0.881/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:46:11.000000 tencentcloud-sdk-python-nlp-3.0.881/tencentcloud/nlp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:46:11.000000 tencentcloud-sdk-python-nlp-3.0.881/tencentcloud/nlp/v20190408/
--rw-r--r--   0 root         (0) root         (0)     5316 2023-04-25 00:46:11.000000 tencentcloud-sdk-python-nlp-3.0.881/tencentcloud/nlp/v20190408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    29728 2023-04-25 00:46:11.000000 tencentcloud-sdk-python-nlp-3.0.881/tencentcloud/nlp/v20190408/nlp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:46:11.000000 tencentcloud-sdk-python-nlp-3.0.881/tencentcloud/nlp/v20190408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56111 2023-04-25 00:46:11.000000 tencentcloud-sdk-python-nlp-3.0.881/tencentcloud/nlp/v20190408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:46:11.000000 tencentcloud-sdk-python-nlp-3.0.881/tencentcloud/nlp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:46:11.000000 tencentcloud-sdk-python-nlp-3.0.881/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:46:11.000000 tencentcloud-sdk-python-nlp-3.0.881/tencentcloud_sdk_python_nlp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:46:11.000000 tencentcloud-sdk-python-nlp-3.0.881/tencentcloud_sdk_python_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-25 00:46:11.000000 tencentcloud-sdk-python-nlp-3.0.881/tencentcloud_sdk_python_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:46:11.000000 tencentcloud-sdk-python-nlp-3.0.881/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:46:11.000000 tencentcloud-sdk-python-nlp-3.0.881/tencentcloud_sdk_python_nlp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:46:11.000000 tencentcloud-sdk-python-nlp-3.0.881/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-25 00:46:11.000000 tencentcloud-sdk-python-nlp-3.0.881/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:46:11.000000 tencentcloud-sdk-python-nlp-3.0.881/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:39:36.000000 tencentcloud-sdk-python-nlp-3.0.882/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-26 03:39:36.000000 tencentcloud-sdk-python-nlp-3.0.882/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:39:36.000000 tencentcloud-sdk-python-nlp-3.0.882/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:39:36.000000 tencentcloud-sdk-python-nlp-3.0.882/tencentcloud/nlp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:39:36.000000 tencentcloud-sdk-python-nlp-3.0.882/tencentcloud/nlp/v20190408/
+-rw-r--r--   0 root         (0) root         (0)     5906 2023-04-26 03:39:36.000000 tencentcloud-sdk-python-nlp-3.0.882/tencentcloud/nlp/v20190408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    37659 2023-04-26 03:39:36.000000 tencentcloud-sdk-python-nlp-3.0.882/tencentcloud/nlp/v20190408/nlp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:39:36.000000 tencentcloud-sdk-python-nlp-3.0.882/tencentcloud/nlp/v20190408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80999 2023-04-26 03:39:36.000000 tencentcloud-sdk-python-nlp-3.0.882/tencentcloud/nlp/v20190408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:39:36.000000 tencentcloud-sdk-python-nlp-3.0.882/tencentcloud/nlp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 03:39:36.000000 tencentcloud-sdk-python-nlp-3.0.882/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:39:36.000000 tencentcloud-sdk-python-nlp-3.0.882/tencentcloud_sdk_python_nlp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:39:36.000000 tencentcloud-sdk-python-nlp-3.0.882/tencentcloud_sdk_python_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-26 03:39:36.000000 tencentcloud-sdk-python-nlp-3.0.882/tencentcloud_sdk_python_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:39:36.000000 tencentcloud-sdk-python-nlp-3.0.882/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 03:39:36.000000 tencentcloud-sdk-python-nlp-3.0.882/tencentcloud_sdk_python_nlp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:39:36.000000 tencentcloud-sdk-python-nlp-3.0.882/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-26 03:39:36.000000 tencentcloud-sdk-python-nlp-3.0.882/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 03:39:36.000000 tencentcloud-sdk-python-nlp-3.0.882/setup.cfg
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.881/README.rst` & `tencentcloud-sdk-python-nlp-3.0.882/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-nlp-3.0.881/tencentcloud/nlp/v20190408/errorcodes.py` & `tencentcloud-sdk-python-nlp-3.0.882/tencentcloud/nlp/v20190408/errorcodes.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,26 +22,35 @@
 
 # 余额不足，开通失败，请充值后再开通。
 FAILEDOPERATION_BALANCEINSUFFICIENT = 'FailedOperation.BalanceInsufficient'
 
 # 非法文本输入导致返回异常
 FAILEDOPERATION_ILLEGALTEXTERROR = 'FailedOperation.IllegalTextError'
 
+# 服务内部错误，请重试。
+FAILEDOPERATION_INNERERROR = 'FailedOperation.InnerError'
+
 # 暂无春联生成，请更换关键词重试。
 FAILEDOPERATION_NOCOUPLETS = 'FailedOperation.NoCouplets'
 
 # 暂无诗词生成，请更换关键词重试。
 FAILEDOPERATION_NOPOETRY = 'FailedOperation.NoPoetry'
 
+# 暂无结果，请更换文本重试。
+FAILEDOPERATION_NORESULTS = 'FailedOperation.NoResults'
+
 # 未查询到结果。
 FAILEDOPERATION_NOTFOUNDDATA = 'FailedOperation.NotFoundData'
 
 # 后端服务超时。
 FAILEDOPERATION_REQUESTTIMEOUT = 'FailedOperation.RequestTimeout'
 
+# 服务器繁忙，请稍后再试。
+FAILEDOPERATION_RESOURCEBUSY = 'FailedOperation.ResourceBusy'
+
 # RPC请求失败，一般为算法微服务故障。
 FAILEDOPERATION_RPCFAIL = 'FailedOperation.RpcFail'
 
 # 文本向量化失败
 FAILEDOPERATION_TEXTEMBEDDINGFAILED = 'FailedOperation.TextEmbeddingFailed'
 
 # 内部错误。
@@ -64,20 +73,29 @@
 
 # 内部服务调用失败。
 INTERNALERROR_SERVICEERROR = 'InternalError.ServiceError'
 
 # 参数错误。
 INVALIDPARAMETER = 'InvalidParameter'
 
+# 服务调用失败。
+INVALIDPARAMETER_SERVICEERROR = 'InvalidParameter.ServiceError'
+
+# 文本长度超过限制。
+INVALIDPARAMETER_TEXTTOOLONGCODE = 'InvalidParameter.TextTooLongCode'
+
 # 参数空值错误
 INVALIDPARAMETERVALUE_EMPTYVALUEERROR = 'InvalidParameterValue.EmptyValueError'
 
 # Genre非法，请参考Genre参数说明。
 INVALIDPARAMETERVALUE_GENRE = 'InvalidParameterValue.Genre'
 
+# 参数不合法。
+INVALIDPARAMETERVALUE_INVALIDPARAMETER = 'InvalidParameterValue.InvalidParameter'
+
 # PoetryType非法，请参考PoetryType参数说明。
 INVALIDPARAMETERVALUE_POETRYTYPE = 'InvalidParameterValue.PoetryType'
 
 # Text输入含有敏感信息。
 INVALIDPARAMETERVALUE_SENSITIVETEXT = 'InvalidParameterValue.SensitiveText'
 
 # TargetType非法，请参考TargetType参数说明。
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.881/tencentcloud/nlp/v20190408/nlp_client.py` & `tencentcloud-sdk-python-nlp-3.0.882/tencentcloud/nlp/v20190408/nlp_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -253,14 +253,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def EvaluateSentenceSimilarity(self, request):
+        """通过计算句子间的语义相似性，帮助您快速找到文本中重复或相似的句子，用于文本聚类、相似问题检索等应用场景。
+
+        :param request: Request instance for EvaluateSentenceSimilarity.
+        :type request: :class:`tencentcloud.nlp.v20190408.models.EvaluateSentenceSimilarityRequest`
+        :rtype: :class:`tencentcloud.nlp.v20190408.models.EvaluateSentenceSimilarityResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("EvaluateSentenceSimilarity", params, headers=headers)
+            response = json.loads(body)
+            model = models.EvaluateSentenceSimilarityResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def EvaluateWordSimilarity(self, request):
+        """评估两个词语在语义空间的相似程度，为您的场景应用提供有力支持，如关键词过滤、热门话题挖掘等。（目前仅支持中文）
+
+        :param request: Request instance for EvaluateWordSimilarity.
+        :type request: :class:`tencentcloud.nlp.v20190408.models.EvaluateWordSimilarityRequest`
+        :rtype: :class:`tencentcloud.nlp.v20190408.models.EvaluateWordSimilarityResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("EvaluateWordSimilarity", params, headers=headers)
+            response = json.loads(body)
+            model = models.EvaluateWordSimilarityResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def GenerateCouplet(self, request):
         """根据用户输入的命题关键词自动生成一副春联，包括上联、下联和横批。（如需开通请联系商务）
 
         :param request: Request instance for GenerateCouplet.
         :type request: :class:`tencentcloud.nlp.v20190408.models.GenerateCoupletRequest`
         :rtype: :class:`tencentcloud.nlp.v20190408.models.GenerateCoupletResponse`
 
@@ -276,14 +322,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def GenerateKeywordSentence(self, request):
+        """提取文本中的关键信息，生成简洁明了的关键句子，便于用户快速获取核心观点。
+
+        :param request: Request instance for GenerateKeywordSentence.
+        :type request: :class:`tencentcloud.nlp.v20190408.models.GenerateKeywordSentenceRequest`
+        :rtype: :class:`tencentcloud.nlp.v20190408.models.GenerateKeywordSentenceResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("GenerateKeywordSentence", params, headers=headers)
+            response = json.loads(body)
+            model = models.GenerateKeywordSentenceResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def GeneratePoetry(self, request):
         """根据用户输入的命题关键词自动生成一首七言律诗或五言律诗。（如需开通请联系商务）
 
         :param request: Request instance for GeneratePoetry.
         :type request: :class:`tencentcloud.nlp.v20190408.models.GeneratePoetryRequest`
         :rtype: :class:`tencentcloud.nlp.v20190408.models.GeneratePoetryResponse`
 
@@ -353,14 +422,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ParseWords(self, request):
+        """通过精准地对文本进行分词、词性标注、命名实体识别等功能，助您更好地理解文本内容，挖掘出潜在的价值信息。
+
+        :param request: Request instance for ParseWords.
+        :type request: :class:`tencentcloud.nlp.v20190408.models.ParseWordsRequest`
+        :rtype: :class:`tencentcloud.nlp.v20190408.models.ParseWordsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ParseWords", params, headers=headers)
+            response = json.loads(body)
+            model = models.ParseWordsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def RetrieveSimilarWords(self, request):
+        """基于大数据和深度学习技术，可以快速地找到与给定词语高度相似的其他词语，有助于提高搜索和推荐的准确性。（目前仅支持中文）
+
+        :param request: Request instance for RetrieveSimilarWords.
+        :type request: :class:`tencentcloud.nlp.v20190408.models.RetrieveSimilarWordsRequest`
+        :rtype: :class:`tencentcloud.nlp.v20190408.models.RetrieveSimilarWordsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("RetrieveSimilarWords", params, headers=headers)
+            response = json.loads(body)
+            model = models.RetrieveSimilarWordsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def SearchWordItems(self, request):
         """查询指定自定义词库中的词条是否存在。
 
         :param request: Request instance for SearchWordItems.
         :type request: :class:`tencentcloud.nlp.v20190408.models.SearchWordItemsRequest`
         :rtype: :class:`tencentcloud.nlp.v20190408.models.SearchWordItemsResponse`
 
@@ -376,14 +491,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def SentenceCorrection(self, request):
+        """智能识别并纠正句子中的语法、拼写、用词等错误，确保文本的准确性和可读性。
+
+        :param request: Request instance for SentenceCorrection.
+        :type request: :class:`tencentcloud.nlp.v20190408.models.SentenceCorrectionRequest`
+        :rtype: :class:`tencentcloud.nlp.v20190408.models.SentenceCorrectionResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("SentenceCorrection", params, headers=headers)
+            response = json.loads(body)
+            model = models.SentenceCorrectionResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def SentenceEmbedding(self, request):
         """句向量接口能够将输入的句子映射成一个固定维度的向量，用来表示这个句子的语义特征，可用于文本聚类、文本相似度、文本分类等任务，能够显著提高它们的效果。
 
         该句向量服务由腾讯云自然语言处理团队联合微信智言团队共同打造，基于千亿级大规模互联网语料并采用Bert等领先的深度神经网络模型训练而成，在腾讯内部诸多业务的NLP任务上实测效果显著。
 
         :param request: Request instance for SentenceEmbedding.
         :type request: :class:`tencentcloud.nlp.v20190408.models.SentenceEmbeddingRequest`
@@ -528,14 +666,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def TextEmbellish(self, request):
+        """运用先进的自然语言处理技术，对原始文本进行优化润色，提升文本的通顺性、表达力和语言质量。
+
+        :param request: Request instance for TextEmbellish.
+        :type request: :class:`tencentcloud.nlp.v20190408.models.TextEmbellishRequest`
+        :rtype: :class:`tencentcloud.nlp.v20190408.models.TextEmbellishResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("TextEmbellish", params, headers=headers)
+            response = json.loads(body)
+            model = models.TextEmbellishResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def TextSimilarity(self, request):
         """句子相似度接口能够基于深度学习技术来计算一个源句子和多个目标句子的相似度，相似度分值越大的两个句子在语义上越相似。目前仅支持短文本（不超过500字符）的相似度计算，长文本的相似度计算也即将推出。
 
         鉴于句子相似度是一个应用非常广泛的功能，腾讯云自然语言处理团队在Bert等领先的深度神经网络模型的基础上，专门针对文本相似任务进行了优化，并持续迭代更新。基于句子相似度，可以轻松实现诸如文本去重、相似推荐等功能。
 
         接口将以句子数量为单位消耗资源包，而不是调用接口次数为单位。
 
@@ -580,14 +741,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def TextWriting(self, request):
+        """通过自动补全文本片段，帮助用户快速生成高质量、连贯的完整文本，提高创作效率。
+
+        :param request: Request instance for TextWriting.
+        :type request: :class:`tencentcloud.nlp.v20190408.models.TextWritingRequest`
+        :rtype: :class:`tencentcloud.nlp.v20190408.models.TextWritingResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("TextWriting", params, headers=headers)
+            response = json.loads(body)
+            model = models.TextWritingResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def UpdateDict(self, request):
         """修改自定义词库元数据信息，包括名称、描述。
 
         :param request: Request instance for UpdateDict.
         :type request: :class:`tencentcloud.nlp.v20190408.models.UpdateDictRequest`
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.881/tencentcloud/nlp/v20190408/models.py` & `tencentcloud-sdk-python-nlp-3.0.882/tencentcloud/nlp/v20190408/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -64,14 +64,50 @@
 
 
     def _deserialize(self, params):
         self.Summary = params.get("Summary")
         self.RequestId = params.get("RequestId")
 
 
+class BasicParticiple(AbstractModel):
+    """基础粒度分词和词性标注的结果
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Word: 基础词。
+        :type Word: str
+        :param BeginOffset: 基础词在NormalText中的起始位置。
+        :type BeginOffset: int
+        :param Length: 基础词的长度。
+        :type Length: int
+        :param Pos: 词性。
+        :type Pos: str
+        """
+        self.Word = None
+        self.BeginOffset = None
+        self.Length = None
+        self.Pos = None
+
+
+    def _deserialize(self, params):
+        self.Word = params.get("Word")
+        self.BeginOffset = params.get("BeginOffset")
+        self.Length = params.get("Length")
+        self.Pos = params.get("Pos")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class CCIToken(AbstractModel):
     """文本纠错结果
 
     """
 
     def __init__(self):
         r"""
@@ -213,14 +249,109 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class CompoundParticiple(AbstractModel):
+    """复合粒度分词和词性标注的结果。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Word: 基础词。
+        :type Word: str
+        :param BeginOffset: 基础词在NormalText中的起始位置。
+        :type BeginOffset: int
+        :param Length: 基础词的长度。
+        :type Length: int
+        :param Pos: 词性。
+        :type Pos: str
+        """
+        self.Word = None
+        self.BeginOffset = None
+        self.Length = None
+        self.Pos = None
+
+
+    def _deserialize(self, params):
+        self.Word = params.get("Word")
+        self.BeginOffset = params.get("BeginOffset")
+        self.Length = params.get("Length")
+        self.Pos = params.get("Pos")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CorrectionItem(AbstractModel):
+    """纠错结果列表
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Order: 纠错句子的序号。
+        :type Order: int
+        :param BeginOffset: 错误的起始位置，从0开始。
+        :type BeginOffset: int
+        :param Len: 错误内容长度。
+        :type Len: int
+        :param Word: 错误内容。
+        :type Word: str
+        :param CorrectWord: 纠错结果，当为删除类错误时，结果为null。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CorrectWord: list of str
+        :param CorrectionType: 纠错类型。0：替换；1：插入；2：删除。
+        :type CorrectionType: int
+        :param Confidence: 纠错信息置信度。0：error；1：warning；error的置信度更高。（仅供参考）
+        :type Confidence: int
+        :param DescriptionZh: 纠错信息中文描述。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DescriptionZh: str
+        :param DescriptionEn: 纠错信息英文描述。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DescriptionEn: str
+        """
+        self.Order = None
+        self.BeginOffset = None
+        self.Len = None
+        self.Word = None
+        self.CorrectWord = None
+        self.CorrectionType = None
+        self.Confidence = None
+        self.DescriptionZh = None
+        self.DescriptionEn = None
+
+
+    def _deserialize(self, params):
+        self.Order = params.get("Order")
+        self.BeginOffset = params.get("BeginOffset")
+        self.Len = params.get("Len")
+        self.Word = params.get("Word")
+        self.CorrectWord = params.get("CorrectWord")
+        self.CorrectionType = params.get("CorrectionType")
+        self.Confidence = params.get("Confidence")
+        self.DescriptionZh = params.get("DescriptionZh")
+        self.DescriptionEn = params.get("DescriptionEn")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class CreateDictRequest(AbstractModel):
     """CreateDict请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -726,14 +857,191 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class Embellish(AbstractModel):
+    """文本润色结果
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Text: 润色后的文本。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Text: str
+        :param EmbellishType: 润色类型。类型列表
+expansion：扩写
+rewriting：改写
+translation_m2a：从现代文改写为古文
+translation_a2m：从古文改写为现代文
+
+
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EmbellishType: str
+        """
+        self.Text = None
+        self.EmbellishType = None
+
+
+    def _deserialize(self, params):
+        self.Text = params.get("Text")
+        self.EmbellishType = params.get("EmbellishType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class Entity(AbstractModel):
+    """实体识别结果。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Word: 基础词。
+        :type Word: str
+        :param BeginOffset: 基础词在NormalText中的起始位置。
+        :type BeginOffset: int
+        :param Length: 基础词的长度。
+        :type Length: int
+        :param Type: 实体类型的标准名字。
+        :type Type: str
+        :param Name: 类型名字的自然语言表达。（中文或英文）
+        :type Name: str
+        """
+        self.Word = None
+        self.BeginOffset = None
+        self.Length = None
+        self.Type = None
+        self.Name = None
+
+
+    def _deserialize(self, params):
+        self.Word = params.get("Word")
+        self.BeginOffset = params.get("BeginOffset")
+        self.Length = params.get("Length")
+        self.Type = params.get("Type")
+        self.Name = params.get("Name")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class EvaluateSentenceSimilarityRequest(AbstractModel):
+    """EvaluateSentenceSimilarity请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SentencePairList: 待分析的句子对数组。句子对应不超过5对，支持中英文文本，原句子与目标句子均应不超过500字符。
+        :type SentencePairList: list of SentencePair
+        """
+        self.SentencePairList = None
+
+
+    def _deserialize(self, params):
+        if params.get("SentencePairList") is not None:
+            self.SentencePairList = []
+            for item in params.get("SentencePairList"):
+                obj = SentencePair()
+                obj._deserialize(item)
+                self.SentencePairList.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class EvaluateSentenceSimilarityResponse(AbstractModel):
+    """EvaluateSentenceSimilarity返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ScoreList: 每个句子对的相似度分值。
+        :type ScoreList: list of float
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.ScoreList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.ScoreList = params.get("ScoreList")
+        self.RequestId = params.get("RequestId")
+
+
+class EvaluateWordSimilarityRequest(AbstractModel):
+    """EvaluateWordSimilarity请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SourceWord: 计算相似度的源词。（仅支持UTF-8格式，不超过10字符）
+
+        :type SourceWord: str
+        :param TargetWord: 计算相似度的目标词。（仅支持UTF-8格式，不超过10字符）
+
+        :type TargetWord: str
+        """
+        self.SourceWord = None
+        self.TargetWord = None
+
+
+    def _deserialize(self, params):
+        self.SourceWord = params.get("SourceWord")
+        self.TargetWord = params.get("TargetWord")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class EvaluateWordSimilarityResponse(AbstractModel):
+    """EvaluateWordSimilarity返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Similarity: 词相似度分值。
+        :type Similarity: float
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Similarity = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Similarity = params.get("Similarity")
+        self.RequestId = params.get("RequestId")
+
+
 class GenerateCoupletRequest(AbstractModel):
     """GenerateCouplet请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -783,14 +1091,76 @@
     def _deserialize(self, params):
         self.TopScroll = params.get("TopScroll")
         self.Content = params.get("Content")
         self.RandomCause = params.get("RandomCause")
         self.RequestId = params.get("RequestId")
 
 
+class GenerateKeywordSentenceRequest(AbstractModel):
+    """GenerateKeywordSentence请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param WordList: 生成句子的关键词，关键词个数需不超过4个，中文关键词长度应不超过10字符，英文关键词长度不超过3个单词。关键词中不可包含标点符号。
+        :type WordList: list of str
+        :param Number: 返回生成句子的个数。数量需>=1且<=5。
+（注意实际结果可能小于指定个数）
+        :type Number: int
+        :param Domain: 指定生成句子的领域，支持领域列表
+general：通用领域，支持中英文
+academic：学术领域，仅支持英文
+默认为general（通用领域）。
+        :type Domain: str
+        """
+        self.WordList = None
+        self.Number = None
+        self.Domain = None
+
+
+    def _deserialize(self, params):
+        self.WordList = params.get("WordList")
+        self.Number = params.get("Number")
+        self.Domain = params.get("Domain")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class GenerateKeywordSentenceResponse(AbstractModel):
+    """GenerateKeywordSentence返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param KeywordSentenceList: 生成的句子列表。
+        :type KeywordSentenceList: list of KeywordSentence
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.KeywordSentenceList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("KeywordSentenceList") is not None:
+            self.KeywordSentenceList = []
+            for item in params.get("KeywordSentenceList"):
+                obj = KeywordSentence()
+                obj._deserialize(item)
+                self.KeywordSentenceList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class GeneratePoetryRequest(AbstractModel):
     """GeneratePoetry请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -868,14 +1238,38 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class KeywordSentence(AbstractModel):
+    """通过关键词生成的句子信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TargetText: 通过关键词生成的句子。
+        :type TargetText: str
+        """
+        self.TargetText = None
+
+
+    def _deserialize(self, params):
+        self.TargetText = params.get("TargetText")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class KeywordsExtractionRequest(AbstractModel):
     """KeywordsExtraction请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1033,14 +1427,88 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ParseWordsRequest(AbstractModel):
+    """ParseWords请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Text: 待分析的文本（支持中英文文本，不超过500字符）
+        :type Text: str
+        """
+        self.Text = None
+
+
+    def _deserialize(self, params):
+        self.Text = params.get("Text")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ParseWordsResponse(AbstractModel):
+    """ParseWords返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param NormalText: 输入文本正则化的结果。（包括对英文文本中的开头和实体进行大写等）
+        :type NormalText: str
+        :param BasicParticiples: 基础粒度分词和词性标注的结果。（词性表请参见附录）
+
+        :type BasicParticiples: list of BasicParticiple
+        :param CompoundParticiples: 复合粒度分词和词性标注的结果。（词性表请参见附录）
+        :type CompoundParticiples: list of CompoundParticiple
+        :param Entities: 实体识别结果。（实体类型数据请参见附录）
+
+        :type Entities: list of Entity
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.NormalText = None
+        self.BasicParticiples = None
+        self.CompoundParticiples = None
+        self.Entities = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.NormalText = params.get("NormalText")
+        if params.get("BasicParticiples") is not None:
+            self.BasicParticiples = []
+            for item in params.get("BasicParticiples"):
+                obj = BasicParticiple()
+                obj._deserialize(item)
+                self.BasicParticiples.append(obj)
+        if params.get("CompoundParticiples") is not None:
+            self.CompoundParticiples = []
+            for item in params.get("CompoundParticiples"):
+                obj = CompoundParticiple()
+                obj._deserialize(item)
+                self.CompoundParticiples.append(obj)
+        if params.get("Entities") is not None:
+            self.Entities = []
+            for item in params.get("Entities"):
+                obj = Entity()
+                obj._deserialize(item)
+                self.Entities.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class PosToken(AbstractModel):
     """分词&词性标注结果
 
     """
 
     def __init__(self):
         r"""
@@ -1069,14 +1537,63 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class RetrieveSimilarWordsRequest(AbstractModel):
+    """RetrieveSimilarWords请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Text: 输入的词语。（仅支持UTF-8格式，不超过10字符）
+        :type Text: str
+        :param Number: 召回的相似词个数，取值范围为1-20。
+        :type Number: int
+        """
+        self.Text = None
+        self.Number = None
+
+
+    def _deserialize(self, params):
+        self.Text = params.get("Text")
+        self.Number = params.get("Number")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class RetrieveSimilarWordsResponse(AbstractModel):
+    """RetrieveSimilarWords返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param WordList: 召回的相似词数组。
+        :type WordList: list of str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.WordList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.WordList = params.get("WordList")
+        self.RequestId = params.get("RequestId")
+
+
 class SearchResult(AbstractModel):
     """词条搜索的结果，主要描述该词条是否存在以及相关的词性。
 
     """
 
     def __init__(self):
         r"""
@@ -1165,14 +1682,65 @@
             for item in params.get("Results"):
                 obj = SearchResult()
                 obj._deserialize(item)
                 self.Results.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class SentenceCorrectionRequest(AbstractModel):
+    """SentenceCorrection请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TextList: 待纠错的句子列表。可以以数组方式在一次请求中填写多个待纠错的句子。文本统一使用utf-8格式编码，每个中文句子的长度不超过150字符，每个英文句子的长度不超过100个单词，且数组长度需小于150，即句子总数需少于150句。
+        :type TextList: list of str
+        """
+        self.TextList = None
+
+
+    def _deserialize(self, params):
+        self.TextList = params.get("TextList")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SentenceCorrectionResponse(AbstractModel):
+    """SentenceCorrection返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CorrectionList: 纠错结果列表。
+（注意仅展示错误句子的纠错结果，若句子无错则不展示，若全部待纠错句子都被认为无错，则可能返回数组为空）
+        :type CorrectionList: list of CorrectionItem
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.CorrectionList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("CorrectionList") is not None:
+            self.CorrectionList = []
+            for item in params.get("CorrectionList"):
+                obj = CorrectionItem()
+                obj._deserialize(item)
+                self.CorrectionList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class SentenceEmbeddingRequest(AbstractModel):
     """SentenceEmbedding请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1214,14 +1782,43 @@
 
     def _deserialize(self, params):
         self.Vector = params.get("Vector")
         self.Dimension = params.get("Dimension")
         self.RequestId = params.get("RequestId")
 
 
+class SentencePair(AbstractModel):
+    """待分析的句子对
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SourceText: 需要与目标句子计算相似度的源句子。（仅支持UTF-8格式，不超过500字符）
+        :type SourceText: str
+        :param TargetText: 目标句子。（仅支持UTF-8格式，不超过500字符）
+
+        :type TargetText: str
+        """
+        self.SourceText = None
+        self.TargetText = None
+
+
+    def _deserialize(self, params):
+        self.SourceText = params.get("SourceText")
+        self.TargetText = params.get("TargetText")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class SentimentAnalysisRequest(AbstractModel):
     """SentimentAnalysis请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1532,14 +2129,85 @@
                 obj = CCIToken()
                 obj._deserialize(item)
                 self.CCITokens.append(obj)
         self.ResultText = params.get("ResultText")
         self.RequestId = params.get("RequestId")
 
 
+class TextEmbellishRequest(AbstractModel):
+    """TextEmbellish请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Text: 待润色的文本。中文文本长度需<=50字符；英文文本长度需<=30个单词。
+        :type Text: str
+        :param SourceLang: 待润色文本的语言类型，支持语言列表
+zh：中文
+en：英文
+        :type SourceLang: str
+        :param Number: 返回润色结果的个数。数量需>=1且<=5。
+（注意实际结果可能小于指定个数）
+        :type Number: int
+        :param Style: 控制润色类型，类型列表
+both：同时返回改写和扩写
+expansion：扩写
+rewriting：改写
+m2a：从现代文改写为古文
+a2m：从古文改写为现代文
+默认为both。
+        :type Style: str
+        """
+        self.Text = None
+        self.SourceLang = None
+        self.Number = None
+        self.Style = None
+
+
+    def _deserialize(self, params):
+        self.Text = params.get("Text")
+        self.SourceLang = params.get("SourceLang")
+        self.Number = params.get("Number")
+        self.Style = params.get("Style")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class TextEmbellishResponse(AbstractModel):
+    """TextEmbellish返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EmbellishList: 润色结果列表。
+        :type EmbellishList: list of Embellish
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.EmbellishList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("EmbellishList") is not None:
+            self.EmbellishList = []
+            for item in params.get("EmbellishList"):
+                obj = Embellish()
+                obj._deserialize(item)
+                self.EmbellishList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class TextSimilarityProRequest(AbstractModel):
     """TextSimilarityPro请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1640,14 +2308,91 @@
             for item in params.get("Similarity"):
                 obj = Similarity()
                 obj._deserialize(item)
                 self.Similarity.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class TextWritingRequest(AbstractModel):
+    """TextWriting请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Text: 待续写的句子，文本统一使用utf-8格式编码，长度不超过200字符。
+        :type Text: str
+        :param SourceLang: 待续写文本的语言类型，支持语言列表
+zh：中文
+en：英文
+        :type SourceLang: str
+        :param Number: 返回续写结果的个数。数量需>=1且<=5。
+（注意实际结果可能小于指定个数）
+        :type Number: int
+        :param Domain: 指定续写领域，支持领域列表
+general：通用领域，支持中英文补全
+academic：学术领域，仅支持英文补全
+默认为general（通用领域）。
+        :type Domain: str
+        :param Style: 指定续写风格，支持风格列表
+science_fiction：科幻
+military_history：军事
+xuanhuan_wuxia：武侠
+urban_officialdom：职场
+默认为xuanhuan_wuxia（武侠）。
+        :type Style: str
+        """
+        self.Text = None
+        self.SourceLang = None
+        self.Number = None
+        self.Domain = None
+        self.Style = None
+
+
+    def _deserialize(self, params):
+        self.Text = params.get("Text")
+        self.SourceLang = params.get("SourceLang")
+        self.Number = params.get("Number")
+        self.Domain = params.get("Domain")
+        self.Style = params.get("Style")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class TextWritingResponse(AbstractModel):
+    """TextWriting返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param WritingList: 续写结果列表。
+        :type WritingList: list of Writing
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.WritingList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("WritingList") is not None:
+            self.WritingList = []
+            for item in params.get("WritingList"):
+                obj = Writing()
+                obj._deserialize(item)
+                self.WritingList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class UpdateDictRequest(AbstractModel):
     """UpdateDict请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1816,8 +2561,36 @@
         """
         self.Similarity = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.Similarity = params.get("Similarity")
-        self.RequestId = params.get("RequestId")
+        self.RequestId = params.get("RequestId")
+
+
+class Writing(AbstractModel):
+    """文本续写结果
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TargetText: 续写的文本。
+        :type TargetText: str
+        :param PrefixText: 续写的前缀。
+        :type PrefixText: str
+        """
+        self.TargetText = None
+        self.PrefixText = None
+
+
+    def _deserialize(self, params):
+        self.TargetText = params.get("TargetText")
+        self.PrefixText = params.get("PrefixText")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.881/tencentcloud/__init__.py` & `tencentcloud-sdk-python-nlp-3.0.882/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.881'
+__version__ = '3.0.882'
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.881/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-nlp-3.0.882/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-nlp
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Nlp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.881/PKG-INFO` & `tencentcloud-sdk-python-nlp-3.0.882/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-nlp
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Nlp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.881/setup.py` & `tencentcloud-sdk-python-nlp-3.0.882/setup.py`

 * *Files identical despite different names*

