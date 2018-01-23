### **KEYGEN - What you need to know**

#### MDN Page

[https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Keygen](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Keygen)

##### Scary Warnings

1. Deprecated

This feature has been removed from the Web standards. Though some browsers may still support it, it is in the process of being dropped. Avoid using it and update existing code if possible; see the

[compatibility table](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Keygen#Browser_compatibility)

at the bottom of this page to guide your decision. Be aware that this feature may cease to work at any time.

1. There is currently discussion among Web browser makers whether to keep this feature or not. Until a decision is reached, it is better to continue to consider this feature as deprecated and going away.

#### **Tag Guidance**

[https://w3ctag.github.io/client-certificates/](https://w3ctag.github.io/client-certificates/)

#### Issues Raised

[https://github.com/whatwg/html/issues/102](https://github.com/whatwg/html/issues/102)

#### **Keygen pages**

#### **Browser Compatibility**

Working in Firefox

Not working in Chrome, Opera

#### Example SPKAC

```
SPKAC=MIICSzCCATMwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIBAQCrZsGntIjcNwRhRyBKF/fw3N4eJyOseG2bGyxqtp7
dXJ0nL2qzmDlw2bttqxAIWZnXMG0DNnUcMHiaJ5IfHr62QtfpSJyj7QmPp2NgHsaps26tS+pdroPEajwbffLUBcZxm9DnQDpMvifx
V9ZfXJBaBjPZwrtyLnk1Cy7S7ZYg/2x4VisgqHnIP0Rcz6PJZxGcIypy49LTAjk/tdk2FD5hMQixDvnJl0C2Yq4k+UOgAFIWDJ4YK
tqaa4zDHcAaCQtkguUMSIRXNBKZ+J8nHwYgBkk6KYq+jS0wJBjbZAjtVpv2RlSgU3ZjkJemGU+44SnQXbI1TgRaMnZP65YiGdbTAg
MBAAEWC3JhbmRvbWNoYXJzMA0GCSqGSIb3DQEBBAUAA4IBAQBpJhkVm5YKxpkm3OJYkioNa9ZCyOVr30Yi3MGqcRXMh4LfMpc5zOz
DucQvi46BhZUU8dcKjvHlaGV5f0624N5/HET/RQlRoOWHJ0zskugHiAcE25Hrd3oQOw+Hg4nDejvPdJUwflWrz06gRKGyJhe0209Y
6zLvWReR0opaaUZgRW0jc6kHWr10mhCgbsZzIKTb4vDUQ8QnnMvSryHy4TZOXq4zS8rE26Yyep7+wxw2iy8I97/S3UCks/iN9RiCW
I8JBGJR13Xr0vNvMDcjDCbuYIbiHcScBV2PyENX7SZ+9cCbnUekN4O5FjCciyGY1aTWpdl7nXJ9iYEKaYVmzjiY
CN=Joe
emailAddress=joe@example.org
0.OU=AA Ltd client certificate
organizationName=AA Ltd
countryName=AA
stateOrProvinceName=AA
localityName=AA
```

#### Client code

[https://gist.github.com/melvincarvalho/d9acb32ea07dbd4b3ca11f0e2d2756fe](https://gist.github.com/melvincarvalho/d9acb32ea07dbd4b3ca11f0e2d2756fe)

#### Server Code

make sure all the openssl cnf fields are populated

optionally uncomment suject alternative name

make sure index.txt is empty

openssl ca -batch -spkac /tmp/tmp1234.spkac -passin pass:a &gt; spkac.pem

#### Useful Links

Stackoverflow keygen alternatives:

[https://security.stackexchange.com/questions/106257/alternatives-to-htmls-deprecated-keygen-for-client-certs](https://security.stackexchange.com/questions/106257/alternatives-to-htmls-deprecated-keygen-for-client-certs)

PHP reference

[http://phpmylogin.sourceforge.net/wiki/doku.php?id=keygen\_attribute](http://phpmylogin.sourceforge.net/wiki/doku.php?id=keygen_attribute)

