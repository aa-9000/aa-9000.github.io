---
title: "General"
date: 2022-03-18T22:18:51Z
draft: false
---

### Git
```shell
git remote set-url --push upstream no_push
```
```shell
git config --global credential.helper osxkeychain
```

```shell
git whatchanged -p --since="1 week ago"
```

### OpenSSL
```shell
openssl req x509 -newkey rsa:4096 -keyout key.pem -out cert.pem -days 365 -nodes
```
```shell
openssl genrsa -des3 -out rootCA.key 4096
```

Check cert belongs to private key
```shell
openssl x509 -noout -modulus -in CERTIFICATE.crt | openssl md5
openssl req -noout -modulus -in CSR.csr | openssl md5
openssl rsa -noout -modulus -in PRIVATEKEY.key | openssl md5
```

### sed
```shell
https://www.gnu.org/software/sed/manual/html_node/Multiline-techniques.html
```

### Misc

```shell
checkip.amazonaws.com
aws-shell https://github.com/awslabs/aws-shell
stress-ng https://wiki.ubuntu.com/Kernel/Reference/stress-ng
lsd https://github.com/Peltoche/lsd
```