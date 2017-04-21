biosocks2
=========

Simple efficient socks5 server

1. Edit the settings at the top of the biosocks2.cpp file.
2. Compile with: g++ biosocks2.cpp -O2 -pthread -o biosocks2
3. Run as ./biosocks

NOTE: You can optionally pass -f switch to run in foreground for debugging.


## Docker

MANDATORY ENV:
```
LISTEN_IP
LOGIN
PASSWORD
```

Exposed port: `8080`

### Example usage:
```
docker run --rm -p 8080:8080 -e LISTEN_IP=0.0.0.0 -e LOGIN=foo -e PASSWORD=bar sbani/biosocks2
```
