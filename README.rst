===============
How to Develope
===============

.. image:: https://github.com/siongui/master-mingyi/workflows/Pelican%20site%20CI/badge.svg
    :target: https://github.com/siongui/master-mingyi/blob/master/.github/workflows/pelican.yml


Development Tool: Pelican_ (static site generator written in Python)

Development Environment: `Ubuntu 22.04`_


First-time Setup
----------------

1. Install git_ and pip_:

   .. code-block:: bash

     $ sudo apt-get install git
     $ sudo apt-get install python-pip

2. Install language packages to add locale (English, Traditional Chinese, and
   Thai in this example):

   .. code-block:: bash

     $ sudo apt-get install language-pack-en
     $ sudo apt-get install language-pack-zh-hant
     $ sudo apt-get install language-pack-th

3. git clone source code:

   .. code-block:: bash

     $ cd
     $ mkdir dev
     $ cd ~/dev/
     $ git clone https://github.com/siongui/pelican-template.git YOUR_REPO

4. Install Python tools:

   .. code-block:: bash

     $ cd ~/dev/YOUR_REPO/
     $ sudo pip install -r requirements.txt

5. Install Pelican `i18n_subsites`_ plugin and download `normalize.css`_:

   .. code-block:: bash

     $ cd ~/dev/YOUR_REPO/
     $ make download

6. Generate CSS file:

   .. code-block:: bash

     $ cd ~/dev/YOUR_REPO/
     $ make scss


Daily Development
-----------------

.. code-block:: bash

    # start edit and develope
    $ cd ~/dev/YOUR_REPO/
    # re-generate the website and start dev server
    $ make
    # open your browser and preview the website at http://localhost:8000/


UNLICENSE
---------

All works, including posts and code, of Siong-Ui Te are released in public domain.
Please see UNLICENSE_.


References
----------

.. [1] | JINJA_FILTERS in `Settings — Pelican documentation <http://docs.getpelican.com/en/latest/settings.html>`_
       | `Jinja custom filters documentation <http://jinja.pocoo.org/docs/dev/api/#custom-filters>`_

.. [2] `法眼寺 <http://www.fayansi.org/>`_

.. _Pelican: http://blog.getpelican.com/
.. _Ubuntu 22.04: https://releases.ubuntu.com/22.04/
.. _UNLICENSE: http://unlicense.org/
.. _git: https://git-scm.com/
.. _pip: https://pypi.python.org/pypi/pip
.. _i18n_subsites: https://github.com/getpelican/pelican-plugins/tree/master/i18n_subsites
.. _normalize.css: https://necolas.github.io/normalize.css/
.. _Travis CI: https://travis-ci.org/
.. _Getting started - Travis CI: https://docs.travis-ci.com/user/getting-started/
.. _global: https://docs.travis-ci.com/user/environment-variables/#Global-Variables
.. _secure: https://docs.travis-ci.com/user/environment-variables/#Encrypted-Variables
.. _environment variable: https://docs.travis-ci.com/user/environment-variables/
.. _personal access token: https://help.github.com/articles/creating-an-access-token-for-command-line-use/
.. _Travis CI command line client: https://github.com/travis-ci/travis.rb
.. _Google Adsense: https://www.google.com/search?q=Google+AdSense
