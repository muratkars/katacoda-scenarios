Getting started with OpenEBS on your Kubernetes cluster is easy.

Before we start, make sure that your K8s master node is functional by confirming the node status:

`kubectl get nodes`{{execute}}

Wait until you see **Ready** under STATUS field before you go to the next step.

1) Clone the OpenEBS repo from github:

`git clone https://github.com/openebs/openebs.git && cd openebs/k8s`{{execute}}

2) Use the following command to apply OpenEBS operators:

`kubectl apply -f openebs-operator.yaml `{{execute}}

Congratulations!!! The OpenEBS has been installed.

3) Check its status by running:

`kubectl get pods -l "name=maya-apiserver" `{{execute}}

**Optional:**
4) Use the following command to apply predefined OpenEBS storage classes:

`kubectl apply -f openebs-storageclasses.yaml `{{execute}}

5) Check available storage classes by running:

`kubectl get sc`{{execute}}
