Test PM2 config

\[{

"name"      : "LD Node 8000",

"script"    : "bin/solid.js",

"args"      : "start -v --no-reject-unauthorized",

"env": {

```
"DEBUG": "\*",

"iNODE\_TLS\_REJECT\_UNAUTHORIZED": "0"
```

}

}\]



New docs allow deployment and ecosystems

https://pm2.io/doc/en/runtime/guide/easy-deploy-with-ssh/



