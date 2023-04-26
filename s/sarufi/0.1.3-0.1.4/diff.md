# Comparing `tmp/sarufi-0.1.3-py3-none-any.whl.zip` & `tmp/sarufi-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 13612 bytes, number of entries: 6
--rw-rw-r--  2.0 unx    35461 b- defN 23-Apr-19 17:17 sarufi/__init__.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Apr-19 17:20 sarufi-0.1.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx     6322 b- defN 23-Apr-19 17:20 sarufi-0.1.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-19 17:20 sarufi-0.1.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Apr-19 17:20 sarufi-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      457 b- defN 23-Apr-19 17:20 sarufi-0.1.3.dist-info/RECORD
-6 files, 53696 bytes uncompressed, 12790 bytes compressed:  76.2%
+Zip file size: 13228 bytes, number of entries: 6
+-rw-rw-rw-  2.0 unx    32469 b- defN 23-Apr-25 23:46 sarufi/__init__.py
+-rw-rw-rw-  2.0 unx    11357 b- defN 23-Apr-26 00:02 sarufi-0.1.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 unx     6288 b- defN 23-Apr-26 00:02 sarufi-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-Apr-26 00:02 sarufi-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        7 b- defN 23-Apr-26 00:02 sarufi-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      457 b- defN 23-Apr-26 00:02 sarufi-0.1.4.dist-info/RECORD
+6 files, 50670 bytes uncompressed, 12406 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: sarufi/__init__.py
 Comment: 
 
-Filename: sarufi-0.1.3.dist-info/LICENSE
+Filename: sarufi-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: sarufi-0.1.3.dist-info/METADATA
+Filename: sarufi-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: sarufi-0.1.3.dist-info/WHEEL
+Filename: sarufi-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: sarufi-0.1.3.dist-info/top_level.txt
+Filename: sarufi-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: sarufi-0.1.3.dist-info/RECORD
+Filename: sarufi-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sarufi/__init__.py

```diff
@@ -1,53 +1,53 @@
-"""
-**Sarufi** is a python SDK for the [Sarufi Conversational AI Platform](https://sarufi.io/).
+"""**Sarufi** is a python SDK for the [Sarufi Conversational AI Platform](https://sarufi.io/).
 
 To get started with Sarufi, you need to create an account at [sarufi.io](https://sarufi.io/).
 
-Here an article that explains how to get started with Sarufi: [getting-started-with-sarufi](https://blog.neurotech.africa/what-is-sarufi/)
+Here an article that explains how to get started with Sarufi
 
+[getting-started-with-sarufi](https://blog.neurotech.africa/what-is-sarufi/)
 """
 from __future__ import annotations
 import os
 import json
 import logging
-import requests
 from uuid import uuid4
 from pathlib import Path
+from logging.handlers import WatchedFileHandler
+from typing import Dict, Any, List, Union, Optional
 from yaml import safe_load
-from typing import Dict, Dict, Any, List, Union, Optional
-
-# Set up logging
-logging.basicConfig(
-    level=logging.INFO, format="%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-)
+import requests
 
+# Create logger instance
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
+
+# Set up logging handler for lazy reloading
+handler = WatchedFileHandler("sarufi.log")
+handler.setFormatter(logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s"))
+logger.addHandler(handler)
 
 class Sarufi(object):
     """Sarufi Class"""
 
-    _BASE_URL: str = "https://api.sarufi.io/"
+    _BASE_URL: str = "https://developers.sarufi.io/"
 
     def __init__(
         self,
-        client_id: Optional[str] = None,
-        client_secret: Optional[str] = None,
-        token: Optional[str] = None,
+        api_key:str 
     ) -> None:
-        """Initialize the Sarufi class with client_id and client_secret or token
+        """Initialize the Sarufi class with API Key
 
 
         Args:
-            client_id (Optional[str], optional): Sarufi API Client ID. Defaults to None.
-            client_secret (Optional[str], optional): Sarufi API Client Secret. Defaults to None.
-            token (Optional[str], optional): Sarufi API token. Defaults to None.
+            api_key (str): API Key for the Sarufi account
 
         Examples:
 
-        >>> sarufi = Sarufi(client_id="client_id", client_secret="client_secret")
+        >>> sarufi = Sarufi(api_key="YOUR_API_KEY")
         >>> dir(sarufi)
                 [
                     "...",
                     "bots",
                     "chat",
                     "create_bot",
                     "create_from_file",
@@ -56,45 +56,23 @@
                     "get_bot",
                     "headers",
                     "token",
                     "update_bot",
                     "update_from_file",
                 ]
         """
-        self.__client_id = client_id
-        self.__client_secret = client_secret
-        if token:
-            self.token = {"access_token":token}
-        else:
-            self.token = self.__get_token()
-
-    def __get_token(self):
-        logging.info("Getting token")
-        url = self._BASE_URL + "api/access_token/"
-        data = json.dumps(
-            {"client_id": self.__client_id, "client_secret": self.__client_secret}
-        )
-        response = requests.post(
-            url, data=data, headers={"Content-Type": "application/json"}
-        )
-        return response.json()
-
-    def __update_token(self):
-        self.token = self.__get_token()
-        if self.token.get("access_token"):
-            return True
-        logging.error("Error updating token")
+        self.token = api_key
 
     @staticmethod
     def __strip_of_nones(data: Dict[str, str]):
         if isinstance(data, dict):
             return {k: v for k, v in data.items() if v is not None}
-        logging.error("Data is not a dict")
-        logging.error(data)
-        logging.error(type(data))
+        error_message = f"{data} should be dict not {type(data)}"
+        logging.error(error_message)
+
 
     @staticmethod
     def _read_file(_file: Union[Path, str]) -> Dict[Any, Any]:
         """_read_file
             Reads a file and returns the contents as a dict
         Args:
             _file (Union[Path, str]): File to read(path or filename) | (intents, flows)
@@ -106,178 +84,137 @@
             Dict[Any, Any]: Contents of the file as a dict
         """
         # Get full path of file
         _file = os.path.realpath(_file)
         if os.path.exists(_file):
             try:
                 if any([_file.endswith(ext) for ext in [".yaml", ".yml"]]):
-                    logging.info(f"Reading {_file} as YAML")
-                    return safe_load(open(_file))
+                    logger.info(f"Reading {_file} as YAML")
+                    return safe_load(open(_file, encoding='utf-8'))
                 elif _file.endswith(".json"):
-                    logging.info(f"Reading {_file} as JSON")
-                    return json.load(open(_file))
+                    logger.info(f"Reading {_file} as JSON")
+                    return json.load(open(_file, encoding='utf-8'))
                 else:
                     raise FileNotFoundError(f"{_file} is not a valid file")
-            except Exception as e:
-                logging.error(e)
+            except Exception as error:
+                logging.error(error)
                 logging.error("Could not read file")
                 return None
         raise FileNotFoundError(f"File {_file} not found")
 
     @property
     def headers(self):
-        if self.token.get("access_token"):
-            return {
-                "Authorization": "Bearer " + self.token.get("access_token"),
-                "Content-Type": "application/json",
-            }
-        else:
-            # Log error
-            logging.error(self.token.get("message"))
-            logging.error("Please check your credentials\nand try again")
+        """headers
+            Creates a header with the Bearer token using the token property
+        """
+        return {
+            "Authorization": "Bearer " + self.token,
+            "Content-Type": "application/json",
+        }
 
     def _get_req(
         self,
         url: str,
         _headers: Dict[str, str] = None,
-        retry: int = 1,
     ):
         """get
 
         Simplifies making get requests
 
         Args:
             url (str): _description_
             _headers (Dict[str, str], optional): Authenticated header with Bearer token. Defaults to None.
-            retry (int, optional): Number of time to rety incase token fails. Defaults to 1.
         """
 
-        response = requests.get(url, headers=_headers or self.headers)
+        response = requests.get(url, headers=_headers or self.headers, timeout=10)
         if response.status_code == 200:
             return response
-        elif response.status_code == 400 and (
-            response.json().get("detail") == "Token invalid"
-            or response.json().get("detail") == "Token Expired"
-        ):
-            logging.info("Token invalid[REFRESHING]")
-            self.__update_token()
-            if retry > 0:
-                return self._get_req(url=url, retry=retry - 1)
-        logging.error("Error [GET]")
+        elif response.status_code == 400:
+            logger.debug(response.json())
         return response
 
     def _post_req(
         self,
         url: str,
         body: Dict[str, Any],
         _headers: Dict[str, str] = None,
-        retry: int = 1,
     ) -> Union[type[Bot], Dict[Any, Any]]:
         """post
 
         Simplifies the process of making a post request to sarufi engine
 
         Args:
             url (str): URL to make the request to
             body (Dict[str, Any]): Body of the request
             _headers (Dict[str, str], optional): Request headers. Defaults to None.
-            retry (int, optional): Number of time to retry when tokens are invalid . Defaults to 1.
 
         Returns:
             Union[type[Bot], Dict[Any, Any]]: Bot object if request is successful otherwise dict with error message
         """
 
         _data = json.dumps(self.__strip_of_nones(body))  # remove None values
         _headers = _headers or self.headers
-        response = requests.post(url, data=_data, headers=_headers)
+        response = requests.post(url, data=_data, headers=_headers, timeout=10)
         if response.status_code == 200:
             return response
-
-        elif response.status_code == 400 and (
-            response.json().get("detail") == "Token invalid"
-            or response.json().get("detail") == "Token Expired"
-        ):
-            logging.info("Token invalid[REFRESHING]")
-            self.__update_token()  # Refresh token
-            if retry > 0:
-                # Retry
-                return self._post_req(body=body, url=url, retry=retry - 1)
-
-        logging.error("Error [POST]")
+        elif response.status_code == 400:
+            logger.debug(response.json())
         return response
 
     def _put_req(
         self,
         url: str,
         body: Dict[str, Any],
         _headers: Dict[str, str] = None,
-        retry: int = 1,
     ) -> Union[type[Bot], Dict[Any, Any]]:
         """put
 
         Simplifies the process of making a put request to sarufi engine
 
         Args:
             url (str): URL to make the request to
             body (Dict[str, Any]): Body of the request
             _headers (Dict[str, str], optional): Request headers. Defaults to None.
-            retry (int, optional): Number of time to retry when tokens are invalid . Defaults to 1.
 
         Returns:
             Union[type[Bot], Dict[Any, Any]]: Bot object if request is successful otherwise dict with error message
         """
 
         _data = json.dumps(self.__strip_of_nones(body))
         _headers = _headers or self.headers
-        response = requests.put(url, data=_data, headers=_headers)
+        response = requests.put(url, data=_data, headers=_headers, timeout=10)
         if response.status_code == 200:
             return response
-        elif response.status_code == 400 and (
-            response.json().get("detail") == "Token invalid"
-            or response.json().get("detail") == "Token Expired"
-        ):
-            logging.info("Token invalid[REFRESHING]")
-            self.__update_token()
-            if retry > 0:
-                return self._put_req(url=url, body=body, retry=retry - 1)
-        logging.error("Error [PUT]")
+        elif response.status_code == 400:
+            logger.debug(response.json())
         return response
 
     def _delete_req(
         self,
         url: str,
         _headers: Dict[str, str] = None,
-        retry: int = 1,
     ) -> Union[type[Bot], Dict[Any, Any]]:
         """delete
 
         Simplifies the process of making a delete request to sarufi engine
 
         Args:
             url (str): URL to make the request to
             _headers (Dict[str, str], optional): Request headers. Defaults to None.
-            retry (int, optional): Number of time to retry when tokens are invalid . Defaults to 1.
 
         Returns:
             Union[type[Bot], Dict[Any, Any]]: Bot object if request is successful otherwise dict with error message
         """
 
         _headers = _headers or self.headers
-        response = requests.delete(url, headers=_headers)
+        response = requests.delete(url, headers=_headers,timeout=10)
         if response.status_code == 200:
             return response
-        elif response.status_code == 400 and (
-            response.json().get("detail") == "Token invalid"
-            or response.json().get("detail") == "Token Expired"
-        ):
-            logging.info("Token invalid[REFRESHING]")
-            self.__update_token()
-            if retry > 0:
-                return self._delete_req(url=url, retry=retry - 1)
-        logging.error("Error [DELETE]")
+        elif response.status_code == 400:
+            logger.debug(response.json())
         return response
 
     def create_bot(
         self,
         name: str,
         description: str = None,
         industry: str = None,
@@ -299,37 +236,37 @@
 
         Returns:
             Union[Bot, Dict]: Chatbot object if bot created successfully otherwise dict with error message
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
+        >>> sarufi = Sarufi(api_key='YOUR_API_KEY')
         2022-08-23 15:03:00,928 - root - INFO - Getting token
         >>> bot = sarufi.create_bot(name='Maria')
         2022-08-23 15:03:09,891 - root - INFO - Creating bot
         >>> bot
         Bot(id=5, name=Maria, description=PUT DESCRIPTION HERE)
         """
 
-        logging.info("Creating bot")
+        logger.info("Creating bot")
         url = self._BASE_URL + "chatbot"
         data = {
             "name": name,
             "description": description,
             "intents": intents,
             "flows": flow,
             "industry": industry,
             "webhook_url": webhook_url,
             "webhook_trigger_intents": webhook_trigger_intents,
             "visible_on_community": visible_on_community,
         }
         response = self._post_req(body=data, url=url)
         if response.status_code == 200:
-            return Bot(response.json(), token=self.token)
+            return Bot(data=response.json(), api_key=self.token)
         return response.json()
 
     def create_from_file(
         self,
         intents: Union[Path, str] = None,
         flow: Union[Path, str] = None,
         metadata: Union[Path, str] = None,
@@ -345,15 +282,15 @@
 
         Returns:
             Union[type[Bot], Dict[Any, Any]]: Chatbot object if bot created successfully otherwise dict with error message
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('client_id', 'client_secret')
+        >>> sarufi = Sarufi(api_key='Your API KEY')
         >>> bot = sarufi.create_from_file(
         ...     intents='data/intents.json',
         ...     flow='data/flow.json',
         ...     metadata='data/metadata.json'
             )"""
 
         if intents:
@@ -403,40 +340,40 @@
 
         Returns:
             Union[type[Bot], Dict[Any, Any]]: Chatbot object if bot updated successfully otherwise dict with error message
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
+        >>> sarufi = Sarufi(api_key='Your API KEY')
         >>> bot = sarufi.update_bot(
             ...     id=5,
             ...     name='Maria',
             ...     description='A chatbot that does this and that',
             ...     intents={...},
             ...     flow={...},
             ...     industry='healthcare',
             ...     visible_on_community=True
             ... )
         """
-        logging.info("Updating bot")
+        logger.info("Updating bot")
         url = self._BASE_URL + f"chatbot/{id}"
         data = {
             "name": name,
             "description": description,
             "intents": intents,
             "flows": flow,
             "industry": industry,
             "webhook_url": webhook_url,
             "webhook_trigger_intents": webhook_trigger_intents,
             "visible_on_community": visible_on_community,
         }
         response = self._put_req(body=data, url=url)
         if response.status_code == 200:
-            return Bot(response.json(), token=self.token)
+            return Bot(data=response.json(), api_key=self.token)
         return response.json()
 
     def update_from_file(
         self,
         id: int,
         intents: Union[Path, str] = None,
         flow: Union[Path, str] = None,
@@ -454,15 +391,15 @@
 
         Returns:
             Union[type[Bot], Dict[Any, Any]]: Chatbot object if bot updated successfully otherwise dict with error message
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
+        >>> sarufi = Sarufi(api_key='Your API KEY')
         >>> bot = sarufi.update_from_file(
             ...     id=5,
             ...     intents='data/intents.json',
             ...     flow='data/flow.json',
             ...     metadata='data/metadata.json'
             ... )
         """
@@ -497,57 +434,57 @@
 
         Returns:
             Union[Bot, Dict[Any, Any]]: Chatbot object if bot found otherwise dict with error message
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
+        >>> sarufi = Sarufi(api_key='Your API KEY')
         >>> bot = sarufi.get_bot(id=5)
         >>> print(bot)
         Bot(name='iBank', id=23)
         """
-        logging.info("Getting bot with id: {}".format(id))
+        logger.info("Getting bot with id: {}".format(id))
         url = self._BASE_URL + "chatbot/" + str(id)
         response = self._get_req(url=url)
         if response.status_code == 200:
-            return Bot(response.json(), token=self.token)
+            return Bot(data=response.json(), api_key=self.token)
         return response.json()
 
     def bots(self) -> Union[List[type[Bot]], Dict]:
         """bots
 
         Gets all user chatbots from sarufi engine
 
         Returns:
             Union[List[Bot], Dict]: List of chatbots if successful otherwise dict with error message
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
+        >>> sarufi = Sarufi(api_key='Your API KEY')
         2022-08-23 15:03:00,928 - root - INFO - Getting token
         >>> sarufi.bots()
         2022-08-23 15:03:57,845 - root - INFO - Getting bots
         [Bot(id=4, name=iBank, description=PUT DESCRIPTION HERE), Bot(id=5, name=Maria, description=Swahili Cognitive Mental Health Chatbot)]
 
         """
-        logging.info("Getting bots")
+        logger.info("Getting bots")
         url = self._BASE_URL + "chatbots"
         response = self._get_req(url=url)
         if response.status_code == 200:
-            return [Bot(bot, token=self.token) for bot in response.json()]
+            return [Bot(data=bot, api_key=self.token) for bot in response.json()]
         return response.json()
 
     def _fetch_response(
         self, bot_id: int, chat_id: str, message: str, message_type: str, channel: str
     ):
         url = self._BASE_URL + "conversation/"
         if channel == "whatsapp":
-            logging.info("Sending message to bot via whatsapp")
+            logger.info("Sending message to bot via whatsapp")
             url = url + "whatsapp/"
 
         data = {
             "chat_id": chat_id,
             "bot_id": bot_id,
             "message": message,
             "message_type": message_type,
@@ -572,33 +509,33 @@
             message_type (_type_): message type (text, image, audio, video, file)
 
         Returns:
             response (json): bot response
 
         Examples:
             >>> from sarufi import Sarufi
-            >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
+            >>> sarufi = Sarufi(api_key='Your API KEY')
             >>> sarufi.chat(bot_id=5, chat_id='123456789', message='Hello')
 
             # You can also send direct from bot instance
 
             >>> mybot = sarufi.get_bot(id=5)
             >>> mybot.respond(chat_id='123456789', message='Hello')
         """
-        logging.info("Sending message to bot and returning response")
+        logger.info("Sending message to bot and returning response")
         response = self._fetch_response(
             bot_id=bot_id,
             chat_id=chat_id,
             message=message,
             message_type=message_type,
             channel=channel,
         )
-        logging.info(f"Status code: {response.status_code}")
+        logger.info(f"Status code: {response.status_code}")
         if response.status_code == 200:
-            logging.info("Message sent successfully")
+            logger.info("Message sent successfully")
             return response.json()
 
         logging.error("Message not sent[CHAT]")
         return response.json()
 
     def chat_status(self, bot_id: int, chat_id: str):
         """
@@ -612,28 +549,28 @@
 
         Returns:
             response (json): bot response
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
+        >>> sarufi = Sarufi(api_key='Your API KEY')
         >>> sarufi.chat_status(bot_id=5, chat_id='chat_id')
         >>> {'current_state': 'greetings', 'next_state':'end'}
 
         """
-        logging.info("Sending message to bot and returning response")
+        logger.info("Sending message to bot and returning response")
         url = self._BASE_URL + "conversation/allchannels/status"
         data = {
             "chat_id": chat_id,
             "bot_id": str(bot_id),
         }
         response = self._post_req(url=url, body=data)
         if response.status_code == 200:
-            logging.info("Message sent successfully")
+            logger.info("Message sent successfully")
             return response.json()
 
         logging.error("Message not sent[CHAT]")
         return response.json()
 
     def update_conversation_state(self, bot_id: int, chat_id: str, next_state: str):
         """
@@ -648,29 +585,29 @@
 
         Returns:
             response (json): bot response
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
+        >>> sarufi = Sarufi(api_key='Your API KEY')
         >>> sarufi.update_conversation_state(bot_id=5, chat_id='chat_id', state='greetings')
         >>> {..new state machine..}
 
         """
-        logging.info("Sending message to bot and returning response")
+        logger.info("Sending message to bot and returning response")
         url = self._BASE_URL + "conversation-state"
         data = {
             "chat_id": chat_id,
             "bot_id": str(bot_id),
             "next_state": next_state,
         }
         response = self._post_req(url=url, body=data)
         if response.status_code == 200:
-            logging.info("Message sent successfully")
+            logger.info("Message sent successfully")
             return response.json()
 
         logging.error("Message not sent[CHAT]")
         return response.json()
 
     def delete_bot(self, id: int) -> Dict[Any, Any]:
         """delete_bot
@@ -682,34 +619,34 @@
 
         Returns:
             Dict[Any, Any]: Dict with error message if bot not found otherwise dict with success message
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
+        >>> sarufi = Sarufi(api_key='Your API KEY')
         >>> sarufi.delete_bot(5)
         {'message': 'Bot with ID 5 deleted successfully'}
         """
-        logging.info("Deleting bot")
+        logger.info("Deleting bot")
         url = self._BASE_URL + f"chatbot/{id}"
         response = self._delete_req(url=url)
         return response.json()
 
 
 class Bot(Sarufi):
     """
     BOT OBJECT
 
     has `Helper` functions to access bot data in easy way
 
     Examples:
 
     >>> from sarufi import Sarufi
-    >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
+    >>> sarufi = Sarufi(api_key='Your API KEY')
     >>> bot = sarufi.get_bot(4)
 
     ### Get bot name
     >>> bot.name
     'iBank'
 
     ### Get bot description
@@ -739,16 +676,16 @@
     ### Update bot name
     >>> bot.name = 'New name'
 
     ### Update bot description
     >>> bot.description = 'New description'
     """
 
-    def __init__(self, data: Dict, token=None):
-        super().__init__(token=token)
+    def __init__(self, data: Dict, api_key=None):
+        super().__init__(api_key=api_key)
         self.data = data
         self.chat_id = str(uuid4())
 
     # Getter only
     @property
     def id(self):
         return self.data.get("id")
@@ -759,15 +696,15 @@
         Returns the evaluation metrics of bot
 
         Returns(Dict): Evaluation Metrics of a bot
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('testing@xyz.com', '123')
+        >>> sarufi = Sarufi(api_key='Your API KEY')
         >>> mybot = sarufi.get_bot(bot_id)
         >>> mybot.evaluation_metrics
         ... None
         """
         return self.data.get("evaluation_metrics")
 
     # Getter and setters
@@ -778,71 +715,71 @@
         return self.data.get("name")
 
     @name.setter
     def name(self, name: str):
         if isinstance(name, str):
             self.data["name"] = name
             r = self.update_bot(id=self.id, name=name)
-            logging.info(r)
+            logger.info(r)
         else:
             raise TypeError("name must be a string")
 
     # Industry attribute
     @property
     def industry(self):
         return self.data.get("industry")
 
     @industry.setter
     def industry(self, industry: str):
         if isinstance(industry, str):
             self.data["industry"] = industry
             r = self.update_bot(self.id, industry=industry)
-            logging.info(r)
+            logger.info(r)
         else:
             raise TypeError("industry must be a string")
 
     # Description attribute
     @property
     def description(self):
         return self.data.get("description")
 
     @description.setter
     def description(self, description: str):
         if isinstance(description, str):
             self.data["description"] = description
             r = self.update_bot(self.id, description=description)
-            logging.info(r)
+            logger.info(r)
         else:
             raise TypeError("description must be a string")
 
     # visible_on_community attribute
     @property
     def visible_on_community(self):
         return self.data.get("visible_on_community")
 
     @visible_on_community.setter
     def visible_on_community(self, visible_on_community: bool):
         if isinstance(visible_on_community, bool):
             self.data["visible_on_community"] = visible_on_community
             r = self.update_bot(self.id, visible_on_community=visible_on_community)
-            logging.info(r)
+            logger.info(r)
         else:
             raise TypeError("visible_on_community must be a boolean")
 
     # intents attribute
     @property
     def intents(self):
         return self.data.get("intents")
 
     @intents.setter
     def intents(self, intents: Dict):
         if isinstance(intents, dict):
             self.data["intents"] = intents
             r = self.update_bot(self.id, intents=intents)
-            logging.info(r)
+            logger.info(r)
         else:
             raise TypeError("intents must be a Dictionary")
 
     def add_intent(self, intents: Dict[str, List[str]]):
         """add_intent
 
         Appends an intent to the bot's intents
@@ -852,37 +789,37 @@
 
         Raises:
             TypeError: If intent is not a dictionary
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('testing@gmail.com', '123')
+        >>> sarufi = Sarufi(api_key='Your API KEY')
         >>> chatbot = sarufi.get_bot(1)
         >>> chatbot.add_intent({'greeting': ['hello', 'hi']})
         """
         if isinstance(intents, dict):
             updated_intents = self.intents
             updated_intents.update(intents)
             self.intents = updated_intents
-            logging.info(f'A new intents "{list(intents.keys())}" has been added')
+            logger.info(f'A new intents "{list(intents.keys())}" has been added')
         else:
             raise TypeError("intent must be a dictionary {intent_name: [utterances]}")
 
     # flow attribute
     @property
     def flow(self):
         return self.data.get("flows")
 
     @flow.setter
     def flow(self, flow: Dict):
         if isinstance(flow, dict):
             self.data["flows"] = flow
             r = self.update_bot(self.id, flow=flow)
-            logging.info(r)
+            logger.info(r)
         else:
             raise TypeError("flow must be a Dictionary")
 
     def add_flow(self, flow: Dict[str, Any]):
         """add_flow
 
         Appends a flow to the bot's flows
@@ -892,38 +829,38 @@
 
         Raises:
             TypeError: If flow is not a dictionary
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('testing@gmail.com', '123')
+        >>> sarufi = Sarufi(api_key='Your API KEY')
         >>> sarufi.get_bot(1)
         >>> chatbot.add_flow({'greeting': {'message': ['hello'], 'next_state': 'greeting'}})
         """
         if isinstance(flow, dict):
             updated_flows = self.flow
             updated_flows.update(flow)
             self.flow = updated_flows
-            logging.info(f'A new flow "{list(flow.keys())}" has been added')
+            logger.info(f'A new flow "{list(flow.keys())}" has been added')
         else:
             raise TypeError("flow must be a dictionary {flow_name: flow_data}")
 
     # webhooh_url attribute
     @property
     def webhook_url(self) -> str:
         """
         Returns the Webhook to be triggered by the chatbot
 
         Returns(str): The Webhook of a chatbot
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('testing@xyz.com', '123')
+        >>> sarufi = Sarufi(api_key='Your API KEY')
         >>> mybot = sarufi.get_bot(bot_id)
         >>> mybot.webhook_url
         ... https://www.xyz.com/hook
         """
         return self.data.get("webhook_url")
 
     @webhook_url.setter
@@ -933,49 +870,49 @@
         Args:
             url (str): The new webhook URL (eg. https://www.xyx.com/hook)
 
         Returns:
             str: The updated Webhook URL for the chatbot
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('testing@xyz.com', '123')
+        >>> sarufi = Sarufi(api_key='Your API KEY')
         >>> mybot = sarufi.get_bot(bot_id)
         >>> mybot.webhook_url = "https://www.xyx.com/hook"
         ...https://www.xyz.com/hook"
         """
         if isinstance(url, str):
             self.data["webhook_url"] = url
             r = self.update_bot(self.id, webhook_url=url)
-            logging.info(r)
+            logger.info(r)
         else:
             raise TypeError("webhook_url must be a string")
 
     # webhook_trigger_intents attribute
     @property
     def webhook_trigger_intents(self) -> List[str]:
         """
         Returns Intents that trigger the webhook
 
         Returns(List[str]): List of intents that trigger the webhook
 
         Examples:
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('testing@xyz.com', '123')
+        >>> sarufi = Sarufi(api_key='Your API KEY')
         >>> mybot = sarufi.get_bot(bot_id)
         >>> mybot.webhook_trigger_intents
         ... ['greeting']
         """
         return self.data.get("webhook_trigger_intent")
 
     @webhook_trigger_intents.setter
     def webhook_trigger_intents(self, intents: List[str]) -> List[str]:
         if isinstance(intents, list):
             self.data["webhook_trigger_intents"] = intents
             r = self.update_bot(self.id, webhook_trigger_intents=intents)
-            logging.info(r)
+            logger.info(r)
         else:
             raise TypeError("intents Trigger must be a list of strings")
 
     # Get response from a bot
     def respond(
         self,
         message: str,
@@ -993,15 +930,15 @@
 
         Returns:
             Dict | None: The response from the bot
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
+        >>> sarufi = Sarufi(api_key='Your API KEY')
         >>> chatbot = sarufi.get_bot(1)
         >>> chatbot.respond('hello')
         {'message': ['Hello, how can I help you?'], 'next_state': 'greeting'}
         """
         return self.chat(
             bot_id=self.id,
             chat_id=chat_id or self.chat_id,
@@ -1023,15 +960,15 @@
 
         Returns:
             Dict[bool, str, float]: An object containing the intent, status and the confidence of prediction
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
+        >>> sarufi = Sarufi(api_key='Your API KEY')
         >>> bot = sarufi.get_bot(id=5)
         >>> print(bot.predict_intent("your message"))
         {
             intent: "an_intent",
             status: true
             confidence: 0.75,
         }
@@ -1052,29 +989,29 @@
             chat_id (str): The chat id to get the state of
 
         Returns:
             Union[Dict, None]: The state of the chat
 
         Examples:
             >>> from sarufi import Sarufi
-            >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
+            >>> sarufi = Sarufi(api_key='Your API KEY')
             >>> chatbot = sarufi.get_bot(1)
             >>> chatbot.chat_state('chat_id')
             >>> {'current_state': 'greeting', 'next_state': 'main_menu'}
         """
         return self.chat_status(bot_id=self.id, chat_id=chat_id)
 
     def delete(self):
         """
         delete the bot with the given id
 
         Examples:
 
         >>> from sarufi import Sarufi
-        >>> sarufi = Sarufi('your-client-id', 'your-client-secret')
+        >>> sarufi = Sarufi(api_key='Your API KEY')
         >>> chatbot = sarufi.get_bot(1)
         >>> chatbot.delete()
         """
         return self.delete_bot(self.id)
 
     def __str__(self) -> str:
         return f"Bot(id={self.id}, name={self.name})"
```

## Comparing `sarufi-0.1.3.dist-info/LICENSE` & `sarufi-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sarufi-0.1.3.dist-info/METADATA` & `sarufi-0.1.4.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: sarufi
-Version: 0.1.3
+Version: 0.1.4
 Summary: Opensource python wrapper to Sarufi Conversation API
 Home-page: https://github.com/Neurotech-HQ/sarufi-python-sdk
+Download-URL: https://github.com/Neurotech-HQ/sarufi-python-sdk/archive/refs/tags/v0.0.2.tar.gz
 Author: Jordan Kalebu
 Author-email: isaackeinstein@gmail.com
 License: MIT
-Download-URL: https://github.com/Neurotech-HQ/sarufi-python-sdk/archive/refs/tags/v0.0.2.tar.gz
 Keywords: sarufi,Sarufi Python SDK,Conversation API python,Swahili Conversational API,Conversational platform Python
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: pyyaml
 Requires-Dist: python-telegram-bot
 
 <samp>
 
 # sarufi-python-sdk
@@ -42,15 +42,15 @@
 
 ## Authentication
 
 To authenticate you're bot, you have to specify your client_id and password for Sarufi Platform just as shown below;
 
 ```python
 >>> from sarufi import Sarufi
->>> sarufi = Sarufi('client_id', 'client_secret')
+>>> sarufi = Sarufi(api_key='your API KEY')
 ```
 
 ## Creating a Bot
 
 To create you're bot with sarufi, you have to be aware of two importants idea or concepts which is **intents** and **flow**.
 
 Here an example on how to create your bot;
@@ -86,15 +86,15 @@
 ### Creating a Bot from file
 
 You can create your bot from a file, Here is an example on how to create your bot from a file;
 
 ```python
 from sarufi import Sarufi
 
-sarufi = Sarufi("client_id", "client_secret")
+sarufi = Sarufi(api_key='your API KEY')
 
 
 if __name__ == "__main__":
     response = sarufi.create_from_file(
         intents="data/intents.yaml",
         flow="data/flows.yaml",
         metadata="data/metadata.yaml",
@@ -138,15 +138,15 @@
 ### Update a bot from file
 
 You can update your bot from a file as follows;
 
 ```python
 from sarufi import Sarufi
 
-sarufi = Sarufi("client_id", "client_secret")
+sarufi = Sarufi(api_key='your API KEY')
 
 
 if __name__ == "__main__":
     response = sarufi.update_from_file(
         id=5,
         intents="data/intents.yaml",
         flow="data/flows.yaml",
@@ -157,15 +157,15 @@
 
 ## Using it in a conversation
 
 Here you have to know the bot ID and also specify your user unique ID;
 
 ```python
 >>> from sarufi import Sarufi
->>> sarufi = Sarufi('client_id', 'client_secret')
+>>> sarufi = Sarufi(api_key='your API KEY')
 2022-08-23 18:30:32,918 - root - INFO - Getting token
 >>> bots = sarufi.bots()
 2022-08-23 18:30:38,223 - root - INFO - Getting bots
 >>> bots
 [Bot(id=4, name=iBank), Bot(id=5, name=Maria)]
 >>> maria = bots[1]
 >>> maria.respond('Hi')
@@ -182,35 +182,33 @@
 
 ### Get a bot
 
 Query a bot by ID
 
 ```python
 >>> from sarufi import Sarufi
->>> sarufi = Sarufi('client_id', 'client_secret')
+>>> sarufi = Sarufi(api_key='your API KEY')
 >>> maria= sarufi.get_bot(5)
 2022-08-23 18:44:05,473 - root - INFO - Getting token
 >>> maria
 Bot(id=5, name=Maria)
 ```
 
 ## Deleting a bot
 
 Delete a bot by ID
 
 ```python
 >>> from sarufi import Sarufi
->>> sarufi = Sarufi('client_id', 'client_secret')
+>>> sarufi = Sarufi(api_key='your API KEY')
 >>> sarufi.delete_bot(5)
 ```
 
 ### Issues ?
 
 Are you facing any issue with the usage of the package, please raise one
 
 ## Contributors
 
 1. [kalebu](https://github.com/kalebu/)
 2. [Anthony Mipawa](https://github.com/Tonyloyt)
 </samp>
-
-
```

