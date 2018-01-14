Browsers

By hand

By script

Other

Generating a self signed X.509 cert : [https://www.akadia.com/services/ssh\_test\_certificate.html](https://www.akadia.com/services/ssh_test_certificate.html)

or

```
$ openssl genrsa 2048 >../localhost.key
```

```
$ openssl req -new -x509 -nodes -sha256 -days 3650 -key ../localhost.key -subj '/CN=*.localhost' > ../localhost.cert
```



