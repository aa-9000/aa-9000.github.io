---
title: "Helm"
date: 2022-03-18T22:30:56Z
draft: false
tags: ['helm']
---

Helm2 - https://helm.sh/docs/faq/changes_since_helm2/#changes-since-helm-2
```shell
helm install -n web-app -f values.yaml ./chart-dir/web-app
```
```shell
helm template . -x templates/deployment.yaml
```


