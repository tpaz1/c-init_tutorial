# c-init tutorial

In this tutorial I've created a Deployment Spec that creates a simple nginx application with a volume of type EmptyDir and an init container (containers that run before the main container runs with your containerized application).

The init container's role is to clone a git repository to our EmptyDir volume before each time our main container starts.

The outcome is that whenever a new container starts, it will start with the most recent committed repo mounted in its filesystem.

In the following lab we will use:

* Volume
* C-INIT
* ConfigMap
* SERVICE type ClusterIp
* Ingress
* LoadBalancer as a proxy to ingress
 



