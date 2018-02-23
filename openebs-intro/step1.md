Getting started with OpenEBS on your Kubernetes cluster is easy.

Clone the OpenEBS repo from github:

`git clone https://github.com/openebs/openebs.git && cd openebs/k8s`{{execute}}

Use the following command to apply OpenEBS operators:

`kubectl apply -f openebs-operator.yaml`{{execute}}

Congrats!!! The OpenEBS has been installed. Check its status by running:

`kubectl get pods -l "name=maya-apiserver" `{{execute}}

**Optional:***
Use the following command to apply predefined OpenEBS storage classes:

'kubectl apply -f https://openebs.github.io/charts/openebs-operator.yaml`{{execute}}

Check available storae classes by running:

`kubectl get sc`{{execute}}

**Note:**
To use OpenEBS Volumes, your nodes should have the iSCSI initiator installed.  
You can also install OpenEBS using Helm charts.
Please visit http://openebs.readthedocs.io/en/latest/getting_started/quick_install.html for environment requirements and detailed instructions .
