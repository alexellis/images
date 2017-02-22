### Squid for Docker on Alpine Linux

Squid provides a HTTP/HTTPs proxy with connect and tunnelling abilities

This Dockerfile will enable you to share your internet connection without having to use IPTables / Firewalls / ICS Internet Connection Sharing etc.

Usage:

```
$ docker build -t alexellis2/squid:latest .
$ docker run --name proxy -p 3128:3128 -d alexellis2/squid:latest
$ curl -v google.com -x localhost:3128
```
