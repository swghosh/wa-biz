Create service-account for whatsapp and grant it anyuid scc.

```
$ oc create serviceaccount whatsapp
$ oc adm policy add-scc-to-user anyuid system:serviceaccount:whatsapp-client-containers:whatsapp-db
```

