# Comparing `tmp/pyppms-2.2.0.tar.gz` & `tmp/pyppms-2.2.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyppms-2.2.0.tar", max compression
+gzip compressed data, was "pyppms-2.2.0.dev2.tar", max compression
```

## Comparing `pyppms-2.2.0.tar` & `pyppms-2.2.0.dev2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2942 2022-04-20 07:35:38.348949 pyppms-2.2.0/README.md
--rw-r--r--   0        0        0     1177 2023-04-26 16:06:50.736103 pyppms-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      231 2023-04-26 16:03:26.526029 pyppms-2.2.0/src/pyppms/__init__.py
--rw-r--r--   0        0        0     5609 2023-04-26 16:03:26.526029 pyppms-2.2.0/src/pyppms/booking.py
--rw-r--r--   0        0        0     7051 2022-04-19 16:41:02.244253 pyppms-2.2.0/src/pyppms/common.py
--rw-r--r--   0        0        0    46011 2023-04-26 16:03:26.526029 pyppms-2.2.0/src/pyppms/ppms.py
--rw-r--r--   0        0        0     3961 2023-04-26 16:03:26.526029 pyppms-2.2.0/src/pyppms/system.py
--rw-r--r--   0        0        0     2287 2022-04-20 14:50:49.117838 pyppms-2.2.0/src/pyppms/user.py
--rw-r--r--   0        0        0     3772 1970-01-01 00:00:00.000000 pyppms-2.2.0/setup.py
--rw-r--r--   0        0        0     3787 1970-01-01 00:00:00.000000 pyppms-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2942 2022-04-20 07:35:38.348949 pyppms-2.2.0.dev2/README.md
+-rw-r--r--   0        0        0     1030 2022-09-17 07:21:31.793638 pyppms-2.2.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0      236 2022-09-17 07:21:31.973644 pyppms-2.2.0.dev2/src/pyppms/__init__.py
+-rw-r--r--   0        0        0     5379 2022-09-17 07:21:25.753439 pyppms-2.2.0.dev2/src/pyppms/booking.py
+-rw-r--r--   0        0        0     7051 2022-04-19 16:41:02.244253 pyppms-2.2.0.dev2/src/pyppms/common.py
+-rw-r--r--   0        0        0    45849 2022-09-16 19:08:20.964242 pyppms-2.2.0.dev2/src/pyppms/ppms.py
+-rw-r--r--   0        0        0     3961 2022-09-16 14:47:58.247637 pyppms-2.2.0.dev2/src/pyppms/system.py
+-rw-r--r--   0        0        0     2287 2022-04-20 14:50:49.117838 pyppms-2.2.0.dev2/src/pyppms/user.py
+-rw-r--r--   0        0        0     3773 2022-09-17 07:21:37.097667 pyppms-2.2.0.dev2/setup.py
+-rw-r--r--   0        0        0     3741 2022-09-17 07:21:37.098015 pyppms-2.2.0.dev2/PKG-INFO
```

### Comparing `pyppms-2.2.0/README.md` & `pyppms-2.2.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `pyppms-2.2.0/src/pyppms/booking.py` & `pyppms-2.2.0.dev2/src/pyppms/booking.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,18 +145,14 @@
             microsecond=0,
         )
         self.endtime = end
         LOG.debug("New endtime: %s", self)
 
     def __str__(self):
         def fmt_time(time):
-            # in case a booking was created from a "nextbooking" response it will not
-            # have the `endtime` attribute set, so treat this separately:
-            if time is None:
-                return "===UNDEFINED==="
             return datetime.strftime(time, "%Y-%m-%d %H:%M")
 
         msg = (
             f"PpmsBooking(username=[{self.username}], "
             f"system_id=[{self.system_id}], "
             f"starttime=[{fmt_time(self.starttime)}], "
             f"endtime=[{fmt_time(self.endtime)}]"
```

### Comparing `pyppms-2.2.0/src/pyppms/common.py` & `pyppms-2.2.0.dev2/src/pyppms/common.py`

 * *Files identical despite different names*

### Comparing `pyppms-2.2.0/src/pyppms/ppms.py` & `pyppms-2.2.0.dev2/src/pyppms/ppms.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #       of instance attributes, public methods or other stuff:
 # pylint: disable-msg=too-many-instance-attributes
 # pylint: disable-msg=too-many-public-methods
 
 import logging
 import os
 import os.path
-import shutil
 from io import open
 
 import requests
 
 from .common import dict_from_single_response, parse_multiline_response
 from .user import PpmsUser
 from .system import PpmsSystem
@@ -53,14 +52,18 @@
         object's lifetime (can be empty if no calls to the :py:meth:`get_systems()` have
         been done yet).
     status : dict
         A dict with keys ``auth_state``, ``auth_response`` and
         ``auth_httpstatus``
     """
 
+    # TODO: all methods returning a list of user objects (get_group_users,
+    # get_admins, ...) should be refactored to return a dict with those objects
+    # instead, having the username ('login') as the key.
+
     def __init__(self, url, api_key, timeout=10, cache=""):
         """Constructor for the PPMS connection object.
 
         Open a connection to the PUMAPI defined in `url` and try to authenticate
         against it using the given API key (or use cache-only mode if key is an
         empty string). If an optional path to a caching location is specified,
         responses will be read from that location unless no matching file can be
@@ -346,133 +349,290 @@
                 intercept_file,
                 len(response.text.splitlines()),
             )
         except Exception as err:  # pylint: disable-msg=broad-except
             LOG.error("Storing response text in [%s] failed: %s", intercept_file, err)
             LOG.error("Response text was:\n--------\n%s\n--------", response.text)
 
-    def flush_cache(self, keep_users=False):
-        """Flush the PyPPMS on-disk cache.
+    ############ users / groups ############
+
+    def new_user(  # pylint: disable-msg=too-many-arguments
+        self, login, lname, fname, email, ppms_group, phone=None, password=None
+    ):
+        """Create a new user in PPMS.
 
-        Optionally flushes everything *except* the `getuser` cache if the
-        `keep_users` flag is set to `True`, as this is clearly the most
-        time-consuming operation when fetching data from PUMAPI and therefore
-        might want to be retained.
-
-        Please note that the `getusers` cache (plural, including the `s` suffix)
-        will be flushed no matter what, as this is simply a list of user IDs
-        that can be fetched with a single request. In consequence this means
-        that using the `keep_users` flag will allow you to have reasonably fast
-        reaction times while still getting information on *new* users live from
-        PUMAPI at the only cost of possibly having outdated information on
-        *existing* users.
+        The method is asking PPMS to create a new user account with the given details.
+        In case an account with that login name already exists, it will log a warning
+        and return without sending any further requests to PPMS.
 
         Parameters
         ----------
-        keep_users : bool, optional
-            If set to `True` the `getuser` sub-directory in the cache location
-            will be kept, by default `False`.
+        login : str
+            The unique identifier for the user.
+        lname : str
+            The last name of the user.
+        fname : str
+            The first name of the user.
+        email : str
+            The email address of the user.
+        ppms_group : str
+            The unique identifier of the primary group of the new user. A new group will
+            be created if no group with the given name exists.
+        phone : str, optional
+            The phone number of the user.
+        password : str, optional
+            The password for the user. If no password is set the user will not be able
+            to log on to PPMS.
+
+        Raises
+        ------
+        RuntimeError
+            Will be raised in case creating the user fails.
         """
-        if self.cache_path == "":
-            LOG.info("No cache path configured, not flushing!")
+        if self.user_exists(login):
+            LOG.warning("NOT creating user [%s] as it already exists!", login)
             return
 
-        dirs_to_remove = [self.cache_path]  # by default remove the entire cache dir
-        keep_msg = ""
-        if keep_users:
-            keep_msg = " (keeping user details dirs)"
-            dirs_to_remove = []
-            cache_dirs = os.listdir(self.cache_path)
-            for subdir in cache_dirs:
-                if subdir == "getuser":
-                    continue
-                dirs_to_remove.append(os.path.join(self.cache_path, subdir))
+        req_data = {
+            "login": login,
+            "lname": lname,
+            "fname": fname,
+            "email": email,
+            "unitlogin": ppms_group,
+        }
+        if phone:
+            req_data["phone"] = phone
+        if password:
+            req_data["pwd"] = password
 
-        LOG.info("Flushing the on-disk cache at [%s]%s...", self.cache_path, keep_msg)
-        for directory in dirs_to_remove:
-            try:
-                shutil.rmtree(directory)
-                LOG.debug("Removed directory [%s].", directory)
-            except Exception as ex:  # pylint: disable-msg=broad-except
-                LOG.warning("Removing the cache at [%s] failed: %s", directory, ex)
+        response = self.request("newuser", req_data)
+        if not "OK newuser" in response.text:
+            msg = f"Creating new user failed: {response.text}"
+            LOG.error(msg)
+            raise RuntimeError(msg)
 
-    def get_admins(self):
-        """Get all PPMS administrator users.
+        LOG.info("Created user [%s] in PPMS.", login)
+        LOG.debug("Response was: %s", response.text)
+
+    def get_user_ids(self, active=False):
+        """Get a list with all user IDs in the PPMS system.
+
+        Parameters
+        ----------
+        active : bool, optional
+            Request only users marked as active in PPMS, by default False.
+            NOTE: "active" is a tri-state parameter in PPMS: "true", "false"
+            or empty!
 
         Returns
         -------
-        list(pyppms.user.PpmsUser)
-            A list with PpmsUser objects that are PPMS administrators.
+        list
+            A list of all (or active-only) user IDs in PPMS.
         """
-        response = self.request("getadmins")
+        # TODO: describe format of returned list and / or give an example!
+        parameters = {}
+        if active:
+            parameters["active"] = "true"
 
-        admins = response.text.splitlines()
-        users = []
-        for username in admins:
-            user = self.get_user(username)
-            users.append(user)
-        LOG.debug("%s admins in the PPMS database: %s", len(admins), ", ".join(admins))
-        return users
+        response = self.request("getusers", parameters)
 
-    def get_booking(self, system_id, booking_type="get"):
-        """Get the current or next booking of a system.
+        users = response.text.splitlines()
+        active_desc = "active " if active else ""
+        LOG.info("%s %susers in the PPMS database", len(users), active_desc)
+        LOG.debug(", ".join(users))
+        return users
 
-        WARNING: if the next booking is requested but it is too far in the future,
-        PUMAPI silently ignores it - the response is identical to a system that has no
-        future bookings and there is no error reported either. Currently it is unclear
-        where the cutoff is (e.g. lookups for a booking that is two years from now still
-        work fine, but a booking in about 10 years is silently skipped).
+    def get_user_dict(self, login_name, skip_cache=False):
+        """Get details on a given user from PPMS.
 
         Parameters
         ----------
-        system_id : int or int-like
-            The ID of the system in PPMS.
-        booking_type : {'get', 'next'}, optional
-            The type of booking to request, one of `get` (requesting the
-            currently running booking) and `next` (requesting the next upcoming
-            booking), by default `get`.
-            NOTE: if `next` is requested the resulting booking object will **NOT** have
-            an end time (`endtime` will be `None`) as PUMAPI doesn't provide one in that
-            case!
+        login_name : str
+            The PPMS account / login name of the user to query.
+        skip_cache : bool, optional
+            Passed as-is to the :py:meth:`request()` method
 
         Returns
         -------
-        pyppms.booking.PpmsBooking or None
-            The booking object, or None if there is no booking for the system or the
-            request is refused by PUMAPI (e.g. "not authorized").
+        dict
+            A dict with the user details returned by the PUMAPI.
+
+        Example
+        -------
+        >>> conn.get_user_dict('pyppms')
+        ... {
+        ...     u'active': True,
+        ...     u'affiliation': u'',
+        ...     u'bcode': u'',
+        ...     u'email': u'pyppms@python-facility.example',
+        ...     u'fname': u'PumAPI',
+        ...     u'lname': u'Python',
+        ...     u'login': u'pyppms',
+        ...     u'mustchbcode': False,
+        ...     u'mustchpwd': False',
+        ...     u'phone': u'+98 (76) 54 3210',
+        ...     u'unitlogin': u'pyppms'
+        ... }
 
         Raises
         ------
+        KeyError
+            Raised in case the user account is unknown to PPMS.
         ValueError
-            Raised if the specified `booking_type` is invalid.
+            Raised if the user details can't be parsed from the PUMAPI response.
         """
-        valid = ["get", "next"]
-        if booking_type not in valid:
-            raise ValueError(
-                f"Value for 'booking_type' ({booking_type}) not in {valid}!"
-            )
+        response = self.request("getuser", {"login": login_name}, skip_cache=skip_cache)
+
+        if not response.text:
+            msg = f"User [{login_name}] is unknown to PPMS"
+            LOG.error(msg)
+            raise KeyError(msg)
+
+        # EXAMPLE:
+        # response.text = (
+        #     u'login,lname,fname,email,'
+        #     u'phone,bcode,affiliation,unitlogin,mustchpwd,mustchbcode,'
+        #     u'active\r\n'
+        #     u'"pyppms","Python","PumAPI","pyppms@python-facility.example",'
+        #     u'"+98 (76) 54 3210","","","pyppms",false,false,'
+        #     u'true\r\n'
+        # )
+        details = dict_from_single_response(response.text)
+        LOG.debug("Details for user [%s]: %s", login_name, details)
+        return details
+
+    def get_user(self, login_name, skip_cache=False):
+        """Fetch user details from PPMS and create a PpmsUser object from it.
+
+        Parameters
+        ----------
+        login_name : str
+            The user's PPMS login name.
+        skip_cache : bool, optional
+            Passed as-is to the :py:meth:`request()` method
+
+        Returns
+        -------
+        pyppms.user.PpmsUser
+            The user object created from the PUMAPI response. The object will be
+            additionally stored in the self.users dict using the login_name as
+            the dict's key.
+
+        Raises
+        ------
+        KeyError
+            Raised if the user doesn't exist in PPMS.
+        """
+        response = self.request("getuser", {"login": login_name}, skip_cache=skip_cache)
+
+        if not response.text:
+            msg = f"User [{login_name}] is unknown to PPMS"
+            LOG.error(msg)
+            raise KeyError(msg)
 
+        user = PpmsUser(response.text)
+        self.users[user.username] = user  # update / add to the cached user objs
+        self.fullname_mapping[user.fullname] = user.username
+        return user
+
+    def user_exists(self, login):
+        """Check if an account with the given login name already exists in PPMS.
+
+        Parameters
+        ----------
+        login : str
+            The login name to check for.
+
+        Returns
+        -------
+        bool
+            True in case an account with that name exists in PPMS, false otherwise.
+        """
         try:
-            response = self.request(booking_type + "booking", {"id": system_id})
-        except requests.exceptions.ConnectionError:
-            LOG.error("Requesting booking status for system %s failed!", system_id)
-            return None
+            self.get_user(login)
+            return True
+        except KeyError:
+            return False
 
-        desc = "any future bookings"
-        if booking_type == "get":
-            desc = "a currently active booking"
-        if not response.text.strip():
-            LOG.debug("System [%s] doesn't have %s", system_id, desc)
-            return None
+    def get_users(self, force_refresh=False):
+        """Get user objects for all (or cached) PPMS users.
 
-        return PpmsBooking(response.text, booking_type, system_id)
+        Parameters
+        ----------
+        force_refresh : bool, optional
+            Re-request information from PPMS even if user details have been
+            cached locally before, by default False.
 
-    def get_current_booking(self, system_id):
-        """Wrapper for `get_booking()` with 'booking_type' set to 'get'."""
-        return self.get_booking(system_id, "get")
+        Returns
+        -------
+        dict(pyppms.user.PpmsUser)
+            A dict of PpmsUser objects with the username (login) as key.
+        """
+        if self.users and not force_refresh:
+            LOG.debug("Using cached details for %s users", len(self.users))
+        else:
+            self.update_users()
+
+        return self.users
+
+    def update_users(self, user_ids=[]):
+        """Update cached details for a list of users from PPMS.
+
+        Get the user details on a list of users (or all active ones) from PPMS and store
+        them in the object's `users` dict. As a side effect, this will also fill the
+        cache directory in case the object's `cache_path` attribute is set.
+
+        WARNING - very slow, especially when the PPMS instance has many users!
+
+        Parameters
+        ----------
+        user_ids : list(str), optional
+            A list of user IDs (login names) to request the cache for, by
+            default [] which will result in all *active* users to be requested.
+        """
+        if not user_ids:
+            user_ids = self.get_user_ids(active=True)
+
+        LOG.debug("Updating details on %s users", len(user_ids))
+        for user_id in user_ids:
+            self.get_user(user_id, skip_cache=True)
+
+        LOG.debug("Collected details on %s users", len(self.users))
+
+    def get_admins(self):
+        """Get all PPMS administrator users.
+
+        Returns
+        -------
+        list(pyppms.user.PpmsUser)
+            A list with PpmsUser objects that are PPMS administrators.
+        """
+        response = self.request("getadmins")
+
+        admins = response.text.splitlines()
+        users = []
+        for username in admins:
+            user = self.get_user(username)
+            users.append(user)
+        LOG.debug("%s admins in the PPMS database: %s", len(admins), ", ".join(admins))
+        return users
+
+    def get_groups(self):
+        """Get a list of all groups in PPMS.
+
+        Returns
+        -------
+        list(str)
+            A list with the group identifiers in PPMS.
+        """
+        response = self.request("getgroups")
+
+        groups = response.text.splitlines()
+        LOG.debug("%s groups in the PPMS database: %s", len(groups), ", ".join(groups))
+        return groups
 
     def get_group(self, group_id):
         """Fetch group details from PPMS and create a dict from them.
 
         Parameters
         ----------
         group_id : str
@@ -521,167 +681,148 @@
             "%s members in PPMS group [%s]: %s",
             len(members),
             unitlogin,
             ", ".join(members),
         )
         return users
 
-    def get_groups(self):
-        """Get a list of all groups in PPMS.
+    def get_user_experience(self, login=None, system_id=None):
+        """Get user experience ("User rights") from PPMS.
+
+        Parameters
+        ----------
+        login : str, optional
+            An optional login name to request the experience / permissions for,
+            by default None
+        system_id : int, optional
+            An optional system ID to request the experience / permissions for,
+            by default None
 
         Returns
         -------
-        list(str)
-            A list with the group identifiers in PPMS.
+        list(dict)
+            A list with dicts parsed from the user experience response.
         """
-        response = self.request("getgroups")
-
-        groups = response.text.splitlines()
-        LOG.debug("%s groups in the PPMS database: %s", len(groups), ", ".join(groups))
-        return groups
-
-    def get_next_booking(self, system_id):
-        """Wrapper for `get_booking()` with 'booking_type' set to 'next'."""
-        return self.get_booking(system_id, "next")
-
-    def get_running_sheet(self, core_facility_ref, date, ignore_uncached_users=False):
-        """Get the running sheet for a specific day on the given facility.
+        data = {}
+        if login is not None:
+            data["login"] = login
+        if system_id is not None:
+            data["id"] = system_id
+        response = self.request("getuserexp", parameters=data)
 
-        The so-called "running-sheet" consists of all bookings / reservations of
-        a facility on a specifc day.
+        parsed = parse_multiline_response(response.text)
+        LOG.debug(
+            "Received %s experience entries for filters [user:%s] and [id:%s]",
+            len(parsed),
+            login,
+            system_id,
+        )
+        return parsed
 
-        WARNING: PUMAPI doesn't return a proper unique user identifier with the
-        'getrunningsheet' request, instead the so called "full name" is given to
-        identify the user - unfortunately this can lead to ambiguities as
-        multiple different accounts can have the same full name.
+    def get_users_emails(self, users=None, active=False):
+        """Get a list of user email addresses. WARNING - very slow!
 
         Parameters
         ----------
-        core_facility_ref : int or int-like
-            The core facility ID for PPMS.
-        date : datetime.datetime
-            The date to request the running sheet for, e.g. ``datetime.now()`` or
-            similar. Note that only the date part is relevant, time will be ignored.
-        ignore_uncached_users : bool, optional
-            If set to `True` any booking for a user that is not present in the instance
-            attribuge `fullname_mapping` will be ignored in the resulting list.
+        users : list(str), optional
+            A list of login names to retrieve the email addresses for, if
+            omitted addresses for all (or active ones) will be requested.
+        active : bool, optional
+            Request only addresses of users marked as active in PPMS, by default
+            False. Will be ignored if a list of usernames is given explicitly.
 
         Returns
         -------
-        list(pyppms.booking.PpmsBooking)
-            A list with `PpmsBooking` objects for the given day. Empty in case
-            there are no bookings or parsing the response failed.
+        list(str)
+            Email addresses of the users requested.
         """
-        bookings = []
-        parameters = {
-            "plateformid": f"{core_facility_ref}",
-            "day": date.strftime("%Y-%m-%d"),
-        }
-        LOG.debug("Requesting runningsheet for %s", parameters["day"])
-        response = self.request("getrunningsheet", parameters)
-        try:
-            entries = parse_multiline_response(response.text, graceful=False)
-        except Exception as err:  # pylint: disable-msg=broad-except
-            LOG.error("Parsing runningsheet details failed: %s", err)
-            # NOTE: in case no future bookings exist the response will be empty!
-            LOG.error("Possibly the runningsheet is empty as no bookings exist?")
-            LOG.debug("Runningsheet PUMPAI response was: %s", response.text)
-            return bookings
-
-        for entry in entries:
-            full = entry["User"]
-            if full not in self.fullname_mapping:
-                if ignore_uncached_users:
-                    LOG.debug("Ignoring booking for uncached user [%s]", full)
-                    continue
-
-                LOG.info("Booking for an uncached user (%s) found!", full)
-                self.update_users()
-
-            if full not in self.fullname_mapping:
-                LOG.error("PPMS doesn't seem to know user [%s], skipping", full)
-                continue
-
-            LOG.info(
-                "Booking for user '%s' (%s) found", self.fullname_mapping[full], full
-            )
-            system_name = entry["Object"]
-            system_ids = self.get_systems_matching("", [system_name])
-            if len(system_ids) != 1:
-                # NOTE: more than one result should not happen as PPMS doesn't allow for
-                # multiple systems having the same name - no result might happen though!
-                LOG.error("Ignoring booking for unknown system [%s]", system_name)
+        emails = []
+        if users is None:
+            users = self.get_user_ids(active=active)
+        for user in users:
+            email = self.get_user_dict(user)["email"]
+            if not email:
+                LOG.warning("--- WARNING: no email for user [%s]! ---", user)
                 continue
+            # LOG.debug("%s: %s", user, email)
+            emails.append(email)
 
-            booking = PpmsBooking.from_runningsheet(
-                entry,
-                system_ids[0],
-                self.fullname_mapping[full],
-                date,
-            )
-            bookings.append(booking)
+        return emails
 
-        return bookings
+    ############ resources ############
 
     def get_systems(self, force_refresh=False):
         """Get a dict with all systems in PPMS.
 
-        Parameters
-        ----------
-        force_refresh : bool, optional
-            If `True` the list of systems will be refreshed even if the object's
-            attribute `self.systems` is non-empty, by default `False`. Please
-            note that this will NOT skip the on-disk cache in case that exists!
-
         Returns
         -------
         dict(pyppms.system.PpmsSystem)
             A dict with `PpmsSystem` objects parsed from the PUMAPI response where
             the system ID (int) is used as the dict's key. If parsing a system
             fails for any reason, the system is skipped entirely.
         """
         if self.systems and not force_refresh:
             LOG.debug("Using cached details for %s systems", len(self.systems))
         else:
             self.update_systems()
 
         return self.systems
 
+    def update_systems(self):
+        """Update cached details for all bookable systems from PPMS.
+
+        Get the details on all bookable systems from PPMS and store them in the local
+        cache. If parsing the PUMAPI response for a system fails for any reason, the
+        system is skipped entirely.
+        """
+        LOG.debug("Updating list of bookable systems...")
+        systems = {}
+        parse_fails = 0
+        response = self.request("getsystems")
+        details = parse_multiline_response(response.text, graceful=False)
+        for detail in details:
+            try:
+                system = PpmsSystem(detail)
+            except ValueError as err:
+                LOG.error("Error processing `getsystems` response: %s", err)
+                parse_fails += 1
+                continue
+
+            systems[system.system_id] = system
+
+        LOG.debug(
+            "Updated %s bookable systems from PPMS (%s systems failed parsing)",
+            len(systems),
+            parse_fails,
+        )
+
+        self.systems = systems
+
     def get_systems_matching(self, localisation, name_contains):
         """Query PPMS for systems with a specific location and name.
 
         This method assembles a list of PPMS system IDs whose "localisation"
         (room) field matches a given string and where the system name contains
         at least one of the strings given as the `name_contains` parameter.
 
         Parameters
         ----------
         localisation : str
             A string that the system's "localisation" (i.e. the "Room" field in
-            the PPMS web interface) has to match. Can be an empty string which
-            will result in no filtering being done on the "Room" attribute.
+            the PPMS web interface) has to match.
         name_contains : list(str)
             A list of valid names (categories) of which the system's name has to
             match at least one for being included. Supply an empty list for
             skipping this filter.
 
         Returns
         -------
         list(int)
             A list with PPMS system IDs matching all of the given criteria.
-
-        Raises
-        ------
-        TypeError
-            Raised in case the `name_contains` parameter is of type `str` (it
-            needs to be `list(str)` instead).
         """
-        if isinstance(name_contains, str):
-            raise TypeError("`name_contains` must be a list of str, not str!")
-
         loc = localisation
         loc_desc = f"with location matching [{localisation}]"
         if localisation == "":
             loc_desc = "(no location filter given)"
 
         LOG.info(
             "Querying PPMS for systems %s, name matching any of %s",
@@ -713,218 +854,15 @@
             #     LOG.debug('System [%s] does NOT match a valid name: %s',
             #               system.name, name_contains)
 
         LOG.info("Found %s bookable systems %s", len(system_ids), loc_desc)
         LOG.debug("IDs of matching bookable systems %s: %s", loc_desc, system_ids)
         return system_ids
 
-    def get_user(self, login_name, skip_cache=False):
-        """Fetch user details from PPMS and create a PpmsUser object from it.
-
-        Parameters
-        ----------
-        login_name : str
-            The user's PPMS login name.
-        skip_cache : bool, optional
-            Passed as-is to the :py:meth:`request()` method
-
-        Returns
-        -------
-        pyppms.user.PpmsUser
-            The user object created from the PUMAPI response. The object will be
-            additionally stored in the self.users dict using the login_name as
-            the dict's key.
-
-        Raises
-        ------
-        KeyError
-            Raised if the user doesn't exist in PPMS.
-        """
-        response = self.request("getuser", {"login": login_name}, skip_cache=skip_cache)
-
-        if not response.text:
-            msg = f"User [{login_name}] is unknown to PPMS"
-            LOG.error(msg)
-            raise KeyError(msg)
-
-        user = PpmsUser(response.text)
-        self.users[user.username] = user  # update / add to the cached user objs
-        self.fullname_mapping[user.fullname] = user.username
-        return user
-
-    def get_user_dict(self, login_name, skip_cache=False):
-        """Get details on a given user from PPMS.
-
-        Parameters
-        ----------
-        login_name : str
-            The PPMS account / login name of the user to query.
-        skip_cache : bool, optional
-            Passed as-is to the :py:meth:`request()` method
-
-        Returns
-        -------
-        dict
-            A dict with the user details returned by the PUMAPI.
-
-        Example
-        -------
-        >>> conn.get_user_dict('pyppms')
-        ... {
-        ...     u'active': True,
-        ...     u'affiliation': u'',
-        ...     u'bcode': u'',
-        ...     u'email': u'pyppms@python-facility.example',
-        ...     u'fname': u'PumAPI',
-        ...     u'lname': u'Python',
-        ...     u'login': u'pyppms',
-        ...     u'mustchbcode': False,
-        ...     u'mustchpwd': False',
-        ...     u'phone': u'+98 (76) 54 3210',
-        ...     u'unitlogin': u'pyppms'
-        ... }
-
-        Raises
-        ------
-        KeyError
-            Raised in case the user account is unknown to PPMS.
-        ValueError
-            Raised if the user details can't be parsed from the PUMAPI response.
-        """
-        response = self.request("getuser", {"login": login_name}, skip_cache=skip_cache)
-
-        if not response.text:
-            msg = f"User [{login_name}] is unknown to PPMS"
-            LOG.error(msg)
-            raise KeyError(msg)
-
-        # EXAMPLE:
-        # response.text = (
-        #     u'login,lname,fname,email,'
-        #     u'phone,bcode,affiliation,unitlogin,mustchpwd,mustchbcode,'
-        #     u'active\r\n'
-        #     u'"pyppms","Python","PumAPI","pyppms@python-facility.example",'
-        #     u'"+98 (76) 54 3210","","","pyppms",false,false,'
-        #     u'true\r\n'
-        # )
-        details = dict_from_single_response(response.text)
-        LOG.debug("Details for user [%s]: %s", login_name, details)
-        return details
-
-    def get_user_experience(self, login=None, system_id=None):
-        """Get user experience ("User rights") from PPMS.
-
-        Parameters
-        ----------
-        login : str, optional
-            An optional login name to request the experience / permissions for,
-            by default None
-        system_id : int, optional
-            An optional system ID to request the experience / permissions for,
-            by default None
-
-        Returns
-        -------
-        list(dict)
-            A list with dicts parsed from the user experience response.
-        """
-        data = {}
-        if login is not None:
-            data["login"] = login
-        if system_id is not None:
-            data["id"] = system_id
-        response = self.request("getuserexp", parameters=data)
-
-        parsed = parse_multiline_response(response.text)
-        LOG.debug(
-            "Received %s experience entries for filters [user:%s] and [id:%s]",
-            len(parsed),
-            login,
-            system_id,
-        )
-        return parsed
-
-    def get_user_ids(self, active=False):
-        """Get a list with all user IDs in the PPMS system.
-
-        Parameters
-        ----------
-        active : bool, optional
-            Request only users marked as active in PPMS, by default False.
-            NOTE: "active" is a tri-state parameter in PPMS: "true", "false"
-            or empty!
-
-        Returns
-        -------
-        list
-            A list of all (or active-only) user IDs in PPMS.
-        """
-        # TODO: describe format of returned list and / or give an example!
-        parameters = {}
-        if active:
-            parameters["active"] = "true"
-
-        response = self.request("getusers", parameters)
-
-        users = response.text.splitlines()
-        active_desc = "active " if active else ""
-        LOG.info("%s %susers in the PPMS database", len(users), active_desc)
-        LOG.debug(", ".join(users))
-        return users
-
-    def get_users(self, force_refresh=False):
-        """Get user objects for all (or cached) PPMS users.
-
-        Parameters
-        ----------
-        force_refresh : bool, optional
-            Re-request information from PPMS even if user details have been
-            cached locally before, by default False.
-
-        Returns
-        -------
-        dict(pyppms.user.PpmsUser)
-            A dict of PpmsUser objects with the username (login) as key.
-        """
-        if self.users and not force_refresh:
-            LOG.debug("Using cached details for %s users", len(self.users))
-        else:
-            self.update_users()
-
-        return self.users
-
-    def get_users_emails(self, users=None, active=False):
-        """Get a list of user email addresses. WARNING - very slow!
-
-        Parameters
-        ----------
-        users : list(str), optional
-            A list of login names to retrieve the email addresses for, if
-            omitted addresses for all (or active ones) will be requested.
-        active : bool, optional
-            Request only addresses of users marked as active in PPMS, by default
-            False. Will be ignored if a list of usernames is given explicitly.
-
-        Returns
-        -------
-        list(str)
-            Email addresses of the users requested.
-        """
-        emails = []
-        if users is None:
-            users = self.get_user_ids(active=active)
-        for user in users:
-            email = self.get_user_dict(user)["email"]
-            if not email:
-                LOG.warning("--- WARNING: no email for user [%s]! ---", user)
-                continue
-            # LOG.debug("%s: %s", user, email)
-            emails.append(email)
-
-        return emails
+    ############ system / user permissions ############
 
     def get_users_with_access_to_system(self, system_id):
         """Get a list of usernames allowed to book the system with the given ID.
 
         Parameters
         ----------
         system_id : int or int-like
@@ -968,110 +906,14 @@
                 f"ERROR: {err}"
             )
             LOG.error(msg)
             raise ValueError(msg) from err
 
         return users
 
-    def give_user_access_to_system(self, username, system_id):
-        """Add permissions for a user to book a given system in PPMS.
-
-        Parameters
-        ----------
-        username : str
-            The username ('login') to allow for booking the system.
-        system_id : int or int-like
-            The ID of the system to add the permission for.
-
-        Returns
-        -------
-        bool
-            True in case the given username now has the permissions to book the
-            system with the specified ID (or if the user already had them
-            before), False otherwise.
-        """
-        return self.set_system_booking_permissions(username, system_id, "A")
-
-    def new_user(  # pylint: disable-msg=too-many-arguments
-        self, login, lname, fname, email, ppms_group, phone=None, password=None
-    ):
-        """Create a new user in PPMS.
-
-        The method is asking PPMS to create a new user account with the given details.
-        In case an account with that login name already exists, it will log a warning
-        and return without sending any further requests to PPMS.
-
-        Parameters
-        ----------
-        login : str
-            The unique identifier for the user.
-        lname : str
-            The last name of the user.
-        fname : str
-            The first name of the user.
-        email : str
-            The email address of the user.
-        ppms_group : str
-            The unique identifier of the primary group of the new user. A new group will
-            be created if no group with the given name exists.
-        phone : str, optional
-            The phone number of the user.
-        password : str, optional
-            The password for the user. If no password is set the user will not be able
-            to log on to PPMS.
-
-        Raises
-        ------
-        RuntimeError
-            Will be raised in case creating the user fails.
-        """
-        if self.user_exists(login):
-            LOG.warning("NOT creating user [%s] as it already exists!", login)
-            return
-
-        req_data = {
-            "login": login,
-            "lname": lname,
-            "fname": fname,
-            "email": email,
-            "unitlogin": ppms_group,
-        }
-        if phone:
-            req_data["phone"] = phone
-        if password:
-            req_data["pwd"] = password
-
-        response = self.request("newuser", req_data)
-        if not "OK newuser" in response.text:
-            msg = f"Creating new user failed: {response.text}"
-            LOG.error(msg)
-            raise RuntimeError(msg)
-
-        LOG.info("Created user [%s] in PPMS.", login)
-        LOG.debug("Response was: %s", response.text)
-
-    def remove_user_access_from_system(self, username, system_id):
-        """Remove permissions for a user to book a given system in PPMS.
-
-        Parameters
-        ----------
-        username : str
-            The username ('login') to remove booking permissions on the system.
-        system_id : int or int-like
-            The ID of the system to modify the permission for.
-
-        Returns
-        -------
-        bool
-            True in case the given username now has the permissions to book the
-            system with the specified ID (or if the user already had them
-            before), False otherwise.
-        """
-        return self.set_system_booking_permissions(username, system_id, "D")
-
     def set_system_booking_permissions(self, login, system_id, permission):
         """Set permissions for a user on a given system in PPMS.
 
         Parameters
         ----------
         username : str
             The username ('login') to allow for booking the system.
@@ -1151,79 +993,260 @@
                 "Unable to set permissions for system %s: %s", system_id, response.text
             )
         else:
             LOG.error("Unexpected response, assuming request failed: %s", response.text)
 
         return False
 
-    def update_systems(self):
-        """Update cached details for all bookable systems from PPMS.
+    def give_user_access_to_system(self, username, system_id):
+        """Add permissions for a user to book a given system in PPMS.
 
-        Get the details on all bookable systems from PPMS and store them in the local
-        cache. If parsing the PUMAPI response for a system fails for any reason, the
-        system is skipped entirely.
+        Parameters
+        ----------
+        username : str
+            The username ('login') to allow for booking the system.
+        system_id : int or int-like
+            The ID of the system to add the permission for.
+
+        Returns
+        -------
+        bool
+            True in case the given username now has the permissions to book the
+            system with the specified ID (or if the user already had them
+            before), False otherwise.
         """
-        LOG.debug("Updating list of bookable systems...")
-        systems = {}
-        parse_fails = 0
-        response = self.request("getsystems")
-        details = parse_multiline_response(response.text, graceful=False)
-        for detail in details:
-            try:
-                system = PpmsSystem(detail)
-            except ValueError as err:
-                LOG.error("Error processing `getsystems` response: %s", err)
-                parse_fails += 1
-                continue
+        return self.set_system_booking_permissions(username, system_id, "A")
 
-            systems[system.system_id] = system
+    def remove_user_access_from_system(self, username, system_id):
+        """Remove permissions for a user to book a given system in PPMS.
 
-        LOG.debug(
-            "Updated %s bookable systems from PPMS (%s systems failed parsing)",
-            len(systems),
-            parse_fails,
-        )
+        Parameters
+        ----------
+        username : str
+            The username ('login') to remove booking permissions on the system.
+        system_id : int or int-like
+            The ID of the system to modify the permission for.
 
-        self.systems = systems
+        Returns
+        -------
+        bool
+            True in case the given username now has the permissions to book the
+            system with the specified ID (or if the user already had them
+            before), False otherwise.
+        """
+        return self.set_system_booking_permissions(username, system_id, "D")
 
-    def update_users(self, user_ids=[]):
-        """Update cached details for a list of users from PPMS.
+    ############ bookings ############
 
-        Get the user details on a list of users (or all active ones) from PPMS and store
-        them in the object's `users` dict. As a side effect, this will also fill the
-        cache directory in case the object's `cache_path` attribute is set.
+    def get_booking(self, system_id, booking_type="get"):
+        """Get the current or next booking of a system.
 
-        WARNING - very slow, especially when the PPMS instance has many users!
+        WARNING: if the next booking is requested but it is too far in the future,
+        PUMAPI silently ignores it - the response is identical to a system that has no
+        future bookings and there is no error reported either. Currently it is unclear
+        where the cutoff is (e.g. lookups for a booking that is two years from now still
+        work fine, but a booking in about 10 years is silently skipped).
 
         Parameters
         ----------
-        user_ids : list(str), optional
-            A list of user IDs (login names) to request the cache for, by
-            default [] which will result in all *active* users to be requested.
+        system_id : int or int-like
+            The ID of the system in PPMS.
+        booking_type : {'get', 'next'}, optional
+            The type of booking to request, one of `get` (requesting the
+            currently running booking) and `next` (requesting the next upcoming
+            booking), by default `get`.
+
+        Returns
+        -------
+        pyppms.booking.PpmsBooking or None
+            The booking object, or None if there is no booking for the system or the
+            request is refused by PUMAPI (e.g. "not authorized").
+
+        Raises
+        ------
+        ValueError
+            Raised if the specified `booking_type` is invalid.
         """
-        if not user_ids:
-            user_ids = self.get_user_ids(active=True)
+        valid = ["get", "next"]
+        if booking_type not in valid:
+            raise ValueError(
+                f"Value for 'booking_type' ({booking_type}) not in {valid}!"
+            )
 
-        LOG.debug("Updating details on %s users", len(user_ids))
-        for user_id in user_ids:
-            self.get_user(user_id, skip_cache=True)
+        try:
+            response = self.request(booking_type + "booking", {"id": system_id})
+        except requests.exceptions.ConnectionError:
+            LOG.error("Requesting booking status for system %s failed!", system_id)
+            return None
 
-        LOG.debug("Collected details on %s users", len(self.users))
+        desc = "any future bookings"
+        if booking_type == "get":
+            desc = "a currently active booking"
+        if not response.text.strip():
+            LOG.debug("System [%s] doesn't have %s", system_id, desc)
+            return None
 
-    def user_exists(self, login):
-        """Check if an account with the given login name already exists in PPMS.
+        return PpmsBooking(response.text, booking_type, system_id)
+
+    def get_current_booking(self, system_id):
+        """Wrapper for `get_booking()` with 'booking_type' set to 'get'."""
+        return self.get_booking(system_id, "get")
+
+    def get_next_booking(self, system_id):
+        """Wrapper for `get_booking()` with 'booking_type' set to 'next'."""
+        return self.get_booking(system_id, "next")
+
+    def get_running_sheet(self, core_facility_ref, date, ignore_uncached_users=False):
+        """Get the running sheet for a specific day on the given facility.
+
+        The so-called "running-sheet" consists of all bookings / reservations of
+        a facility on a specifc day.
+
+        WARNING: PUMAPI doesn't return a proper unique user identifier with the
+        'getrunningsheet' request, instead the so called "full name" is given to
+        identify the user - unfortunately this can lead to ambiguities as
+        multiple different accounts can have the same full name.
 
         Parameters
         ----------
-        login : str
-            The login name to check for.
+        core_facility_ref : int or int-like
+            The core facility ID for PPMS.
+        date : datetime.datetime
+            The date to request the running sheet for, e.g. ``datetime.now()`` or
+            similar. Note that only the date part is relevant, time will be ignored.
+        ignore_uncached_users : bool, optional
+            If set to `True` any booking for a user that is not present in the instance
+            attribuge `fullname_mapping` will be ignored in the resulting list.
 
         Returns
         -------
-        bool
-            True in case an account with that name exists in PPMS, false otherwise.
+        list(pyppms.booking.PpmsBooking)
+            A list with `PpmsBooking` objects for the given day. Empty in case
+            there are no bookings or parsing the response failed.
         """
+        bookings = []
+        parameters = {
+            "plateformid": f"{core_facility_ref}",
+            "day": date.strftime("%Y-%m-%d"),
+        }
+        LOG.debug("Requesting runningsheet for %s", parameters["day"])
+        response = self.request("getrunningsheet", parameters)
         try:
-            self.get_user(login)
-            return True
-        except KeyError:
-            return False
+            entries = parse_multiline_response(response.text, graceful=False)
+        except Exception as err:  # pylint: disable-msg=broad-except
+            LOG.error("Parsing runningsheet details failed: %s", err)
+            # NOTE: in case no future bookings exist the response will be empty!
+            LOG.error("Possibly the runningsheet is empty as no bookings exist?")
+            LOG.debug("Runningsheet PUMPAI response was: %s", response.text)
+            return bookings
+
+        for entry in entries:
+            full = entry["User"]
+            if full not in self.fullname_mapping:
+                if ignore_uncached_users:
+                    LOG.debug("Ignoring booking for uncached user [%s]", full)
+                    continue
+
+                LOG.info("Booking for an uncached user (%s) found!", full)
+                self.update_users()
+
+            if full not in self.fullname_mapping:
+                LOG.error("PPMS doesn't seem to know user [%s], skipping", full)
+                continue
+
+            LOG.info(
+                "Booking for user '%s' (%s) found", self.fullname_mapping[full], full
+            )
+            booking = PpmsBooking.from_runningsheet(
+                entry,
+                self._get_system_with_name(entry["Object"]),
+                self.fullname_mapping[full],
+                date,
+            )
+            bookings.append(booking)
+
+        return bookings
+
+    ############ deprecated methods ############
+
+    # TODO: remove methods below with one of the next releases
+
+    def _get_system_with_name(self, system_name):
+        """Get the system ID from the system's name.
+
+        Parameters
+        ----------
+        system_name : str
+            The system name to look for in PPMS.
+
+        Returns
+        -------
+        int
+            The ID of the system with the given name or '-1' if no system with
+            that name could be found.
+
+        Raises
+        ------
+        DeprecationWarning
+            This method will be removed in one of the next releases.
+        """
+        # raise DeprecationWarning('Use get_systems_matching() instead!')
+        sys_ids = self.get_systems_matching("", [system_name])
+        if sys_ids:
+            return sys_ids[0]
+
+        return -1
+
+    def _get_machine_catalogue_from_system(self, system_name, catalogue_names=[]):
+        """Get the machine catalog (location / category) of a system.
+
+        WARNING: deprecated method from the legacy API!
+
+        Parameters
+        ----------
+        system_name : str
+            The name of the system to check PPMS for.
+        catalogue_names : list(str), optional
+            [description], by default []
+
+        Returns
+        -------
+        str
+            The machine catalog / location / category of the system. Will be an
+            empty string ('') if none is found.
+        """
+        # raise DeprecationWarning('Use get_systems_matching() instead!')
+        for category in catalogue_names:
+            sys_ids = self.get_systems_matching(category, [system_name])
+            if sys_ids:
+                LOG.debug(
+                    "Found system(s) %s to be in category [%s]", sys_ids, category
+                )
+                return category
+
+        LOG.warning("No category found for system [%s]", system_name)
+        return ""
+
+    def get_bookable_ids(self, localisation, name_contains):
+        """Legacy method for getting IDs of specific systems (name + location).
+
+        This method is not implemented any more, use `get_systems_matching()` with
+        appropriate parameters to select the desired systems instead.
+
+        Raises
+        ------
+        NotImplementedError
+        """
+        raise NotImplementedError("Use get_systems_matching() instead!")
+
+    def get_system(self, system_id):
+        """Legacy method for getting details of a specific system.
+
+        This method is not implemented any more, use `get_systems()` instead and access
+        the desired system by using the respective system ID as the key on the returned
+        dict, e.g. `get_systems()[42]`.
+
+        Raises
+        ------
+        NotImplementedError
+        """
+        raise NotImplementedError("Use get_systems()[system_id] instead!")
```

### Comparing `pyppms-2.2.0/src/pyppms/system.py` & `pyppms-2.2.0.dev2/src/pyppms/system.py`

 * *Files identical despite different names*

### Comparing `pyppms-2.2.0/src/pyppms/user.py` & `pyppms-2.2.0.dev2/src/pyppms/user.py`

 * *Files identical despite different names*

### Comparing `pyppms-2.2.0/setup.py` & `pyppms-2.2.0.dev2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.25.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'pyppms',
-    'version': '2.2.0',
+    'version': '2.2.0.dev2',
     'description': "A Python package to communicate with Stratocore's PUMAPI.",
     'long_description': '# PyPPMS\n\n## PUMAPI - Python Interface\n\n[Stratocore][3]\'s *PPMS* booking system offers an API (the so-called *PUMAPI*, short for\nPPMS Utility Management API) for fetching information from the booking system as well as\nchanging its state and properties.\n\nThis is a Python 3 package for talking to the *PUMAPI*.\n\n## Usage Example\n\nFetch email addresses of all active users:\n\n```Python\nfrom pyppms import ppms\nfrom credentials_ppms import PPMS_URL, PPMS_API_KEY\n\nconn = ppms.PpmsConnection(PPMS_URL, PPMS_API_KEY)\n\nprint("Querying PPMS for emails of active users, can take minutes...")\nemails = ppms.get_users_emails(active=True)\nprint(f"Got {len(emails)} email addresses from PPMS:")\nprint("\\n".join(emails))\n```\n\n## Testing\n\nAutomated testing is described in the [`TESTING` document on github][2].\n\n## Note\n\nThe PPMS API sometimes exposes a bit of a surprising behavior. During\ndevelopment of the package, we came across several issues (this list is\ncertainly incomplete):\n\n* HTTP status return code is always `200`, even on failed authentication.\n* Results of queries are a mixture of CSV (with headers) and and text with\n  newlines (with no headers and therefore without structural information on\n  the data). JSON is implemented in some cases only.\n* The CSV headers sometimes do contain spaces between the colons, sometimes\n  they don\'t.\n* Some fields are quoted in the CSV output, some are not. Difficult to separate\n  the values since there are colons in the values too.\n* Semantics of keys is not consistent. Sometimes `user` is the user id,\n  sometimes it refers to the user\'s full name.\n* Using an invalid permission level (e.g. `Z`) with the `setright` action is\n  silently ignored by PUMAPI, the response is still `done` even though this\n  doesn\'t make any sense.\n* There is no (obvious) robust way to derive the user id from the user\'s full\n  name that is returned e.g. by `getrunningsheet`, making it very hard to\n  cross-reference it with data from `getuser`.\n* The result of the `getrunningsheet` query in general is not suited very well\n  for automated processing, it seems to be rather tailored for humans and\n  subject to (mis-) interpretation.\n* Unfortunately `Username` and `Systemname` are not the unique id, they are\n  rather the full description. Therefore sometimes looping over all users and\n  systems is necessary.\n* Some results have a very strange format - for example, the starting time of\n  the next booking is given as *minutes from now* instead of an absolute time.\n* Official documentation is rather rudimentary, i.e. it contains almost no\n  information on what is returned in case wrong / invalid parameters are\n  supplied and similar situations.\n\n## References\n\n* [Imagopole PPMS Java client][1]\n\n[1]: https://github.com/imagopole/ppms-http-client/blob/master/src/main/java/org/imagopole/ppms/api/PumapiRequest.java\n[2]: https://github.com/imcf/pyppms/blob/master/TESTING.md\n[3]: https://www.stratocore.com/\n',
     'author': 'Niko Ehrenfeuchter',
     'author_email': 'nikolaus.ehrenfeuchter@unibas.ch',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
+    'maintainer': None,
+    'maintainer_email': None,
     'url': 'https://pypi.org/project/pyppms/',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `pyppms-2.2.0/PKG-INFO` & `pyppms-2.2.0.dev2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: pyppms
-Version: 2.2.0
+Version: 2.2.0.dev2
 Summary: A Python package to communicate with Stratocore's PUMAPI.
 Home-page: https://pypi.org/project/pyppms/
 License: GPLv3
 Keywords: ppms,pumapi,booking-system,reservation-system
 Author: Niko Ehrenfeuchter
 Author-email: nikolaus.ehrenfeuchter@unibas.ch
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Project-URL: Documentation, https://imcf.one/apidocs/pyppms/pyppms.html
 Project-URL: Repository, https://github.com/imcf/pyppms
 Description-Content-Type: text/markdown
 
 # PyPPMS
```

