### **Command Line Integration - Notes**

#### **TLS**

Solid server in TLS mode \(gold / node-solid-server auth=tls\) can operate via curl with an X.509 certificate

#### **OIDC**

Steps

* gets the client\_id / client\_secret

* uses those two to get back the bearer token

##### _**Static registration**_

google, facebook, twitter and others, have a web form that you can fill out to register an application

and it gives you a token \(which you then paste into that application's config, or pass it as a cli param, etc\)

so that's static registration

our Solid auth clients use dynamic registration \(we don't have the 'register an app' form implemented\)

##### _**Dynamic registration**_

for a cli app \(or any sort of server-side app\) to get a solid server auth token, it has to do the following -- 1\) perform dynamic registration \(if it hasn't already -- if it has, it loads that registration from storage\). 2\) generate an authorization URL, for a user to open. 3\) at the same time, the app has to listen on a localhost port, for the return callback. 4\) The user opens the authz link, logs in, and is redirected by the server to the callback url \(which the app is listening on\)

the app parses the callback url, extracts the token from it

since you have a TLS cert already, you should be able to skip several of those steps

but that functionality needs to be implemented.

##### **Howto**

how to register at the /register endpoint, which params to provide, and document it

Example:

[https://solidtest.space/register](https://solidtest.space/register)

[https://github.com/solid/webid-oidc-spec/blob/master/example-workflow.md\#23-dynamic-client-registration-first-time-only](https://github.com/solid/webid-oidc-spec/blob/master/example-workflow.md#23-dynamic-client-registration-first-time-only)

If this is the first time a Provider and a Relying Party are encountering each other, the RP must perform Dynamic Client Registration. Note: This is an operation that happens under the hood, and does not involve the user. All compliant OIDC clients have this functionality built in.

