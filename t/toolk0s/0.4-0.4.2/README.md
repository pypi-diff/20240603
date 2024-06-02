# Comparing `tmp/toolk0s-0.4.tar.gz` & `tmp/toolk0s-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/toolk0s-0.4.tar", last modified: Mon Dec 19 20:28:31 2016, max compression
+gzip compressed data, was "toolk0s-0.4.2.tar", last modified: Sun Jun  2 22:50:41 2024, max compression
```

## Comparing `toolk0s-0.4.tar` & `toolk0s-0.4.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jehammel   (501) staff       (20)        0 2016-12-19 20:28:31.000000 toolk0s-0.4/
--rw-r--r--   0 jehammel   (501) staff       (20)    17918 2016-12-19 20:28:31.000000 toolk0s-0.4/PKG-INFO
--rw-r--r--   0 jehammel   (501) staff       (20)    14949 2016-12-19 20:26:22.000000 toolk0s-0.4/README.txt
--rw-r--r--   0 jehammel   (501) staff       (20)       59 2016-12-19 20:28:31.000000 toolk0s-0.4/setup.cfg
--rw-r--r--   0 jehammel   (501) staff       (20)     1134 2016-12-19 20:27:49.000000 toolk0s-0.4/setup.py
-drwxr-xr-x   0 jehammel   (501) staff       (20)        0 2016-12-19 20:28:31.000000 toolk0s-0.4/test/
--rwxr-xr-x   0 jehammel   (501) staff       (20)     4438 2016-12-19 20:26:22.000000 toolk0s-0.4/test/test.py
-drwxr-xr-x   0 jehammel   (501) staff       (20)        0 2016-12-19 20:28:31.000000 toolk0s-0.4/toolbox/
--rw-r--r--   0 jehammel   (501) staff       (20)        2 2016-12-19 20:26:22.000000 toolk0s-0.4/toolbox/__init__.py
--rw-r--r--   0 jehammel   (501) staff       (20)     4184 2016-12-19 20:26:22.000000 toolk0s-0.4/toolbox/dispatcher.py
--rw-r--r--   0 jehammel   (501) staff       (20)     2658 2016-12-19 20:26:22.000000 toolk0s-0.4/toolbox/factory.py
--rw-r--r--   0 jehammel   (501) staff       (20)    21019 2016-12-19 20:26:22.000000 toolk0s-0.4/toolbox/handlers.py
--rw-r--r--   0 jehammel   (501) staff       (20)    15394 2016-12-19 20:26:22.000000 toolk0s-0.4/toolbox/model.py
--rw-r--r--   0 jehammel   (501) staff       (20)     3461 2016-12-19 20:26:22.000000 toolk0s-0.4/toolbox/search.py
--rw-r--r--   0 jehammel   (501) staff       (20)     1405 2016-12-19 20:26:22.000000 toolk0s-0.4/toolbox/util.py
-drwxr-xr-x   0 jehammel   (501) staff       (20)        0 2016-12-19 20:28:31.000000 toolk0s-0.4/toolk0s.egg-info/
--rw-r--r--   0 jehammel   (501) staff       (20)        1 2016-12-19 20:28:30.000000 toolk0s-0.4/toolk0s.egg-info/dependency_links.txt
--rw-r--r--   0 jehammel   (501) staff       (20)      229 2016-12-19 20:28:30.000000 toolk0s-0.4/toolk0s.egg-info/entry_points.txt
--rw-r--r--   0 jehammel   (501) staff       (20)        1 2016-12-19 20:28:30.000000 toolk0s-0.4/toolk0s.egg-info/not-zip-safe
--rw-r--r--   0 jehammel   (501) staff       (20)    17918 2016-12-19 20:28:30.000000 toolk0s-0.4/toolk0s.egg-info/PKG-INFO
--rw-r--r--   0 jehammel   (501) staff       (20)       96 2016-12-19 20:28:30.000000 toolk0s-0.4/toolk0s.egg-info/requires.txt
--rw-r--r--   0 jehammel   (501) staff       (20)      382 2016-12-19 20:28:30.000000 toolk0s-0.4/toolk0s.egg-info/SOURCES.txt
--rw-r--r--   0 jehammel   (501) staff       (20)        8 2016-12-19 20:28:30.000000 toolk0s-0.4/toolk0s.egg-info/top_level.txt
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-06-02 22:50:41.681261 toolk0s-0.4.2/
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      248 2024-06-02 22:50:41.681261 toolk0s-0.4.2/PKG-INFO
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)    14946 2024-06-02 22:46:39.000000 toolk0s-0.4.2/README.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       38 2024-06-02 22:50:41.681261 toolk0s-0.4.2/setup.cfg
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     1359 2024-06-02 22:50:07.000000 toolk0s-0.4.2/setup.py
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-06-02 22:50:41.677261 toolk0s-0.4.2/test/
+-rwxrwxr-x   0 jhammel   (1000) jhammel   (1000)     4438 2024-06-02 22:30:59.000000 toolk0s-0.4.2/test/test.py
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-06-02 22:50:41.681261 toolk0s-0.4.2/toolbox/
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        2 2024-06-02 22:30:59.000000 toolk0s-0.4.2/toolbox/__init__.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     4179 2024-06-02 22:30:59.000000 toolk0s-0.4.2/toolbox/dispatcher.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     2661 2024-06-02 22:30:59.000000 toolk0s-0.4.2/toolbox/factory.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)    20892 2024-06-02 22:30:59.000000 toolk0s-0.4.2/toolbox/handlers.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)    15270 2024-06-02 22:30:59.000000 toolk0s-0.4.2/toolbox/model.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     2731 2024-06-02 22:30:59.000000 toolk0s-0.4.2/toolbox/search.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     1406 2024-06-02 22:30:59.000000 toolk0s-0.4.2/toolbox/util.py
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-06-02 22:50:41.681261 toolk0s-0.4.2/toolk0s.egg-info/
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      248 2024-06-02 22:50:41.000000 toolk0s-0.4.2/toolk0s.egg-info/PKG-INFO
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      382 2024-06-02 22:50:41.000000 toolk0s-0.4.2/toolk0s.egg-info/SOURCES.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        1 2024-06-02 22:50:41.000000 toolk0s-0.4.2/toolk0s.egg-info/dependency_links.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      229 2024-06-02 22:50:41.000000 toolk0s-0.4.2/toolk0s.egg-info/entry_points.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        1 2024-06-02 22:31:01.000000 toolk0s-0.4.2/toolk0s.egg-info/not-zip-safe
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       86 2024-06-02 22:50:41.000000 toolk0s-0.4.2/toolk0s.egg-info/requires.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        8 2024-06-02 22:50:41.000000 toolk0s-0.4.2/toolk0s.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `toolk0s-0.4/PKG-INFO` & `toolk0s-0.4.2/README.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,353 +1,343 @@
-Metadata-Version: 1.0
-Name: toolk0s
-Version: 0.4
-Summary: a place to list links + tools
-Home-page: http://k0s.org/hg/toolbox/
-Author: Jeff Hammel
-Author-email: jhammel@mozilla.com
-License: MPL
-Description: The Story of Toolbox
-        ====================
-        
-        Toolbox is fundamentally a document-oriented approach to resource
-        indexing.  A "tool" consists three mandatory string fields -- name,
-        description, and URL -- that are generic to the large class of problems
-        of web resources, as well as classifiers, such as author, usage, type,
-        etc. A tool may have an arbitrary number of classifier fields as
-        needed.  Each classifier consists of a set of values with which a tool
-        is tagged. This gives toolbox the flexibility to fit a large number of
-        data models, such as PYPI, DOAP, and others.
-        
-        
-        Running Toolbox
-        ---------------
-        
-        You can download and run the toolbox software yourself:
-        http://github.com/k0s/toolbox
-        
-        To serve in baseline mode, install the software and run::
-        
-         paster serve paste.ini
-        
-        This will serve the handlers and static content using the paste
-        (http://pythonpaste.org) webserver using ``README.txt`` as the
-        ``/about`` page and serving the data in ``sample``.
-        
-        The dispatcher (``toolbox.dispatcher:Dispatcher``) is the central (WSGI)
-        webapp that designates per-request to a number of handlers (from
-        ``handlers.py``).  The dispatcher has a few options:
-        
-        * about: path to a restructured text file to serve at ``/about``
-        * model_type: name of the backend to use (memory_cache, file_cache, or couch)
-        * template_dir: extra directory to look for templates
-        
-        These may be configured in the ``paste.ini`` file in the
-        ``[app:toolbox]`` section by prepending with the namespace
-        ``toolbox.``. It is advisable that you copy the example ``paste.ini``
-        file for your own usage needs.  Additional ``toolbox.``-namespaced
-        arguments will be passed to the model.  For instance, to specify the
-        directory for the ``file_cache`` model, the provided ``paste.ini`` uses
-        ``toolbox.directory = %(here)s/sample``.
-        
-        
-        Architecture
-        ------------
-        
-        Toolbox uses a fairly simple architecture with a single abstract data
-        model allowing an arbitrary number of implementations to be constructed::
-        
-         Interfaces            Implementations
-        
-         +----+              +-+-----+
-         |HTTP|              | |files|
-         +----+---\  +-----+ | +-----+
-                   |-|model|-+-+-----+
-         +------+-/  +-----+ | |couch|
-         |script|            | +-----+
-         +------+            +-+------+
-                             | |memory|
-                             | +------+
-                             +-+---+
-                               |...|
-                               +---+
-        
-        Toolbox was originally intended to use a directory of files, one per project,
-        as the backend. These were originally intended to be HTML files as the
-        above model may be clearly mapped as HTML::
-        
-         <div class="project"><h1><a href="{{url}}">{{name}}</a></h1>
-         <p class="description">{{description}}</p>
-         {{for field in fields}}
-          <ul class="{{field}}">
-          {{for value in values[field]}}
-           <li>{{value}}</li>
-          {{endfor}}
-         {{endfor}}
-         </div>
-        
-        This microformat approach allows not only easy editing of the HTML
-        documents, but the documents may be indepently served and displayed
-        without the toolbox server-side. 
-        
-        The HTML microformat was never implemented (though, since the model
-        backend is pluggable, it easily could be). Instead, the original
-        implementation used JSON blobs stored in one file per tool. This
-        approach loses the displayable aspect, though since JSON is a defined
-        format with several good tools for exploring and manipulating the data
-        perhaps this disavantage is offset.
-        
-        A couch backend was also written.
-        
-              +------------+-----------+------------+
-              |Displayable?|File-based?|Concurrency?|
-        +-----+------------+-----------+------------+
-        |HTML |Yes         |Yes        |No          |
-        +-----+------------+-----------+------------+
-        |JSON |Not really  |Yes        |No          |
-        +-----+------------+-----------+------------+
-        |Couch|No          |No         |Yes?        |
-        +-----+------------+-----------+------------+
-        
-        The concurrency issue with file-based documennt backends may be
-        overcome by using locked files.  Ideally, this is accomplished at the
-        filesystem level.  If your filesystem does not promote this
-        functionality, it may be introduced programmatically.  A rough cartoon
-        of a good implementation is as follows:
-        
-        1. A worker thread is spawned to write the data asynchronously. The
-        data is sent to the worker thread.
-        
-        2. The worker checks for the presence of a lockfile (herein further
-        detailed). If the lockfile exists and is owned by an active process,
-        the worker waits until said process is done with it. (For a more
-        robust implementation, the worker sends a request to write the file to
-        some controller.)
-        
-        3. The worker owns a lockfile based on its PID in some directory
-        parallel to the directory root under consideration (for example,
-        ``/tmp/toolbox/lock/${PID}-${filename}.lck``).
-        
-        4. The worker writes to the file.
-        
-        5. The worker removes the lock
-        
-        The toolbox web service uses a dispatcher->handler framework.  The
-        handlers are loosely pluggable (they are assigned in the dispatcher),
-        but could (and probably should) be made completely pluggable.  That
-        said, the toolbox web system features an integration of templates,
-        static resources (javascript, css, images), and handlers, so true
-        pluggability is further away than just supporting pluggable handlers
-        in the dispatcher.
-        
-        Deployment, however, may be tailored as desired.  Any of the given
-        templates may be overridden via passing a ``template_dir`` parameter
-        with a path to a directory that have templates of the appropriate
-        names as found in toolbox's ``templates`` directory. 
-        
-        Likewise, the static files (css, js, etc.) are served using ``paste``'s 
-        ``StaticURLParser`` out of toolbox's ``static`` directory. (See
-        toolbox's ``factory.py``.) Notably this is *not* done using the WSGI
-        app itself.  Doing it with middleware allows the deployment to be
-        customizable by writing your own factory.  For example, instead of
-        using the ``paste`` webserver and the included ``paste.ini``, you
-        could use nginx or apache and ``mod_wsgi`` with a factory file
-        invoking ``Dispatcher`` with the desired arguments and serving the
-        static files with an arbitrary static file server.
-        
-        It is common sense, if rarely followed, that deployment should be
-        simple.  If you want to get toolbox running on your desktop and/or for
-        testing, you should be able to do this easily (see the ``INSTALL.sh``
-        for a simple installation using ``bash``; you'll probably want to
-        perform these steps by hand for any sort of real-world deployment).
-        If you want a highly customized deployment, then this will require
-        more expertise and manual setup.
-        
-        The template data and the JSON are closely tied together.  This has the
-        distinct advantage of avoiding data translation steps and avoiding
-        code duplication.
-        
-        Toolbox uses several light-footprint libraries:
-        
-        * webob for Request/Response handling: http://pythonpaste.org/webob/
-        
-        * tempita for (HTML) templates: http://pythonpaste.org/tempita/
-        
-        * whoosh for search.  This pure-python implementation of full-text
-          search is relatively fast (for python) and should scale decently to
-          the target scale of toolbox (1000s or 10000s of tools). While not as
-          fast as lucene, whoosh is easy to deploy and has a good API and
-          preserves toolbox as a deployable software product versus an
-          instance that requires the expert configuration, maintainence, and
-          tuning of several disparate software products that is both
-          non-automatable (cannot be installed with a script) and
-          time-consuming. http://packages.python.org/Whoosh/
-        
-        * jQuery: jQuery is the best JavaScript library and everyone
-          should use it. http://jquery.com/
-        
-        * jeditable for AJAXy editing: http://www.appelsiini.net/projects/jeditable
-        
-        * jquery-token for autocomplete: http://loopj.com/jquery-tokeninput/
-        
-        * less for dynamic stylesheets: http://lesscss.org/
-        
-        
-        User Interaction
-        ----------------
-        
-        A user will typically interact with Toolbox through the AJAX web
-        interface.  The server side returns relatively simple (HTML) markup,
-        but structured in such a way that JavaScript may be utilized to
-        promote rich interaction.  The simple HTML + complex JS manifests
-        several things:
-        
-        1. The document is a document. The tools HTML presented to the user (with
-        the current objectionable exception of the per-project Delete button)
-        is a document form of the data. It can be clearly and easily
-        translated to data (for e.g. import/export) or simply marked up using
-        (e.g.) JS to add functionality. By keeping concerns seperate
-        (presentation layer vs. interaction layer) a self-evident clarity is
-        maintained.
-        
-        2. Computation is shifted client-side. Often, an otherwise lightweight
-        webapp loses considerable performance rendering complex templates. By
-        keeping the templates light-weight and doing control presentation and
-        handling in JS, high performance is preserved.
-        
-        
-        What Toolbox Doesn't Do
-        -----------------------
-        
-        * versioning: toolbox exposes editing towards a canonical document.
-          It doesn't do versioning.  A model instance may do whatever
-          versioning it desires, and since the models are pluggable, it would
-          be relatively painless to subclass e.g. the file-based model and
-          have a post-save hook which does an e.g. ``hg commit``. Customized
-          templates could be used to display this information.
-        
-        * authentication: the information presented by toolbox is freely
-          readable and editable. This is by intention, as by going to a "wiki"
-          model and presenting a easy to use, context-switching-free interface
-          curation is encouraged (ignoring the possibly imaginary problem of
-          wiki-spam). Access-level auth could be implemented using WSGI
-          middleware (e.g. repoze.who or bitsyauth) or through a front end
-          "webserver" integration layer such as Apache or nginx. Finer grained
-          control of the presentation layer could be realized by using custom
-          templates.
-        
-        
-        What Toolbox Would Like To Do
-        -----------------------------
-        
-        Ultimately, toolbox should be as federated as possible.  The basic
-        architecture of toolbox as a web service + supporting scripts makes
-        this feasible and more self-contained than most proposed federated
-        services.  The basic federated model has proved, in practice,
-        difficult to achieve through purely the (HTTP) client-server model, as
-        without complete federation and adherence to protocol offline cron
-        jobs should be utilized to pull external data sources. If a webservice
-        only desires to talk to others of its own type and are willing to keep
-        a queue of requests for when hosts are offline, entire HTTP federation
-        may be implemented with only a configuration-specified discovery
-        service to find the nodes.
-        
-        
-        Evolution
-        ---------
-        
-        Often, a piece software is presented as a state out of context (that
-        is minus the evolution which led it to be and led it to look further
-        out towards beyond the horizon).  While this is an interesting special
-        effect for an art project, software being communication this
-        is only conducive to software in the darkest of black-box approaches.
-        
-        "Beers are like web frameworks: if they're not micro, you don't know
-        what you're talking about." - hipsterhacker
-        
-        For sites that fit the architecture of a given framework, it may be
-        advisable to make use of them.  However, for most webapp/webservice
-        categories which have a finite scope and definitive intent, it is
-        often easier, more maintainable, and more legible to build a complete
-        HTTP->WSGI->app architecture than to try to hammer a framework into
-        fitting your problem or redefining the problem to fit the framework.
-        This approach was used for toolbox.
-        
-        The GenshiView template, http://k0s.org/hg/GenshiView, was invoked to
-        generate a basic dispatcher->handler system.  The cruft was removed,
-        leaving only the basic structure and the TempitaHandler since tempita
-        is lightweight and it was envisioned that filesystem tempita templates
-        (MakeItSo!) would be used elsewhere in the project.  The basic
-        handlers (projects views, field-sorted view, new, etc.) were written
-        and soon a usable interface was constructed.
-        
-        A ``sample`` directory was created to hold the JSON blobs. Because
-        this was done early on, two goals were achieved: 
-        
-        1. the software could be dogfooded immediately using actual applicable
-        data. This helped expose a number of issues concerning the data format
-        right away.
-        
-        2. There was a place to put tools before the project reached a
-        deployable state (previously, a few had lived in a static state using
-        a rough sketch of the HTML microformat discussed above on
-        k0s.org). Since the main point of toolbox is to record Mozilla tools,
-        the wealth of references mentioned in passing could be put somewhere,
-        instead of passed by and forgotten.  One wishes that they do not miss
-        the train while purchasing a ticket.
-        
-        The original intent, when the file-based JSON blob approach was to be
-        the deployed backend, was to have two repositories: one for the code
-        and one for the JSON blobs.  When this approach was scrapped, the
-        file-based JSON blobs were relegated to the ``sample`` directory, with
-        the intent to be to import them into e.g. a couch database on actual
-        deployment (using an import script). The samples could then be used
-        for testing.
-        
-        The model has a single "setter" function, ``def update``, used for
-        both creating and updating projects.  Due to this and due to the fact
-        the model was ABC/pluggable from the beginning, a converter ``export``
-        function could be trivially written at the ABC-level::
-        
-            def export(self, other):
-                """export the current model to another model instance"""
-                for project in self.get():
-                    other.update(project)
-        
-        This with an accompanying CLI utility was used to migrate from JSON
-        blob files in the ``sample`` directory to the couch instance.  This
-        particular methodology as applied to an unexpected problem (the
-        unanticipated switch from JSON blobs to couch) is a good example of
-        the power of using a problem to drive the software forward (in this
-        case, creation of a universal export function and associated command
-        line utility). The alternative, a one-off manual data migration, would
-        have been just as time consuming, would not be repeatable, would not
-        have extended toolbox, and may have (like many one-offs do) infected
-        the code base with associated semi-permanant vestiges.  In general,
-        problems should be used to drive innovation.  This can only be done if
-        the software is kept in a reasonably good state.  Otherwise
-        considerable (though probably worthwhile) refactoring should be done
-        prior to feature extension which will become cost-prohibitive in
-        time-critical situations where a one-off is (more) likely to be employed.
-        
-        
-        Use Cases
-        ---------
-        
-        The target use-case is software tools for Mozilla, or, more generally,
-        a software index.  For this case, the default fields uses are given in
-        the paste.ini file: usage, author, type, language. More fields may be
-        added to the running instance in the future.
-        
-        However, the classifier classification can be used for a wide variety
-        of web-locatable resources.  A few examples:
-        
-        * songs: artist, album, genre, instruments
-        * de.li.cio.us: type, media, author, site
-        
-        
-        Resources
-        ---------
-        
-        * http://readthedocs.org/
-        
-Platform: UNKNOWN
+The Story of Toolbox
+====================
+
+Toolbox is fundamentally a document-oriented approach to resource
+indexing.  A "tool" consists three mandatory string fields -- name,
+description, and URL -- that are generic to the large class of problems
+of web resources, as well as classifiers, such as author, usage, type,
+etc. A tool may have an arbitrary number of classifier fields as
+needed.  Each classifier consists of a set of values with which a tool
+is tagged. This gives toolbox the flexibility to fit a large number of
+data models, such as PYPI, DOAP, and others.
+
+
+Running Toolbox
+---------------
+
+You can download and run the toolbox software yourself:
+http://github.com/k0s/toolbox
+
+To serve in baseline mode, install the software and run::
+
+ paster serve paste.ini
+
+This will serve the handlers and static content using the paste
+(http://pythonpaste.org) webserver using ``README.txt`` as the
+``/about`` page and serving the data in ``sample``.
+
+The dispatcher (``toolbox.dispatcher:Dispatcher``) is the central (WSGI)
+webapp that designates per-request to a number of handlers (from
+``handlers.py``).  The dispatcher has a few options:
+
+* about: path to a restructured text file to serve at ``/about``
+* model_type: name of the backend to use (memory_cache, file_cache, or couch)
+* template_dir: extra directory to look for templates
+
+These may be configured in the ``paste.ini`` file in the
+``[app:toolbox]`` section by prepending with the namespace
+``toolbox.``. It is advisable that you copy the example ``paste.ini``
+file for your own usage needs.  Additional ``toolbox.``-namespaced
+arguments will be passed to the model.  For instance, to specify the
+directory for the ``file_cache`` model, the provided ``paste.ini`` uses
+``toolbox.directory = %(here)s/sample``.
+
+
+Architecture
+------------
+
+Toolbox uses a fairly simple architecture with a single abstract data
+model allowing an arbitrary number of implementations to be constructed::
+
+ Interfaces            Implementations
+
+ +----+              +-+-----+
+ |HTTP|              | |files|
+ +----+---\  +-----+ | +-----+
+           |-|model|-+-+-----+
+ +------+-/  +-----+ | |couch|
+ |script|            | +-----+
+ +------+            +-+------+
+                     | |memory|
+                     | +------+
+                     +-+---+
+                       |...|
+                       +---+
+
+Toolbox was originally intended to use a directory of files, one per project,
+as the backend. These were originally intended to be HTML files as the
+above model may be clearly mapped as HTML::
+
+ <div class="project"><h1><a href="{{url}}">{{name}}</a></h1>
+ <p class="description">{{description}}</p>
+ {{for field in fields}}
+  <ul class="{{field}}">
+  {{for value in values[field]}}
+   <li>{{value}}</li>
+  {{endfor}}
+ {{endfor}}
+ </div>
+
+This microformat approach allows not only easy editing of the HTML
+documents, but the documents may be indepently served and displayed
+without the toolbox server-side.
+
+The HTML microformat was never implemented (though, since the model
+backend is pluggable, it easily could be). Instead, the original
+implementation used JSON blobs stored in one file per tool. This
+approach loses the displayable aspect, though since JSON is a defined
+format with several good tools for exploring and manipulating the data
+perhaps this disavantage is offset.
+
+A couch backend was also written.
+
+      +------------+-----------+------------+
+      |Displayable |File-based |Concurrency |
++-----+------------+-----------+------------+
+|HTML |Yes         |Yes        |No          |
++-----+------------+-----------+------------+
+|JSON |Not really  |Yes        |No          |
++-----+------------+-----------+------------+
+|Couch|No          |No         |Yes         |
++-----+------------+-----------+------------+
+
+The concurrency issue with file-based documennt backends may be
+overcome by using locked files.  Ideally, this is accomplished at the
+filesystem level.  If your filesystem does not promote this
+functionality, it may be introduced programmatically.  A rough cartoon
+of a good implementation is as follows:
+
+1. A worker thread is spawned to write the data asynchronously. The
+data is sent to the worker thread.
+
+2. The worker checks for the presence of a lockfile (herein further
+detailed). If the lockfile exists and is owned by an active process,
+the worker waits until said process is done with it. (For a more
+robust implementation, the worker sends a request to write the file to
+some controller.)
+
+3. The worker owns a lockfile based on its PID in some directory
+parallel to the directory root under consideration (for example,
+``/tmp/toolbox/lock/${PID}-${filename}.lck``).
+
+4. The worker writes to the file.
+
+5. The worker removes the lock
+
+The toolbox web service uses a dispatcher->handler framework.  The
+handlers are loosely pluggable (they are assigned in the dispatcher),
+but could (and probably should) be made completely pluggable.  That
+said, the toolbox web system features an integration of templates,
+static resources (javascript, css, images), and handlers, so true
+pluggability is further away than just supporting pluggable handlers
+in the dispatcher.
+
+Deployment, however, may be tailored as desired.  Any of the given
+templates may be overridden via passing a ``template_dir`` parameter
+with a path to a directory that have templates of the appropriate
+names as found in toolbox's ``templates`` directory.
+
+Likewise, the static files (css, js, etc.) are served using ``paste``'s
+``StaticURLParser`` out of toolbox's ``static`` directory. (See
+toolbox's ``factory.py``.) Notably this is *not* done using the WSGI
+app itself.  Doing it with middleware allows the deployment to be
+customizable by writing your own factory.  For example, instead of
+using the ``paste`` webserver and the included ``paste.ini``, you
+could use nginx or apache and ``mod_wsgi`` with a factory file
+invoking ``Dispatcher`` with the desired arguments and serving the
+static files with an arbitrary static file server.
+
+It is common sense, if rarely followed, that deployment should be
+simple.  If you want to get toolbox running on your desktop and/or for
+testing, you should be able to do this easily (see the ``INSTALL.sh``
+for a simple installation using ``bash``; you'll probably want to
+perform these steps by hand for any sort of real-world deployment).
+If you want a highly customized deployment, then this will require
+more expertise and manual setup.
+
+The template data and the JSON are closely tied together.  This has the
+distinct advantage of avoiding data translation steps and avoiding
+code duplication.
+
+Toolbox uses several light-footprint libraries:
+
+* webob for Request/Response handling: http://pythonpaste.org/webob/
+
+* tempita for (HTML) templates: http://pythonpaste.org/tempita/
+
+* whoosh for search.  This pure-python implementation of full-text
+  search is relatively fast (for python) and should scale decently to
+  the target scale of toolbox (1000s or 10000s of tools). While not as
+  fast as lucene, whoosh is easy to deploy and has a good API and
+  preserves toolbox as a deployable software product versus an
+  instance that requires the expert configuration, maintainence, and
+  tuning of several disparate software products that is both
+  non-automatable (cannot be installed with a script) and
+  time-consuming. http://packages.python.org/Whoosh/
+
+* jQuery: jQuery is the best JavaScript library and everyone
+  should use it. http://jquery.com/
+
+* jeditable for AJAXy editing: http://www.appelsiini.net/projects/jeditable
+
+* jquery-token for autocomplete: http://loopj.com/jquery-tokeninput/
+
+* less for dynamic stylesheets: http://lesscss.org/
+
+
+User Interaction
+----------------
+
+A user will typically interact with Toolbox through the AJAX web
+interface.  The server side returns relatively simple (HTML) markup,
+but structured in such a way that JavaScript may be utilized to
+promote rich interaction.  The simple HTML + complex JS manifests
+several things:
+
+1. The document is a document. The tools HTML presented to the user (with
+the current objectionable exception of the per-project Delete button)
+is a document form of the data. It can be clearly and easily
+translated to data (for e.g. import/export) or simply marked up using
+(e.g.) JS to add functionality. By keeping concerns seperate
+(presentation layer vs. interaction layer) a self-evident clarity is
+maintained.
+
+2. Computation is shifted client-side. Often, an otherwise lightweight
+webapp loses considerable performance rendering complex templates. By
+keeping the templates light-weight and doing control presentation and
+handling in JS, high performance is preserved.
+
+
+What Toolbox Doesn't Do
+-----------------------
+
+* versioning: toolbox exposes editing towards a canonical document.
+  It doesn't do versioning.  A model instance may do whatever
+  versioning it desires, and since the models are pluggable, it would
+  be relatively painless to subclass e.g. the file-based model and
+  have a post-save hook which does an e.g. ``hg commit``. Customized
+  templates could be used to display this information.
+
+* authentication: the information presented by toolbox is freely
+  readable and editable. This is by intention, as by going to a "wiki"
+  model and presenting a easy to use, context-switching-free interface
+  curation is encouraged (ignoring the possibly imaginary problem of
+  wiki-spam). Access-level auth could be implemented using WSGI
+  middleware (e.g. repoze.who or bitsyauth) or through a front end
+  "webserver" integration layer such as Apache or nginx. Finer grained
+  control of the presentation layer could be realized by using custom
+  templates.
+
+
+What Toolbox Would Like To Do
+-----------------------------
+
+Ultimately, toolbox should be as federated as possible.  The basic
+architecture of toolbox as a web service + supporting scripts makes
+this feasible and more self-contained than most proposed federated
+services.  The basic federated model has proved, in practice,
+difficult to achieve through purely the (HTTP) client-server model, as
+without complete federation and adherence to protocol offline cron
+jobs should be utilized to pull external data sources. If a webservice
+only desires to talk to others of its own type and are willing to keep
+a queue of requests for when hosts are offline, entire HTTP federation
+may be implemented with only a configuration-specified discovery
+service to find the nodes.
+
+
+Evolution
+---------
+
+Often, a piece software is presented as a state out of context (that
+is minus the evolution which led it to be and led it to look further
+out towards beyond the horizon).  While this is an interesting special
+effect for an art project, software being communication this
+is only conducive to software in the darkest of black-box approaches.
+
+"Beers are like web frameworks: if they're not micro, you don't know
+what you're talking about." - hipsterhacker
+
+For sites that fit the architecture of a given framework, it may be
+advisable to make use of them.  However, for most webapp/webservice
+categories which have a finite scope and definitive intent, it is
+often easier, more maintainable, and more legible to build a complete
+HTTP->WSGI->app architecture than to try to hammer a framework into
+fitting your problem or redefining the problem to fit the framework.
+This approach was used for toolbox.
+
+The GenshiView template, http://k0s.org/hg/GenshiView, was invoked to
+generate a basic dispatcher->handler system.  The cruft was removed,
+leaving only the basic structure and the TempitaHandler since tempita
+is lightweight and it was envisioned that filesystem tempita templates
+(MakeItSo!) would be used elsewhere in the project.  The basic
+handlers (projects views, field-sorted view, new, etc.) were written
+and soon a usable interface was constructed.
+
+A ``sample`` directory was created to hold the JSON blobs. Because
+this was done early on, two goals were achieved: 
+
+1. the software could be dogfooded immediately using actual applicable
+data. This helped expose a number of issues concerning the data format
+right away.
+
+2. There was a place to put tools before the project reached a
+deployable state (previously, a few had lived in a static state using
+a rough sketch of the HTML microformat discussed above on
+k0s.org). Since the main point of toolbox is to record Mozilla tools,
+the wealth of references mentioned in passing could be put somewhere,
+instead of passed by and forgotten.  One wishes that they do not miss
+the train while purchasing a ticket.
+
+The original intent, when the file-based JSON blob approach was to be
+the deployed backend, was to have two repositories: one for the code
+and one for the JSON blobs.  When this approach was scrapped, the
+file-based JSON blobs were relegated to the ``sample`` directory, with
+the intent to be to import them into e.g. a couch database on actual
+deployment (using an import script). The samples could then be used
+for testing.
+
+The model has a single "setter" function, ``def update``, used for
+both creating and updating projects.  Due to this and due to the fact
+the model was ABC/pluggable from the beginning, a converter ``export``
+function could be trivially written at the ABC-level::
+
+    def export(self, other):
+        """export the current model to another model instance"""
+        for project in self.get():
+            other.update(project)
+
+This with an accompanying CLI utility was used to migrate from JSON
+blob files in the ``sample`` directory to the couch instance.  This
+particular methodology as applied to an unexpected problem (the
+unanticipated switch from JSON blobs to couch) is a good example of
+the power of using a problem to drive the software forward (in this
+case, creation of a universal export function and associated command
+line utility). The alternative, a one-off manual data migration, would
+have been just as time consuming, would not be repeatable, would not
+have extended toolbox, and may have (like many one-offs do) infected
+the code base with associated semi-permanant vestiges.  In general,
+problems should be used to drive innovation.  This can only be done if
+the software is kept in a reasonably good state.  Otherwise
+considerable (though probably worthwhile) refactoring should be done
+prior to feature extension which will become cost-prohibitive in
+time-critical situations where a one-off is (more) likely to be employed.
+
+
+Use Cases
+---------
+
+The target use-case is software tools for Mozilla, or, more generally,
+a software index.  For this case, the default fields uses are given in
+the paste.ini file: usage, author, type, language. More fields may be
+added to the running instance in the future.
+
+However, the classifier classification can be used for a wide variety
+of web-locatable resources.  A few examples:
+
+* songs: artist, album, genre, instruments
+* de.li.cio.us: type, media, author, site
+
+
+Resources
+---------
+
+* http://readthedocs.org/
```

#### html2text {}

```diff
@@ -1,59 +1,56 @@
-Metadata-Version: 1.0 Name: toolk0s Version: 0.4 Summary: a place to list links
-+ tools Home-page: http://k0s.org/hg/toolbox/ Author: Jeff Hammel Author-email:
-jhammel@mozilla.com License: MPL Description: The Story of Toolbox
-==================== Toolbox is fundamentally a document-oriented approach to
-resource indexing. A "tool" consists three mandatory string fields -- name,
-description, and URL -- that are generic to the large class of problems of web
-resources, as well as classifiers, such as author, usage, type, etc. A tool may
-have an arbitrary number of classifier fields as needed. Each classifier
-consists of a set of values with which a tool is tagged. This gives toolbox the
-flexibility to fit a large number of data models, such as PYPI, DOAP, and
-others. Running Toolbox --------------- You can download and run the toolbox
-software yourself: http://github.com/k0s/toolbox To serve in baseline mode,
-install the software and run:: paster serve paste.ini This will serve the
-handlers and static content using the paste (http://pythonpaste.org) webserver
-using ``README.txt`` as the ``/about`` page and serving the data in ``sample``.
-The dispatcher (``toolbox.dispatcher:Dispatcher``) is the central (WSGI) webapp
-that designates per-request to a number of handlers (from ``handlers.py``). The
-dispatcher has a few options: * about: path to a restructured text file to
-serve at ``/about`` * model_type: name of the backend to use (memory_cache,
-file_cache, or couch) * template_dir: extra directory to look for templates
-These may be configured in the ``paste.ini`` file in the ``[app:toolbox]``
-section by prepending with the namespace ``toolbox.``. It is advisable that you
-copy the example ``paste.ini`` file for your own usage needs. Additional
-``toolbox.``-namespaced arguments will be passed to the model. For instance, to
-specify the directory for the ``file_cache`` model, the provided ``paste.ini``
-uses ``toolbox.directory = %(here)s/sample``. Architecture ------------ Toolbox
-uses a fairly simple architecture with a single abstract data model allowing an
-arbitrary number of implementations to be constructed:: Interfaces
-Implementations +----+ +-+-----+ |HTTP| | |files| +----+---\ +-----+ | +-----
-+ |-|model|-+-+-----+ +------+-/ +-----+ | |couch| |script| | +-----+ +------
-+ +-+------+ | |memory| | +------+ +-+---+ |...| +---+ Toolbox was originally
-intended to use a directory of files, one per project, as the backend. These
-were originally intended to be HTML files as the above model may be clearly
-mapped as HTML::
+The Story of Toolbox ==================== Toolbox is fundamentally a document-
+oriented approach to resource indexing. A "tool" consists three mandatory
+string fields -- name, description, and URL -- that are generic to the large
+class of problems of web resources, as well as classifiers, such as author,
+usage, type, etc. A tool may have an arbitrary number of classifier fields as
+needed. Each classifier consists of a set of values with which a tool is
+tagged. This gives toolbox the flexibility to fit a large number of data
+models, such as PYPI, DOAP, and others. Running Toolbox --------------- You can
+download and run the toolbox software yourself: http://github.com/k0s/toolbox
+To serve in baseline mode, install the software and run:: paster serve
+paste.ini This will serve the handlers and static content using the paste
+(http://pythonpaste.org) webserver using ``README.txt`` as the ``/about`` page
+and serving the data in ``sample``. The dispatcher (``toolbox.dispatcher:
+Dispatcher``) is the central (WSGI) webapp that designates per-request to a
+number of handlers (from ``handlers.py``). The dispatcher has a few options: *
+about: path to a restructured text file to serve at ``/about`` * model_type:
+name of the backend to use (memory_cache, file_cache, or couch) * template_dir:
+extra directory to look for templates These may be configured in the
+``paste.ini`` file in the ``[app:toolbox]`` section by prepending with the
+namespace ``toolbox.``. It is advisable that you copy the example ``paste.ini``
+file for your own usage needs. Additional ``toolbox.``-namespaced arguments
+will be passed to the model. For instance, to specify the directory for the
+``file_cache`` model, the provided ``paste.ini`` uses ``toolbox.directory = %
+(here)s/sample``. Architecture ------------ Toolbox uses a fairly simple
+architecture with a single abstract data model allowing an arbitrary number of
+implementations to be constructed:: Interfaces Implementations +----+ +-+-----
++ |HTTP| | |files| +----+---\ +-----+ | +-----+ |-|model|-+-+-----+ +------+-
+/ +-----+ | |couch| |script| | +-----+ +------+ +-+------+ | |memory| | +------
++ +-+---+ |...| +---+ Toolbox was originally intended to use a directory of
+files, one per project, as the backend. These were originally intended to be
+HTML files as the above model may be clearly mapped as HTML::
 ************ _{{_{{_nn_aa_mm_ee_}}_}} ************
 {{description}}
 {{for field in fields}}
     * {{for value in values[field]}}
     * {{value}}
     * {{endfor}} {{endfor}}
 This microformat approach allows not only easy editing of the HTML documents,
 but the documents may be indepently served and displayed without the toolbox
 server-side. The HTML microformat was never implemented (though, since the
 model backend is pluggable, it easily could be). Instead, the original
 implementation used JSON blobs stored in one file per tool. This approach loses
 the displayable aspect, though since JSON is a defined format with several good
 tools for exploring and manipulating the data perhaps this disavantage is
 offset. A couch backend was also written. +------------+-----------+-----------
--+ |Displayable?|File-based?|Concurrency?| +-----+------------+-----------+----
+-+ |Displayable |File-based |Concurrency | +-----+------------+-----------+----
 --------+ |HTML |Yes |Yes |No | +-----+------------+-----------+------------
 + |JSON |Not really |Yes |No | +-----+------------+-----------+------------
-+ |Couch|No |No |Yes? | +-----+------------+-----------+------------+ The
++ |Couch|No |No |Yes | +-----+------------+-----------+------------+ The
 concurrency issue with file-based documennt backends may be overcome by using
 locked files. Ideally, this is accomplished at the filesystem level. If your
 filesystem does not promote this functionality, it may be introduced
 programmatically. A rough cartoon of a good implementation is as follows: 1. A
 worker thread is spawned to write the data asynchronously. The data is sent to
 the worker thread. 2. The worker checks for the presence of a lockfile (herein
 further detailed). If the lockfile exists and is owned by an active process,
@@ -189,8 +186,8 @@
 situations where a one-off is (more) likely to be employed. Use Cases --------
 - The target use-case is software tools for Mozilla, or, more generally, a
 software index. For this case, the default fields uses are given in the
 paste.ini file: usage, author, type, language. More fields may be added to the
 running instance in the future. However, the classifier classification can be
 used for a wide variety of web-locatable resources. A few examples: * songs:
 artist, album, genre, instruments * de.li.cio.us: type, media, author, site
-Resources --------- * http://readthedocs.org/ Platform: UNKNOWN
+Resources --------- * http://readthedocs.org/
```

### Comparing `toolk0s-0.4/setup.py` & `toolk0s-0.4.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 from setuptools import setup
 
-try:
-    description = file('README.txt').read()
-except IOError:
-    description = ''
+description = "a place to list links + tools",
 
-version = "0.4"
+# :( `twine check` does not like the README
+# because restructured text changed their tbale format
+# https://sublime-and-sphinx-guide.readthedocs.io/en/latest/tables.html
+#try:
+#    description = open('README.txt').read()
+#except IOError:
+#    description = ''
+long_description = description
+
+version = "0.4.2"
 
 # dependencies
 dependencies = [
     'WebOb',
     'tempita',
     'paste',
     'pastescript', # technically optional, but here for ease of install
     'whoosh >= 2.5',
     'couchdb',
     'docutils',
     'pyloader',
     'theslasher',
-    'pyes == 0.15',
+    'pyes',
     ]
 
 setup(name='toolk0s',
       version=version,
-      description="a place to list links + tools",
-      long_description=description,
+      description=description,
+      long_description=long_description,
       classifiers=[], # Get strings from http://www.python.org/pypi?%3Aaction=list_classifiers
       author='Jeff Hammel',
-      author_email='jhammel@mozilla.com',
+      author_email='k0scist@gmail.com',
       url='http://k0s.org/hg/toolbox/',
       license="MPL",
       packages=['toolbox'],
       include_package_data=True,
       zip_safe=False,
       install_requires=dependencies,
       entry_points="""
@@ -39,8 +45,8 @@
       [console_scripts]
       toolbox-convert-model = toolbox.model:convert
       toolbox-serve = toolbox.factory:main
 
       [paste.app_factory]
       toolbox = toolbox.factory:paste_factory
       """,
-      )
+)
```

### Comparing `toolk0s-0.4/test/test.py` & `toolk0s-0.4.2/test/test.py`

 * *Files identical despite different names*

### Comparing `toolk0s-0.4/toolbox/dispatcher.py` & `toolk0s-0.4.2/toolbox/dispatcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
 request dispatcher WSGI app:
 data persisting across requests should go here
 """
 
 import os
 
-from handlers import CreateProjectView
-from handlers import DeleteProjectHandler
-from handlers import FieldView
-from handlers import ProjectView
-from handlers import QueryView
-from handlers import TagsView
-from handlers import AboutView
-from handlers import NotFound
+from .handlers import CreateProjectView
+from .handlers import DeleteProjectHandler
+from .handlers import FieldView
+from .handlers import ProjectView
+from .handlers import QueryView
+from .handlers import TagsView
+from .handlers import AboutView
+from .handlers import NotFound
 
-from model import models
-from util import strsplit
+from .model import models
+from .util import strsplit
 from webob import Request, Response, exc
 
 here = os.path.dirname(os.path.abspath(__file__))
 
 class Dispatcher(object):
     """toolbox WSGI app which dispatchers to associated handlers"""
 
@@ -47,19 +47,19 @@
         # set instance parameters from kw and defaults
         for key in self.defaults:
             setattr(self, key, kw.pop(key, self.defaults[key]))
         if self.item_plural is None:
             self.item_plural = self.item_name + 's'
 
         # should templates be reloaded?
-        if isinstance(self.reload, basestring):
+        if isinstance(self.reload, str):
             self.reload = self.reload.lower() == 'true'
 
         # model: backend storage and associated methods
-        if 'fields' in kw and isinstance(kw['fields'], basestring):
+        if 'fields' in kw and isinstance(kw['fields'], str):
             # split fields if given as a string
             kw['fields'] = strsplit(kw['fields'])
         if hasattr(self.model_type, '__call__'):
             model = self.model_type
         elif self.model_type in models:
             model = models[self.model_type]
         else:
@@ -97,15 +97,15 @@
                     self.reserved.add(handler.handler_path[0])
 
     def __call__(self, environ, start_response):
 
         # get a request object
         request = Request(environ)
 
-        # get the path 
+        # get the path
         path = request.path_info.strip('/').split('/')
         if path == ['']:
             path = []
         request.environ['path'] = path
 
         # load any new data
         self.model.load()
```

### Comparing `toolk0s-0.4/toolbox/factory.py` & `toolk0s-0.4.2/toolbox/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/usr/bin/env python
 
 """
 WSGI -> HTTP server factories for toolbox
 """
 
+import argparse
 import os
 import sys
 
-from dispatcher import Dispatcher
+from .dispatcher import Dispatcher
 from paste.urlparser import StaticURLParser
 from pkg_resources import resource_filename
 from theslasher import TheSlasher
 
+
 class PassthroughFileserver(object):
     """serve files if they exist"""
 
     def __init__(self, app, directory):
         self.app = app
         self.directory = directory
         self.fileserver = StaticURLParser(self.directory)
@@ -42,39 +44,39 @@
 def wsgiref_factory(host='0.0.0.0', port=8080):
     """wsgiref factory; for testing only"""
 
     from wsgiref import simple_server
     app = Dispatcher()
     app = PassthroughFileserver(app, resource_filename(__name__, 'static'))
     server = simple_server.make_server(host=host, port=int(port), app=app)
-    fqdn = '127.0.0.1' if host =='0.0.0.0' else host
-    print "Serving toolbox at http://%s:%d/" % (fqdn, port)
+    fqdn = '127.0.0.1' if host == '0.0.0.0' else host
+    print("Serving toolbox at http://%s:%d/" % (fqdn, port))
     server.serve_forever()
 
 
 # WSGI factories available
 factories = {'paste': paste_factory,
              'wsgiref': wsgiref_factory}
 
 def main(args=sys.argv[1:]):
     """CLI entry point"""
 
     # parse command line
     usage = '%prog [options]'
-    import argparse
+
     parser = argparse.ArgumentParser(usage=usage, description=__doc__.strip())
     parser.add_argument('--factory', default='wsgiref',
                         choices=factories.keys(),
                         help="factory to use")
     parser.add_argument('--port', type=int, default=8080,
                         help="port to serve on")
     args = parser.parse_args()
 
     # serve toolbox
     factory = factories[args.__dict__.pop('factory')]
     factory_args = args.__dict__
-    print "Serving using factory: %s" % getattr(factory, '__name__', str(factory))
-    print "Factory arguments: %s" % factory_args
+    print("Serving using factory: %s" % getattr(factory, '__name__', str(factory)))
+    print("Factory arguments: %s" % factory_args)
     factory(**factory_args)
 
 if __name__ == '__main__':
     main()
```

### Comparing `toolk0s-0.4/toolbox/handlers.py` & `toolk0s-0.4.2/toolbox/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 these are instantiated for every request, then called
 """
 
 import cgi
 import os
 from datetime import datetime
 from pkg_resources import resource_filename
-from urllib import quote as _quote
-from urlparse import urlparse
-from util import strsplit
-from util import JSONEncoder
+from urllib.parse import quote as _quote
+from urllib.parse import urlparse
+from .util import strsplit
+from .util import JSONEncoder
 from webob import Response, exc
 from tempita import HTMLTemplate
 from time import time
 
 # this is necessary because WSGI stupidly follows the CGI convention wrt encoding slashes
 # http://comments.gmane.org/gmane.comp.web.pylons.general/5922
 encoded_slash = '%25%32%66'
@@ -39,26 +39,26 @@
     handler_path = [] # path elements to match
 
     @classmethod
     def match(cls, app, request):
 
         # check the method
         if request.method not in cls.methods:
-            return None
+            return
 
         # check the path
         if request.environ['path'] != cls.handler_path:
-            return None
+            return
 
         # check the constructor
         try:
             return cls(app, request)
         except HandlerMatchException:
-            return None
-    
+            return
+
     def __init__(self, app, request):
         self.app = app
         self.request = request
         self.check_json() # is this a JSON request?
 
     def __call__(self):
         return getattr(self, self.request.method.title())()
@@ -133,22 +133,22 @@
 
     less = ['css/style.less']
 
     js = ['js/jquery-1.6.min.js',
           'js/less-1.0.41.min.js',
           'js/jquery.timeago.js',
           'js/main.js']
-    
+
     def __init__(self, app, request):
         Handler.__init__(self, app, request)
 
         # add application template_dir if specified
         if app.template_dir:
             self.template_dirs = self.template_dirs[:] + [app.template_dir]
-            
+
         self.data = { 'request': request,
                       'css': self.css,
                       'item_name': self.app.item_name,
                       'item_plural': self.app.item_plural,
                       'less': self.less,
                       'js':  self.js,
                       'site_name': app.site_name,
@@ -158,15 +158,15 @@
                       'link': self.link}
 
     def find_template(self, name):
         """find a template of a given name"""
         # the application caches a dict of the templates if app.reload is False
         if name in self.template_cache:
             return self.template_cache[name]
-        
+
         for d in self.template_dirs:
             path = os.path.join(d, name)
             if os.path.exists(path):
                 template = HTMLTemplate.from_filename(path)
                 if not self.app.reload:
                     self.template_cache[name] = template
                 return template
@@ -190,15 +190,15 @@
     """abstract base class for views of projects"""
 
     js = TempitaHandler.js[:]
     js.extend(['js/jquery.tokeninput.js',
                'js/jquery.jeditable.js',
                'js/jquery.autolink.js',
                'js/project.js'])
-               
+
     less = TempitaHandler.less[:]
     less.extend(['css/project.less'])
 
     css = TempitaHandler.css[:]
     css.extend(['css/token-input.css',
                 'css/token-input-facebook.css'])
 
@@ -228,15 +228,15 @@
         """return a string representation of a timestamp"""
         format_string = '%Y-%m-%dT%H:%M:%SZ'
         return datetime.utcfromtimestamp(timestamp).strftime(format_string)
 
 
 class QueryView(ProjectsView):
     """general index view to query projects"""
-    
+
     template = 'index.html'
     methods = set(['GET'])
 
     def __init__(self, app, request):
         ProjectsView.__init__(self, app, request)
 
         # pop non-query parameters;
@@ -258,17 +258,17 @@
             if search:
                 sort_type = 'search'
             else:
                 # default
                 sort_type = '-modified'
         self.data['sort_type'] = sort_type
         if sort_type != 'search':
-            # preserve search order results 
+            # preserve search order results
             self.sort(sort_type)
-            
+
         self.data['fields'] = self.app.model.fields()
         self.data['title'] = self.app.site_name
 
 
 class ProjectView(ProjectsView):
     """view of a particular project"""
 
@@ -432,35 +432,34 @@
                                           for name in project_set])
 
     def Post(self):
         field = self.data['field']
         for key in self.request.POST.iterkeys():
             value = self.request.POST[key]
             self.app.model.rename_field_value(field, key, value)
-        
         return self.redirect(field, anchor=value)
-        
+
     def get_json(self):
         return self.data['values']
 
-        
+
 class CreateProjectView(TempitaHandler):
     """view to create a new project"""
 
     template = 'new.html'
     methods = set(['GET', 'POST'])
     handler_path = ['new']
     js = TempitaHandler.js[:]
     js.extend(['js/jquery.tokeninput.js',
                'js/queryString.js',
                'js/new.js'])
-               
+
     less = TempitaHandler.less[:]
     less.extend(['css/new.less'])
-    
+
     css = TempitaHandler.css[:]
     css.extend(['css/token-input.css',
                 'css/token-input-facebook.css'])
 
     def __init__(self, app, request):
         TempitaHandler.__init__(self, app, request)
         self.data['title'] = 'Add a ' + app.item_name
@@ -530,15 +529,15 @@
 
 
 class DeleteProjectHandler(Handler):
 
     methods = set(['POST'])
     handler_path = ['delete']
 
-    def Post(self):        
+    def Post(self):
         post_data = self.post_data()
         project = post_data.get('project')
         if project:
             try:
                 self.app.model.delete(project)
             except:
                 pass # XXX better than internal server error
@@ -564,15 +563,15 @@
         ommitted = dict([(field, set()) for field in fields])
         for name in omit:
             project = self.app.model.project(name)
             if not project:
                 continue
             for field in fields:
                 ommitted[field].update(project.get(field, []))
-            
+
         for project in self.app.model.get():
             if project in omit:
                 continue
             # TODO: cache this for speed somehow
             # possibly at the model level
             for field in fields:
                 for value in project.get(field, []):
```

### Comparing `toolk0s-0.4/toolbox/model.py` & `toolk0s-0.4.2/toolbox/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 """
 models for toolbox
 """
 
 import couchdb
+import json
 import os
 import pyes
 import sys
+
 from copy import deepcopy
-from search import WhooshSearch
 from time import time
-from util import str2filename
-
-try:
-    import json
-except ImportError:
-    import simplejson as json
+from .search import WhooshSearch
+from .util import str2filename
 
 # TODO: types of fields:
 # - string: a single string: {'type': 'string', 'name': 'name', 'required': True}
 # - field: a list of strings: {'type': 'field', 'name', 'usage'}
 # - dict: a subclassifier: {'type': '???', 'name': 'url', 'required': True}
 # - computed values, such as modified
 
@@ -109,25 +106,24 @@
 
 class MemoryCache(ProjectsModel):
     """
     sample implementation keeping everything in memory
     """
 
     def __init__(self, fields=None, whoosh_index=None):
-        
+
         ProjectsModel.__init__(self, fields=fields, whoosh_index=whoosh_index)
 
         # indices
         self._projects = {}
         self.index = {}
-        
         self.load()
 
     def update(self, project, load=False):
-        
+
         if project['name'] in self._projects and project == self._projects[project['name']]:
             return # nothing to do
         if not load:
             project['modified'] = time()
         if self._fields is None:
             fields = [i for i in project if i not in self.reserved]
             self.field_set.update(fields)
@@ -139,15 +135,15 @@
                 if not _set:
                     self.index[field].pop(key)
             if field not in project:
                 continue
             project[field] = list(set([i.strip() for i in project[field] if i.strip()]))
             index = self.index.setdefault(field, {})
             values = project[field]
-            if isinstance(values, basestring):
+            if isinstance(values, str):
                 values = [values]
             for value in values:
                 index.setdefault(value, set()).update([project['name']])
         self._projects[project['name']] = deepcopy(project)
         self.update_search(project)
         if not load:
             self.save(project)
@@ -161,15 +157,15 @@
         if search:
             results = self.search(search)
             order = dict([(j,i) for i,j in enumerate(results)])
         else:
             results = self._projects.keys()
         results = set(results)
         for key, values in query.items():
-            if isinstance(values, basestring):
+            if isinstance(values, str):
                 values = [values]
             for value in values:
                 results.intersection_update(self.index.get(key, {}).get(value, set()))
         if order:
             # preserve search order
             results = sorted(list(results), key=lambda x: order[x])
         return [deepcopy(self._projects[project]) for project in results]
@@ -193,15 +189,15 @@
         del self._projects[project]
         for field, classifiers in self.index.items():
             for key, values in classifiers.items():
                 classifiers[key].discard(project)
                 if not classifiers[key]:
                     del classifiers[key]
         self.search.delete(project)
-        
+
     def load(self):
         """for subclasses; in memory, load nothing"""
 
     def save(self, project):
         """for subclasses; in memory, save nothing"""
 
 
@@ -228,35 +224,34 @@
     def load(self):
         """load JSON from the directory"""
         for i in os.listdir(self.directory):
             if not i.endswith('.json'):
                 continue
             filename = os.path.join(self.directory, i)
             try:
-                project = json.loads(file(filename).read())
+                project = json.loads(open(filename).read())
             except:
-                print 'File: ' + i
+                print('File: {}'.format(i))
                 raise
             self.files[project['name']] = i
             self.update(project, load='modified' in project)
 
     def save(self, project):
 
         filename = self.files.get(project['name'])
         if not filename:
             filename = str2filename(project['name']) + '.json'
         filename = filename.encode('ascii', 'ignore')
         filename = os.path.join(self.directory, filename)
         try:
-            f = file(filename, 'w')
-        except Exception, e:
-            print filename, repr(filename)
+            with open(filename, 'w') as f:
+                f.write(json.dumps(project))
+        except Exception as e:
+            print('{} {}'.format(filename, repr(filename)))
             raise
-        f.write(json.dumps(project))
-        f.close()
 
 
 class ElasticSearchCache(MemoryCache):
     """
     store json in ElasticSearch
     """
 
@@ -360,15 +355,15 @@
         for id in self.db:
             doc = self.db[id]
             try:
                 project = doc['project']
             except KeyError:
                 continue   # it's prob a design doc
             self.update(project, load=True)
-            
+
     def save(self, project):
         name = project['name']
         try:
              updated = self.db[name]
         except:
              updated = {}
         updated['project'] = project
@@ -399,29 +394,29 @@
                       help="list arguments for a model")
 
     options, args = parser.parse_args(args)
 
     # process global options
     if options.list_models:
         for name in sorted(models.keys()):
-            print name # could conceivably print docstring
+            print(name)
         parser.exit()
     if options.list_args:
         if not options.list_args in models:
             parser.error("Model '%s' not found. (Choose from: %s)" % (options.list_args, models.keys()))
         ctor = models[options.list_args].__init__
         import inspect
         argspec = inspect.getargspec(ctor)
         defaults = [[i, None] for i in argspec.args[1:]] # ignore self
         for index, value in enumerate(reversed(argspec.defaults), 1):
             defaults[-index][-1] = value
         defaults = [[i,j] for i, j in defaults if i != 'fields']
-        print '%s arguments:' % options.list_args
+        print('%s arguments:' % options.list_args)
         for arg, value in defaults:
-            print ' -%s %s' % (arg, value or '')
+            print(' -%s %s' % (arg, value or ''))
         parser.exit()
 
     # parse models and their ctor args
     sects = []
     _models = []
     for arg in args:
         if arg.startswith('-'):
```

### Comparing `toolk0s-0.4/toolbox/search.py` & `toolk0s-0.4.2/toolbox/search.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,60 +48,40 @@
             raise
 
         # add keywords
         for key in kw:
             if key not in self.keywords:
                 writer.add_field(key, fields.KEYWORD)
                 self.keywords.add(key)
-            if not isinstance(kw[key], basestring):
+            if not isinstance(kw[key], str):
                 kw[key] = ' '.join(kw[key])
-            kw[key] = unicode(kw[key])
-
-        # convert to unicode for whoosh
-        # really whoosh should do this for us
-        # and really python should be unicode-based :(
-        name = unicode(name)
-        description = unicode(description)
+            kw[key] = str(kw[key])
 
         writer.update_document(name=name, description=description, **kw)
         writer.commit()
 
     def delete(self, name):
         """delete a document of a given name"""
         writer = self.ix.writer()
-        name = unicode(name)
         writer.delete_by_term('name', name)
         writer.commit()
 
     def __call__(self, query):
         """search"""
-        query = unicode(query)
         query_parser = QueryParser("description", schema=self.ix.schema)
         myquery = query_parser.parse(query)
 
-# Old code: too strict
-#        extendedquery = Or([myquery] +
-#                           [Term(field, query) for field in self.keywords])
-
 
         # New code: too permissive
-#        extendedquery = [myquery]
         excluded = set(['AND', 'OR', 'NOT'])
         terms = [i for i in query.split() if i not in excluded]
-#        for field in self.keywords:
-#            extendedquery.extend([Term(field, term) for term in terms])
-#        extendedquery = Or(extendedquery)
-
-        # Code should look something like
-        #Or([myquery] + [Or(
-        # extendedquery = [myquery]
         extendedquery = And([Or([myquery] + [Term('description', term), Term('name', term)] +
                                 [Term(field, term) for field in self.keywords]) for term in terms])
 
         # perform the search
         searcher = self.ix.searcher()
         return [i['name'] for i in searcher.search(extendedquery, limit=None)]
-        
+
     def __del__(self):
         if self.tempdir:
             # delete the temporary directory, if present
             shutil.rmtree(self.index)
```

### Comparing `toolk0s-0.4/toolbox/util.py` & `toolk0s-0.4.2/toolbox/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,8 +52,8 @@
     # test date encoding
     from datetime import datetime
     testjson['date'] = datetime.now()
 
     # test set encoding
     testjson['set'] = set([1,2,3,2])
 
-    print json.dumps(testjson, cls=JSONEncoder)
+    print(json.dumps(testjson, cls=JSONEncoder))
```

