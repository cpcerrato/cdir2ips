Description
================

This script takes a CDIR specified by command line arguments, displays info about it and returns the corresponding IP range for it.


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
Feel free to place the script in any path you want.

Usage
=====

Shows information specified by command line arguments, furthermore, it expands CDIR into an IP range.

```bash
Usage: cdir2ips -c <ADDRESS>[/<NETMASK>]

    -h Print this help.
    -c CDIR argument.
    -e expand IP list included in CDIR argument.

```

Examples:

Display CDIR info:
```bash
$ cdir2ips -c 173.194.0.0/28

        Address:        173.194.0.0
        Netmask:        255.255.255.240 = 28
        Network:        173.194.0.0/28
        First Host:     173.194.0.1
        Last Host:      173.194.0.14
        Broadcast:      173.194.0.15
        Hosts:          14
        Class:          Class B

```

Expands CDIR into an IP range:
```bash
$ cdir2ips -c 173.194.0.0/28 -e 
173.194.0.0
173.194.0.1
173.194.0.2
173.194.0.3
173.194.0.4
173.194.0.5
173.194.0.6
173.194.0.7
173.194.0.8
173.194.0.9
173.194.0.10
173.194.0.11
173.194.0.12
173.194.0.13
173.194.0.14
173.194.0.15
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
