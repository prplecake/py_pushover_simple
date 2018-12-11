py_pushover_simple
==================


.. image:: https://img.shields.io/github/issues/mtthwjrgnsn/py_pushover_simple.svg
    :alt: GitHub issues
    :target: https://github.com/mtthwjrgnsn/py_pushover_simple/issues


.. image:: https://img.shields.io/github/license/mtthwjrgnsn/py_pushover_simple.svg
    :alt: GitHub license
    :target: https://github.com/mtthwjrgnsn/py_pushover_simple/blob/master/LICENSE


.. image:: https://badge.fury.io/py/py-pushover-simple.svg
    :target: https://badge.fury.io/py/py-pushover-simple.svg
    :alt: PyPi Version

.. image:: https://readthedocs.org/projects/py-pushover-simple/badge/?version=latest
    :target: https://py-pushover-simple.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status


This is a very simple python pushover wrapper for sending quick messages from command line scripts.

Installation Instructions
-------------------------

1. Download from PyPi::
    
    python3 -m pip install py_pushover_simple

2. Add it to your script::

    from py_pushover_simple import pushover

    def send_message(message):
        p = pushover.Pushover()
        p.user = 'user_key'
        p.token = 'app_token'

        p.sendMessage(message)
    

For a working demo, see `ippush.py <https://github.com/mtthwjrgnsn/ip_push/blob/master/ippush.py>`_ from the `ip_push <https://github.com/mtthwjrgnsn/ip_push/>`_ project.

Debugging
---------

``py_pushover_simple`` has some simple debugging features:

For a full list of arguments::

    $ python -m py_suchover_simple.pushover -h
    usage: pushover.py [-h] [-u <string>] [-t <string>]
    
    optional arguments:
      -h, --help   show this help message and exit
      -u <string>  pushover user token
      -t <string>  pushover app token


Contributors
------------

* Matthew Jorgensen

License
-------

This project is licensed inder the terms of the MIT license.
