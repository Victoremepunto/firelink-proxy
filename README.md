# Firelink Proxy


To test in an ephemeral environment:

```bash
$ oc apply -f deploy/secret.yaml -n $NS
$ oc process -f deploy/deploy.yaml | oc apply -n $NS -f -
```

When you deploy IRL you'll need the secret named `firelink-proxy` created elsewhere as it isn't in the template.