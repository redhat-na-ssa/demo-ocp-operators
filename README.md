# Demo Operators on OpenShift

Show the value of operators on the OpenShift platform

## Quickstart

Setup Enhanced Web Terminal

```sh
# apply firmly
until oc apply -k  https://github.com/redhat-na-ssa/ocp-web-terminal-enhanced/bootstrap; do : ; done

# delete old web terminal
$(wtoctl | grep 'oc delete')
```

Apply Demo

```sh
oc apply -k gitops
```

## Examples

- [x] [Declarative Example](gitops/app-configs/namespace/sandbox.yaml)
- [x] [Kustomize Example](gitops/branding/kustomization.yaml)
- [x] [Advanced Kustomize Example](gitops/cluster-configs/adhoc-admin)
- [x] [OpenShift Helm Charts (default)](https://charts.openshift.io)
