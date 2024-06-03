# Comparing `tmp/websockify-0.8.0.tar.gz` & `tmp/websockify-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/websockify-0.8.0.tar", last modified: Thu Feb 18 19:13:04 2016, max compression
+gzip compressed data, was "dist/websockify-0.9.0.tar", last modified: Tue Aug 13 11:53:45 2019, max compression
```

## Comparing `websockify-0.8.0.tar` & `websockify-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,25 @@
-drwxr-xr-x   0 directxman12  (1000) directxman12  (1000)        0 2016-02-18 19:13:04.000000 websockify-0.8.0/
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)     1548 2016-02-18 19:02:47.000000 websockify-0.8.0/setup.py
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)    13525 2016-02-18 19:13:04.000000 websockify-0.8.0/PKG-INFO
-drwxr-xr-x   0 directxman12  (1000) directxman12  (1000)        0 2016-02-18 19:13:04.000000 websockify-0.8.0/websockify/
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)    40950 2016-02-18 18:43:30.000000 websockify-0.8.0/websockify/websocket.py
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)       75 2016-01-06 23:03:14.000000 websockify-0.8.0/websockify/__init__.py
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)     2872 2016-01-06 23:03:14.000000 websockify-0.8.0/websockify/auth_plugins.py
--rwxr-xr-x   0 directxman12  (1000) directxman12  (1000)    21774 2016-01-06 23:03:14.000000 websockify-0.8.0/websockify/websocketproxy.py
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)     2299 2016-01-06 23:03:14.000000 websockify-0.8.0/websockify/token_plugins.py
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)       59 2016-02-18 19:13:04.000000 websockify-0.8.0/setup.cfg
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)       56 2016-01-06 22:38:39.000000 websockify-0.8.0/MANIFEST.in
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)      612 2014-05-05 18:35:02.000000 websockify-0.8.0/LICENSE.txt
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)     7908 2016-01-06 23:03:14.000000 websockify-0.8.0/README.md
-drwxr-xr-x   0 directxman12  (1000) directxman12  (1000)        0 2016-02-18 19:13:04.000000 websockify-0.8.0/include/
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)     4729 2014-05-05 18:35:02.000000 websockify-0.8.0/include/keysym.js
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)    12323 2014-05-05 18:35:02.000000 websockify-0.8.0/include/util.js
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)     4016 2014-05-05 18:35:02.000000 websockify-0.8.0/include/base64.js
-drwxr-xr-x   0 directxman12  (1000) directxman12  (1000)        0 2016-02-18 19:13:04.000000 websockify-0.8.0/include/web-socket-js/
--rwxr-xr-x   0 directxman12  (1000) directxman12  (1000)    13039 2014-05-05 18:35:02.000000 websockify-0.8.0/include/web-socket-js/web_socket.js
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)   177139 2016-01-06 23:03:14.000000 websockify-0.8.0/include/web-socket-js/WebSocketMain.swf
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)    10220 2014-05-05 18:35:02.000000 websockify-0.8.0/include/web-socket-js/swfobject.js
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)     5971 2014-05-05 18:35:02.000000 websockify-0.8.0/include/web-socket-js/README.txt
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)    22231 2014-05-05 18:35:02.000000 websockify-0.8.0/include/VT100.js
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)    11575 2016-01-06 23:03:14.000000 websockify-0.8.0/include/websock.js
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)     5170 2014-05-05 18:35:02.000000 websockify-0.8.0/include/wsirc.js
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)     5978 2014-05-05 18:35:02.000000 websockify-0.8.0/include/webutil.js
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)     9512 2014-05-05 18:35:02.000000 websockify-0.8.0/include/wstelnet.js
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)     2693 2016-02-18 19:11:10.000000 websockify-0.8.0/CHANGES.txt
-drwxr-xr-x   0 directxman12  (1000) directxman12  (1000)        0 2016-02-18 19:13:04.000000 websockify-0.8.0/websockify.egg-info/
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)       74 2016-02-18 19:13:04.000000 websockify-0.8.0/websockify.egg-info/entry_points.txt
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)    13525 2016-02-18 19:13:04.000000 websockify-0.8.0/websockify.egg-info/PKG-INFO
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)        6 2016-02-18 19:13:04.000000 websockify-0.8.0/websockify.egg-info/requires.txt
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)      712 2016-02-18 19:13:04.000000 websockify-0.8.0/websockify.egg-info/SOURCES.txt
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)        1 2016-02-18 19:13:04.000000 websockify-0.8.0/websockify.egg-info/not-zip-safe
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)        1 2016-02-18 19:13:04.000000 websockify-0.8.0/websockify.egg-info/dependency_links.txt
--rw-r--r--   0 directxman12  (1000) directxman12  (1000)       11 2016-02-18 19:13:04.000000 websockify-0.8.0/websockify.egg-info/top_level.txt
+drwxrwxr-x   0 ossman     (210) ossman   (20210)        0 2019-08-13 11:53:45.000000 websockify-0.9.0/
+drwxrwxr-x   0 ossman     (210) ossman   (20210)        0 2019-08-13 11:53:45.000000 websockify-0.9.0/websockify.egg-info/
+-rw-rw-r--   0 ossman     (210) ossman   (20210)       74 2019-08-13 11:53:45.000000 websockify-0.9.0/websockify.egg-info/entry_points.txt
+-rw-rw-r--   0 ossman     (210) ossman   (20210)       11 2019-08-13 11:53:45.000000 websockify-0.9.0/websockify.egg-info/top_level.txt
+-rw-rw-r--   0 ossman     (210) ossman   (20210)      524 2019-08-13 11:53:45.000000 websockify-0.9.0/websockify.egg-info/SOURCES.txt
+-rw-rw-r--   0 ossman     (210) ossman   (20210)        6 2019-08-13 11:53:45.000000 websockify-0.9.0/websockify.egg-info/requires.txt
+-rw-rw-r--   0 ossman     (210) ossman   (20210)        1 2019-08-13 11:53:45.000000 websockify-0.9.0/websockify.egg-info/dependency_links.txt
+-rw-rw-r--   0 ossman     (210) ossman   (20210)    13502 2019-08-13 11:53:45.000000 websockify-0.9.0/websockify.egg-info/PKG-INFO
+-rw-rw-r--   0 ossman     (210) ossman   (20210)        1 2019-08-13 11:44:54.000000 websockify-0.9.0/websockify.egg-info/not-zip-safe
+-rw-rw-r--   0 ossman     (210) ossman   (20210)       38 2019-08-13 11:53:45.000000 websockify-0.9.0/setup.cfg
+-rw-rw-r--   0 ossman     (210) ossman   (20210)     7348 2019-08-13 11:38:15.000000 websockify-0.9.0/README.md
+-rw-rw-r--   0 ossman     (210) ossman   (20210)     3279 2019-08-13 11:38:15.000000 websockify-0.9.0/CHANGES.txt
+-rw-rw-r--   0 ossman     (210) ossman   (20210)       56 2017-01-19 13:54:49.000000 websockify-0.9.0/MANIFEST.in
+-rw-rw-r--   0 ossman     (210) ossman   (20210)     1167 2019-08-13 11:53:28.000000 websockify-0.9.0/setup.py
+drwxrwxr-x   0 ossman     (210) ossman   (20210)        0 2019-08-13 11:53:45.000000 websockify-0.9.0/websockify/
+-rw-rw-r--   0 ossman     (210) ossman   (20210)     4072 2018-09-10 14:39:42.000000 websockify-0.9.0/websockify/sysloghandler.py
+-rw-rw-r--   0 ossman     (210) ossman   (20210)       94 2019-06-17 13:22:03.000000 websockify-0.9.0/websockify/__main__.py
+-rw-rw-r--   0 ossman     (210) ossman   (20210)    29877 2019-05-17 09:27:22.000000 websockify-0.9.0/websockify/websocketproxy.py
+-rw-rw-r--   0 ossman     (210) ossman   (20210)       75 2017-01-19 13:54:49.000000 websockify-0.9.0/websockify/__init__.py
+-rw-rw-r--   0 ossman     (210) ossman   (20210)     5019 2019-07-03 10:34:55.000000 websockify-0.9.0/websockify/token_plugins.py
+-rw-rw-r--   0 ossman     (210) ossman   (20210)     3338 2019-05-09 13:51:55.000000 websockify-0.9.0/websockify/auth_plugins.py
+-rw-rw-r--   0 ossman     (210) ossman   (20210)    32279 2019-04-25 08:06:08.000000 websockify-0.9.0/websockify/websockifyserver.py
+-rw-rw-r--   0 ossman     (210) ossman   (20210)    28119 2019-04-02 15:15:15.000000 websockify-0.9.0/websockify/websocket.py
+-rw-rw-r--   0 ossman     (210) ossman   (20210)     3354 2018-08-15 15:07:43.000000 websockify-0.9.0/websockify/websocketserver.py
+-rw-rw-r--   0 ossman     (210) ossman   (20210)    13502 2019-08-13 11:53:45.000000 websockify-0.9.0/PKG-INFO
```

### Comparing `websockify-0.8.0/setup.py` & `websockify-0.9.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 from setuptools import setup, find_packages
 
-version = '0.8.0'
+version = '0.9.0'
 name = 'websockify'
 long_description = open("README.md").read() + "\n" + \
     open("CHANGES.txt").read() + "\n"
 
 setup(name=name,
       version=version,
       description="Websockify.",
       long_description=long_description,
+      long_description_content_type="text/markdown",
       classifiers=[
           "Programming Language :: Python",
           "Programming Language :: Python :: 2",
           "Programming Language :: Python :: 2.6",
           "Programming Language :: Python :: 2.7",
           "Programming Language :: Python :: 3",
           "Programming Language :: Python :: 3.3",
           "Programming Language :: Python :: 3.4"
         ],
-      data_files=[('share/websockify/include',
-                      ['include/util.js',
-                       'include/base64.js',
-                       'include/websock.js']),
-                  ('share/websockify/include/web-socket-js',
-                      ['include/web-socket-js/WebSocketMain.swf',
-                       'include/web-socket-js/swfobject.js',
-                       'include/web-socket-js/web_socket.js'])],
       keywords='noVNC websockify',
       license='LGPLv3',
-      url="https://github.com/kanaka/websockify",
+      url="https://github.com/novnc/websockify",
       author="Joel Martin",
       author_email="github@martintribe.org",
 
       packages=['websockify'],
       include_package_data=True,
       install_requires=['numpy'],
       zip_safe=False,
```

### Comparing `websockify-0.8.0/PKG-INFO` & `websockify-0.9.0/websockify.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: websockify
-Version: 0.8.0
+Version: 0.9.0
 Summary: Websockify.
-Home-page: https://github.com/kanaka/websockify
+Home-page: https://github.com/novnc/websockify
 Author: Joel Martin
 Author-email: github@martintribe.org
 License: LGPLv3
 Description: ## websockify: WebSockets support for any application/server
         
         websockify was formerly named wsproxy and was part of the
-        [noVNC](https://github.com/kanaka/noVNC) project.
+        [noVNC](https://github.com/novnc/noVNC) project.
         
         At the most basic level, websockify just translates WebSockets traffic
         to normal socket traffic. Websockify accepts the WebSockets handshake,
         parses it, and then begins forwarding traffic between the client and
         the target in both directions.
         
         ### News/help/contact
@@ -23,38 +23,30 @@
         
         If you are a websockify developer/integrator/user (or want to be)
         please join the <a
         href="https://groups.google.com/forum/?fromgroups#!forum/novnc">noVNC/websockify
         discussion group</a>
         
         Bugs and feature requests can be submitted via [github
-        issues](https://github.com/kanaka/websockify/issues).
+        issues](https://github.com/novnc/websockify/issues).
         
         If you want to show appreciation for websockify you could donate to a great
         non-profits such as: [Compassion
         International](http://www.compassion.com/), [SIL](http://www.sil.org),
         [Habitat for Humanity](http://www.habitat.org), [Electronic Frontier
         Foundation](https://www.eff.org/), [Against Malaria
         Foundation](http://www.againstmalaria.com/), [Nothing But
         Nets](http://www.nothingbutnets.net/), etc. Please tweet <a
         href="http://www.twitter.com/noVNC">@noVNC</a> if you do.
         
         ### WebSockets binary data
         
         Starting with websockify 0.5.0, only the HyBi / IETF
-        6455 WebSocket protocol is supported.
-        
-        Websockify negotiates whether to base64 encode traffic to and from the
-        client via the subprotocol header (Sec-WebSocket-Protocol). The valid
-        subprotocol values are 'binary' and 'base64' and if the client sends
-        both then the server (the python implementation) will prefer 'binary'.
-        The 'binary' subprotocol indicates that the data will be sent raw
-        using binary WebSocket frames. Some HyBi clients (such as the Flash
-        fallback and older Chrome and iOS versions) do not support binary data
-        which is why the negotiation is necessary.
+        6455 WebSocket protocol is supported. There is no support for the older
+        Base64 encoded data format.
         
         
         ### Encrypted WebSocket connections (wss://)
         
         To encrypt the traffic using the WebSocket 'wss://' URI scheme you need to
         generate a certificate and key for Websockify to load. By default, Websockify
         loads a certificate file name `self.pem` but the `--cert=CERT` and `--key=KEY`
@@ -75,77 +67,66 @@
         
         If you have a commercial/valid SSL certificate with one ore more intermediate
         certificates, concat them into one file, server certificate first, then the
         intermediate(s) from the CA, etc. Point to this file with the `--cert` option
         and then also to the key with `--key`. Finally, use `--ssl-only` as needed.
         
         
-        ### Websock Javascript library
-        
-        
-        The `include/websock.js` Javascript library library provides a Websock
-        object that is similar to the standard WebSocket object but Websock
-        enables communication with raw TCP sockets (i.e. the binary stream)
-        via websockify. This is accomplished by base64 encoding the data
-        stream between Websock and websockify.
-        
-        Websock has built-in receive queue buffering; the message event
-        does not contain actual data but is simply a notification that
-        there is new data available. Several rQ* methods are available to
-        read binary data off of the receive queue.
-        
-        The Websock API is documented on the [websock.js API wiki page](https://github.com/kanaka/websockify/wiki/websock.js)
-        
-        See the "Wrap a Program" section below for an example of using Websock
-        and websockify as a browser telnet client (`wstelnet.html`).
-        
-        
         ### Additional websockify features
         
         These are not necessary for the basic operation.
         
         * Daemonizing: When the `-D` option is specified, websockify runs
           in the background as a daemon process.
         
         * SSL (the wss:// WebSockets URI): This is detected automatically by
           websockify by sniffing the first byte sent from the client and then
           wrapping the socket if the data starts with '\x16' or '\x80'
           (indicating SSL).
         
-        * Flash security policy: websockify detects flash security policy
-          requests (again by sniffing the first packet) and answers with an
-          appropriate flash security policy response (and then closes the
-          port). This means no separate flash security policy server is needed
-          for supporting the flash WebSockets fallback emulator.
-        
         * Session recording: This feature that allows recording of the traffic
           sent and received from the client to a file using the `--record`
           option.
         
         * Mini-webserver: websockify can detect and respond to normal web
-          requests on the same port as the WebSockets proxy and Flash security
-          policy. This functionality is activated with the `--web DIR` option
-          where DIR is the root of the web directory to serve.
+          requests on the same port as the WebSockets proxy. This functionality
+          is activated with the `--web DIR` option where DIR is the root of the
+          web directory to serve.
         
         * Wrap a program: see the "Wrap a Program" section below.
         
         * Log files: websockify can save all logging information in a file.
           This functionality is activated with the `--log-file FILE` option
           where FILE is the file where the logs should be saved.
         
-        ### Implementations of websockify
+        * Authentication plugins: websockify can demand authentication for
+          websocket connections and, if you use `--web-auth`, also for normal
+          web requests. This functionality is activated with the
+          `--auth-plugin CLASS` and `--auth-source ARG` options, where CLASS is
+          usually one from auth_plugins.py and ARG is the plugin's configuration.
+        
+        * Token plugins: a single instance of websockify can connect clients to
+          multiple different pre-configured targets, depending on the token sent
+          by the client using the `token` URL parameter, or the hostname used to
+          reach websockify, if you use `--host-token`. This functionality is
+          activated with the `--token-plugin CLASS` and `--token-source ARG`
+          options, where CLASS is usually one from token_plugins.py and ARG is
+          the plugin's configuration.
+        
+        ### Other implementations of websockify
         
         The primary implementation of websockify is in python. There are
-        several alternate implementations in other languages (C, Node.js,
-        Clojure, Ruby) in the `other/` subdirectory (with varying levels of
-        functionality).
+        several alternate implementations in other languages available in
+        our sister repositories [websockify-js](https://github.com/novnc/websockify-js)
+        (JavaScript/Node.js) and [websockify-other](https://github.com/novnc/websockify-other)
+         (C, Clojure, Ruby).
         
         In addition there are several other external projects that implement
         the websockify "protocol". See the alternate implementation [Feature
-        Matrix](https://github.com/kanaka/websockify/wiki/Feature_Matrix) for
+        Matrix](https://github.com/novnc/websockify/wiki/Feature_Matrix) for
         more information.
         
         
         ### Wrap a Program
         
         In addition to proxying from a source address to a target address
         (which may be on a different system), websockify has the ability to
@@ -164,54 +145,62 @@
             `./run 2023 -- PROGRAM ARGS`
         
         The `--wrap-mode` option can be used to indicate what action to take
         when the wrapped program exits or daemonizes.
         
         Here is an example of using websockify to wrap the vncserver command
         (which backgrounds itself) for use with
-        [noVNC](https://github.com/kanaka/noVNC):
+        [noVNC](https://github.com/novnc/noVNC):
         
             `./run 5901 --wrap-mode=ignore -- vncserver -geometry 1024x768 :1`
         
         Here is an example of wrapping telnetd (from krb5-telnetd). telnetd
         exits after the connection closes so the wrap mode is set to respawn
         the command:
         
             `sudo ./run 2023 --wrap-mode=respawn -- telnetd -debug 2023`
         
-        The `wstelnet.html` page demonstrates a simple WebSockets based telnet
-        client (use 'localhost' and '2023' for the host and port
-        respectively).
-        
-        
-        ### Building the Python ssl module (for python 2.5 and older)
-        
-        * Install the build dependencies. On Ubuntu use this command:
-        
-            `sudo aptitude install python-dev bluetooth-dev`
-        
-        * At the top level of the websockify repostory, download, build and
-          symlink the ssl module:
-        
-            `wget --no-check-certificate http://pypi.python.org/packages/source/s/ssl/ssl-1.15.tar.gz`
-        
-            `tar xvzf ssl-1.15.tar.gz`
-        
-            `cd ssl-1.15`
-        
-            `make`
-        
-            `cd ../`
-        
-            `ln -sf ssl-1.15/build/lib.linux-*/ssl ssl`
+        The `wstelnet.html` page in the [websockify-js](https://github.com/novnc/websockify-js)
+        project demonstrates a simple WebSockets based telnet client (use
+        'localhost' and '2023' for the host and port respectively).
+        
+        
+        ### Installing websockify
+        
+        Download one of the releases or the latest development version, extract
+        it and run `python setup.py install` as root in the directory where you
+        extracted the files. Normally, this will also install numpy for better
+        performance, if you don't have it installed already. However, numpy is
+        optional. If you don't want to install numpy or if you can't compile it,
+        you can edit setup.py and remove the `install_requires=['numpy'],` line
+        before running `python setup.py install`.
         
+        Afterwards, websockify should be available in your path. Run
+        `websockify --help` to confirm it's installed correctly.
         
         Changes
         =======
         
+        0.9.0
+        -----
+        
+        * Base64 support removed and binary mode is now required
+        * Low level WebSocket protocol handling now has its own class
+        * Authentication now optionally required for web server
+        * Server hostname can be used as the token
+        * JWT/JWS/JWE can be used for the token
+        * redis can be used for the token
+        * Can now log to syslog
+        * Improved latency by disabling Nagle for proxied connection
+        * Added client certificate authentication
+        * Support for password protected certificate key file
+        * TLS ciphers and options are now configurable
+        * Can be invoked via inetd
+        * Lots of minor fixes...
+        
         0.8.0
         -----
         
         * Make websockify properly terminate children on SIGTERM (#226)
         * Remove logging in signal handlers (this can cause Python to hang under certain conditions) (#219)
         * Make it easier to log to a file (#205)
         * Add support for IPv6 addresses in tokens in the TokenFile token plugins (#197)
@@ -303,7 +292,8 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
+Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,143 +1,143 @@
-Metadata-Version: 1.1 Name: websockify Version: 0.8.0 Summary: Websockify.
-Home-page: https://github.com/kanaka/websockify Author: Joel Martin Author-
+Metadata-Version: 2.1 Name: websockify Version: 0.9.0 Summary: Websockify.
+Home-page: https://github.com/novnc/websockify Author: Joel Martin Author-
 email: github@martintribe.org License: LGPLv3 Description: ## websockify:
 WebSockets support for any application/server websockify was formerly named
-wsproxy and was part of the [noVNC](https://github.com/kanaka/noVNC) project.
-At the most basic level, websockify just translates WebSockets traffic to
-normal socket traffic. Websockify accepts the WebSockets handshake, parses it,
-and then begins forwarding traffic between the client and the target in both
+wsproxy and was part of the [noVNC](https://github.com/novnc/noVNC) project. At
+the most basic level, websockify just translates WebSockets traffic to normal
+socket traffic. Websockify accepts the WebSockets handshake, parses it, and
+then begins forwarding traffic between the client and the target in both
 directions. ### News/help/contact Notable commits, announcements and news are
 posted to _@_n_o_V_N_C If you are a websockify developer/integrator/user (or want to
 be) please join the _n_o_V_N_C_/_w_e_b_s_o_c_k_i_f_y_ _d_i_s_c_u_s_s_i_o_n_ _g_r_o_u_p Bugs and feature requests
-can be submitted via [github issues](https://github.com/kanaka/websockify/
+can be submitted via [github issues](https://github.com/novnc/websockify/
 issues). If you want to show appreciation for websockify you could donate to a
 great non-profits such as: [Compassion International](http://
 www.compassion.com/), [SIL](http://www.sil.org), [Habitat for Humanity](http://
 www.habitat.org), [Electronic Frontier Foundation](https://www.eff.org/),
 [Against Malaria Foundation](http://www.againstmalaria.com/), [Nothing But
 Nets](http://www.nothingbutnets.net/), etc. Please tweet _@_n_o_V_N_C if you do. ###
 WebSockets binary data Starting with websockify 0.5.0, only the HyBi / IETF
-6455 WebSocket protocol is supported. Websockify negotiates whether to base64
-encode traffic to and from the client via the subprotocol header (Sec-
-WebSocket-Protocol). The valid subprotocol values are 'binary' and 'base64' and
-if the client sends both then the server (the python implementation) will
-prefer 'binary'. The 'binary' subprotocol indicates that the data will be sent
-raw using binary WebSocket frames. Some HyBi clients (such as the Flash
-fallback and older Chrome and iOS versions) do not support binary data which is
-why the negotiation is necessary. ### Encrypted WebSocket connections (wss://
-) To encrypt the traffic using the WebSocket 'wss://' URI scheme you need to
-generate a certificate and key for Websockify to load. By default, Websockify
-loads a certificate file name `self.pem` but the `--cert=CERT` and `--key=KEY`
-options can override the file name. You can generate a self-signed certificate
-using openssl. When asked for the common name, use the hostname of the server
-where the proxy will be running: ``` openssl req -new -x509 -days 365 -nodes -
-out self.pem -keyout self.pem ``` For a self-signed certificate to work, you
-need to make your client/browser understand it. You can do this by installing
-it as accepted certificate, or by using that same certificate for a HTTPS
-connection to which you navigate first and approve. Browsers generally don't
-give you the "trust certificate?" prompt by opening a WSS socket with invalid
-certificate, hence you need to have it acccept it by either of those two
-methods. If you have a commercial/valid SSL certificate with one ore more
-intermediate certificates, concat them into one file, server certificate first,
-then the intermediate(s) from the CA, etc. Point to this file with the `--cert`
-option and then also to the key with `--key`. Finally, use `--ssl-only` as
-needed. ### Websock Javascript library The `include/websock.js` Javascript
-library library provides a Websock object that is similar to the standard
-WebSocket object but Websock enables communication with raw TCP sockets (i.e.
-the binary stream) via websockify. This is accomplished by base64 encoding the
-data stream between Websock and websockify. Websock has built-in receive queue
-buffering; the message event does not contain actual data but is simply a
-notification that there is new data available. Several rQ* methods are
-available to read binary data off of the receive queue. The Websock API is
-documented on the [websock.js API wiki page](https://github.com/kanaka/
-websockify/wiki/websock.js) See the "Wrap a Program" section below for an
-example of using Websock and websockify as a browser telnet client
-(`wstelnet.html`). ### Additional websockify features These are not necessary
-for the basic operation. * Daemonizing: When the `-D` option is specified,
-websockify runs in the background as a daemon process. * SSL (the wss:/
-/ WebSockets URI): This is detected automatically by websockify by sniffing the
-first byte sent from the client and then wrapping the socket if the data starts
-with '\x16' or '\x80' (indicating SSL). * Flash security policy: websockify
-detects flash security policy requests (again by sniffing the first packet) and
-answers with an appropriate flash security policy response (and then closes the
-port). This means no separate flash security policy server is needed for
-supporting the flash WebSockets fallback emulator. * Session recording: This
-feature that allows recording of the traffic sent and received from the client
-to a file using the `--record` option. * Mini-webserver: websockify can detect
-and respond to normal web requests on the same port as the WebSockets proxy and
-Flash security policy. This functionality is activated with the `--web DIR`
-option where DIR is the root of the web directory to serve. * Wrap a program:
-see the "Wrap a Program" section below. * Log files: websockify can save all
-logging information in a file. This functionality is activated with the `--log-
-file FILE` option where FILE is the file where the logs should be saved. ###
-Implementations of websockify The primary implementation of websockify is in
-python. There are several alternate implementations in other languages (C,
-Node.js, Clojure, Ruby) in the `other/` subdirectory (with varying levels of
-functionality). In addition there are several other external projects that
-implement the websockify "protocol". See the alternate implementation [Feature
-Matrix](https://github.com/kanaka/websockify/wiki/Feature_Matrix) for more
-information. ### Wrap a Program In addition to proxying from a source address
-to a target address (which may be on a different system), websockify has the
-ability to launch a program on the local system and proxy WebSockets traffic to
-a normal TCP port owned/bound by the program. The is accomplished with a small
+6455 WebSocket protocol is supported. There is no support for the older Base64
+encoded data format. ### Encrypted WebSocket connections (wss://) To encrypt
+the traffic using the WebSocket 'wss://' URI scheme you need to generate a
+certificate and key for Websockify to load. By default, Websockify loads a
+certificate file name `self.pem` but the `--cert=CERT` and `--key=KEY` options
+can override the file name. You can generate a self-signed certificate using
+openssl. When asked for the common name, use the hostname of the server where
+the proxy will be running: ``` openssl req -new -x509 -days 365 -nodes -out
+self.pem -keyout self.pem ``` For a self-signed certificate to work, you need
+to make your client/browser understand it. You can do this by installing it as
+accepted certificate, or by using that same certificate for a HTTPS connection
+to which you navigate first and approve. Browsers generally don't give you the
+"trust certificate?" prompt by opening a WSS socket with invalid certificate,
+hence you need to have it acccept it by either of those two methods. If you
+have a commercial/valid SSL certificate with one ore more intermediate
+certificates, concat them into one file, server certificate first, then the
+intermediate(s) from the CA, etc. Point to this file with the `--cert` option
+and then also to the key with `--key`. Finally, use `--ssl-only` as needed. ###
+Additional websockify features These are not necessary for the basic operation.
+* Daemonizing: When the `-D` option is specified, websockify runs in the
+background as a daemon process. * SSL (the wss:// WebSockets URI): This is
+detected automatically by websockify by sniffing the first byte sent from the
+client and then wrapping the socket if the data starts with '\x16' or '\x80'
+(indicating SSL). * Session recording: This feature that allows recording of
+the traffic sent and received from the client to a file using the `--record`
+option. * Mini-webserver: websockify can detect and respond to normal web
+requests on the same port as the WebSockets proxy. This functionality is
+activated with the `--web DIR` option where DIR is the root of the web
+directory to serve. * Wrap a program: see the "Wrap a Program" section below. *
+Log files: websockify can save all logging information in a file. This
+functionality is activated with the `--log-file FILE` option where FILE is the
+file where the logs should be saved. * Authentication plugins: websockify can
+demand authentication for websocket connections and, if you use `--web-auth`,
+also for normal web requests. This functionality is activated with the `--auth-
+plugin CLASS` and `--auth-source ARG` options, where CLASS is usually one from
+auth_plugins.py and ARG is the plugin's configuration. * Token plugins: a
+single instance of websockify can connect clients to multiple different pre-
+configured targets, depending on the token sent by the client using the `token`
+URL parameter, or the hostname used to reach websockify, if you use `--host-
+token`. This functionality is activated with the `--token-plugin CLASS` and `--
+token-source ARG` options, where CLASS is usually one from token_plugins.py and
+ARG is the plugin's configuration. ### Other implementations of websockify The
+primary implementation of websockify is in python. There are several alternate
+implementations in other languages available in our sister repositories
+[websockify-js](https://github.com/novnc/websockify-js) (JavaScript/Node.js)
+and [websockify-other](https://github.com/novnc/websockify-other) (C, Clojure,
+Ruby). In addition there are several other external projects that implement the
+websockify "protocol". See the alternate implementation [Feature Matrix](https:
+//github.com/novnc/websockify/wiki/Feature_Matrix) for more information. ###
+Wrap a Program In addition to proxying from a source address to a target
+address (which may be on a different system), websockify has the ability to
+launch a program on the local system and proxy WebSockets traffic to a normal
+TCP port owned/bound by the program. The is accomplished with a small
 LD_PRELOAD library (`rebind.so`) which intercepts bind() system calls by the
 program. The specified port is moved to a new localhost/loopback free high
 port. websockify then proxies WebSockets traffic directed to the original port
 to the new (moved) port of the program. The program wrap mode is invoked by
 replacing the target with `--` followed by the program command line to wrap.
 `./run 2023 -- PROGRAM ARGS` The `--wrap-mode` option can be used to indicate
 what action to take when the wrapped program exits or daemonizes. Here is an
 example of using websockify to wrap the vncserver command (which backgrounds
-itself) for use with [noVNC](https://github.com/kanaka/noVNC): `./run 5901 --
+itself) for use with [noVNC](https://github.com/novnc/noVNC): `./run 5901 --
 wrap-mode=ignore -- vncserver -geometry 1024x768 :1` Here is an example of
 wrapping telnetd (from krb5-telnetd). telnetd exits after the connection closes
 so the wrap mode is set to respawn the command: `sudo ./run 2023 --wrap-
-mode=respawn -- telnetd -debug 2023` The `wstelnet.html` page demonstrates a
+mode=respawn -- telnetd -debug 2023` The `wstelnet.html` page in the
+[websockify-js](https://github.com/novnc/websockify-js) project demonstrates a
 simple WebSockets based telnet client (use 'localhost' and '2023' for the host
-and port respectively). ### Building the Python ssl module (for python 2.5 and
-older) * Install the build dependencies. On Ubuntu use this command: `sudo
-aptitude install python-dev bluetooth-dev` * At the top level of the websockify
-repostory, download, build and symlink the ssl module: `wget --no-check-
-certificate http://pypi.python.org/packages/source/s/ssl/ssl-1.15.tar.gz` `tar
-xvzf ssl-1.15.tar.gz` `cd ssl-1.15` `make` `cd ../` `ln -sf ssl-1.15/build/
-lib.linux-*/ssl ssl` Changes ======= 0.8.0 ----- * Make websockify properly
-terminate children on SIGTERM (#226) * Remove logging in signal handlers (this
-can cause Python to hang under certain conditions) (#219) * Make it easier to
-log to a file (#205) * Add support for IPv6 addresses in tokens in the
-TokenFile token plugins (#197) * Improve auth plugin framework to enable better
-support for HTTP auth (#194, #201) * Fix bug in JSONTokenAPI token plugin
-(#192) * Fix a missing variable in the exception handler (#178) 0.7.0 ----- *
-Python 3 support fixes (#140, #155, #159) * Generic token-parsing plugins
-support (#162) * Generic authentication plugins support (#172) * Fixed frame
-corruption on big-endian systems (#161) * Support heartbeats (via PING) and
-automatic responses to PONG (#169) * Automatically reject unmasked client
-frames by default (strict mode) (#174) * Automatically restart interrupted
-select calls (#175) * Make 'run' respect environment settings (including
-virtualenv) (#176) 0.6.1 - May 11, 2015 -------------------- * **PATCH
-RELEASE**: Fixes a bug causing file_only to not be passed properly 0.6.0 - Feb
-18, 2014 -------------------- * **NOTE** : 0.6.0 will break existing code that
-sub-classes WebsocketProxy * Refactor to use standard SocketServer
-RequestHandler design * Fix zombie process bug on certain systems when using
-multiprocessing * Add better unit tests * Log information via python `logging`
-module 0.5.1 - Jun 27, 2013 -------------------- * use upstream einaros/ws
-(>=0.4.27) with websockify.js * file_only and no_parent security options for
-WSRequestHandler * Update build of web-socket-js (c0855c6cae) * add include/
-web-socket-js-project submodule to gimite/web-socket-js for DSFG compliance. *
-drop Hixie protocol support 0.4.1 - Mar 12, 2013 -------------------- *
-***NOTE*** : 0.5.0 will drop Hixie protocol support * add include/ directory
-and remove some dev files from source distribution. 0.4.0 - Mar 12, 2013 ------
--------------- * ***NOTE*** : 0.5.0 will drop Hixie protocol support * use
-Buffer base64 support in Node.js implementation 0.3.0 - Jan 15, 2013 ----------
----------- * refactor into modules: websocket, websocketproxy * switch to web-
-socket-js that uses IETF 6455 * change to MPL 2.0 license for include/*.js *
-fix session recording 0.2.1 - Oct 15, 2012 -------------------- * re-released
-with updated version number 0.2.0 - Sep 17, 2012 -------------------- * Binary
-data support in websock.js * Target config file/dir and multiple targets with
-token selector * IPv6 fixes * SSL target support * Proxy to/from unix socket
-0.1.0 - May 11, 2012 -------------------- * Initial versioned release.
-Keywords: noVNC websockify Platform: UNKNOWN Classifier: Programming Language
-:: Python Classifier: Programming Language :: Python :: 2 Classifier:
-Programming Language :: Python :: 2.6 Classifier: Programming Language ::
-Python :: 2.7 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.3 Classifier: Programming Language ::
-Python :: 3.4
+and port respectively). ### Installing websockify Download one of the releases
+or the latest development version, extract it and run `python setup.py install`
+as root in the directory where you extracted the files. Normally, this will
+also install numpy for better performance, if you don't have it installed
+already. However, numpy is optional. If you don't want to install numpy or if
+you can't compile it, you can edit setup.py and remove the `install_requires=
+['numpy'],` line before running `python setup.py install`. Afterwards,
+websockify should be available in your path. Run `websockify --help` to confirm
+it's installed correctly. Changes ======= 0.9.0 ----- * Base64 support removed
+and binary mode is now required * Low level WebSocket protocol handling now has
+its own class * Authentication now optionally required for web server * Server
+hostname can be used as the token * JWT/JWS/JWE can be used for the token *
+redis can be used for the token * Can now log to syslog * Improved latency by
+disabling Nagle for proxied connection * Added client certificate
+authentication * Support for password protected certificate key file * TLS
+ciphers and options are now configurable * Can be invoked via inetd * Lots of
+minor fixes... 0.8.0 ----- * Make websockify properly terminate children on
+SIGTERM (#226) * Remove logging in signal handlers (this can cause Python to
+hang under certain conditions) (#219) * Make it easier to log to a file (#205)
+* Add support for IPv6 addresses in tokens in the TokenFile token plugins
+(#197) * Improve auth plugin framework to enable better support for HTTP auth
+(#194, #201) * Fix bug in JSONTokenAPI token plugin (#192) * Fix a missing
+variable in the exception handler (#178) 0.7.0 ----- * Python 3 support fixes
+(#140, #155, #159) * Generic token-parsing plugins support (#162) * Generic
+authentication plugins support (#172) * Fixed frame corruption on big-endian
+systems (#161) * Support heartbeats (via PING) and automatic responses to PONG
+(#169) * Automatically reject unmasked client frames by default (strict mode)
+(#174) * Automatically restart interrupted select calls (#175) * Make 'run'
+respect environment settings (including virtualenv) (#176) 0.6.1 - May 11, 2015
+-------------------- * **PATCH RELEASE**: Fixes a bug causing file_only to not
+be passed properly 0.6.0 - Feb 18, 2014 -------------------- * **NOTE** : 0.6.0
+will break existing code that sub-classes WebsocketProxy * Refactor to use
+standard SocketServer RequestHandler design * Fix zombie process bug on certain
+systems when using multiprocessing * Add better unit tests * Log information
+via python `logging` module 0.5.1 - Jun 27, 2013 -------------------- * use
+upstream einaros/ws (>=0.4.27) with websockify.js * file_only and no_parent
+security options for WSRequestHandler * Update build of web-socket-js
+(c0855c6cae) * add include/web-socket-js-project submodule to gimite/web-
+socket-js for DSFG compliance. * drop Hixie protocol support 0.4.1 - Mar 12,
+2013 -------------------- * ***NOTE*** : 0.5.0 will drop Hixie protocol support
+* add include/ directory and remove some dev files from source distribution.
+0.4.0 - Mar 12, 2013 -------------------- * ***NOTE*** : 0.5.0 will drop Hixie
+protocol support * use Buffer base64 support in Node.js implementation 0.3.0 -
+Jan 15, 2013 -------------------- * refactor into modules: websocket,
+websocketproxy * switch to web-socket-js that uses IETF 6455 * change to MPL
+2.0 license for include/*.js * fix session recording 0.2.1 - Oct 15, 2012 -----
+--------------- * re-released with updated version number 0.2.0 - Sep 17, 2012
+-------------------- * Binary data support in websock.js * Target config file/
+dir and multiple targets with token selector * IPv6 fixes * SSL target support
+* Proxy to/from unix socket 0.1.0 - May 11, 2012 -------------------- * Initial
+versioned release. Keywords: noVNC websockify Platform: UNKNOWN Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.6 Classifier: Programming
+Language :: Python :: 2.7 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.3 Classifier: Programming
+Language :: Python :: 3.4 Description-Content-Type: text/markdown
```

### Comparing `websockify-0.8.0/websockify/websocket.py` & `websockify-0.9.0/websockify/websockifyserver.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,98 +1,83 @@
 #!/usr/bin/env python
 
 '''
-Python WebSocket library with support for "wss://" encryption.
+Python WebSocket server base with support for "wss://" encryption.
 Copyright 2011 Joel Martin
+Copyright 2016 Pierre Ossman
 Licensed under LGPL version 3 (see docs/LICENSE.LGPL-3)
 
-Supports following protocol versions:
-    - http://tools.ietf.org/html/draft-ietf-hybi-thewebsocketprotocol-07
-    - http://tools.ietf.org/html/draft-ietf-hybi-thewebsocketprotocol-10
-    - http://tools.ietf.org/html/rfc6455
-
 You can make a cert/key with openssl using:
 openssl req -new -x509 -days 365 -nodes -out self.pem -keyout self.pem
 as taken from http://docs.python.org/dev/library/ssl.html#certificates
 
 '''
 
 import os, sys, time, errno, signal, socket, select, logging
-import array, struct
-from base64 import b64encode, b64decode
+import multiprocessing
 
 # Imports that vary by python version
 
 # python 3.0 differences
 if sys.hexversion > 0x3000000:
-    b2s = lambda buf: buf.decode('latin_1')
     s2b = lambda s: s.encode('latin_1')
-    s2a = lambda s: s
 else:
-    b2s = lambda buf: buf  # No-op
     s2b = lambda s: s      # No-op
-    s2a = lambda s: [ord(c) for c in s]
-try:    from io import StringIO
-except: from cStringIO import StringIO
-try:    from http.server import SimpleHTTPRequestHandler
-except: from SimpleHTTPServer import SimpleHTTPRequestHandler
-
-# python 2.6 differences
-try:    from hashlib import sha1
-except: from sha import sha as sha1
 
-# python 2.5 differences
 try:
-    from struct import pack, unpack_from
-except:
-    from struct import pack
-    def unpack_from(fmt, buf, offset=0):
-        slice = buffer(buf, offset, struct.calcsize(fmt))
-        return struct.unpack(fmt, slice)
+    from http.server import SimpleHTTPRequestHandler
+except ImportError:
+    from SimpleHTTPServer import SimpleHTTPRequestHandler
 
 # Degraded functionality if these imports are missing
-for mod, msg in [('numpy', 'HyBi protocol will be slower'),
-                 ('ssl', 'TLS/SSL/wss is disabled'),
-                 ('multiprocessing', 'Multi-Processing is disabled'),
+for mod, msg in [('ssl', 'TLS/SSL/wss is disabled'),
                  ('resource', 'daemonizing is disabled')]:
     try:
         globals()[mod] = __import__(mod)
     except ImportError:
         globals()[mod] = None
         print("WARNING: no '%s' module, %s" % (mod, msg))
 
-if multiprocessing and sys.platform == 'win32':
+if sys.platform == 'win32':
     # make sockets pickle-able/inheritable
     import multiprocessing.reduction
 
+from websockify.websocket import WebSocket, WebSocketWantReadError, WebSocketWantWriteError
+from websockify.websocketserver import WebSocketRequestHandlerMixIn
+
+class CompatibleWebSocket(WebSocket):
+    def select_subprotocol(self, protocols):
+        # Handle old websockify clients that still specifiy a sub-protocol
+        if 'binary' in protocols:
+            return 'binary'
+        else:
+            return ''
 
 # HTTP handler with WebSocket upgrade support
-class WebSocketRequestHandler(SimpleHTTPRequestHandler):
+class WebSockifyRequestHandler(WebSocketRequestHandlerMixIn, SimpleHTTPRequestHandler):
     """
     WebSocket Request Handler Class, derived from SimpleHTTPRequestHandler.
     Must be sub-classed with new_websocket_client method definition.
     The request handler can be configured by setting optional
     attributes on the server object:
 
     * only_upgrade: If true, SimpleHTTPRequestHandler will not be enabled,
       only websocket is allowed.
     * verbose: If true, verbose logging is activated.
     * daemon: Running as daemon, do not write to console etc
     * record: Record raw frame data as JavaScript array into specified filename
     * run_once: Handle a single request
     * handler_id: A sequence number for this connection, appended to record filename
     """
-    buffer_size = 65536
-
-    GUID = "258EAFA5-E914-47DA-95CA-C5AB0DC85B11"
-
     server_version = "WebSockify"
 
     protocol_version = "HTTP/1.1"
 
+    SocketClass = CompatibleWebSocket
+
     # An exception while the WebSocket client was connected
     class CClose(Exception):
         pass
 
     def __init__(self, req, addr, server):
         # Retrieve a few configuration variables from the server
         self.only_upgrade = getattr(server, "only_upgrade", False)
@@ -100,179 +85,25 @@
         self.daemon = getattr(server, "daemon", False)
         self.record = getattr(server, "record", False)
         self.run_once = getattr(server, "run_once", False)
         self.rec        = None
         self.handler_id = getattr(server, "handler_id", False)
         self.file_only = getattr(server, "file_only", False)
         self.traffic = getattr(server, "traffic", False)
-        self.auto_pong = getattr(server, "auto_pong", False)
-        self.strict_mode = getattr(server, "strict_mode", True)
+        self.web_auth = getattr(server, "web_auth", False)
+        self.host_token = getattr(server, "host_token", False)
 
         self.logger = getattr(server, "logger", None)
         if self.logger is None:
-            self.logger = WebSocketServer.get_logger()
+            self.logger = WebSockifyServer.get_logger()
 
         SimpleHTTPRequestHandler.__init__(self, req, addr, server)
 
     def log_message(self, format, *args):
-        self.logger.info("%s - - [%s] %s" % (self.address_string(), self.log_date_time_string(), format % args))
-
-    @staticmethod
-    def unmask(buf, hlen, plen):
-        pstart = hlen + 4
-        pend = pstart + plen
-        if numpy:
-            b = c = s2b('')
-            if plen >= 4:
-                dtype=numpy.dtype('<u4')
-                if sys.byteorder == 'big':
-                    dtype = dtype.newbyteorder('>')
-                mask = numpy.frombuffer(buf, dtype, offset=hlen, count=1)
-                data = numpy.frombuffer(buf, dtype, offset=pstart,
-                        count=int(plen / 4))
-                #b = numpy.bitwise_xor(data, mask).data
-                b = numpy.bitwise_xor(data, mask).tostring()
-
-            if plen % 4:
-                #self.msg("Partial unmask")
-                dtype=numpy.dtype('B')
-                if sys.byteorder == 'big':
-                    dtype = dtype.newbyteorder('>')
-                mask = numpy.frombuffer(buf, dtype, offset=hlen,
-                        count=(plen % 4))
-                data = numpy.frombuffer(buf, dtype,
-                        offset=pend - (plen % 4), count=(plen % 4))
-                c = numpy.bitwise_xor(data, mask).tostring()
-            return b + c
-        else:
-            # Slower fallback
-            mask = buf[hlen:hlen+4]
-            data = array.array('B')
-            mask = s2a(mask)
-            data.fromstring(buf[pstart:pend])
-            for i in range(len(data)):
-                data[i] ^= mask[i % 4]
-            return data.tostring()
-
-    @staticmethod
-    def encode_hybi(buf, opcode, base64=False):
-        """ Encode a HyBi style WebSocket frame.
-        Optional opcode:
-            0x0 - continuation
-            0x1 - text frame (base64 encode buf)
-            0x2 - binary frame (use raw buf)
-            0x8 - connection close
-            0x9 - ping
-            0xA - pong
-        """
-        if base64:
-            buf = b64encode(buf)
-
-        b1 = 0x80 | (opcode & 0x0f) # FIN + opcode
-        payload_len = len(buf)
-        if payload_len <= 125:
-            header = pack('>BB', b1, payload_len)
-        elif payload_len > 125 and payload_len < 65536:
-            header = pack('>BBH', b1, 126, payload_len)
-        elif payload_len >= 65536:
-            header = pack('>BBQ', b1, 127, payload_len)
-
-        #self.msg("Encoded: %s", repr(header + buf))
-
-        return header + buf, len(header), 0
-
-    @staticmethod
-    def decode_hybi(buf, base64=False, logger=None, strict=True):
-        """ Decode HyBi style WebSocket packets.
-        Returns:
-            {'fin'          : 0_or_1,
-             'opcode'       : number,
-             'masked'       : boolean,
-             'hlen'         : header_bytes_number,
-             'length'       : payload_bytes_number,
-             'payload'      : decoded_buffer,
-             'left'         : bytes_left_number,
-             'close_code'   : number,
-             'close_reason' : string}
-        """
-
-        f = {'fin'          : 0,
-             'opcode'       : 0,
-             'masked'       : False,
-             'hlen'         : 2,
-             'length'       : 0,
-             'payload'      : None,
-             'left'         : 0,
-             'close_code'   : 1000,
-             'close_reason' : ''}
-
-        if logger is None:
-            logger = WebSocketServer.get_logger()
-
-        blen = len(buf)
-        f['left'] = blen
-
-        if blen < f['hlen']:
-            return f # Incomplete frame header
-
-        b1, b2 = unpack_from(">BB", buf)
-        f['opcode'] = b1 & 0x0f
-        f['fin'] = (b1 & 0x80) >> 7
-        f['masked'] = (b2 & 0x80) >> 7
-
-        f['length'] = b2 & 0x7f
-
-        if f['length'] == 126:
-            f['hlen'] = 4
-            if blen < f['hlen']:
-                return f # Incomplete frame header
-            (f['length'],) = unpack_from('>xxH', buf)
-        elif f['length'] == 127:
-            f['hlen'] = 10
-            if blen < f['hlen']:
-                return f # Incomplete frame header
-            (f['length'],) = unpack_from('>xxQ', buf)
-
-        full_len = f['hlen'] + f['masked'] * 4 + f['length']
-
-        if blen < full_len: # Incomplete frame
-            return f # Incomplete frame header
-
-        # Number of bytes that are part of the next frame(s)
-        f['left'] = blen - full_len
-
-        # Process 1 frame
-        if f['masked']:
-            # unmask payload
-            f['payload'] = WebSocketRequestHandler.unmask(buf, f['hlen'],
-                                                  f['length'])
-        else:
-            logger.debug("Unmasked frame: %s" % repr(buf))
-
-            if strict:
-                raise WebSocketRequestHandler.CClose(1002, "The client sent an unmasked frame.")
-
-            f['payload'] = buf[(f['hlen'] + f['masked'] * 4):full_len]
-
-        if base64 and f['opcode'] in [1, 2]:
-            try:
-                f['payload'] = b64decode(f['payload'])
-            except:
-                logger.exception("Exception while b64decoding buffer: %s" %
-                                 (repr(buf)))
-                raise
-
-        if f['opcode'] == 0x08:
-            if f['length'] >= 2:
-                f['close_code'] = unpack_from(">H", f['payload'])[0]
-            if f['length'] > 3:
-                f['close_reason'] = f['payload'][2:]
-
-        return f
-
+        self.logger.info("%s - - [%s] %s" % (self.client_address[0], self.log_date_time_string(), format % args))
 
     #
     # WebSocketRequestHandler logging/output functions
     #
 
     def print_traffic(self, token="."):
         """ Show traffic flow mode. """
@@ -297,283 +128,186 @@
 
     #
     # Main WebSocketRequestHandler methods
     #
     def send_frames(self, bufs=None):
         """ Encode and send WebSocket frames. Any frames already
         queued will be sent first. If buf is not set then only queued
-        frames will be sent. Returns the number of pending frames that
-        could not be fully sent. If returned pending frames is greater
-        than 0, then the caller should call again when the socket is
-        ready. """
+        frames will be sent. Returns True if any frames could not be
+        fully sent, in which case the caller should call again when
+        the socket is ready. """
 
         tdelta = int(time.time()*1000) - self.start_time
 
         if bufs:
             for buf in bufs:
-                if self.base64:
-                    encbuf, lenhead, lentail = self.encode_hybi(buf, opcode=1, base64=True)
-                else:
-                    encbuf, lenhead, lentail = self.encode_hybi(buf, opcode=2, base64=False)
-
                 if self.rec:
-                    self.rec.write("%s,\n" %
-                            repr("{%s{" % tdelta
-                                + encbuf[lenhead:len(encbuf)-lentail]))
+                    # Python 3 compatible conversion
+                    bufstr = buf.decode('latin1').encode('unicode_escape').decode('ascii').replace("'", "\\'")
+                    self.rec.write("'{{{0}{{{1}',\n".format(tdelta, bufstr))
+                self.send_parts.append(buf)
 
-                self.send_parts.append(encbuf)
+        # Flush any previously queued data
+        try:
+            self.request.sendmsg('')
+        except WebSocketWantWriteError:
+            return True
 
         while self.send_parts:
             # Send pending frames
             buf = self.send_parts.pop(0)
-            sent = self.request.send(buf)
-
-            if sent == len(buf):
-                self.print_traffic("<")
-            else:
+            try:
+                self.request.sendmsg(buf)
+            except WebSocketWantWriteError:
                 self.print_traffic("<.")
-                self.send_parts.insert(0, buf[sent:])
-                break
+                return True
+            self.print_traffic("<")
 
-        return len(self.send_parts)
+        return False
 
     def recv_frames(self):
         """ Receive and decode WebSocket frames.
 
         Returns:
             (bufs_list, closed_string)
         """
 
         closed = False
         bufs = []
         tdelta = int(time.time()*1000) - self.start_time
 
-        buf = self.request.recv(self.buffer_size)
-        if len(buf) == 0:
-            closed = {'code': 1000, 'reason': "Client closed abruptly"}
-            return bufs, closed
-
-        if self.recv_part:
-            # Add partially received frames to current read buffer
-            buf = self.recv_part + buf
-            self.recv_part = None
-
-        while buf:
-            frame = self.decode_hybi(buf, base64=self.base64,
-                                     logger=self.logger,
-                                     strict=self.strict_mode)
-            #self.msg("Received buf: %s, frame: %s", repr(buf), frame)
-
-            if frame['payload'] == None:
-                # Incomplete/partial frame
+        while True:
+            try:
+                buf = self.request.recvmsg()
+            except WebSocketWantReadError:
                 self.print_traffic("}.")
-                if frame['left'] > 0:
-                    self.recv_part = buf[-frame['left']:]
                 break
-            else:
-                if frame['opcode'] == 0x8: # connection close
-                    closed = {'code': frame['close_code'],
-                              'reason': frame['close_reason']}
-                    break
-                elif self.auto_pong and frame['opcode'] == 0x9: # ping
-                    self.print_traffic("} ping %s\n" %
-                        repr(frame['payload']))
-                    self.send_pong(frame['payload'])
-                    return [], False
-                elif frame['opcode'] == 0xA: # pong
-                    self.print_traffic("} pong %s\n" %
-                        repr(frame['payload']))
-                    return [], False
+
+            if buf is None:
+                closed = {'code': self.request.close_code,
+                          'reason': self.request.close_reason}
+                return bufs, closed
 
             self.print_traffic("}")
 
             if self.rec:
-                start = frame['hlen']
-                end = frame['hlen'] + frame['length']
-                if frame['masked']:
-                    recbuf = WebSocketRequestHandler.unmask(buf, frame['hlen'],
-                                                   frame['length'])
-                else:
-                    recbuf = buf[frame['hlen']:frame['hlen'] +
-                                               frame['length']]
-                self.rec.write("%s,\n" %
-                        repr("}%s}" % tdelta + recbuf))
+                # Python 3 compatible conversion
+                bufstr = buf.decode('latin1').encode('unicode_escape').decode('ascii').replace("'", "\\'")
+                self.rec.write("'}}{0}}}{1}',\n".format(tdelta, bufstr))
 
+            bufs.append(buf)
 
-            bufs.append(frame['payload'])
-
-            if frame['left']:
-                buf = buf[-frame['left']:]
-            else:
-                buf = ''
+            if not self.request.pending():
+                break
 
         return bufs, closed
 
     def send_close(self, code=1000, reason=''):
         """ Send a WebSocket orderly close frame. """
+        self.request.shutdown(socket.SHUT_RDWR, code, reason)
 
-        msg = pack(">H%ds" % len(reason), code, s2b(reason))
-        buf, h, t = self.encode_hybi(msg, opcode=0x08, base64=False)
-        self.request.send(buf)
-
-    def send_pong(self, data=''):
+    def send_pong(self, data=''.encode('ascii')):
         """ Send a WebSocket pong frame. """
-        buf, h, t = self.encode_hybi(s2b(data), opcode=0x0A, base64=False)
-        self.request.send(buf)
+        self.request.pong(data)
 
-    def send_ping(self, data=''):
+    def send_ping(self, data=''.encode('ascii')):
         """ Send a WebSocket ping frame. """
-        buf, h, t = self.encode_hybi(s2b(data), opcode=0x09, base64=False)
-        self.request.send(buf)
-
-    def do_websocket_handshake(self):
-        h = self.headers
-
-        prot = 'WebSocket-Protocol'
-        protocols = h.get('Sec-'+prot, h.get(prot, '')).split(',')
-
-        ver = h.get('Sec-WebSocket-Version')
-        if ver:
-            # HyBi/IETF version of the protocol
-
-            # HyBi-07 report version 7
-            # HyBi-08 - HyBi-12 report version 8
-            # HyBi-13 reports version 13
-            if ver in ['7', '8', '13']:
-                self.version = "hybi-%02d" % int(ver)
-            else:
-                self.send_error(400, "Unsupported protocol version %s" % ver)
-                return False
+        self.request.ping(data)
 
-            key = h['Sec-WebSocket-Key']
+    def handle_upgrade(self):
+        # ensure connection is authorized, and determine the target
+        self.validate_connection()
+        self.auth_connection()
 
-            # Choose binary if client supports it
-            if 'binary' in protocols:
-                self.base64 = False
-            elif 'base64' in protocols:
-                self.base64 = True
-            else:
-                self.send_error(400, "Client must support 'binary' or 'base64' protocol")
-                return False
-
-            # Generate the hash value for the accept header
-            accept = b64encode(sha1(s2b(key + self.GUID)).digest())
-
-            self.send_response(101, "Switching Protocols")
-            self.send_header("Upgrade", "websocket")
-            self.send_header("Connection", "Upgrade")
-            self.send_header("Sec-WebSocket-Accept", b2s(accept))
-            if self.base64:
-                self.send_header("Sec-WebSocket-Protocol", "base64")
-            else:
-                self.send_header("Sec-WebSocket-Protocol", "binary")
-            self.end_headers()
-            return True
-        else:
-            self.send_error(400, "Missing Sec-WebSocket-Version header. Hixie protocols not supported.")
-
-        return False
+        WebSocketRequestHandlerMixIn.handle_upgrade(self)
 
     def handle_websocket(self):
-        """Upgrade a connection to Websocket, if requested. If this succeeds,
-        new_websocket_client() will be called. Otherwise, False is returned.
-        """
-
-        if (self.headers.get('upgrade') and
-            self.headers.get('upgrade').lower() == 'websocket'):
+        # Indicate to server that a Websocket upgrade was done
+        self.server.ws_connection = True
+        # Initialize per client settings
+        self.send_parts = []
+        self.recv_part  = None
+        self.start_time = int(time.time()*1000)
+
+        # client_address is empty with, say, UNIX domain sockets
+        client_addr = ""
+        is_ssl = False
+        try:
+            client_addr = self.client_address[0]
+            is_ssl = self.client_address[2]
+        except IndexError:
+            pass
 
-            # ensure connection is authorized, and determine the target
-            self.validate_connection()
+        if is_ssl:
+            self.stype = "SSL/TLS (wss://)"
+        else:
+            self.stype = "Plain non-SSL (ws://)"
 
-            if not self.do_websocket_handshake():
-                return False
+        self.log_message("%s: %s WebSocket connection", client_addr,
+                         self.stype)
+        if self.path != '/':
+            self.log_message("%s: Path: '%s'", client_addr, self.path)
 
-            # Indicate to server that a Websocket upgrade was done
-            self.server.ws_connection = True
-            # Initialize per client settings
-            self.send_parts = []
-            self.recv_part  = None
-            self.start_time = int(time.time()*1000)
-
-            # client_address is empty with, say, UNIX domain sockets
-            client_addr = ""
-            is_ssl = False
-            try:
-                client_addr = self.client_address[0]
-                is_ssl = self.client_address[2]
-            except IndexError:
-                pass
+        if self.record:
+            # Record raw frame data as JavaScript array
+            fname = "%s.%s" % (self.record,
+                               self.handler_id)
+            self.log_message("opening record file: %s", fname)
+            self.rec = open(fname, 'w+')
+            self.rec.write("var VNC_frame_data = [\n")
 
-            if is_ssl:
-                self.stype = "SSL/TLS (wss://)"
-            else:
-                self.stype = "Plain non-SSL (ws://)"
+        try:
+            self.new_websocket_client()
+        except self.CClose:
+            # Close the client
+            _, exc, _ = sys.exc_info()
+            self.send_close(exc.args[0], exc.args[1])
 
-            self.log_message("%s: %s WebSocket connection", client_addr,
-                             self.stype)
-            self.log_message("%s: Version %s, base64: '%s'", client_addr,
-                             self.version, self.base64)
-            if self.path != '/':
-                self.log_message("%s: Path: '%s'", client_addr, self.path)
-
-            if self.record:
-                # Record raw frame data as JavaScript array
-                fname = "%s.%s" % (self.record,
-                                   self.handler_id)
-                self.log_message("opening record file: %s", fname)
-                self.rec = open(fname, 'w+')
-                encoding = "binary"
-                if self.base64: encoding = "base64"
-                self.rec.write("var VNC_frame_encoding = '%s';\n"
-                               % encoding)
-                self.rec.write("var VNC_frame_data = [\n")
+    def do_GET(self):
+        if self.web_auth:
+            # ensure connection is authorized, this seems to apply to list_directory() as well
+            self.auth_connection()
 
-            try:
-                self.new_websocket_client()
-            except self.CClose:
-                # Close the client
-                _, exc, _ = sys.exc_info()
-                self.send_close(exc.args[0], exc.args[1])
-            return True
+        if self.only_upgrade:
+            self.send_error(405, "Method Not Allowed")
         else:
-            return False
-
-    def do_GET(self):
-        """Handle GET request. Calls handle_websocket(). If unsuccessful,
-        and web server is enabled, SimpleHTTPRequestHandler.do_GET will be called."""
-        if not self.handle_websocket():
-            if self.only_upgrade:
-                self.send_error(405, "Method Not Allowed")
-            else:
-                SimpleHTTPRequestHandler.do_GET(self)
+            SimpleHTTPRequestHandler.do_GET(self)
 
     def list_directory(self, path):
         if self.file_only:
             self.send_error(404, "No such file")
         else:
             return SimpleHTTPRequestHandler.list_directory(self, path)
 
     def new_websocket_client(self):
         """ Do something with a WebSockets client connection. """
         raise Exception("WebSocketRequestHandler.new_websocket_client() must be overloaded")
 
     def validate_connection(self):
-        """ Ensure that the connection is a valid connection, and set the target. """
+        """ Ensure that the connection has a valid token, and set the target. """
+        pass
+
+    def auth_connection(self):
+        """ Ensure that the connection is authorized. """
         pass
 
     def do_HEAD(self):
+        if self.web_auth:
+            self.auth_connection()
+
         if self.only_upgrade:
             self.send_error(405, "Method Not Allowed")
         else:
             SimpleHTTPRequestHandler.do_HEAD(self)
 
     def finish(self):
         if self.rec:
             self.rec.write("'EOF'];\n")
             self.rec.close()
+        SimpleHTTPRequestHandler.finish(self)
 
     def handle(self):
         # When using run_once, we have a single process, so
         # we cannot loop in BaseHTTPRequestHandler.handle; we
         # must return and handle new connections
         if self.run_once:
             self.handle_one_request()
@@ -581,15 +315,15 @@
             SimpleHTTPRequestHandler.handle(self)
 
     def log_request(self, code='-', size='-'):
         if self.verbose:
             SimpleHTTPRequestHandler.log_request(self, code, size)
 
 
-class WebSocketServer(object):
+class WebSockifyServer(object):
     """
     WebSockets server class.
     As an alternative, the standard library SocketServer can be used
     """
 
     policy_response = """<cross-domain-policy><allow-access-from domain="*" to-ports="*" /></cross-domain-policy>\n"""
     log_prefix = "websocket"
@@ -597,74 +331,87 @@
     # An exception before the WebSocket connection was established
     class EClose(Exception):
         pass
 
     class Terminate(Exception):
         pass
 
-    def __init__(self, RequestHandlerClass, listen_host='',
-                 listen_port=None, source_is_ipv6=False,
-            verbose=False, cert='', key='', ssl_only=None,
-            daemon=False, record='', web='',
+    def __init__(self, RequestHandlerClass, listen_fd=None,
+            listen_host='', listen_port=None, source_is_ipv6=False,
+            verbose=False, cert='', key='', key_password=None, ssl_only=None,
+            verify_client=False, cafile=None,
+            daemon=False, record='', web='', web_auth=False,
             file_only=False,
             run_once=False, timeout=0, idle_timeout=0, traffic=False,
             tcp_keepalive=True, tcp_keepcnt=None, tcp_keepidle=None,
-            tcp_keepintvl=None, auto_pong=False, strict_mode=True):
+            tcp_keepintvl=None, ssl_ciphers=None, ssl_options=0):
 
         # settings
         self.RequestHandlerClass = RequestHandlerClass
         self.verbose        = verbose
+        self.listen_fd      = listen_fd
         self.listen_host    = listen_host
         self.listen_port    = listen_port
         self.prefer_ipv6    = source_is_ipv6
         self.ssl_only       = ssl_only
+        self.ssl_ciphers    = ssl_ciphers
+        self.ssl_options    = ssl_options
+        self.verify_client  = verify_client
         self.daemon         = daemon
         self.run_once       = run_once
         self.timeout        = timeout
         self.idle_timeout   = idle_timeout
         self.traffic        = traffic
         self.file_only      = file_only
-        self.strict_mode    = strict_mode
+        self.web_auth       = web_auth
 
         self.launch_time    = time.time()
         self.ws_connection  = False
         self.handler_id     = 1
+        self.terminating    = False
 
         self.logger         = self.get_logger()
         self.tcp_keepalive  = tcp_keepalive
         self.tcp_keepcnt    = tcp_keepcnt
         self.tcp_keepidle   = tcp_keepidle
         self.tcp_keepintvl  = tcp_keepintvl
 
-        self.auto_pong      = auto_pong
+        # keyfile path must be None if not specified
+        self.key = None
+        self.key_password = key_password
+
         # Make paths settings absolute
         self.cert = os.path.abspath(cert)
-        self.key = self.web = self.record = ''
+        self.web = self.record = self.cafile = ''
         if key:
             self.key = os.path.abspath(key)
         if web:
             self.web = os.path.abspath(web)
         if record:
             self.record = os.path.abspath(record)
+        if cafile:
+            self.cafile = os.path.abspath(cafile)
 
         if self.web:
             os.chdir(self.web)
         self.only_upgrade = not self.web
 
         # Sanity checks
         if not ssl and self.ssl_only:
             raise Exception("No 'ssl' module and SSL-only specified")
         if self.daemon and not resource:
             raise Exception("Module 'resource' required to daemonize")
 
         # Show configuration
         self.msg("WebSocket server settings:")
-        self.msg("  - Listen on %s:%s",
-                self.listen_host, self.listen_port)
-        self.msg("  - Flash security policy server")
+        if self.listen_fd != None:
+            self.msg("  - Listen for inetd connections")
+        else:
+            self.msg("  - Listen on %s:%s",
+                    self.listen_host, self.listen_port)
         if self.web:
             if self.file_only:
                 self.msg("  - Web server (no directory listings). Web root: %s", self.web)
             else:
                 self.msg("  - Web server. Web root: %s", self.web)
         if ssl:
             if os.path.exists(self.cert):
@@ -677,22 +424,22 @@
             self.msg("  - No SSL/TLS support (no 'ssl' module)")
         if self.daemon:
             self.msg("  - Backgrounding (daemon)")
         if self.record:
             self.msg("  - Recording to '%s.*'", self.record)
 
     #
-    # WebSocketServer static methods
+    # WebSockifyServer static methods
     #
 
     @staticmethod
     def get_logger():
         return logging.getLogger("%s.%s" % (
-            WebSocketServer.log_prefix,
-            WebSocketServer.__class__.__name__))
+            WebSockifyServer.log_prefix,
+            WebSockifyServer.__class__.__name__))
 
     @staticmethod
     def socket(host, port=None, connect=False, prefer_ipv6=False,
                unix_socket=None, use_ssl=False, tcp_keepalive=True,
                tcp_keepcnt=None, tcp_keepidle=None, tcp_keepintvl=None):
         """ Resolve a host (and optional port) to an IPv4 or IPv6
         address. Create a socket. Bind to it if listen is set,
@@ -785,60 +532,72 @@
         os.dup2(os.open(os.devnull, os.O_RDWR), sys.stdout.fileno())
         os.dup2(os.open(os.devnull, os.O_RDWR), sys.stderr.fileno())
 
     def do_handshake(self, sock, address):
         """
         do_handshake does the following:
         - Peek at the first few bytes from the socket.
-        - If the connection is Flash policy request then answer it,
-          close the socket and return.
         - If the connection is an HTTPS/SSL/TLS connection then SSL
           wrap the socket.
         - Read from the (possibly wrapped) socket.
         - If we have received a HTTP GET request and the webserver
           functionality is enabled, answer it, close the socket and
           return.
         - Assume we have a WebSockets connection, parse the client
           handshake data.
         - Send a WebSockets handshake server response.
         - Return the socket for this WebSocket client.
         """
         ready = select.select([sock], [], [], 3)[0]
 
-
         if not ready:
-            raise self.EClose("ignoring socket not ready")
+            raise self.EClose("")
         # Peek, but do not read the data so that we have a opportunity
         # to SSL wrap the socket first
         handshake = sock.recv(1024, socket.MSG_PEEK)
         #self.msg("Handshake [%s]" % handshake)
 
         if not handshake:
-            raise self.EClose("ignoring empty handshake")
-
-        elif handshake.startswith(s2b("<policy-file-request/>")):
-            # Answer Flash policy request
-            handshake = sock.recv(1024)
-            sock.send(s2b(self.policy_response))
-            raise self.EClose("Sending flash policy response")
+            raise self.EClose("")
 
         elif handshake[0] in ("\x16", "\x80", 22, 128):
             # SSL wrap the connection
             if not ssl:
                 raise self.EClose("SSL connection but no 'ssl' module")
             if not os.path.exists(self.cert):
                 raise self.EClose("SSL connection but '%s' not found"
                                   % self.cert)
             retsock = None
             try:
-                retsock = ssl.wrap_socket(
-                        sock,
-                        server_side=True,
-                        certfile=self.cert,
-                        keyfile=self.key)
+                if (hasattr(ssl, 'create_default_context') 
+                    and callable(ssl.create_default_context)):
+                    # create new-style SSL wrapping for extended features
+                    context = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
+                    if self.ssl_ciphers is not None:
+                        context.set_ciphers(self.ssl_ciphers)
+                    context.options = self.ssl_options
+                    context.load_cert_chain(certfile=self.cert, keyfile=self.key, password=self.key_password)
+                    if self.verify_client:
+                        context.verify_mode = ssl.CERT_REQUIRED
+                        if self.cafile:
+                            context.load_verify_locations(cafile=self.cafile)
+                        else:
+                            context.set_default_verify_paths()
+                    retsock = context.wrap_socket(
+                            sock,
+                            server_side=True)
+                else:
+                    if self.verify_client:
+                        raise self.EClose("Client certificate verification requested, but this Python is too old.")
+                    # new-style SSL wrapping is not needed, using to old style
+                    retsock = ssl.wrap_socket(
+                            sock,
+                            server_side=True,
+                            certfile=self.cert,
+                            keyfile=self.key)
             except ssl.SSLError:
                 _, x, _ = sys.exc_info()
                 if x.args[0] == ssl.SSL_ERROR_EOF:
                     if len(x.args) > 1:
                         raise self.EClose(x.args[1])
                     else:
                         raise self.EClose("Got SSL_ERROR_EOF")
@@ -859,15 +618,15 @@
 
         self.RequestHandlerClass(retsock, address, self)
 
         # Return the WebSockets socket which may be SSL wrapped
         return retsock
 
     #
-    # WebSocketServer logging/output functions
+    # WebSockifyServer logging/output functions
     #
 
     def msg(self, *args, **kwargs):
         """ Output message as info """
         self.logger.log(logging.INFO, *args, **kwargs)
 
     def vmsg(self, *args, **kwargs):
@@ -888,15 +647,17 @@
 
     def poll(self):
         """ Run periodically while waiting for connections. """
         #self.vmsg("Running poll()")
         pass
 
     def terminate(self):
-        raise self.Terminate()
+        if not self.terminating:
+            self.terminating = True
+            raise self.Terminate()
 
     def multiprocessing_SIGCHLD(self, sig, stack):
         # TODO: figure out a way to actually log this information without
         #       calling `log` in the signal handlers
         multiprocessing.active_children()
 
     def fallback_SIGCHLD(self, sig, stack):
@@ -929,15 +690,15 @@
             try:
                 client = self.do_handshake(startsock, address)
             except self.EClose:
                 _, exc, _ = sys.exc_info()
                 # Connection was not a WebSockets connection
                 if exc.args[0]:
                     self.msg("%s: %s" % (address[0], exc.args[0]))
-            except WebSocketServer.Terminate:
+            except WebSockifyServer.Terminate:
                 raise
             except Exception:
                 _, exc, _ = sys.exc_info()
                 self.msg("handler exception: %s" % str(exc))
                 self.vmsg("exception", exc_info=True)
         finally:
 
@@ -961,56 +722,61 @@
     def start_server(self):
         """
         Daemonize if requested. Listen for for connections. Run
         do_handshake() method for each connection. If the connection
         is a WebSockets client then call new_websocket_client() method (which must
         be overridden) for each new client connection.
         """
-        lsock = self.socket(self.listen_host, self.listen_port, False,
-                            self.prefer_ipv6,
-                            tcp_keepalive=self.tcp_keepalive,
-                            tcp_keepcnt=self.tcp_keepcnt,
-                            tcp_keepidle=self.tcp_keepidle,
-                            tcp_keepintvl=self.tcp_keepintvl)
+
+        if self.listen_fd != None:
+            lsock = socket.fromfd(self.listen_fd, socket.AF_INET, socket.SOCK_STREAM)
+            if sys.hexversion < 0x3000000:
+                # For python 2 we have to wrap the "raw" socket into a socket object,
+                # otherwise ssl wrap_socket doesn't work.
+                lsock = socket.socket(_sock=lsock)
+        else:
+            lsock = self.socket(self.listen_host, self.listen_port, False,
+                                self.prefer_ipv6,
+                                tcp_keepalive=self.tcp_keepalive,
+                                tcp_keepcnt=self.tcp_keepcnt,
+                                tcp_keepidle=self.tcp_keepidle,
+                                tcp_keepintvl=self.tcp_keepintvl)
 
         if self.daemon:
             keepfd = self.get_log_fd()
             keepfd.append(lsock.fileno())
             self.daemonize(keepfd=keepfd, chdir=self.web)
 
         self.started()  # Some things need to happen after daemonizing
 
         # Allow override of signals
         original_signals = {
             signal.SIGINT: signal.getsignal(signal.SIGINT),
             signal.SIGTERM: signal.getsignal(signal.SIGTERM),
-            signal.SIGCHLD: signal.getsignal(signal.SIGCHLD),
         }
+        if getattr(signal, 'SIGCHLD', None) is not None:
+            original_signals[signal.SIGCHLD] = signal.getsignal(signal.SIGCHLD)
         signal.signal(signal.SIGINT, self.do_SIGINT)
         signal.signal(signal.SIGTERM, self.do_SIGTERM)
-        if not multiprocessing:
-            # os.fork() (python 2.4) child reaper
-            signal.signal(signal.SIGCHLD, self.fallback_SIGCHLD)
-        else:
-            # make sure that _cleanup is called when children die
-            # by calling active_children on SIGCHLD
+        # make sure that _cleanup is called when children die
+        # by calling active_children on SIGCHLD
+        if getattr(signal, 'SIGCHLD', None) is not None:
             signal.signal(signal.SIGCHLD, self.multiprocessing_SIGCHLD)
 
         last_active_time = self.launch_time
         try:
             while True:
                 try:
                     try:
                         startsock = None
                         pid = err = 0
                         child_count = 0
 
-                        if multiprocessing:
-                            # Collect zombie child processes
-                            child_count = len(multiprocessing.active_children())
+                        # Collect zombie child processes
+                        child_count = len(multiprocessing.active_children())
 
                         time_elapsed = time.time() - self.launch_time
                         if self.timeout and time_elapsed > self.timeout:
                             self.msg('listener exit due to --timeout %s'
                                     % self.timeout)
                             break
 
@@ -1054,37 +820,29 @@
                         if self.run_once:
                             # Run in same process if run_once
                             self.top_new_client(startsock, address)
                             if self.ws_connection :
                                 self.msg('%s: exiting due to --run-once'
                                         % address[0])
                                 break
-                        elif multiprocessing:
+                        else:
                             self.vmsg('%s: new handler Process' % address[0])
                             p = multiprocessing.Process(
                                     target=self.top_new_client,
                                     args=(startsock, address))
                             p.start()
                             # child will not return
-                        else:
-                            # python 2.4
-                            self.vmsg('%s: forking handler' % address[0])
-                            pid = os.fork()
-                            if pid == 0:
-                                # child handler process
-                                self.top_new_client(startsock, address)
-                                break  # child process exits
 
                         # parent process
                         self.handler_id += 1
 
                     except (self.Terminate, SystemExit, KeyboardInterrupt):
                         self.msg("In exit")
                         # terminate all child processes
-                        if multiprocessing and not self.run_once:
+                        if not self.run_once:
                             children = multiprocessing.active_children()
 
                             for child in children:
                                 self.msg("Terminating child %s" % child.pid)
                                 child.terminate()
 
                         break
```

### Comparing `websockify-0.8.0/websockify/websocketproxy.py` & `websockify-0.9.0/websockify/websocketproxy.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,29 +7,37 @@
 
 You can make a cert/key with openssl using:
 openssl req -new -x509 -days 365 -nodes -out self.pem -keyout self.pem
 as taken from http://docs.python.org/dev/library/ssl.html#certificates
 
 '''
 
-import signal, socket, optparse, time, os, sys, subprocess, logging, errno
-try:    from socketserver import ForkingMixIn
-except: from SocketServer import ForkingMixIn
-try:    from http.server import HTTPServer
-except: from BaseHTTPServer import HTTPServer
+import signal, socket, optparse, time, os, sys, subprocess, logging, errno, ssl
+try:
+    from socketserver import ThreadingMixIn
+except ImportError:
+    from SocketServer import ThreadingMixIn
+
+try:
+    from http.server import HTTPServer
+except ImportError:
+    from BaseHTTPServer import HTTPServer
+
 import select
-from websockify import websocket
+from websockify import websockifyserver
 from websockify import auth_plugins as auth
 try:
     from urllib.parse import parse_qs, urlparse
-except:
+except ImportError:
     from cgi import parse_qs
     from urlparse import urlparse
 
-class ProxyRequestHandler(websocket.WebSocketRequestHandler):
+class ProxyRequestHandler(websockifyserver.WebSockifyRequestHandler):
+
+    buffer_size = 65536
 
     traffic_legend = """
 Traffic Legend:
     }  - Client receive
     }. - Client receive partial
     {  - Target receive
 
@@ -44,26 +52,50 @@
         self.send_header('Content-Type', 'text/html')
         for name, val in ex.headers.items():
             self.send_header(name, val)
         
         self.end_headers()
     
     def validate_connection(self):
-        if self.server.token_plugin: 
-            (self.server.target_host, self.server.target_port) = self.get_target(self.server.token_plugin, self.path)
+        if not self.server.token_plugin:
+            return
 
-        if self.server.auth_plugin:
-            try:
-                self.server.auth_plugin.authenticate(
-                    headers=self.headers, target_host=self.server.target_host,
-                    target_port=self.server.target_port)
-            except auth.AuthenticationError:
-                ex = sys.exc_info()[1]
-                self.send_auth_error(ex)
-                raise
+        host, port = self.get_target(self.server.token_plugin)
+        if host == 'unix_socket':
+            self.server.unix_target = port
+
+        else:
+            self.server.target_host = host
+            self.server.target_port = port
+
+    def auth_connection(self):
+        if not self.server.auth_plugin:
+            return
+
+        try:
+            # get client certificate data
+            client_cert_data = self.request.getpeercert()
+            # extract subject information
+            client_cert_subject = client_cert_data['subject']
+            # flatten data structure
+            client_cert_subject = dict([x[0] for x in client_cert_subject])
+            # add common name to headers (apache +StdEnvVars style)
+            self.headers['SSL_CLIENT_S_DN_CN'] = client_cert_subject['commonName']
+        except (TypeError, AttributeError, KeyError):
+            # not a SSL connection or client presented no certificate with valid data
+            pass
+            
+        try:
+            self.server.auth_plugin.authenticate(
+                headers=self.headers, target_host=self.server.target_host,
+                target_port=self.server.target_port)
+        except auth.AuthenticationError:
+            ex = sys.exc_info()[1]
+            self.send_auth_error(ex)
+            raise
 
     def new_websocket_client(self):
         """
         Called after a new WebSocket connection has been established.
         """
         # Checking for a token is done in validate_connection()
 
@@ -76,48 +108,73 @@
             msg = "connecting to: %s:%s" % (
                                     self.server.target_host, self.server.target_port)
 
         if self.server.ssl_target:
             msg += " (using SSL)"
         self.log_message(msg)
 
-        tsock = websocket.WebSocketServer.socket(self.server.target_host,
-                                                 self.server.target_port,
-                connect=True, use_ssl=self.server.ssl_target, unix_socket=self.server.unix_target)
+        try:
+            tsock = websockifyserver.WebSockifyServer.socket(self.server.target_host,
+                                                           self.server.target_port,
+                                                           connect=True,
+                                                           use_ssl=self.server.ssl_target,
+                                                           unix_socket=self.server.unix_target)
+        except Exception:
+            self.log_message("Failed to connect to %s:%s",
+                             self.server.target_host, self.server.target_port)
+            raise self.CClose(1011, "Failed to connect to downstream server")
+
+        self.request.setsockopt(socket.SOL_TCP, socket.TCP_NODELAY, 1)
+        if not self.server.wrap_cmd and not self.server.unix_target:
+            tsock.setsockopt(socket.SOL_TCP, socket.TCP_NODELAY, 1)
 
         self.print_traffic(self.traffic_legend)
 
         # Start proxying
         try:
             self.do_proxy(tsock)
-        except:
+        finally:
             if tsock:
                 tsock.shutdown(socket.SHUT_RDWR)
                 tsock.close()
                 if self.verbose:
                     self.log_message("%s:%s: Closed target",
                             self.server.target_host, self.server.target_port)
-            raise
 
-    def get_target(self, target_plugin, path):
+    def get_target(self, target_plugin):
         """
-        Parses the path, extracts a token, and looks up a target
-        for that token using the token plugin. Sets
-        target_host and target_port if successful
+        Gets a token from either the path or the host,
+        depending on --host-token, and looks up a target
+        for that token using the token plugin. Used by
+        validate_connection() to set target_host and target_port.
         """
         # The files in targets contain the lines
         # in the form of token: host:port
 
-        # Extract the token parameter from url
-        args = parse_qs(urlparse(path)[4]) # 4 is the query from url
+        if self.host_token:
+            # Use hostname as token
+            token = self.headers.get('Host')
+
+            # Remove port from hostname, as it'll always be the one where
+            # websockify listens (unless something between the client and
+            # websockify is redirecting traffic, but that's beside the point)
+            if token:
+                token = token.partition(':')[0]
 
-        if not 'token' in args or not len(args['token']):
-            raise self.server.EClose("Token not present")
+        else:
+            # Extract the token parameter from url
+            args = parse_qs(urlparse(self.path)[4]) # 4 is the query from url
 
-        token = args['token'][0].rstrip('\n')
+            if 'token' in args and len(args['token']):
+                token = args['token'][0].rstrip('\n')
+            else:
+                token = None
+
+        if token is None:
+            raise self.server.EClose("Token not present")
 
         result_pair = target_plugin.lookup(token)
 
         if result_pair is not None:
             return result_pair
         else:
             raise self.server.EClose("Token '%s' not found" % token)
@@ -203,20 +260,18 @@
                         self.log_message("%s:%s: Target closed connection",
                                 self.server.target_host, self.server.target_port)
                     raise self.CClose(1000, "Target closed")
 
                 cqueue.append(buf)
                 self.print_traffic("{")
 
-class WebSocketProxy(websocket.WebSocketServer):
+class WebSocketProxy(websockifyserver.WebSockifyServer):
     """
     Proxy traffic to and from a WebSockets client to a normal TCP
-    socket server target. All traffic to/from the client is base64
-    encoded/decoded to allow binary data to be sent/received to/from
-    the target.
+    socket server target.
     """
 
     buffer_size = 65536
 
     def __init__(self, RequestHandlerClass=ProxyRequestHandler, *args, **kwargs):
         # Save off proxy specific options
         self.target_host    = kwargs.pop('target_host', None)
@@ -224,14 +279,15 @@
         self.wrap_cmd       = kwargs.pop('wrap_cmd', None)
         self.wrap_mode      = kwargs.pop('wrap_mode', None)
         self.unix_target    = kwargs.pop('unix_target', None)
         self.ssl_target     = kwargs.pop('ssl_target', None)
         self.heartbeat      = kwargs.pop('heartbeat', None)
 
         self.token_plugin = kwargs.pop('token_plugin', None)
+        self.host_token = kwargs.pop('host_token', None)
         self.auth_plugin = kwargs.pop('auth_plugin', None)
 
         # Last 3 timestamps command was run
         self.wrap_times    = [0, 0, 0]
 
         if self.wrap_cmd:
             wsdir = os.path.dirname(sys.argv[0])
@@ -258,15 +314,15 @@
             sock.close()
 
             os.environ.update({
                 "LD_PRELOAD": self.rebinder,
                 "REBIND_OLD_PORT": str(kwargs['listen_port']),
                 "REBIND_NEW_PORT": str(self.target_port)})
 
-        websocket.WebSocketServer.__init__(self, RequestHandlerClass, *args, **kwargs)
+        websockifyserver.WebSockifyServer.__init__(self, RequestHandlerClass, *args, **kwargs)
 
     def run_wrap_cmd(self):
         self.msg("Starting '%s'", " ".join(self.wrap_cmd))
         self.wrap_times.append(time.time())
         self.wrap_times.pop(0)
         self.cmd = subprocess.Popen(
                 self.wrap_cmd, env=os.environ, preexec_fn=_subprocess_setup)
@@ -281,20 +337,25 @@
         if self.wrap_cmd:
             dst_string = "'%s' (port %s)" % (" ".join(self.wrap_cmd), self.target_port)
         elif self.unix_target:
             dst_string = self.unix_target
         else:
             dst_string = "%s:%s" % (self.target_host, self.target_port)
 
+        if self.listen_fd != None:
+            src_string = "inetd"
+        else:
+            src_string = "%s:%s" % (self.listen_host, self.listen_port)
+
         if self.token_plugin:
-            msg = "  - proxying from %s:%s to targets generated by %s" % (
-                self.listen_host, self.listen_port, type(self.token_plugin).__name__)
+            msg = "  - proxying from %s to targets generated by %s" % (
+                src_string, type(self.token_plugin).__name__)
         else:
-            msg = "  - proxying from %s:%s to %s" % (
-                self.listen_host, self.listen_port, dst_string)
+            msg = "  - proxying from %s to %s" % (
+                src_string, dst_string)
 
         if self.ssl_target:
             msg += " (using SSL)"
 
         self.msg("%s", msg)
 
         if self.wrap_cmd:
@@ -329,27 +390,73 @@
 
 def _subprocess_setup():
     # Python installs a SIGPIPE handler by default. This is usually not what
     # non-Python successfulbprocesses expect.
     signal.signal(signal.SIGPIPE, signal.SIG_DFL)
 
 
-def logger_init():
-    logger = logging.getLogger(WebSocketProxy.log_prefix)
-    logger.propagate = False
-    logger.setLevel(logging.INFO)
-    h = logging.StreamHandler()
-    h.setLevel(logging.DEBUG)
-    h.setFormatter(logging.Formatter("%(message)s"))
-    logger.addHandler(h)
+try :
+    # First try SSL options for Python 3.4 and above
+    SSL_OPTIONS = {
+        'default': ssl.OP_ALL,
+        'tlsv1_1': ssl.PROTOCOL_TLS | ssl.OP_NO_SSLv2 | ssl.OP_NO_SSLv3 |
+        ssl.OP_NO_TLSv1,
+        'tlsv1_2': ssl.PROTOCOL_TLS | ssl.OP_NO_SSLv2 | ssl.OP_NO_SSLv3 |
+        ssl.OP_NO_TLSv1 | ssl.OP_NO_TLSv1_1,
+        'tlsv1_3': ssl.PROTOCOL_TLS | ssl.OP_NO_SSLv2 | ssl.OP_NO_SSLv3 |
+        ssl.OP_NO_TLSv1 | ssl.OP_NO_TLSv1_1 | ssl.OP_NO_TLSv1_2,
+    }
+except AttributeError:
+    try:
+        # Python 3.3 uses a different scheme for SSL options
+        # tlsv1_3 is not supported on older Python versions
+        SSL_OPTIONS = {
+            'default': ssl.OP_ALL,
+            'tlsv1_1': ssl.PROTOCOL_TLSv1 | ssl.OP_NO_SSLv2 | ssl.OP_NO_SSLv3 |
+            ssl.OP_NO_TLSv1,
+            'tlsv1_2': ssl.PROTOCOL_TLSv1 | ssl.OP_NO_SSLv2 | ssl.OP_NO_SSLv3 |
+            ssl.OP_NO_TLSv1 | ssl.OP_NO_TLSv1_1,
+        }
+    except AttributeError:
+        # Python 2.6 does not support TLS v1.2, and uses a different scheme
+        # for SSL options
+        SSL_OPTIONS = {
+            'default': ssl.PROTOCOL_SSLv23,
+            'tlsv1_1': ssl.PROTOCOL_TLSv1,
+        }
+
+def select_ssl_version(version):
+    """Returns SSL options for the most secure TSL version available on this
+    Python version"""
+    if version in SSL_OPTIONS:
+        return SSL_OPTIONS[version]
+    else:
+        # It so happens that version names sorted lexicographically form a list
+        # from the least to the most secure
+        keys = list(SSL_OPTIONS.keys())
+        keys.sort() 
+        fallback = keys[-1]
+        logger = logging.getLogger(WebSocketProxy.log_prefix)
+        logger.warn("TLS version %s unsupported. Falling back to %s",
+                    version, fallback)
 
+        return SSL_OPTIONS[fallback]
 
 def websockify_init():
-    logger_init()
+    # Setup basic logging to stderr.
+    logger = logging.getLogger(WebSocketProxy.log_prefix)
+    logger.propagate = False
+    logger.setLevel(logging.INFO)
+    stderr_handler = logging.StreamHandler()
+    stderr_handler.setLevel(logging.DEBUG)
+    log_formatter = logging.Formatter("%(message)s")
+    stderr_handler.setFormatter(log_formatter)
+    logger.addHandler(stderr_handler)
 
+    # Setup optparse.
     usage = "\n    %prog [options]"
     usage += " [source_addr:]source_port [target_addr:target_port]"
     usage += "\n    %prog [options]"
     usage += " [source_addr:]source_port -- WRAP_COMMAND_LINE"
     parser = optparse.OptionParser(usage=usage)
     parser.add_option("--verbose", "-v", action="store_true",
             help="verbose messages")
@@ -367,22 +474,41 @@
     parser.add_option("--idle-timeout", type=int, default=0,
             help="server exits after TIMEOUT seconds if there are no "
                  "active connections")
     parser.add_option("--cert", default="self.pem",
             help="SSL certificate file")
     parser.add_option("--key", default=None,
             help="SSL key file (if separate from cert)")
+    parser.add_option("--key-password", default=None,
+            help="SSL key password")
     parser.add_option("--ssl-only", action="store_true",
             help="disallow non-encrypted client connections")
     parser.add_option("--ssl-target", action="store_true",
             help="connect to SSL target as SSL client")
+    parser.add_option("--verify-client", action="store_true",
+            help="require encrypted client to present a valid certificate "
+            "(needs Python 2.7.9 or newer or Python 3.4 or newer)")
+    parser.add_option("--cafile", metavar="FILE",
+            help="file of concatenated certificates of authorities trusted "
+            "for validating clients (only effective with --verify-client). "
+            "If omitted, system default list of CAs is used.")
+    parser.add_option("--ssl-version", type="choice", default="default",
+            choices=["default", "tlsv1_1", "tlsv1_2", "tlsv1_3"], action="store",
+            help="minimum TLS version to use (default, tlsv1_1, tlsv1_2, tlsv1_3)")
+    parser.add_option("--ssl-ciphers", action="store",
+            help="list of ciphers allowed for connection. For a list of "
+            "supported ciphers run `openssl ciphers`")
     parser.add_option("--unix-target",
             help="connect to unix socket target", metavar="FILE")
+    parser.add_option("--inetd",
+            help="inetd mode, receive listening socket from stdin", action="store_true")
     parser.add_option("--web", default=None, metavar="DIR",
             help="run webserver on same port. Serve files from DIR.")
+    parser.add_option("--web-auth", action="store_true",
+            help="require authentication to access webserver.")
     parser.add_option("--wrap-mode", default="exit", metavar="MODE",
             choices=["exit", "ignore", "respawn"],
             help="action to take when the wrapped program exits "
             "or daemonizes: exit (default), ignore, respawn")
     parser.add_option("--prefer-ipv6", "-6",
             action="store_true", dest="source_is_ipv6",
             help="prefer IPv6 when resolving source_addr")
@@ -391,103 +517,178 @@
     parser.add_option("--target-config", metavar="FILE",
             dest="target_cfg",
             help="Configuration file containing valid targets "
             "in the form 'token: host:port' or, alternatively, a "
             "directory containing configuration files of this form "
             "(DEPRECATED: use `--token-plugin TokenFile --token-source "
             " path/to/token/file` instead)")
-    parser.add_option("--token-plugin", default=None, metavar="PLUGIN",
-                      help="use the given Python class to process tokens "
-                           "into host:port pairs")
+    parser.add_option("--token-plugin", default=None, metavar="CLASS",
+                      help="use a Python class, usually one from websockify.token_plugins, "
+                           "such as TokenFile, to process tokens into host:port pairs")
     parser.add_option("--token-source", default=None, metavar="ARG",
-                      help="an argument to be passed to the token plugin"
+                      help="an argument to be passed to the token plugin "
                            "on instantiation")
-    parser.add_option("--auth-plugin", default=None, metavar="PLUGIN",
-                      help="use the given Python class to determine if "
-                           "a connection is allowed")
+    parser.add_option("--host-token", action="store_true",
+                      help="use the host HTTP header as token instead of the "
+                           "token URL query parameter")
+    parser.add_option("--auth-plugin", default=None, metavar="CLASS",
+                      help="use a Python class, usually one from websockify.auth_plugins, "
+                           "such as BasicHTTPAuth, to determine if a connection is allowed")
     parser.add_option("--auth-source", default=None, metavar="ARG",
-                      help="an argument to be passed to the auth plugin"
+                      help="an argument to be passed to the auth plugin "
                            "on instantiation")
-    parser.add_option("--auto-pong", action="store_true",
-            help="Automatically respond to ping frames with a pong")
-    parser.add_option("--heartbeat", type=int, default=0,
-            help="send a ping to the client every HEARTBEAT seconds")
+    parser.add_option("--heartbeat", type=int, default=0, metavar="INTERVAL",
+            help="send a ping to the client every INTERVAL seconds")
     parser.add_option("--log-file", metavar="FILE",
             dest="log_file",
             help="File where logs will be saved")
-
+    parser.add_option("--syslog", default=None, metavar="SERVER",
+            help="Log to syslog server. SERVER can be local socket, "
+                 "such as /dev/log, or a UDP host:port pair.")
+    parser.add_option("--legacy-syslog", action="store_true",
+                      help="Use the old syslog protocol instead of RFC 5424. "
+                           "Use this if the messages produced by websockify seem abnormal.")
 
     (opts, args) = parser.parse_args()
 
-    if opts.log_file:
-        opts.log_file = os.path.abspath(opts.log_file)
-        handler = logging.FileHandler(opts.log_file)
-        handler.setLevel(logging.DEBUG)
-        handler.setFormatter(logging.Formatter("%(message)s"))
-        logging.getLogger(WebSocketProxy.log_prefix).addHandler(handler)
 
-    del opts.log_file
-
-    if opts.verbose:
-        logging.getLogger(WebSocketProxy.log_prefix).setLevel(logging.DEBUG)
+    # Validate options.
 
     if opts.token_source and not opts.token_plugin:
         parser.error("You must use --token-plugin to use --token-source")
 
+    if opts.host_token and not opts.token_plugin:
+        parser.error("You must use --token-plugin to use --host-token")
+
     if opts.auth_source and not opts.auth_plugin:
         parser.error("You must use --auth-plugin to use --auth-source")
 
+    if opts.web_auth and not opts.auth_plugin:
+        parser.error("You must use --auth-plugin to use --web-auth")
+
+    if opts.web_auth and not opts.web:
+        parser.error("You must use --web to use --web-auth")
+
+    if opts.legacy_syslog and not opts.syslog:
+        parser.error("You must use --syslog to use --legacy-syslog")
+
+
+    opts.ssl_options = select_ssl_version(opts.ssl_version)
+    del opts.ssl_version
+
+
+    if opts.log_file:
+        # Setup logging to user-specified file.
+        opts.log_file = os.path.abspath(opts.log_file)
+        log_file_handler = logging.FileHandler(opts.log_file)
+        log_file_handler.setLevel(logging.DEBUG)
+        log_file_handler.setFormatter(log_formatter)
+        logger.addHandler(log_file_handler)
+
+    del opts.log_file
+
+    if opts.syslog:
+        # Determine how to connect to syslog...
+        if opts.syslog.count(':'):
+            # User supplied a host:port pair.
+            syslog_host, syslog_port = opts.syslog.rsplit(':', 1)
+            try:
+                syslog_port = int(syslog_port)
+            except ValueError:
+                parser.error("Error parsing syslog port")
+            syslog_dest = (syslog_host, syslog_port)
+        else:
+            # User supplied a local socket file.
+            syslog_dest = os.path.abspath(opts.syslog)
+
+        from websockify.sysloghandler import WebsockifySysLogHandler
+
+        # Determine syslog facility.
+        if opts.daemon:
+            syslog_facility = WebsockifySysLogHandler.LOG_DAEMON
+        else:
+            syslog_facility = WebsockifySysLogHandler.LOG_USER
+
+        # Start logging to syslog.
+        syslog_handler = WebsockifySysLogHandler(address=syslog_dest,
+                                                 facility=syslog_facility,
+                                                 ident='websockify',
+                                                 legacy=opts.legacy_syslog)
+        syslog_handler.setLevel(logging.DEBUG)
+        syslog_handler.setFormatter(log_formatter)
+        logger.addHandler(syslog_handler)
+
+    del opts.syslog
+    del opts.legacy_syslog
+
+    if opts.verbose:
+        logger.setLevel(logging.DEBUG)
+
 
     # Transform to absolute path as daemon may chdir
     if opts.target_cfg:
         opts.target_cfg = os.path.abspath(opts.target_cfg)
 
     if opts.target_cfg:
         opts.token_plugin = 'TokenFile'
         opts.token_source = opts.target_cfg
 
     del opts.target_cfg
 
-    # Sanity checks
-    if len(args) < 2 and not (opts.token_plugin or opts.unix_target):
-        parser.error("Too few arguments")
     if sys.argv.count('--'):
         opts.wrap_cmd = args[1:]
     else:
         opts.wrap_cmd = None
-        if len(args) > 2:
-            parser.error("Too many arguments")
 
-    if not websocket.ssl and opts.ssl_target:
+    if not websockifyserver.ssl and opts.ssl_target:
         parser.error("SSL target requested and Python SSL module not loaded.");
 
     if opts.ssl_only and not os.path.exists(opts.cert):
         parser.error("SSL only and %s not found" % opts.cert)
 
-    # Parse host:port and convert ports to numbers
-    if args[0].count(':') > 0:
-        opts.listen_host, opts.listen_port = args[0].rsplit(':', 1)
-        opts.listen_host = opts.listen_host.strip('[]')
+    if opts.inetd:
+        opts.listen_fd = sys.stdin.fileno()
     else:
-        opts.listen_host, opts.listen_port = '', args[0]
+        if len(args) < 1:
+            parser.error("Too few arguments")
+        arg = args.pop(0)
+        # Parse host:port and convert ports to numbers
+        if arg.count(':') > 0:
+            opts.listen_host, opts.listen_port = arg.rsplit(':', 1)
+            opts.listen_host = opts.listen_host.strip('[]')
+        else:
+            opts.listen_host, opts.listen_port = '', arg
+
+        try:
+            opts.listen_port = int(opts.listen_port)
+        except ValueError:
+            parser.error("Error parsing listen port")
 
-    try:    opts.listen_port = int(opts.listen_port)
-    except: parser.error("Error parsing listen port")
+    del opts.inetd
 
     if opts.wrap_cmd or opts.unix_target or opts.token_plugin:
         opts.target_host = None
         opts.target_port = None
     else:
-        if args[1].count(':') > 0:
-            opts.target_host, opts.target_port = args[1].rsplit(':', 1)
+        if len(args) < 1:
+            parser.error("Too few arguments")
+        arg = args.pop(0)
+        if arg.count(':') > 0:
+            opts.target_host, opts.target_port = arg.rsplit(':', 1)
             opts.target_host = opts.target_host.strip('[]')
         else:
             parser.error("Error parsing target")
-        try:    opts.target_port = int(opts.target_port)
-        except: parser.error("Error parsing target port")
+
+        try:
+            opts.target_port = int(opts.target_port)
+        except ValueError:
+            parser.error("Error parsing target port")
+
+    if len(args) > 0 and opts.wrap_cmd == None:
+        parser.error("Too many arguments")
 
     if opts.token_plugin is not None:
         if '.' not in opts.token_plugin:
             opts.token_plugin = (
                 'websockify.token_plugins.%s' % opts.token_plugin)
 
         token_plugin_module, token_plugin_cls = opts.token_plugin.rsplit('.', 1)
@@ -521,15 +722,15 @@
         server.serve_forever()
     else:
         # Use internal service framework
         server = WebSocketProxy(**opts.__dict__)
         server.start_server()
 
 
-class LibProxyServer(ForkingMixIn, HTTPServer):
+class LibProxyServer(ThreadingMixIn, HTTPServer):
     """
     Just like WebSocketProxy, but uses standard Python SocketServer
     framework.
     """
 
     def __init__(self, RequestHandlerClass=ProxyRequestHandler, **kwargs):
         # Save off proxy specific options
@@ -570,12 +771,12 @@
         HTTPServer.__init__(self, (listen_host, listen_port),
                             RequestHandlerClass)
 
 
     def process_request(self, request, client_address):
         """Override process_request to implement a counter"""
         self.handler_id += 1
-        ForkingMixIn.process_request(self, request, client_address)
+        ThreadingMixIn.process_request(self, request, client_address)
 
 
 if __name__ == '__main__':
     websockify_init()
```

### Comparing `websockify-0.8.0/README.md` & `websockify-0.9.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ## websockify: WebSockets support for any application/server
 
 websockify was formerly named wsproxy and was part of the
-[noVNC](https://github.com/kanaka/noVNC) project.
+[noVNC](https://github.com/novnc/noVNC) project.
 
 At the most basic level, websockify just translates WebSockets traffic
 to normal socket traffic. Websockify accepts the WebSockets handshake,
 parses it, and then begins forwarding traffic between the client and
 the target in both directions.
 
 ### News/help/contact
@@ -15,38 +15,30 @@
 
 If you are a websockify developer/integrator/user (or want to be)
 please join the <a
 href="https://groups.google.com/forum/?fromgroups#!forum/novnc">noVNC/websockify
 discussion group</a>
 
 Bugs and feature requests can be submitted via [github
-issues](https://github.com/kanaka/websockify/issues).
+issues](https://github.com/novnc/websockify/issues).
 
 If you want to show appreciation for websockify you could donate to a great
 non-profits such as: [Compassion
 International](http://www.compassion.com/), [SIL](http://www.sil.org),
 [Habitat for Humanity](http://www.habitat.org), [Electronic Frontier
 Foundation](https://www.eff.org/), [Against Malaria
 Foundation](http://www.againstmalaria.com/), [Nothing But
 Nets](http://www.nothingbutnets.net/), etc. Please tweet <a
 href="http://www.twitter.com/noVNC">@noVNC</a> if you do.
 
 ### WebSockets binary data
 
 Starting with websockify 0.5.0, only the HyBi / IETF
-6455 WebSocket protocol is supported.
-
-Websockify negotiates whether to base64 encode traffic to and from the
-client via the subprotocol header (Sec-WebSocket-Protocol). The valid
-subprotocol values are 'binary' and 'base64' and if the client sends
-both then the server (the python implementation) will prefer 'binary'.
-The 'binary' subprotocol indicates that the data will be sent raw
-using binary WebSocket frames. Some HyBi clients (such as the Flash
-fallback and older Chrome and iOS versions) do not support binary data
-which is why the negotiation is necessary.
+6455 WebSocket protocol is supported. There is no support for the older
+Base64 encoded data format.
 
 
 ### Encrypted WebSocket connections (wss://)
 
 To encrypt the traffic using the WebSocket 'wss://' URI scheme you need to
 generate a certificate and key for Websockify to load. By default, Websockify
 loads a certificate file name `self.pem` but the `--cert=CERT` and `--key=KEY`
@@ -67,77 +59,66 @@
 
 If you have a commercial/valid SSL certificate with one ore more intermediate
 certificates, concat them into one file, server certificate first, then the
 intermediate(s) from the CA, etc. Point to this file with the `--cert` option
 and then also to the key with `--key`. Finally, use `--ssl-only` as needed.
 
 
-### Websock Javascript library
-
-
-The `include/websock.js` Javascript library library provides a Websock
-object that is similar to the standard WebSocket object but Websock
-enables communication with raw TCP sockets (i.e. the binary stream)
-via websockify. This is accomplished by base64 encoding the data
-stream between Websock and websockify.
-
-Websock has built-in receive queue buffering; the message event
-does not contain actual data but is simply a notification that
-there is new data available. Several rQ* methods are available to
-read binary data off of the receive queue.
-
-The Websock API is documented on the [websock.js API wiki page](https://github.com/kanaka/websockify/wiki/websock.js)
-
-See the "Wrap a Program" section below for an example of using Websock
-and websockify as a browser telnet client (`wstelnet.html`).
-
-
 ### Additional websockify features
 
 These are not necessary for the basic operation.
 
 * Daemonizing: When the `-D` option is specified, websockify runs
   in the background as a daemon process.
 
 * SSL (the wss:// WebSockets URI): This is detected automatically by
   websockify by sniffing the first byte sent from the client and then
   wrapping the socket if the data starts with '\x16' or '\x80'
   (indicating SSL).
 
-* Flash security policy: websockify detects flash security policy
-  requests (again by sniffing the first packet) and answers with an
-  appropriate flash security policy response (and then closes the
-  port). This means no separate flash security policy server is needed
-  for supporting the flash WebSockets fallback emulator.
-
 * Session recording: This feature that allows recording of the traffic
   sent and received from the client to a file using the `--record`
   option.
 
 * Mini-webserver: websockify can detect and respond to normal web
-  requests on the same port as the WebSockets proxy and Flash security
-  policy. This functionality is activated with the `--web DIR` option
-  where DIR is the root of the web directory to serve.
+  requests on the same port as the WebSockets proxy. This functionality
+  is activated with the `--web DIR` option where DIR is the root of the
+  web directory to serve.
 
 * Wrap a program: see the "Wrap a Program" section below.
 
 * Log files: websockify can save all logging information in a file.
   This functionality is activated with the `--log-file FILE` option
   where FILE is the file where the logs should be saved.
 
-### Implementations of websockify
+* Authentication plugins: websockify can demand authentication for
+  websocket connections and, if you use `--web-auth`, also for normal
+  web requests. This functionality is activated with the
+  `--auth-plugin CLASS` and `--auth-source ARG` options, where CLASS is
+  usually one from auth_plugins.py and ARG is the plugin's configuration.
+
+* Token plugins: a single instance of websockify can connect clients to
+  multiple different pre-configured targets, depending on the token sent
+  by the client using the `token` URL parameter, or the hostname used to
+  reach websockify, if you use `--host-token`. This functionality is
+  activated with the `--token-plugin CLASS` and `--token-source ARG`
+  options, where CLASS is usually one from token_plugins.py and ARG is
+  the plugin's configuration.
+
+### Other implementations of websockify
 
 The primary implementation of websockify is in python. There are
-several alternate implementations in other languages (C, Node.js,
-Clojure, Ruby) in the `other/` subdirectory (with varying levels of
-functionality).
+several alternate implementations in other languages available in
+our sister repositories [websockify-js](https://github.com/novnc/websockify-js)
+(JavaScript/Node.js) and [websockify-other](https://github.com/novnc/websockify-other)
+ (C, Clojure, Ruby).
 
 In addition there are several other external projects that implement
 the websockify "protocol". See the alternate implementation [Feature
-Matrix](https://github.com/kanaka/websockify/wiki/Feature_Matrix) for
+Matrix](https://github.com/novnc/websockify/wiki/Feature_Matrix) for
 more information.
 
 
 ### Wrap a Program
 
 In addition to proxying from a source address to a target address
 (which may be on a different system), websockify has the ability to
@@ -156,43 +137,34 @@
     `./run 2023 -- PROGRAM ARGS`
 
 The `--wrap-mode` option can be used to indicate what action to take
 when the wrapped program exits or daemonizes.
 
 Here is an example of using websockify to wrap the vncserver command
 (which backgrounds itself) for use with
-[noVNC](https://github.com/kanaka/noVNC):
+[noVNC](https://github.com/novnc/noVNC):
 
     `./run 5901 --wrap-mode=ignore -- vncserver -geometry 1024x768 :1`
 
 Here is an example of wrapping telnetd (from krb5-telnetd). telnetd
 exits after the connection closes so the wrap mode is set to respawn
 the command:
 
     `sudo ./run 2023 --wrap-mode=respawn -- telnetd -debug 2023`
 
-The `wstelnet.html` page demonstrates a simple WebSockets based telnet
-client (use 'localhost' and '2023' for the host and port
-respectively).
-
-
-### Building the Python ssl module (for python 2.5 and older)
-
-* Install the build dependencies. On Ubuntu use this command:
-
-    `sudo aptitude install python-dev bluetooth-dev`
-
-* At the top level of the websockify repostory, download, build and
-  symlink the ssl module:
-
-    `wget --no-check-certificate http://pypi.python.org/packages/source/s/ssl/ssl-1.15.tar.gz`
-
-    `tar xvzf ssl-1.15.tar.gz`
-
-    `cd ssl-1.15`
-
-    `make`
-
-    `cd ../`
-
-    `ln -sf ssl-1.15/build/lib.linux-*/ssl ssl`
+The `wstelnet.html` page in the [websockify-js](https://github.com/novnc/websockify-js)
+project demonstrates a simple WebSockets based telnet client (use
+'localhost' and '2023' for the host and port respectively).
+
+
+### Installing websockify
+
+Download one of the releases or the latest development version, extract
+it and run `python setup.py install` as root in the directory where you
+extracted the files. Normally, this will also install numpy for better
+performance, if you don't have it installed already. However, numpy is
+optional. If you don't want to install numpy or if you can't compile it,
+you can edit setup.py and remove the `install_requires=['numpy'],` line
+before running `python setup.py install`.
 
+Afterwards, websockify should be available in your path. Run
+`websockify --help` to confirm it's installed correctly.
```

#### html2text {}

```diff
@@ -1,100 +1,93 @@
 ## websockify: WebSockets support for any application/server websockify was
-formerly named wsproxy and was part of the [noVNC](https://github.com/kanaka/
+formerly named wsproxy and was part of the [noVNC](https://github.com/novnc/
 noVNC) project. At the most basic level, websockify just translates WebSockets
 traffic to normal socket traffic. Websockify accepts the WebSockets handshake,
 parses it, and then begins forwarding traffic between the client and the target
 in both directions. ### News/help/contact Notable commits, announcements and
 news are posted to _@_n_o_V_N_C If you are a websockify developer/integrator/user (or
 want to be) please join the _n_o_V_N_C_/_w_e_b_s_o_c_k_i_f_y_ _d_i_s_c_u_s_s_i_o_n_ _g_r_o_u_p Bugs and feature
-requests can be submitted via [github issues](https://github.com/kanaka/
+requests can be submitted via [github issues](https://github.com/novnc/
 websockify/issues). If you want to show appreciation for websockify you could
 donate to a great non-profits such as: [Compassion International](http://
 www.compassion.com/), [SIL](http://www.sil.org), [Habitat for Humanity](http://
 www.habitat.org), [Electronic Frontier Foundation](https://www.eff.org/),
 [Against Malaria Foundation](http://www.againstmalaria.com/), [Nothing But
 Nets](http://www.nothingbutnets.net/), etc. Please tweet _@_n_o_V_N_C if you do. ###
 WebSockets binary data Starting with websockify 0.5.0, only the HyBi / IETF
-6455 WebSocket protocol is supported. Websockify negotiates whether to base64
-encode traffic to and from the client via the subprotocol header (Sec-
-WebSocket-Protocol). The valid subprotocol values are 'binary' and 'base64' and
-if the client sends both then the server (the python implementation) will
-prefer 'binary'. The 'binary' subprotocol indicates that the data will be sent
-raw using binary WebSocket frames. Some HyBi clients (such as the Flash
-fallback and older Chrome and iOS versions) do not support binary data which is
-why the negotiation is necessary. ### Encrypted WebSocket connections (wss://
-) To encrypt the traffic using the WebSocket 'wss://' URI scheme you need to
-generate a certificate and key for Websockify to load. By default, Websockify
-loads a certificate file name `self.pem` but the `--cert=CERT` and `--key=KEY`
-options can override the file name. You can generate a self-signed certificate
-using openssl. When asked for the common name, use the hostname of the server
-where the proxy will be running: ``` openssl req -new -x509 -days 365 -nodes -
-out self.pem -keyout self.pem ``` For a self-signed certificate to work, you
-need to make your client/browser understand it. You can do this by installing
-it as accepted certificate, or by using that same certificate for a HTTPS
-connection to which you navigate first and approve. Browsers generally don't
-give you the "trust certificate?" prompt by opening a WSS socket with invalid
-certificate, hence you need to have it acccept it by either of those two
-methods. If you have a commercial/valid SSL certificate with one ore more
-intermediate certificates, concat them into one file, server certificate first,
-then the intermediate(s) from the CA, etc. Point to this file with the `--cert`
-option and then also to the key with `--key`. Finally, use `--ssl-only` as
-needed. ### Websock Javascript library The `include/websock.js` Javascript
-library library provides a Websock object that is similar to the standard
-WebSocket object but Websock enables communication with raw TCP sockets (i.e.
-the binary stream) via websockify. This is accomplished by base64 encoding the
-data stream between Websock and websockify. Websock has built-in receive queue
-buffering; the message event does not contain actual data but is simply a
-notification that there is new data available. Several rQ* methods are
-available to read binary data off of the receive queue. The Websock API is
-documented on the [websock.js API wiki page](https://github.com/kanaka/
-websockify/wiki/websock.js) See the "Wrap a Program" section below for an
-example of using Websock and websockify as a browser telnet client
-(`wstelnet.html`). ### Additional websockify features These are not necessary
-for the basic operation. * Daemonizing: When the `-D` option is specified,
-websockify runs in the background as a daemon process. * SSL (the wss:/
-/ WebSockets URI): This is detected automatically by websockify by sniffing the
-first byte sent from the client and then wrapping the socket if the data starts
-with '\x16' or '\x80' (indicating SSL). * Flash security policy: websockify
-detects flash security policy requests (again by sniffing the first packet) and
-answers with an appropriate flash security policy response (and then closes the
-port). This means no separate flash security policy server is needed for
-supporting the flash WebSockets fallback emulator. * Session recording: This
-feature that allows recording of the traffic sent and received from the client
-to a file using the `--record` option. * Mini-webserver: websockify can detect
-and respond to normal web requests on the same port as the WebSockets proxy and
-Flash security policy. This functionality is activated with the `--web DIR`
-option where DIR is the root of the web directory to serve. * Wrap a program:
-see the "Wrap a Program" section below. * Log files: websockify can save all
-logging information in a file. This functionality is activated with the `--log-
-file FILE` option where FILE is the file where the logs should be saved. ###
-Implementations of websockify The primary implementation of websockify is in
-python. There are several alternate implementations in other languages (C,
-Node.js, Clojure, Ruby) in the `other/` subdirectory (with varying levels of
-functionality). In addition there are several other external projects that
-implement the websockify "protocol". See the alternate implementation [Feature
-Matrix](https://github.com/kanaka/websockify/wiki/Feature_Matrix) for more
-information. ### Wrap a Program In addition to proxying from a source address
-to a target address (which may be on a different system), websockify has the
-ability to launch a program on the local system and proxy WebSockets traffic to
-a normal TCP port owned/bound by the program. The is accomplished with a small
+6455 WebSocket protocol is supported. There is no support for the older Base64
+encoded data format. ### Encrypted WebSocket connections (wss://) To encrypt
+the traffic using the WebSocket 'wss://' URI scheme you need to generate a
+certificate and key for Websockify to load. By default, Websockify loads a
+certificate file name `self.pem` but the `--cert=CERT` and `--key=KEY` options
+can override the file name. You can generate a self-signed certificate using
+openssl. When asked for the common name, use the hostname of the server where
+the proxy will be running: ``` openssl req -new -x509 -days 365 -nodes -out
+self.pem -keyout self.pem ``` For a self-signed certificate to work, you need
+to make your client/browser understand it. You can do this by installing it as
+accepted certificate, or by using that same certificate for a HTTPS connection
+to which you navigate first and approve. Browsers generally don't give you the
+"trust certificate?" prompt by opening a WSS socket with invalid certificate,
+hence you need to have it acccept it by either of those two methods. If you
+have a commercial/valid SSL certificate with one ore more intermediate
+certificates, concat them into one file, server certificate first, then the
+intermediate(s) from the CA, etc. Point to this file with the `--cert` option
+and then also to the key with `--key`. Finally, use `--ssl-only` as needed. ###
+Additional websockify features These are not necessary for the basic operation.
+* Daemonizing: When the `-D` option is specified, websockify runs in the
+background as a daemon process. * SSL (the wss:// WebSockets URI): This is
+detected automatically by websockify by sniffing the first byte sent from the
+client and then wrapping the socket if the data starts with '\x16' or '\x80'
+(indicating SSL). * Session recording: This feature that allows recording of
+the traffic sent and received from the client to a file using the `--record`
+option. * Mini-webserver: websockify can detect and respond to normal web
+requests on the same port as the WebSockets proxy. This functionality is
+activated with the `--web DIR` option where DIR is the root of the web
+directory to serve. * Wrap a program: see the "Wrap a Program" section below. *
+Log files: websockify can save all logging information in a file. This
+functionality is activated with the `--log-file FILE` option where FILE is the
+file where the logs should be saved. * Authentication plugins: websockify can
+demand authentication for websocket connections and, if you use `--web-auth`,
+also for normal web requests. This functionality is activated with the `--auth-
+plugin CLASS` and `--auth-source ARG` options, where CLASS is usually one from
+auth_plugins.py and ARG is the plugin's configuration. * Token plugins: a
+single instance of websockify can connect clients to multiple different pre-
+configured targets, depending on the token sent by the client using the `token`
+URL parameter, or the hostname used to reach websockify, if you use `--host-
+token`. This functionality is activated with the `--token-plugin CLASS` and `--
+token-source ARG` options, where CLASS is usually one from token_plugins.py and
+ARG is the plugin's configuration. ### Other implementations of websockify The
+primary implementation of websockify is in python. There are several alternate
+implementations in other languages available in our sister repositories
+[websockify-js](https://github.com/novnc/websockify-js) (JavaScript/Node.js)
+and [websockify-other](https://github.com/novnc/websockify-other) (C, Clojure,
+Ruby). In addition there are several other external projects that implement the
+websockify "protocol". See the alternate implementation [Feature Matrix](https:
+//github.com/novnc/websockify/wiki/Feature_Matrix) for more information. ###
+Wrap a Program In addition to proxying from a source address to a target
+address (which may be on a different system), websockify has the ability to
+launch a program on the local system and proxy WebSockets traffic to a normal
+TCP port owned/bound by the program. The is accomplished with a small
 LD_PRELOAD library (`rebind.so`) which intercepts bind() system calls by the
 program. The specified port is moved to a new localhost/loopback free high
 port. websockify then proxies WebSockets traffic directed to the original port
 to the new (moved) port of the program. The program wrap mode is invoked by
 replacing the target with `--` followed by the program command line to wrap.
 `./run 2023 -- PROGRAM ARGS` The `--wrap-mode` option can be used to indicate
 what action to take when the wrapped program exits or daemonizes. Here is an
 example of using websockify to wrap the vncserver command (which backgrounds
-itself) for use with [noVNC](https://github.com/kanaka/noVNC): `./run 5901 --
+itself) for use with [noVNC](https://github.com/novnc/noVNC): `./run 5901 --
 wrap-mode=ignore -- vncserver -geometry 1024x768 :1` Here is an example of
 wrapping telnetd (from krb5-telnetd). telnetd exits after the connection closes
 so the wrap mode is set to respawn the command: `sudo ./run 2023 --wrap-
-mode=respawn -- telnetd -debug 2023` The `wstelnet.html` page demonstrates a
+mode=respawn -- telnetd -debug 2023` The `wstelnet.html` page in the
+[websockify-js](https://github.com/novnc/websockify-js) project demonstrates a
 simple WebSockets based telnet client (use 'localhost' and '2023' for the host
-and port respectively). ### Building the Python ssl module (for python 2.5 and
-older) * Install the build dependencies. On Ubuntu use this command: `sudo
-aptitude install python-dev bluetooth-dev` * At the top level of the websockify
-repostory, download, build and symlink the ssl module: `wget --no-check-
-certificate http://pypi.python.org/packages/source/s/ssl/ssl-1.15.tar.gz` `tar
-xvzf ssl-1.15.tar.gz` `cd ssl-1.15` `make` `cd ../` `ln -sf ssl-1.15/build/
-lib.linux-*/ssl ssl`
+and port respectively). ### Installing websockify Download one of the releases
+or the latest development version, extract it and run `python setup.py install`
+as root in the directory where you extracted the files. Normally, this will
+also install numpy for better performance, if you don't have it installed
+already. However, numpy is optional. If you don't want to install numpy or if
+you can't compile it, you can edit setup.py and remove the `install_requires=
+['numpy'],` line before running `python setup.py install`. Afterwards,
+websockify should be available in your path. Run `websockify --help` to confirm
+it's installed correctly.
```

### Comparing `websockify-0.8.0/CHANGES.txt` & `websockify-0.9.0/CHANGES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,27 @@
 Changes
 =======
 
+0.9.0
+-----
+
+* Base64 support removed and binary mode is now required
+* Low level WebSocket protocol handling now has its own class
+* Authentication now optionally required for web server
+* Server hostname can be used as the token
+* JWT/JWS/JWE can be used for the token
+* redis can be used for the token
+* Can now log to syslog
+* Improved latency by disabling Nagle for proxied connection
+* Added client certificate authentication
+* Support for password protected certificate key file
+* TLS ciphers and options are now configurable
+* Can be invoked via inetd
+* Lots of minor fixes...
+
 0.8.0
 -----
 
 * Make websockify properly terminate children on SIGTERM (#226)
 * Remove logging in signal handlers (this can cause Python to hang under certain conditions) (#219)
 * Make it easier to log to a file (#205)
 * Add support for IPv6 addresses in tokens in the TokenFile token plugins (#197)
```

### Comparing `websockify-0.8.0/websockify.egg-info/PKG-INFO` & `websockify-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: websockify
-Version: 0.8.0
+Version: 0.9.0
 Summary: Websockify.
-Home-page: https://github.com/kanaka/websockify
+Home-page: https://github.com/novnc/websockify
 Author: Joel Martin
 Author-email: github@martintribe.org
 License: LGPLv3
 Description: ## websockify: WebSockets support for any application/server
         
         websockify was formerly named wsproxy and was part of the
-        [noVNC](https://github.com/kanaka/noVNC) project.
+        [noVNC](https://github.com/novnc/noVNC) project.
         
         At the most basic level, websockify just translates WebSockets traffic
         to normal socket traffic. Websockify accepts the WebSockets handshake,
         parses it, and then begins forwarding traffic between the client and
         the target in both directions.
         
         ### News/help/contact
@@ -23,38 +23,30 @@
         
         If you are a websockify developer/integrator/user (or want to be)
         please join the <a
         href="https://groups.google.com/forum/?fromgroups#!forum/novnc">noVNC/websockify
         discussion group</a>
         
         Bugs and feature requests can be submitted via [github
-        issues](https://github.com/kanaka/websockify/issues).
+        issues](https://github.com/novnc/websockify/issues).
         
         If you want to show appreciation for websockify you could donate to a great
         non-profits such as: [Compassion
         International](http://www.compassion.com/), [SIL](http://www.sil.org),
         [Habitat for Humanity](http://www.habitat.org), [Electronic Frontier
         Foundation](https://www.eff.org/), [Against Malaria
         Foundation](http://www.againstmalaria.com/), [Nothing But
         Nets](http://www.nothingbutnets.net/), etc. Please tweet <a
         href="http://www.twitter.com/noVNC">@noVNC</a> if you do.
         
         ### WebSockets binary data
         
         Starting with websockify 0.5.0, only the HyBi / IETF
-        6455 WebSocket protocol is supported.
-        
-        Websockify negotiates whether to base64 encode traffic to and from the
-        client via the subprotocol header (Sec-WebSocket-Protocol). The valid
-        subprotocol values are 'binary' and 'base64' and if the client sends
-        both then the server (the python implementation) will prefer 'binary'.
-        The 'binary' subprotocol indicates that the data will be sent raw
-        using binary WebSocket frames. Some HyBi clients (such as the Flash
-        fallback and older Chrome and iOS versions) do not support binary data
-        which is why the negotiation is necessary.
+        6455 WebSocket protocol is supported. There is no support for the older
+        Base64 encoded data format.
         
         
         ### Encrypted WebSocket connections (wss://)
         
         To encrypt the traffic using the WebSocket 'wss://' URI scheme you need to
         generate a certificate and key for Websockify to load. By default, Websockify
         loads a certificate file name `self.pem` but the `--cert=CERT` and `--key=KEY`
@@ -75,77 +67,66 @@
         
         If you have a commercial/valid SSL certificate with one ore more intermediate
         certificates, concat them into one file, server certificate first, then the
         intermediate(s) from the CA, etc. Point to this file with the `--cert` option
         and then also to the key with `--key`. Finally, use `--ssl-only` as needed.
         
         
-        ### Websock Javascript library
-        
-        
-        The `include/websock.js` Javascript library library provides a Websock
-        object that is similar to the standard WebSocket object but Websock
-        enables communication with raw TCP sockets (i.e. the binary stream)
-        via websockify. This is accomplished by base64 encoding the data
-        stream between Websock and websockify.
-        
-        Websock has built-in receive queue buffering; the message event
-        does not contain actual data but is simply a notification that
-        there is new data available. Several rQ* methods are available to
-        read binary data off of the receive queue.
-        
-        The Websock API is documented on the [websock.js API wiki page](https://github.com/kanaka/websockify/wiki/websock.js)
-        
-        See the "Wrap a Program" section below for an example of using Websock
-        and websockify as a browser telnet client (`wstelnet.html`).
-        
-        
         ### Additional websockify features
         
         These are not necessary for the basic operation.
         
         * Daemonizing: When the `-D` option is specified, websockify runs
           in the background as a daemon process.
         
         * SSL (the wss:// WebSockets URI): This is detected automatically by
           websockify by sniffing the first byte sent from the client and then
           wrapping the socket if the data starts with '\x16' or '\x80'
           (indicating SSL).
         
-        * Flash security policy: websockify detects flash security policy
-          requests (again by sniffing the first packet) and answers with an
-          appropriate flash security policy response (and then closes the
-          port). This means no separate flash security policy server is needed
-          for supporting the flash WebSockets fallback emulator.
-        
         * Session recording: This feature that allows recording of the traffic
           sent and received from the client to a file using the `--record`
           option.
         
         * Mini-webserver: websockify can detect and respond to normal web
-          requests on the same port as the WebSockets proxy and Flash security
-          policy. This functionality is activated with the `--web DIR` option
-          where DIR is the root of the web directory to serve.
+          requests on the same port as the WebSockets proxy. This functionality
+          is activated with the `--web DIR` option where DIR is the root of the
+          web directory to serve.
         
         * Wrap a program: see the "Wrap a Program" section below.
         
         * Log files: websockify can save all logging information in a file.
           This functionality is activated with the `--log-file FILE` option
           where FILE is the file where the logs should be saved.
         
-        ### Implementations of websockify
+        * Authentication plugins: websockify can demand authentication for
+          websocket connections and, if you use `--web-auth`, also for normal
+          web requests. This functionality is activated with the
+          `--auth-plugin CLASS` and `--auth-source ARG` options, where CLASS is
+          usually one from auth_plugins.py and ARG is the plugin's configuration.
+        
+        * Token plugins: a single instance of websockify can connect clients to
+          multiple different pre-configured targets, depending on the token sent
+          by the client using the `token` URL parameter, or the hostname used to
+          reach websockify, if you use `--host-token`. This functionality is
+          activated with the `--token-plugin CLASS` and `--token-source ARG`
+          options, where CLASS is usually one from token_plugins.py and ARG is
+          the plugin's configuration.
+        
+        ### Other implementations of websockify
         
         The primary implementation of websockify is in python. There are
-        several alternate implementations in other languages (C, Node.js,
-        Clojure, Ruby) in the `other/` subdirectory (with varying levels of
-        functionality).
+        several alternate implementations in other languages available in
+        our sister repositories [websockify-js](https://github.com/novnc/websockify-js)
+        (JavaScript/Node.js) and [websockify-other](https://github.com/novnc/websockify-other)
+         (C, Clojure, Ruby).
         
         In addition there are several other external projects that implement
         the websockify "protocol". See the alternate implementation [Feature
-        Matrix](https://github.com/kanaka/websockify/wiki/Feature_Matrix) for
+        Matrix](https://github.com/novnc/websockify/wiki/Feature_Matrix) for
         more information.
         
         
         ### Wrap a Program
         
         In addition to proxying from a source address to a target address
         (which may be on a different system), websockify has the ability to
@@ -164,54 +145,62 @@
             `./run 2023 -- PROGRAM ARGS`
         
         The `--wrap-mode` option can be used to indicate what action to take
         when the wrapped program exits or daemonizes.
         
         Here is an example of using websockify to wrap the vncserver command
         (which backgrounds itself) for use with
-        [noVNC](https://github.com/kanaka/noVNC):
+        [noVNC](https://github.com/novnc/noVNC):
         
             `./run 5901 --wrap-mode=ignore -- vncserver -geometry 1024x768 :1`
         
         Here is an example of wrapping telnetd (from krb5-telnetd). telnetd
         exits after the connection closes so the wrap mode is set to respawn
         the command:
         
             `sudo ./run 2023 --wrap-mode=respawn -- telnetd -debug 2023`
         
-        The `wstelnet.html` page demonstrates a simple WebSockets based telnet
-        client (use 'localhost' and '2023' for the host and port
-        respectively).
-        
-        
-        ### Building the Python ssl module (for python 2.5 and older)
-        
-        * Install the build dependencies. On Ubuntu use this command:
-        
-            `sudo aptitude install python-dev bluetooth-dev`
-        
-        * At the top level of the websockify repostory, download, build and
-          symlink the ssl module:
-        
-            `wget --no-check-certificate http://pypi.python.org/packages/source/s/ssl/ssl-1.15.tar.gz`
-        
-            `tar xvzf ssl-1.15.tar.gz`
-        
-            `cd ssl-1.15`
-        
-            `make`
-        
-            `cd ../`
-        
-            `ln -sf ssl-1.15/build/lib.linux-*/ssl ssl`
+        The `wstelnet.html` page in the [websockify-js](https://github.com/novnc/websockify-js)
+        project demonstrates a simple WebSockets based telnet client (use
+        'localhost' and '2023' for the host and port respectively).
+        
+        
+        ### Installing websockify
+        
+        Download one of the releases or the latest development version, extract
+        it and run `python setup.py install` as root in the directory where you
+        extracted the files. Normally, this will also install numpy for better
+        performance, if you don't have it installed already. However, numpy is
+        optional. If you don't want to install numpy or if you can't compile it,
+        you can edit setup.py and remove the `install_requires=['numpy'],` line
+        before running `python setup.py install`.
         
+        Afterwards, websockify should be available in your path. Run
+        `websockify --help` to confirm it's installed correctly.
         
         Changes
         =======
         
+        0.9.0
+        -----
+        
+        * Base64 support removed and binary mode is now required
+        * Low level WebSocket protocol handling now has its own class
+        * Authentication now optionally required for web server
+        * Server hostname can be used as the token
+        * JWT/JWS/JWE can be used for the token
+        * redis can be used for the token
+        * Can now log to syslog
+        * Improved latency by disabling Nagle for proxied connection
+        * Added client certificate authentication
+        * Support for password protected certificate key file
+        * TLS ciphers and options are now configurable
+        * Can be invoked via inetd
+        * Lots of minor fixes...
+        
         0.8.0
         -----
         
         * Make websockify properly terminate children on SIGTERM (#226)
         * Remove logging in signal handlers (this can cause Python to hang under certain conditions) (#219)
         * Make it easier to log to a file (#205)
         * Add support for IPv6 addresses in tokens in the TokenFile token plugins (#197)
@@ -303,7 +292,8 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
+Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,143 +1,143 @@
-Metadata-Version: 1.1 Name: websockify Version: 0.8.0 Summary: Websockify.
-Home-page: https://github.com/kanaka/websockify Author: Joel Martin Author-
+Metadata-Version: 2.1 Name: websockify Version: 0.9.0 Summary: Websockify.
+Home-page: https://github.com/novnc/websockify Author: Joel Martin Author-
 email: github@martintribe.org License: LGPLv3 Description: ## websockify:
 WebSockets support for any application/server websockify was formerly named
-wsproxy and was part of the [noVNC](https://github.com/kanaka/noVNC) project.
-At the most basic level, websockify just translates WebSockets traffic to
-normal socket traffic. Websockify accepts the WebSockets handshake, parses it,
-and then begins forwarding traffic between the client and the target in both
+wsproxy and was part of the [noVNC](https://github.com/novnc/noVNC) project. At
+the most basic level, websockify just translates WebSockets traffic to normal
+socket traffic. Websockify accepts the WebSockets handshake, parses it, and
+then begins forwarding traffic between the client and the target in both
 directions. ### News/help/contact Notable commits, announcements and news are
 posted to _@_n_o_V_N_C If you are a websockify developer/integrator/user (or want to
 be) please join the _n_o_V_N_C_/_w_e_b_s_o_c_k_i_f_y_ _d_i_s_c_u_s_s_i_o_n_ _g_r_o_u_p Bugs and feature requests
-can be submitted via [github issues](https://github.com/kanaka/websockify/
+can be submitted via [github issues](https://github.com/novnc/websockify/
 issues). If you want to show appreciation for websockify you could donate to a
 great non-profits such as: [Compassion International](http://
 www.compassion.com/), [SIL](http://www.sil.org), [Habitat for Humanity](http://
 www.habitat.org), [Electronic Frontier Foundation](https://www.eff.org/),
 [Against Malaria Foundation](http://www.againstmalaria.com/), [Nothing But
 Nets](http://www.nothingbutnets.net/), etc. Please tweet _@_n_o_V_N_C if you do. ###
 WebSockets binary data Starting with websockify 0.5.0, only the HyBi / IETF
-6455 WebSocket protocol is supported. Websockify negotiates whether to base64
-encode traffic to and from the client via the subprotocol header (Sec-
-WebSocket-Protocol). The valid subprotocol values are 'binary' and 'base64' and
-if the client sends both then the server (the python implementation) will
-prefer 'binary'. The 'binary' subprotocol indicates that the data will be sent
-raw using binary WebSocket frames. Some HyBi clients (such as the Flash
-fallback and older Chrome and iOS versions) do not support binary data which is
-why the negotiation is necessary. ### Encrypted WebSocket connections (wss://
-) To encrypt the traffic using the WebSocket 'wss://' URI scheme you need to
-generate a certificate and key for Websockify to load. By default, Websockify
-loads a certificate file name `self.pem` but the `--cert=CERT` and `--key=KEY`
-options can override the file name. You can generate a self-signed certificate
-using openssl. When asked for the common name, use the hostname of the server
-where the proxy will be running: ``` openssl req -new -x509 -days 365 -nodes -
-out self.pem -keyout self.pem ``` For a self-signed certificate to work, you
-need to make your client/browser understand it. You can do this by installing
-it as accepted certificate, or by using that same certificate for a HTTPS
-connection to which you navigate first and approve. Browsers generally don't
-give you the "trust certificate?" prompt by opening a WSS socket with invalid
-certificate, hence you need to have it acccept it by either of those two
-methods. If you have a commercial/valid SSL certificate with one ore more
-intermediate certificates, concat them into one file, server certificate first,
-then the intermediate(s) from the CA, etc. Point to this file with the `--cert`
-option and then also to the key with `--key`. Finally, use `--ssl-only` as
-needed. ### Websock Javascript library The `include/websock.js` Javascript
-library library provides a Websock object that is similar to the standard
-WebSocket object but Websock enables communication with raw TCP sockets (i.e.
-the binary stream) via websockify. This is accomplished by base64 encoding the
-data stream between Websock and websockify. Websock has built-in receive queue
-buffering; the message event does not contain actual data but is simply a
-notification that there is new data available. Several rQ* methods are
-available to read binary data off of the receive queue. The Websock API is
-documented on the [websock.js API wiki page](https://github.com/kanaka/
-websockify/wiki/websock.js) See the "Wrap a Program" section below for an
-example of using Websock and websockify as a browser telnet client
-(`wstelnet.html`). ### Additional websockify features These are not necessary
-for the basic operation. * Daemonizing: When the `-D` option is specified,
-websockify runs in the background as a daemon process. * SSL (the wss:/
-/ WebSockets URI): This is detected automatically by websockify by sniffing the
-first byte sent from the client and then wrapping the socket if the data starts
-with '\x16' or '\x80' (indicating SSL). * Flash security policy: websockify
-detects flash security policy requests (again by sniffing the first packet) and
-answers with an appropriate flash security policy response (and then closes the
-port). This means no separate flash security policy server is needed for
-supporting the flash WebSockets fallback emulator. * Session recording: This
-feature that allows recording of the traffic sent and received from the client
-to a file using the `--record` option. * Mini-webserver: websockify can detect
-and respond to normal web requests on the same port as the WebSockets proxy and
-Flash security policy. This functionality is activated with the `--web DIR`
-option where DIR is the root of the web directory to serve. * Wrap a program:
-see the "Wrap a Program" section below. * Log files: websockify can save all
-logging information in a file. This functionality is activated with the `--log-
-file FILE` option where FILE is the file where the logs should be saved. ###
-Implementations of websockify The primary implementation of websockify is in
-python. There are several alternate implementations in other languages (C,
-Node.js, Clojure, Ruby) in the `other/` subdirectory (with varying levels of
-functionality). In addition there are several other external projects that
-implement the websockify "protocol". See the alternate implementation [Feature
-Matrix](https://github.com/kanaka/websockify/wiki/Feature_Matrix) for more
-information. ### Wrap a Program In addition to proxying from a source address
-to a target address (which may be on a different system), websockify has the
-ability to launch a program on the local system and proxy WebSockets traffic to
-a normal TCP port owned/bound by the program. The is accomplished with a small
+6455 WebSocket protocol is supported. There is no support for the older Base64
+encoded data format. ### Encrypted WebSocket connections (wss://) To encrypt
+the traffic using the WebSocket 'wss://' URI scheme you need to generate a
+certificate and key for Websockify to load. By default, Websockify loads a
+certificate file name `self.pem` but the `--cert=CERT` and `--key=KEY` options
+can override the file name. You can generate a self-signed certificate using
+openssl. When asked for the common name, use the hostname of the server where
+the proxy will be running: ``` openssl req -new -x509 -days 365 -nodes -out
+self.pem -keyout self.pem ``` For a self-signed certificate to work, you need
+to make your client/browser understand it. You can do this by installing it as
+accepted certificate, or by using that same certificate for a HTTPS connection
+to which you navigate first and approve. Browsers generally don't give you the
+"trust certificate?" prompt by opening a WSS socket with invalid certificate,
+hence you need to have it acccept it by either of those two methods. If you
+have a commercial/valid SSL certificate with one ore more intermediate
+certificates, concat them into one file, server certificate first, then the
+intermediate(s) from the CA, etc. Point to this file with the `--cert` option
+and then also to the key with `--key`. Finally, use `--ssl-only` as needed. ###
+Additional websockify features These are not necessary for the basic operation.
+* Daemonizing: When the `-D` option is specified, websockify runs in the
+background as a daemon process. * SSL (the wss:// WebSockets URI): This is
+detected automatically by websockify by sniffing the first byte sent from the
+client and then wrapping the socket if the data starts with '\x16' or '\x80'
+(indicating SSL). * Session recording: This feature that allows recording of
+the traffic sent and received from the client to a file using the `--record`
+option. * Mini-webserver: websockify can detect and respond to normal web
+requests on the same port as the WebSockets proxy. This functionality is
+activated with the `--web DIR` option where DIR is the root of the web
+directory to serve. * Wrap a program: see the "Wrap a Program" section below. *
+Log files: websockify can save all logging information in a file. This
+functionality is activated with the `--log-file FILE` option where FILE is the
+file where the logs should be saved. * Authentication plugins: websockify can
+demand authentication for websocket connections and, if you use `--web-auth`,
+also for normal web requests. This functionality is activated with the `--auth-
+plugin CLASS` and `--auth-source ARG` options, where CLASS is usually one from
+auth_plugins.py and ARG is the plugin's configuration. * Token plugins: a
+single instance of websockify can connect clients to multiple different pre-
+configured targets, depending on the token sent by the client using the `token`
+URL parameter, or the hostname used to reach websockify, if you use `--host-
+token`. This functionality is activated with the `--token-plugin CLASS` and `--
+token-source ARG` options, where CLASS is usually one from token_plugins.py and
+ARG is the plugin's configuration. ### Other implementations of websockify The
+primary implementation of websockify is in python. There are several alternate
+implementations in other languages available in our sister repositories
+[websockify-js](https://github.com/novnc/websockify-js) (JavaScript/Node.js)
+and [websockify-other](https://github.com/novnc/websockify-other) (C, Clojure,
+Ruby). In addition there are several other external projects that implement the
+websockify "protocol". See the alternate implementation [Feature Matrix](https:
+//github.com/novnc/websockify/wiki/Feature_Matrix) for more information. ###
+Wrap a Program In addition to proxying from a source address to a target
+address (which may be on a different system), websockify has the ability to
+launch a program on the local system and proxy WebSockets traffic to a normal
+TCP port owned/bound by the program. The is accomplished with a small
 LD_PRELOAD library (`rebind.so`) which intercepts bind() system calls by the
 program. The specified port is moved to a new localhost/loopback free high
 port. websockify then proxies WebSockets traffic directed to the original port
 to the new (moved) port of the program. The program wrap mode is invoked by
 replacing the target with `--` followed by the program command line to wrap.
 `./run 2023 -- PROGRAM ARGS` The `--wrap-mode` option can be used to indicate
 what action to take when the wrapped program exits or daemonizes. Here is an
 example of using websockify to wrap the vncserver command (which backgrounds
-itself) for use with [noVNC](https://github.com/kanaka/noVNC): `./run 5901 --
+itself) for use with [noVNC](https://github.com/novnc/noVNC): `./run 5901 --
 wrap-mode=ignore -- vncserver -geometry 1024x768 :1` Here is an example of
 wrapping telnetd (from krb5-telnetd). telnetd exits after the connection closes
 so the wrap mode is set to respawn the command: `sudo ./run 2023 --wrap-
-mode=respawn -- telnetd -debug 2023` The `wstelnet.html` page demonstrates a
+mode=respawn -- telnetd -debug 2023` The `wstelnet.html` page in the
+[websockify-js](https://github.com/novnc/websockify-js) project demonstrates a
 simple WebSockets based telnet client (use 'localhost' and '2023' for the host
-and port respectively). ### Building the Python ssl module (for python 2.5 and
-older) * Install the build dependencies. On Ubuntu use this command: `sudo
-aptitude install python-dev bluetooth-dev` * At the top level of the websockify
-repostory, download, build and symlink the ssl module: `wget --no-check-
-certificate http://pypi.python.org/packages/source/s/ssl/ssl-1.15.tar.gz` `tar
-xvzf ssl-1.15.tar.gz` `cd ssl-1.15` `make` `cd ../` `ln -sf ssl-1.15/build/
-lib.linux-*/ssl ssl` Changes ======= 0.8.0 ----- * Make websockify properly
-terminate children on SIGTERM (#226) * Remove logging in signal handlers (this
-can cause Python to hang under certain conditions) (#219) * Make it easier to
-log to a file (#205) * Add support for IPv6 addresses in tokens in the
-TokenFile token plugins (#197) * Improve auth plugin framework to enable better
-support for HTTP auth (#194, #201) * Fix bug in JSONTokenAPI token plugin
-(#192) * Fix a missing variable in the exception handler (#178) 0.7.0 ----- *
-Python 3 support fixes (#140, #155, #159) * Generic token-parsing plugins
-support (#162) * Generic authentication plugins support (#172) * Fixed frame
-corruption on big-endian systems (#161) * Support heartbeats (via PING) and
-automatic responses to PONG (#169) * Automatically reject unmasked client
-frames by default (strict mode) (#174) * Automatically restart interrupted
-select calls (#175) * Make 'run' respect environment settings (including
-virtualenv) (#176) 0.6.1 - May 11, 2015 -------------------- * **PATCH
-RELEASE**: Fixes a bug causing file_only to not be passed properly 0.6.0 - Feb
-18, 2014 -------------------- * **NOTE** : 0.6.0 will break existing code that
-sub-classes WebsocketProxy * Refactor to use standard SocketServer
-RequestHandler design * Fix zombie process bug on certain systems when using
-multiprocessing * Add better unit tests * Log information via python `logging`
-module 0.5.1 - Jun 27, 2013 -------------------- * use upstream einaros/ws
-(>=0.4.27) with websockify.js * file_only and no_parent security options for
-WSRequestHandler * Update build of web-socket-js (c0855c6cae) * add include/
-web-socket-js-project submodule to gimite/web-socket-js for DSFG compliance. *
-drop Hixie protocol support 0.4.1 - Mar 12, 2013 -------------------- *
-***NOTE*** : 0.5.0 will drop Hixie protocol support * add include/ directory
-and remove some dev files from source distribution. 0.4.0 - Mar 12, 2013 ------
--------------- * ***NOTE*** : 0.5.0 will drop Hixie protocol support * use
-Buffer base64 support in Node.js implementation 0.3.0 - Jan 15, 2013 ----------
----------- * refactor into modules: websocket, websocketproxy * switch to web-
-socket-js that uses IETF 6455 * change to MPL 2.0 license for include/*.js *
-fix session recording 0.2.1 - Oct 15, 2012 -------------------- * re-released
-with updated version number 0.2.0 - Sep 17, 2012 -------------------- * Binary
-data support in websock.js * Target config file/dir and multiple targets with
-token selector * IPv6 fixes * SSL target support * Proxy to/from unix socket
-0.1.0 - May 11, 2012 -------------------- * Initial versioned release.
-Keywords: noVNC websockify Platform: UNKNOWN Classifier: Programming Language
-:: Python Classifier: Programming Language :: Python :: 2 Classifier:
-Programming Language :: Python :: 2.6 Classifier: Programming Language ::
-Python :: 2.7 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.3 Classifier: Programming Language ::
-Python :: 3.4
+and port respectively). ### Installing websockify Download one of the releases
+or the latest development version, extract it and run `python setup.py install`
+as root in the directory where you extracted the files. Normally, this will
+also install numpy for better performance, if you don't have it installed
+already. However, numpy is optional. If you don't want to install numpy or if
+you can't compile it, you can edit setup.py and remove the `install_requires=
+['numpy'],` line before running `python setup.py install`. Afterwards,
+websockify should be available in your path. Run `websockify --help` to confirm
+it's installed correctly. Changes ======= 0.9.0 ----- * Base64 support removed
+and binary mode is now required * Low level WebSocket protocol handling now has
+its own class * Authentication now optionally required for web server * Server
+hostname can be used as the token * JWT/JWS/JWE can be used for the token *
+redis can be used for the token * Can now log to syslog * Improved latency by
+disabling Nagle for proxied connection * Added client certificate
+authentication * Support for password protected certificate key file * TLS
+ciphers and options are now configurable * Can be invoked via inetd * Lots of
+minor fixes... 0.8.0 ----- * Make websockify properly terminate children on
+SIGTERM (#226) * Remove logging in signal handlers (this can cause Python to
+hang under certain conditions) (#219) * Make it easier to log to a file (#205)
+* Add support for IPv6 addresses in tokens in the TokenFile token plugins
+(#197) * Improve auth plugin framework to enable better support for HTTP auth
+(#194, #201) * Fix bug in JSONTokenAPI token plugin (#192) * Fix a missing
+variable in the exception handler (#178) 0.7.0 ----- * Python 3 support fixes
+(#140, #155, #159) * Generic token-parsing plugins support (#162) * Generic
+authentication plugins support (#172) * Fixed frame corruption on big-endian
+systems (#161) * Support heartbeats (via PING) and automatic responses to PONG
+(#169) * Automatically reject unmasked client frames by default (strict mode)
+(#174) * Automatically restart interrupted select calls (#175) * Make 'run'
+respect environment settings (including virtualenv) (#176) 0.6.1 - May 11, 2015
+-------------------- * **PATCH RELEASE**: Fixes a bug causing file_only to not
+be passed properly 0.6.0 - Feb 18, 2014 -------------------- * **NOTE** : 0.6.0
+will break existing code that sub-classes WebsocketProxy * Refactor to use
+standard SocketServer RequestHandler design * Fix zombie process bug on certain
+systems when using multiprocessing * Add better unit tests * Log information
+via python `logging` module 0.5.1 - Jun 27, 2013 -------------------- * use
+upstream einaros/ws (>=0.4.27) with websockify.js * file_only and no_parent
+security options for WSRequestHandler * Update build of web-socket-js
+(c0855c6cae) * add include/web-socket-js-project submodule to gimite/web-
+socket-js for DSFG compliance. * drop Hixie protocol support 0.4.1 - Mar 12,
+2013 -------------------- * ***NOTE*** : 0.5.0 will drop Hixie protocol support
+* add include/ directory and remove some dev files from source distribution.
+0.4.0 - Mar 12, 2013 -------------------- * ***NOTE*** : 0.5.0 will drop Hixie
+protocol support * use Buffer base64 support in Node.js implementation 0.3.0 -
+Jan 15, 2013 -------------------- * refactor into modules: websocket,
+websocketproxy * switch to web-socket-js that uses IETF 6455 * change to MPL
+2.0 license for include/*.js * fix session recording 0.2.1 - Oct 15, 2012 -----
+--------------- * re-released with updated version number 0.2.0 - Sep 17, 2012
+-------------------- * Binary data support in websock.js * Target config file/
+dir and multiple targets with token selector * IPv6 fixes * SSL target support
+* Proxy to/from unix socket 0.1.0 - May 11, 2012 -------------------- * Initial
+versioned release. Keywords: noVNC websockify Platform: UNKNOWN Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.6 Classifier: Programming
+Language :: Python :: 2.7 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.3 Classifier: Programming
+Language :: Python :: 3.4 Description-Content-Type: text/markdown
```

