Now we will install a demo workload to show OpenEBS functionality.

1) List the demo workloads under **demo** folder and run *crunchydb-postgres* example:

`ls demo && ./demo/crunchy-postgres/run.sh`{{execute}}

2) The volume details can be inspected using the standard kubectl commands. To check **persistent volume claims**:

`kubectl get pvc`{{execute}}

3) List the **services**, and you will see pgset, master and replica created:

`kubectl get service`{{execute}}

4) List the **statefulsets**, and you will see pgset listed with two desired and current sets:

`kubectl get statefulset`{{execute}}

Congratulations! Your PostgreSQL workload is now running on persistent OpenEBS volumes.
