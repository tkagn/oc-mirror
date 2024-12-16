# oc-mirror


**Create initial imageset-config.yaml:**

```bash
oc-mirror init --registry infra-services.abc.tkagn.io:5000/ocmirror/metadata:latest | tee imageset-config.yaml
```



oc-mirror list releases
oc mirror list operators
oc-mirror list operators --catalogs --version=4.16

oc-mirror list operators --catalog=registry.redhat.io/redhat/redhat-operator-index:v4.16 --version 4.16
oc-mirror list operators --catalog=registry.redhat.io/redhat/certified-operator-index:v4.16 --version 4.16


 oc-mirror --config=./imageset-config.yaml docker://infra-services.abc.tkagn.io:5000/openshift4

oc adm catalog mirror file://redhat/redhat-operator-index:v4.16 REGISTRY/REPOSITORY
oc adm catalog mirror file://redhat/certified-operator-index:v4.16 REGISTRY/REPOSITORY

**Mirror images**
```bash
 oc-mirror --config=./imageset-config.yaml docker://infra-services.abc.tkagn.io:5000/openshift4
```
