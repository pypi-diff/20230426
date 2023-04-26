# Comparing `tmp/feincms3_cookiecontrol-1.2.5.tar.gz` & `tmp/feincms3_cookiecontrol-1.3.0.tar.gz`

## Comparing `feincms3_cookiecontrol-1.2.5.tar` & `feincms3_cookiecontrol-1.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/admin.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/apps.py
--rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/embedding.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/models.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/views.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/migrations/0001_rework.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/migrations/__init__.py
--rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/static/feincms3_cookiecontrol/build.js
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/templates/feincms3_cookiecontrol/banner.html
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/templates/feincms3_cookiecontrol/embed.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/templatetags/__init__.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/templatetags/feincms3_cookiecontrol.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/.gitignore
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/LICENSE
--rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/README.rst
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/pyproject.toml
--rw-r--r--   0        0        0    11132 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/admin.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/apps.py
+-rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/embedding.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/models.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/views.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/migrations/0001_rework.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/migrations/__init__.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/static/f3cc.js
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/templates/feincms3_cookiecontrol/banner.html
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/templates/feincms3_cookiecontrol/embed.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/templatetags/__init__.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/templatetags/feincms3_cookiecontrol.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/LICENSE
+-rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/README.rst
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    11082 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/PKG-INFO
```

### Comparing `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/embedding.py` & `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/embedding.py`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/models.py` & `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/models.py`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/views.py` & `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/views.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,19 +7,15 @@
 
 from feincms3_cookiecontrol.models import (
     COOKIECONTROL_CACHE_TIMEOUT,
     cookiecontrol_data,
 )
 
 
-BASE = Path(__file__).parent / "static" / "feincms3_cookiecontrol"
-
-
-def read_staticfile(filename):
-    return (BASE / filename).read_text()
+SCRIPT = Path(__file__).parent / "static" / "f3cc.js"
 
 
 @cache_page(COOKIECONTROL_CACHE_TIMEOUT)
 def inject(request, *, privacy_policy_url=None):
     data = cookiecontrol_data()
     if privacy_policy_url:
         data["privacyPolicyURL"] = request.build_absolute_uri(privacy_policy_url)
@@ -28,12 +24,11 @@
         cls=DjangoJSONEncoder,
         ensure_ascii=False,
         separators=(",", ":"),
     )
     content = f"""\
 (function(){{\
 window.f3ccData={serialized};\
-{read_staticfile('build.js')}\
+{SCRIPT.read_text()}\
 }})()\
 """
-
     return HttpResponse(content, content_type="text/javascript; charset=UTF-8")
```

### Comparing `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/migrations/0001_rework.py` & `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/migrations/0001_rework.py`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/static/feincms3_cookiecontrol/build.js` & `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/static/f3cc.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -1,192 +1,175 @@
 (() => {
     (function() {
         var e = document.createElement("style");
         e.textContent = ".f3cc{font-size:16px;line-height:1.3;--_b:var(--f3cc-background,#e9e9e9);--_f:var(--f3cc-foreground,#000000);--_B:var(--f3cc-button-background,#cbcbcb);--_A:var(--f3cc-accept-background,#90f690);--_F:var(--f3cc-button-foreground,var(--_f));--_E:var(--f3cc-accept-foreground,var(--_F));}.f3cc .f3cc-banner{position:fixed;bottom:0;width:100%;background:var(--_b);color:var(--_f);z-index:2000;padding:1rem 1rem 1.25rem;}.f3cc .f3cc-embed{background:var(--_b);color:var(--_f);padding:4rem;}.f3cc .f3cc-container{display:flex;gap:2rem;max-width:70em;margin:0 auto;width:80%;}@media (max-width:60rem){.f3cc .f3cc-container{width:100%;flex-direction:column;}}.f3cc .f3cc-title{font-size:1.5em;font-weight:bold;margin-bottom:0.25em;}.f3cc .f3cc-description a{color:inherit;text-decoration:underline;}.f3cc .f3cc-description a:hover{opacity:0.7;}.f3cc .f3cc-buttons{display:flex;flex-direction:column;gap:1rem;justify-content:center;align-items:stretch;}.f3cc .f3cc-button{display:inline-block;background:var(--_B);color:var(--_F);padding:0.8rem 1.2rem;white-space:nowrap;text-decoration:none;text-align:center;cursor:pointer;border:none;}.f3cc .f3cc-button:hover{opacity:0.7;}.f3cc .f3cc-button.accept{background:var(--_A);color:var(--_E);}.f3cc .f3cc-button.modify{position:fixed;z-index:2000;bottom:1rem;right:1rem;}.f3cc-embed .f3cc-description{margin-bottom:1em;}", document.head.appendChild(e)
     })();
-    var m = (e, t = document) => t.querySelector(e),
-        h = "f3cc",
-        o = window.f3ccData || JSON.parse(m("#f3cc-data").textContent),
-        g = {},
-        l = "f3cc-embed-providers",
-        f, d, s;
-
-    function i(e, t = null, c = []) {
-        let n = document.createElement(e);
-        if (t)
-            for (let [r, a] of Object.entries(t)) r.startsWith("data-") ? n.setAttribute(r, a) : n[r] = a;
-        return n.append(...c), n
-    }
-
-    function u() {
-        if (d) {
-            w(d);
-            return
-        }
-        let e = [i("div", {
-            className: "f3cc-title",
-            textContent: o.heading
-        }), i("div", {
-            className: "f3cc-description",
-            textContent: o.description
-        })];
-        o.privacyPolicyURL && e[1].append(i("br"), i("a", {
-            textContent: o.privacyPolicyTitle,
-            href: o.privacyPolicyURL
-        }));
-        let t = [i("a", {
-            className: "f3cc-button accept",
-            textContent: o.buttonAccept,
-            onclick: R
-        }), i("a", {
-            className: "f3cc-button reject",
-            textContent: o.buttonReject,
-            onclick: A
-        })];
-        d = i("div", {
-            className: "f3cc f3cc-banner"
-        }, [i("div", {
-            className: "f3cc-container"
-        }, [i("div", {
-            className: "f3cc-content"
-        }, e), i("div", {
-            className: "f3cc-buttons"
-        }, t)])]), f.append(d)
-    }
-
-    function p() {
-        if (s) {
-            w(s);
-            return
-        }
-        let e;
-        if (e = m(".f3cc-modify")) {
-            e.addEventListener("click", n => {
-                n.preventDefault(), u()
-            });
-            return
-        }
-        let t = o.privacyPolicyURL,
-            c = window.location;
-        o.buttonModify && (!t || t == `${c.protocol}//${c.host}${c.pathname}`) && (s = i("a", {
-            className: "f3cc-button modify",
-            textContent: o.buttonModify,
-            onclick: n => {
-                n.preventDefault(), b(s), u()
-            }
-        }), f.append(s))
-    }
-
-    function y(e) {
-        let t = `${h}=${e};max-age=31536000;path=/;sameSite=Strict`;
-        o.domain && (t += `;domain=${o.domain}`), document.cookie = t
-    }
-
-    function k() {
-        let e = document.cookie ? document.cookie.split("; ") : [],
-            t = `${h}=`;
-        for (let c of e)
-            if (c.startsWith(t)) return decodeURIComponent(c.substring(t.length))
-    }
-
-    function E() {
-        return ["all", "essential"].includes(k())
-    }
-
-    function x() {
-        return k() === "all"
-    }
-
-    function w(e) {
-        e.style.display = ""
-    }
-
-    function b(e) {
-        e && (e.style.display = "none")
-    }
-
-    function R(e) {
-        e.preventDefault(), y("all"), b(d), p(), C(), v()
-    }
-
-    function A(e) {
-        e.preventDefault(), y("essential"), b(d), p()
-    }
-
-    function C() {
-        for (let e of o.cookies) {
-            let t = g[e.name];
-            t || (g[e.name] = t = document.createElement("div"), t.dataset.name = e.name, f.append(t)), t.innerHTML = e.script, S(t)
-        }
-    }
-
-    function L() {
-        f = i("div", {
-            className: "f3cc"
-        }), document.body.append(f), x() && C(), E() ? p() : u()
-    }
-    var N = {},
-        j = (e, t) => {
+    var b = (e, t = document) => t.querySelector(e),
+        w = document.body,
+        r = "className",
+        s = "textContent",
+        x = "f3cc",
+        i = window.f3ccData || JSON.parse(b("#f3cc-data")[s]),
+        k = {},
+        m = "f3cc-embed-providers",
+        p, f, l, o = (e, t = null, c = []) => {
+            let n = document.createElement(e);
+            if (t)
+                for (let [a, d] of Object.entries(t)) a.startsWith("data-") ? n.setAttribute(a, d) : n[a] = d;
+            return n.append(...c), n
+        },
+        u = () => {
+            if (f) {
+                N(f);
+                return
+            }
+            let e = [o("div", {
+                [r]: "f3cc-title",
+                [s]: i.heading
+            }), o("div", {
+                [r]: "f3cc-description",
+                [s]: i.description
+            })];
+            i.privacyPolicyURL && e[1].append(o("br"), o("a", {
+                [s]: i.privacyPolicyTitle,
+                href: i.privacyPolicyURL
+            }));
+            let t = [o("a", {
+                [r]: "f3cc-button accept",
+                [s]: i.buttonAccept,
+                onclick: D
+            }), o("a", {
+                [r]: "f3cc-button reject",
+                [s]: i.buttonReject,
+                onclick: P
+            })];
+            f = o("div", {
+                [r]: "f3cc f3cc-banner"
+            }, [o("div", {
+                [r]: "f3cc-container"
+            }, [o("div", {
+                [r]: "f3cc-content"
+            }, e), o("div", {
+                [r]: "f3cc-buttons"
+            }, t)])]), p.append(f)
+        },
+        v = () => {
+            if (l) {
+                N(l);
+                return
+            }
+            let e;
+            if (e = b(".f3cc-modify")) {
+                e.addEventListener("click", n => {
+                    n.preventDefault(), u()
+                });
+                return
+            }
+            let t = i.privacyPolicyURL,
+                c = window.location;
+            i.buttonModify && (!t || t == `${c.protocol}//${c.host}${c.pathname}`) && (l = o("a", {
+                [r]: "f3cc-button modify",
+                [s]: i.buttonModify,
+                onclick: n => {
+                    n.preventDefault(), h(l), u()
+                }
+            }), p.append(l))
+        },
+        _ = e => {
+            let t = `${x}=${e};max-age=31536000;path=/;sameSite=Strict`;
+            i.domain && (t += `;domain=${i.domain}`), document.cookie = t
+        },
+        C = () => {
+            let e = `${x}=`;
+            for (let t of document.cookie.split("; "))
+                if (t.startsWith(e)) return decodeURIComponent(t.substring(e.length))
+        },
+        g = "all",
+        S = "essential",
+        $ = () => {
+            let e = C();
+            return g == e || S == e
+        },
+        E = () => C() === g,
+        N = e => {
+            e.style.display = ""
+        },
+        h = e => {
+            e && (e.style.display = "none")
+        },
+        D = e => {
+            e.preventDefault(), _(g), h(f), v(), A(), y()
+        },
+        P = e => {
+            e.preventDefault(), _(S), h(f), v()
+        },
+        A = () => {
+            for (let e of i.cookies) {
+                let t = k[e.name];
+                t || (k[e.name] = t = o("div"), t.dataset.name = e.name, p.append(t)), t.innerHTML = e.script, j(t)
+            }
+        },
+        T = () => {
+            p = o("div", {
+                [r]: "f3cc"
+            }), w.append(p), E() && A(), $() ? v() : u()
+        },
+        R = {},
+        I = (e, t) => {
             try {
                 window.localStorage.setItem(e, JSON.stringify(t))
             } catch {
-                N[e] = t
+                R[e] = t
             }
         },
-        _ = e => {
+        L = e => {
             try {
                 return JSON.parse(window.localStorage.getItem(e))
             } catch {
-                return N[e]
+                return R[e]
             }
         },
-        v = window.f3ccRenderEmbeds = () => {
-            let e = _(l) || [];
+        y = window.f3ccRenderEmbeds = () => {
+            let e = L(m) || [];
             document.querySelectorAll(".f3cc-embed").forEach(c => {
-                let n = m("template", c),
-                    r = c.dataset.provider;
-                if (n && r && (x() || e.some(a => a === r))) {
-                    let a = n.content.cloneNode(!0);
-                    c.closest(".f3cc").replaceWith(a)
+                let n = b("template", c),
+                    a = c.dataset.provider;
+                if (n && a && (E() || e.some(d => d === a))) {
+                    let d = n.content.cloneNode(!0);
+                    c.closest(".f3cc").replaceWith(d)
                 }
             })
-        };
-
-    function $() {
-        document.body.addEventListener("click", e => {
-            let t = e.target.closest(".f3cc-button"),
-                c = t && t.closest(".f3cc-embed");
-            if (t && c) {
-                e.preventDefault();
-                let n = _(l) || [];
-                n.push(c.dataset.provider), j(l, n), v()
-            }
-        })
-    }
-
-    function S(e) {
-        if (P(e) === !0) e.parentNode.replaceChild(D(e), e);
-        else {
-            let t = -1,
-                c = e.childNodes;
-            for (; ++t < c.length;) S(c[t])
-        }
-        return e
-    }
-
-    function D(e) {
-        let t = document.createElement("script");
-        t.text = e.innerHTML;
-        let c = -1,
-            n = e.attributes,
-            r;
-        for (; ++c < n.length;) t.setAttribute((r = n[c]).name, r.value);
-        return t
-    }
-
-    function P(e) {
-        return e.tagName === "SCRIPT"
-    }
-    L();
-    v();
-    $();
+        },
+        M = () => {
+            w.addEventListener("click", e => {
+                let t = e.target.closest(".f3cc-button"),
+                    c = t && t.closest(".f3cc-embed");
+                if (t && c) {
+                    e.preventDefault();
+                    let n = L(m) || [];
+                    n.push(c.dataset.provider), I(m, n), y()
+                }
+            })
+        },
+        j = e => {
+            if (B(e) === !0) e.parentNode.replaceChild(z(e), e);
+            else {
+                let t = -1,
+                    c = e.childNodes;
+                for (; ++t < c.length;) j(c[t])
+            }
+            return e
+        },
+        z = e => {
+            let t = o("script");
+            t.text = e.innerHTML;
+            let c = -1,
+                n = e.attributes,
+                a;
+            for (; ++c < n.length;) t.setAttribute((a = n[c]).name, a.value);
+            return t
+        },
+        B = e => e.tagName === "SCRIPT";
+    T();
+    y();
+    M();
 })();
```

### Comparing `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/templatetags/feincms3_cookiecontrol.py` & `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/templatetags/feincms3_cookiecontrol.py`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.5/LICENSE` & `feincms3_cookiecontrol-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.5/README.rst` & `feincms3_cookiecontrol-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.5/pyproject.toml` & `feincms3_cookiecontrol-1.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,30 +4,29 @@
 
 [project]
 name = "feincms3-cookiecontrol"
 dynamic = ["version"]
 description = "Cookie Control Panel for GDPR compliant feincms3 websites"
 readme = "README.rst"
 license = "BSD-3-Clause"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 authors = [
     { name = "York Schickl", email = "ys@feinheit.ch" },
 ]
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: Django",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
 ]
@@ -53,12 +52,12 @@
     "/feincms3_cookiecontrol",
 ]
 
 [tool.ruff]
 extend-select = ["B", "E", "F", "W", "C90", "I", "N", "UP", "FBT", "C4", "DJ", "PIE"]
 extend-ignore = ["E501"]
 fix = true
-target-version = "py38"
+target-version = "py39"
 
 [tool.ruff.isort]
 combine-as-imports = true
 lines-after-imports = 2
```

### Comparing `feincms3_cookiecontrol-1.2.5/PKG-INFO` & `feincms3_cookiecontrol-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feincms3-cookiecontrol
-Version: 1.2.5
+Version: 1.3.0
 Summary: Cookie Control Panel for GDPR compliant feincms3 websites
 Project-URL: Homepage, https://github.com/feinheit/feincms3-cookiecontrol/
 Author-email: York Schickl <ys@feinheit.ch>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -12,22 +12,21 @@
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Requires-Dist: django>=3.2
 Requires-Dist: feincms3>=0.37
 Provides-Extra: tests
 Requires-Dist: coverage; extra == 'tests'
 Requires-Dist: requests; extra == 'tests'
 Description-Content-Type: text/x-rst
```

