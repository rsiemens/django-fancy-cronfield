#######################
Django Fancy Cron Field
#######################
.. image:: https://api.travis-ci.com/rsiemens/django-fancy-cronfield.svg?branch=master
    :target: https://travis-ci.com/rsiemens/django-fancy-cronfield
.. image:: https://img.shields.io/pypi/v/django-fancy-cronfield-alt.svg
    :target: https://pypi.python.org/pypi/django-fancy-cronfield-alt/

A nice and customizable cron field with great, easy to use UI.


********
Features
********

- Cron widget providing nice gentle select UI
- Cron format validation
- Custom django field
- Ability to specify a daily run limit

************
Requirements
************

Fancy cron field requires Django version 1.11 up to 2.2, Python 3.6, 3.7, 3.8, and python-crontab 1.9.5.

************
Installation
************

.. code:: shell

    python -m pip install django-fancy-cronfield-alt

***********
Basic usage
***********

Add `'fancy_cronfield'` to your `INSTALLED_APPS`, then use `CronField` like
any regular model field:

.. code:: python

    from django.db import models

    from fancy_cronfield.fields import CronField


    class MyModel(models.Model):
        timing = CronField()

*******
Credits
*******

* django-fancy-crontab was created by `@saeedsq <https://github.com/saeedsq>`_.
* Crontab API features borrowed from
  `python-crontab <https://code.launchpad.net/python-crontab>`_.
