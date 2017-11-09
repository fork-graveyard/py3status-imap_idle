# `imap_idle` Module for Py3status

This is an out-of-tree module superseding the `imap` module. *This version is
very experimental* and might crash from time-to-time!

## Installation

1. set up a directory for out-of-tree modules, e.g. `~/.config/i3status/modules/`
2. copy `imap_idle.py` and `imaplib2.py` in your freshly created directory
3. in your `i3` config change the `bar` `status_command` to `--include` said directory; e.g.:    
   `status_command py3status -c ~/.config/i3status/config --include ~/.config/i3status/modules/`
4. in your py3status config rename the `imap` module to `imap_idle` (both in the `order+=` section
   and the configuration section) and add the new setting `use_idle = True`. (see `config.example`)

## Note

This repository contains the `imaplib2` in version 3.5, which has been renamed
from `imaplib2.py3` to `imaplib2.py`. 

## License

This module is based on [`py3status`](https://github.com/ultrabug/py3status)' module `imap` from obb and licensed under 3-clause-BSD (see `LICENSE-py3status`).    
`py3status` by Ultrabug et.al. is released under the three clause BSD license. (see `LICENSE-py3status`)    
[`imaplib2`](https://sourceforge.net/projects/imaplib2/) by Piers Lauder et.al. is released under the CNRI Pyhton License. (see `LICENSE-imaplib2`)    
