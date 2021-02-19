# d-mumblequery

**Query a Mumble server.**

A small D program to query Mumble servers using the
[Mumble UDP query packet](https://wiki.mumble.info/wiki/Protocol#UDP_Ping_packet).

## Build

You must have [Dub](https://dub.pm/) and a [compatible D compiler](https://dlang.org/download.html) installed. With the correct
tooling, d-mumblequery can be built by running `dub build -b release`.

## Usage

Supply the list of hosts, with optional port numbers, as command-line arguments.

```
Usage: ./mumblequery [<host[:port]>...]
```

Example:

```
$ ./mumblequery hedonics.org extremelycorporate.ca
Server: hedonics.org (45.56.66.42:64738)
Version: 1.3.0
Users: 5/500
Bandwidth: 326000 b/s

Server: extremelycorporate.ca (174.95.206.94:64738)
Version: 1.4.0
Users: 6/50
Bandwidth: 256000 b/s

```

# Copyright

d-mumblequery is protected by copyright and is licensed under the MIT License, see `LICENSE.txt` for more details.

Copyright &copy; 2021 - Maxwell Cody [<maxwell&commat;cody&period;sh>](mailto:maxwell&commat;cody&period;sh)