.. .. seealso::
..   * :ref:`Installing <installing>`
..   * :ref:`About Ajenti <man-about>`
..   * :ref:`Plugin development <dev-getting-started>`
..   * :ref:`Core development <dev-getting-started-core>`

Ajenti Web Interface Platform
-----------------------------

Ajenti platform includes following products:

* **Ajenti Core**, a Python library, the platform itself including the HTTP server, socket engine and plugin container.
* **Ajenti Panel**, a startup script and a set of stock plugins such as file manager, network configurator and service manager.

Feature Overview
----------------

HTTP Server
===========

* HTTP 1.1 Support.
* Websockets with fallback to XHR polling.
* Fast event-loop based processing.
* Flexible routing.
* Session sandboxing.
* SSL with client certificate authentication.

Performance
===========

* >1000 requests per second.
* 30 MB RAM footprint + 5 MB per session.

API
===

* Highly modular Python API. Everything is a module and can be removed or replaced.
* Builtin webserver API supports routing, file downloads, GZIP, websockets and more.
* Transparent SSL client authorization.
* Plugin architecture
* Dependency injection
* Server-side push and socket APIs.

Security
========

* Pluggable authentication and authorization.
* Stock authenticators: UNIX account, password, SSL client certificate and Mozilla Persona E-mail authentication.
* Unprivileged sessions isolated in separate processes.
* Fail2ban rule

Frontend
========

* Clean, modern and responsive UI. Single-page, no reloads.
* Live data updates and streaming with Socket.IO support.
* Full mobile and tablet support.
* LESS and CSS, CoffeeScript and JavaScript auto-build support.
* Numerous stock directives.
* AngularJS templating.

Platforms
=========

* Debian 9 or later
* Ubuntu Bionic or later
* RHEL 8 or later
* Can be run on other Linux or BSD systems with minimal modifications.
* Supports Python 3.5+.


.. toctree::
   :maxdepth: 1
   :caption: Users
   :hidden:

   man/install.rst
   man/run.rst
   man/security.rst

.. toctree::
   :maxdepth: 1
   :caption: Plugin Developers
   :hidden:

   dev/about.rst
   dev/intro.rst
   dev/multitool.rst
   dev/ui.rst
   dev/resources.rst
   dev/http.rst
   dev/dash-widgets.rst

.. toctree::
  :maxdepth: 1
  :caption: Core Developers
  :hidden:

  dev/intro-core.rst


.. toctree::
   :maxdepth: 1
   :caption: Python API Reference
   :hidden:

   ref/jadi
   ref/aj
   ref/aj.api.http
   ref/aj.api.endpoint
   ref/aj.config
   ref/aj.core
   ref/aj.entry
   ref/aj.http
   ref/aj.plugins


.. toctree::
   :maxdepth: 1
   :caption: Stock Angular components
   :hidden:

   refjs/core
   refjs/ace
   refjs/augeas
   refjs/filesystem
   refjs/passwd
   refjs/services
   refjs/terminal


.. toctree::
   :maxdepth: 1
   :caption: Plugin API Reference
   :hidden:

   ref/aj.plugins.core.api.push
   ref/aj.plugins.core.api.sidebar
   ref/aj.plugins.core.api.tasks
   ref/aj.plugins.augeas.api
   ref/aj.plugins.auth-users.api
   ref/aj.plugins.dashboard.api
   ref/aj.plugins.check_certificates.api
   ref/aj.plugins.datetime.api
   ref/aj.plugins.network.api
   ref/aj.plugins.packages.api
   ref/aj.plugins.power.api
   ref/aj.plugins.services.api
