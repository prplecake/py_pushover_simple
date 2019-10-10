py\_pushover\_simple
==================

[![PyPI version](https://badge.fury.io/py/py-pushover-simple.svg)](https://badge.fury.io/py/py-pushover-simple)

This is a very simple python pushover wrapper for sending quick messages from command line scripts.

## Installation

1. Obtain the code:

    Download from PyPi *(recommended)*:

        python3 -m pip install py-pushover-simple

    or, clone the repository:

        git clone https://git.sr.ht/~mjorgensen/py_pushover_simple

2. Add it to your script:

        from py_pushover_simple import pushover

        def send_message(message):
            p = pushover.Pushover()
            p.user = 'user key'
            p.token = 'app token'

            p.sendMessage(message)

For a working demo, see [ippush.py] from the [ip_push] project.

## Usage

`py_pushover_simple` can be used on the command line:

For a full list of arguments:

    $ python -m py_pushover_simple.pushover -h
    usage: pushover.py [-h] [-u <string>] [-t <string>]

    optional arguments:
      -h, --help   show this help message and exit
      -u <string>  pushover user token
      -t <string>  pushover app token

[ippush.py]:https://git.sr.ht/~mjorgensen/ip_push/tree/master/ippush.py
[ip_push]:https://git.sr.ht/~mjorgensen/ip_push/

## Resources

Discussion and patches are welcome at my public inbox: 
[~mjorgensen/public-inbox@lists.sr.ht][list]. Please use `--send-prefix PATCH
py_pushover_simple` for clarity when sending patches.

Bugs, issues, and tasks are in the tracker:
[~mjorgensen/py\_pushover\_simple][todo]

This project is licensed under the terms of the MIT license.

[man]: https://man.sr.ht/~mjorgensen/py_pushover_simple
[todo]: https://todo.sr.ht/~mjorgensen/py_pushover_simple
[list]: https://lists.sr.ht/~mjorgensen/public-inbox
