Getting started with OpenEBS on your Kubernetes cluster is easy.

1) Clone the OpenEBS repo from github:

`git clone https://github.com/openebs/openebs.git && cd openebs/k8s`{{execute}}

2) Use the following command to apply OpenEBS operators:

`kubectl apply -f openebs-operator.yaml `{{execute}}

Congratulations!!! The OpenEBS has been installed. Check its status by running:

`kubectl get pods -l "name=maya-apiserver" `{{execute}}

**Optional:**
3) Use the following command to apply predefined OpenEBS storage classes:

`kubectl apply -f openebs-storageclasses.yaml `{{execute}}

4) Check available storage classes by running:

`kubectl get sc`{{execute}}
