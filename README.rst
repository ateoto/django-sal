Sal
============

A Django app for managing and sharing recipes.

Installation
------------

To get the latest stable release from PyPi

.. code-block:: bash

    pip install django-sal

To get the latest commit from GitHub

.. code-block:: bash

    pip install -e git+git://github.com/Ateoto/django-sal.git#egg=sal

TODO: Describe further installation steps (edit / remove the examples below):

Add ``sal`` to your ``INSTALLED_APPS``

.. code-block:: python

    INSTALLED_APPS = (
        ...,
        'sal',
    )

Add the ``sal`` URLs to your ``urls.py``

.. code-block:: python

    urlpatterns = patterns('',
        ...
        url(r'^recipes/', include('sal.urls')),
    )

Before your tags/filters are available in your templates, load them by using

.. code-block:: html

	{% load sal_tags %}


Don't forget to migrate your database

.. code-block:: bash

    ./manage.py migrate sal


Usage
-----

TODO: Describe usage or point to docs. Also describe available settings and
templatetags.


Contribute
----------

If you want to contribute to this project, please perform the following steps

.. code-block:: bash

    # Fork this repository
    # Clone your fork
    mkvirtualenv -p python2.7 django-sal
    make develop

    git co -b feature_branch master
    # Implement your feature and tests
    git add . && git commit
    git push -u origin feature_branch
    # Send us a pull request for your feature branch
