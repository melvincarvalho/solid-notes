Browsers

By hand

By script

Other

**Generating a self signed X.509 cert**

: [https://www.akadia.com/services/ssh\_test\_certificate.html](https://www.akadia.com/services/ssh_test_certificate.html)

or

```
$ openssl genrsa 2048 >../localhost.key
```

```
$ openssl req -new -x509 -nodes -sha256 -days 3650 -key ../localhost.key -subj '/CN=*.localhost' > ../localhost.cert
```

**Generating a WebID X.509 cert**

Scripts

[https://gist.github.com/tomasklapka/ced88b6b72538a5ffe6baffcd898dea8](https://gist.github.com/tomasklapka/ced88b6b72538a5ffe6baffcd898dea8)

[https://gist.github.com/njh/2432427](https://gist.github.com/njh/2432427)

[https://gist.github.com/njh/2432427/forks](https://gist.github.com/njh/2432427/forks)

[https://github.com/AtomGraph/LinkedDataHub/tree/master/scripts](https://github.com/AtomGraph/LinkedDataHub/tree/master/scripts)

https://gist.github.com/olberger \# works!



