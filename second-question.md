**How can I run a solid server using HTTP Only?**

Just don't pass any certificate info and HTTP will be chosen.

seeAlso

[https://github.com/solid/node-solid-server/issues/609](https://github.com/solid/node-solid-server/issues/609)

Example config

```
{
  "root": "/home/ruben/tmp/node-solid-server/data",
  "port": "5500",
  "serverUri": "https://drive.verborgh.org",
  "webid": true,
  "mount": "/",
  "configPath": "./config",
  "dbPath": "./.db",
  "idp": false,
  "corsProxy": "/proxy",
  "auth": "tls",
  "certificateHeader": "X-Client-Certificate"
}
```

##### How can I redirect traffic from port 80?

`    "redirectHTTPFrom": 80`



