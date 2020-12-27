source:
- https://www.digitalocean.com/community/tutorials/how-to-set-up-an-nginx-ingress-with-cert-manager-on-digitalocean-kubernetes


# prerequities:
- helm version 3
- kubectl
- helmfile

# comamnds:

```
$ kubectl apply --validate=false -f https://github.com/jetstack/cert-manager/releases/download/v1.0.0/cert-manager.crds.yaml
$ helmfile --file=helmfile/helmfile.yaml apply  --skip-deps
```