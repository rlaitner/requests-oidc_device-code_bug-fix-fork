Requests-OIDC
=================

.. inclusion-marker-do-not-remove

Implements a simple API for creating a requests ``Session`` that
manages your OIDC-discovered OAuth2 session for you.

::

   pip install requests-oidc

.. code-block:: python

   from requests_oidc import make_auth_code_session
   from requests_oidc.plugins import OSCachedPlugin

   oidc_url = "https://your-oidc-provider.com/.well-known/openid-configuration"
   client_id = "your-app"
   port = 8675
   scope = ["openid", "email", "profile"]

   plugin = OSCachedPlugin("your-app", "your-company")



   session = make_auth_code_session(oidc_url, client_id, port, scope, plugin=plugin)


.. list-table::

   * - Package
     - |pypi| |license| |py status| |formats| |python| |py impls| |downloads|
   * - build
     - |checks| |rtd build| |coverage|
   * - Git
     - |last commit| |commit activity| |commits since| |issues| |prs|

.. |pypi| image:: https://img.shields.io/pypi/v/requests-oidc
   :target: https://pypi.org/project/requests-oidc/
   :alt: PyPI
   
.. |downloads| image:: https://img.shields.io/pypi/dm/requests-oidc
   :target: https://pypistats.org/packages/requests-oidc
   :alt: PyPI - Downloads

.. |formats| image:: https://img.shields.io/pypi/format/requests-oidc
   :target: https://pypi.org/project/requests-oidc/
   :alt: PyPI - Format

.. |py status| image:: https://img.shields.io/pypi/status/requests-oidc
   :target: https://pypi.org/project/requests-oidc/
   :alt: PyPI - Status

.. |py impls| image:: https://img.shields.io/pypi/implementation/requests-oidc
   :target: https://pypi.org/project/requests-oidc/
   :alt: PyPI - Implementation

.. |python| image:: https://img.shields.io/pypi/pyversions/requests-oidc
   :target: https://pypi.org/project/requests-oidc/
   :alt: PyPI - Python Version

.. |license| image:: https://img.shields.io/github/license/tsweeney-dust/requests-oidc
   :target: https://github.com/tsweeney-dust/requests-oidc
   :alt: GitHub

.. |checks| image:: https://img.shields.io/github/checks-status/tsweeney-dust/requests-oidc/main?logo=github
   :target: https://github.com/tsweeney-dust/requests-oidc
   :alt: GitHub branch checks state

.. |rtd build| image:: https://img.shields.io/readthedocs/requests-oidc
   :target: https://requests-oidc.readthedocs.io/en/latest/?badge=latest
   :alt: Read the Docs

.. |coverage| image:: https://coveralls.io/repos/github/tsweeney-dust/requests-oidc/badge.svg?branch=main
   :target: https://coveralls.io/github/tsweeney-dust/requests-oidc?branch=main
   :alt: Coverage

.. |last commit| image:: https://img.shields.io/github/last-commit/tsweeney-dust/requests-oidc
   :target: https://github.com/tsweeney-dust/requests-oidc
   :alt: GitHub last commit

.. |commit activity| image:: https://img.shields.io/github/commit-activity/m/tsweeney-dust/requests-oidc
   :target: https://github.com/tsweeney-dust/requests-oidc
   :alt: GitHub commit activity

.. |commits since| image:: https://img.shields.io/github/commits-since/tsweeney-dust/requests-oidc/latest
   :target: https://github.com/tsweeney-dust/requests-oidc
   :alt: GitHub commits since latest release (by SemVer)

.. |issues| image:: https://img.shields.io/github/issues/tsweeney-dust/requests-oidc
   :target: https://github.com/tsweeney-dust/requests-oidc/issues
   :alt: GitHub issues

.. |prs| image:: https://img.shields.io/github/issues-pr/tsweeney-dust/requests-oidc
   :target: https://github.com/tsweeney-dust/requests-oidc/pulls
   :alt: GitHub pull requests