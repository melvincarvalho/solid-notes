### **KEYGEN - What you need to know**

#### Databox.me

1. Use Firefox Browser
2. Go to [https://databox.me/](https://databox.me/) and get a userID
3. Note down your _**username**_
4. Go to [https://username.databox.me/,accounts/cert](https://username.databox.me/,accounts/cert)
5. Enter your name and in the Webid [https://username.databox.me/profile/card\#me](https://username.databox.me/profile/card#me)

[https://gist.github.com/melvincarvalho/e14753a7137d02d756f19299fed292b4](https://gist.github.com/melvincarvalho/e14753a7137d02d756f19299fed292b4)

#### MDN Page

[https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Keygen](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Keygen)

##### Warnings

1. Deprecated

This feature has been removed from the Web standards. Though some browsers may still support it, it is in the process of being dropped. Avoid using it and update existing code if possible; see the

[compatibility table](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Keygen#Browser_compatibility)

at the bottom of this page to guide your decision. Be aware that this feature may cease to work at any time.

1. There is currently discussion among Web browser makers whether to keep this feature or not. Until a decision is reached, it is better to continue to consider this feature as deprecated and going away.

#### Converting SSH to X.509

[https://gist.github.com/melvincarvalho/dbc6e9f010ecef08194d7cf1a523963d](https://gist.github.com/melvincarvalho/dbc6e9f010ecef08194d7cf1a523963d)

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

#### Questions

Other relevant question are which browsers import them and export them, and which share the system keychain  \(timbl\)

#### Useful Links

Stackoverflow keygen alternatives:

[https://security.stackexchange.com/questions/106257/alternatives-to-htmls-deprecated-keygen-for-client-certs](https://security.stackexchange.com/questions/106257/alternatives-to-htmls-deprecated-keygen-for-client-certs)

PHP reference

[http://phpmylogin.sourceforge.net/wiki/doku.php?id=keygen\_attribute](http://phpmylogin.sourceforge.net/wiki/doku.php?id=keygen_attribute)

Test Pages

[http://id.myopenlink.net/ods/webid\_demo.html](http://id.myopenlink.net/ods/webid_demo.html?webid=http%3A%2F%2Fid.myopenlink.net%2Fpublic_home%2FKingsleyUyiIdehen%2FPublic%2FYouID%2FIDcard_LinkedIn_171227_125502%2F171227_125502_profile.ttl%23identity&pku=...http%3A%2F%2Fid.myopenlink.net%2Fpublic_home%2FKingsleyUyiIdehen%2FPublic%2FYouID%2FIDcard_LinkedIn_171227_125502%2F171227_125502_public_key.ttl%23PublicKey&ts=2018-02-07T00%3A45%3A41.156792&md5=39%3AF1%3A88%3A91%3A07%3A76%3A53%3A0C%3A06%3AE8%3A58%3A15%3A21%3AD1%3A6A%3A15&sha1=C2%3A1D%3A9B%3AF9%3AD5%3AE0%3A9D%3AEC%3ABB%3A46%3A97%3ADD%3A76%3AEF%3ADC%3AAE%3AF8%3A9B%3A29%3AF0&subj=%2FC%3DUS%2FST%3DMA%2FCN%3DKingsley%20Uyi%20Idehen%20%28LinkedIn%29%2FO%3DLinkedIn%20Social%20Network%2FemailAddress%3Dkidehen@openlinksw.com&elapsed=57&signature=ngz%2FTVxgbVTB7f88i%2FK2uZlWsLIvcuakrLzV1tt0oVq3rWi8C3gGIgX8x%2Bq5U6nw8k%2FjU9T5MHkHb9YRArys07lHWe4sE39qFbyeXR83ZPQxX01JohnPtQJHUentLIoyE7XV%2Fc9TeV%2BHySzJ%2F5by6ATFfyWw4QwN7Ipa9F4jRPduE5N7ZAZPlRWT%2Fl%2FNFozajBzLXsaT3jdVQsWdy97SXjShciI%2BrulNCwhiydXH32itj4f4xDt%2FU6zaz3RPgQRYtBlNpW4K4pzsQAsnEXEu3%2BTipMhh40W0vSXfDWga9mazgbDQxEG%2BXp7f44shX1mJbyb1qst6jWNesmg1BKkVDA%3D%3D)

