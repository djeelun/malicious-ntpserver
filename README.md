malicious-ntpserver
=========
forked from limifly/ntpserver

```
usage: ntpserver.py [-h] [--listenPort LISTENPORT] [--isMalicious ISMALICIOUS] monitorList

positional arguments:
  monitorList           path to text file of space-separated ip addresses

optional arguments:
  -h, --help            show this help message and exit
  --listenPort LISTENPORT
                        port to listen on (default 123)
  --isMalicious ISMALICIOUS
                        indicates whether the server should be malicious (default True)
```

### What is this?
Script to run an NTP server that will respond to requests from a list of IPs with a benign response, and all other IPs with a malicious response. Made this for a small research project, trying to trick NTP Pool monitors into thinking a server is benign when it is not.

By default, the server will act malicious. To make it benign, use the `--isMalicious False` flag.

---

Original README.md below

ntpserver
=========

A Python based ntp server.

Tested on Linux and Windows7.

Based on ntplib(https://pypi.python.org/pypi/ntplib/), thanks for their work.

If you have any question, please contact me at limifly@gmail.com.
