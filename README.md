# alpine-node-red-lego
 Node-RED with Lego SSL Cert Renewal in Alpine Linux

## Purpose
This docker is designed to provide automatic SSL Certificate renewal via Lego which uses ACME automatic registration and renewal to maintain a valid certificate


## /data/settings.js
Add entry to define certificate locations and refresh interval
```	https: {
      key: require("fs").readFileSync('/data/certs/server.key'),
      cert: require("fs").readFileSync('/data/certs/server.crt'),
      httpsRefreshInterval: 1
    },```
	