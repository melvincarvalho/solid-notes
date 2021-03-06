### FAQ

### Registration

#### How do I create a WebID X.509 certificate?

See : [https://gist.github.com/melvincarvalho/e14753a7137d02d756f19299fed292b4](https://gist.github.com/melvincarvalho/e14753a7137d02d756f19299fed292b4)

### Auth

#### How do WebID-TLS and WebID-OIDC differ in regards to end-user experience?

A: With WebID-TLS you can manipulate \(operate on\) RDF sentences in target RDF documents \(content-type negotiable\) using a single HTTP Request using CURL. You need a series of CURL invocations to achieve that with WebID-OIDC due to the nature of different flows associated with said protocol.

#### What about CSRF

[https://gitter.im/solid/node-solid-server?at=5accc3697c3a01610dc98575](https://gitter.im/solid/node-solid-server?at=5accc3697c3a01610dc98575)

#### What is the expiry time for an OIDC access token?

Currently 20 minutes

[https://github.com/solid/node-solid-server/blob/dea121afbb92dd8e9ef8929d1d09246cd5ba5180/lib/models/token-service.js\#L15](https://github.com/solid/node-solid-server/blob/dea121afbb92dd8e9ef8929d1d09246cd5ba5180/lib/models/token-service.js#L15)

> In OpenID Connect an access token has an expiry time. For authorization code flow, this is typically short \(eg 20 minutes\) after which you use the refresh token to request a new access token.

[https://stackoverflow.com/questions/25686484/what-is-intent-of-id-token-expiry-time-in-openid-connect](https://stackoverflow.com/questions/25686484/what-is-intent-of-id-token-expiry-time-in-openid-connect)

[https://www.oauth.com/oauth2-servers/access-tokens/access-token-lifetime/](https://www.oauth.com/oauth2-servers/access-tokens/access-token-lifetime/)

### Panes

#### How do I flesh out items related to my Meeting e.g., links to other documents etc?

Various text input fields exist across solid-apps \(e.g., Meetulator, Chat etc..\), so place URIs in any of these with create a draggable object that can be dropped atop any of the visible panes of a particular app instance.

### How do I delete a solid-app pane \(nee Gadget\)?

Select pane, and then click the ALT key -- this reveals a UI completing task.

**SeeAlso**

1. [https://gitter.im/solid/node-solid-server?at=5a959532888332ee3adc5c27](https://gitter.im/solid/node-solid-server?at=5a959532888332ee3adc5c27)

2. [https://gitter.im/solid/node-solid-server?at=5a959f090202dc012e9136a5](https://gitter.im/solid/node-solid-server?at=5a959f090202dc012e9136a5)

### **Architecture**

### **Does Solid rely on DNS**

You can always use an IP address as your WebID if you choose. The role of DNS in the Solid Project is no different to what it is re. TCP/IP at large i.e., it resolves names to numbers. \(kidehen\)

#### Is that possible use solid without a running server? Or do I need something listening 7 x 24 for app requests? I would like to have something locally-ish

I've run solid on a phone before. But a server has the advantage of being always online, so you dont miss stuff.

You can use solid apps on someone else’s server of course, like solid.community.. You can a server on localhost. With aborwser extension ou can use it in file:// space in principle… we did that in earlier projects \(timbl\)

### Would changing IPs be an issue in the case of running it locally? Not sure how apps could find me if my address is dinamic 

I use https://www.noip.com/



