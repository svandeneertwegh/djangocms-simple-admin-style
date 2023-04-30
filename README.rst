=============================
django CMS Simple Admin Style
=============================

|pypi| |django| |djangocms| |djangocms4|

This is an alternative for the `django CMS Admin Style <https://github.com/django-cms/djangocms-admin-style>``.

It does only mildly adapt Django's admin style but changes fonts, colors, and some form rendering to better fit into the django CMS look and feel.


Documentation
=============

See ``REQUIREMENTS`` in the `setup.py <https://github.com/divio/djangocms-admin-style/blob/master/setup.py>`_
file for additional dependencies:

Installation
------------

For a manual install:

* run ``pip install djangocms-simple-admin-style``
* add ``djangocms_simple_admin_style`` to your ``INSTALLED_APPS`` just before ``'django.contrib.admin'``


Configuration
-------------

The django CMS Admin Style overrides django admin's ``base_site.html``,
but you can still partially customize this page. Look at the source of
``templates/admin/base_site.html`` and override the templates that are included in various blocks. For example, you can add your own CSS in
``templates/admin/inc/extrastyle.html``.

To **compile CSS** run the following commands using **node 16**:

* ``nvm use``
* ``npm install``
* ``gulp``

For further options have a look at the ``gulpfile.js``.


.. |pypi| image:: https://badge.fury.io/py/djangocms-admin-style.svg
    :target: http://badge.fury.io/py/djangocms-simple-admin-style
.. |django| image:: https://img.shields.io/badge/django-2.2%2B-blue.svg
    :target: https://www.djangoproject.com/
.. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.6%2B-blue.svg
    :target: https://www.django-cms.org/
.. |djangocms4| image:: https://img.shields.io/badge/django%20CMS-4-blue.svg
    :target: https://www.django-cms.org/