Installation
============

1. Download from PyPi::

    python3 -m pip install py_pushover_simple


2. Add it to your script::

    from py_pushover_simple import pushover

    def send_message(message):
       p = pushover.Pushover()
       p.user = 'user key'
       p.token = 'app_token'

       p.sendMessage(message)

For a working demo, see `ippush.py`_.

.. _ippush.py: https://code.jrgnsn.net/matthew/ip_push/src/branch/master/ippush.py
