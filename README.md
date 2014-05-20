cdir2ips
================

This script take a cdir specified by command line arguments display info and return ip range belongs to.


Installation
============

Checkout the script:

```bash
$ wget https://raw.github.com/cperezcerrato/cdir2ips/master/cdir2ips /usr/local/bin/
```

Set permissions:
```bash
$ chmod +x /usr/local/bin/cdir2ips
```
Feel free to put the script in the path you want.

Usage
=====

Show information specified by command line arguments furthermore it expand cdir into a ip range.

```bash
Usage: cdir2ips -c <ADDRESS>[/<NETMASK>]

    -h Print this help.
    -c CDIR argument.
    -e expand IP list included in CDIR argument.

```

License and Author
==================
Copyright (C) May, 2014 Carlos Perez Cerrato <cperezcerrato@gmail.com>

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0
Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
