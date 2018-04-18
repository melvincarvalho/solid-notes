#### **Installilng**

##### Docker

[https://github.com/solid/node-solid-server/pull/607](https://github.com/solid/node-solid-server/pull/607)

the compile image is here: [https://hub.docker.com/r/reto/node-solid-server/](https://hub.docker.com/r/reto/node-solid-server/)

##### Raspberry pi



LetsEncrypt Wildcard

sudo certbot -d "\*.solid.live" --manual --preferred-challenges dns certonly --server https://acme-v02.api.letsencrypt.org/directory

change \_acme-challenge DNS TXT record

hit enter

