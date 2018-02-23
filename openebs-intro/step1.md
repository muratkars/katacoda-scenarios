Getting started with OpenEBS on your Kubernetes cluster is easy. On your kubemaster, use the following command:

`kubectl apply -f https://openebs.github.io/charts/openebs-operator.yaml`{{execute}}

The OpenEBS has been installed. Check its status by running:

`kubectl get pods -l "name=maya-apiserver" `{{execute}}

Note:
To use OpenEBS Volumes, your nodes should have the iSCSI initiator installed.  
Please visit http://openebs.readthedocs.io/en/latest/getting_started/quick_install.html for environment requirements and detailed instructions .

Note that you can also install OpenEBS using Helm chart.
