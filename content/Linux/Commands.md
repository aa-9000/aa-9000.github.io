---
title: "Commands"
date: 2022-03-18T22:18:51Z
draft: false
tags: ['linux', 'random', 'commands']
---
# ![linux](https://raw.githubusercontent.com/manaten/computing-mascots-pixelart-icons/master/linux.gif)


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

### Random
```shell
https://www.gnu.org/software/sed/manual/html_node/Multiline-techniques.html
```
```shell
hugo new --kind chapter Code/_index.md
hugo new AWS/EKS.md
```

```shell
socat -d -d -d TCP4-LISTEN:8181,fork,reuseaddr TCP4:10.1.2.3:80
```

```shell
ssh -L 80:localhost:8080 10.1.2.3
```

```shell
.mode csv
.import ./all_user_data.csv UserData
```

```shell
set -eu -o pipefail
# Catch unused variables, and failed command pipes
```