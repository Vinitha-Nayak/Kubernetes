what is a kuberenets ingress?
Ingress exposes HTTP and HTTPs routes from outside the cluster to services within the cluster.Traffic routing is controlled by rules defined on the ingress resources.

Problems that are solved by ingress:
1. Enterprise and tls load balance
   Service was providing a simple load balancing capabilities. service was using round robin.
   Ingress provides the enterprise level features like:
   -sticky session
   -ratio based
   -security
   kubernetes was not supporting all of these features

2. Load balancer ip address
   cloud provider will charge for each and every load balancer service type.

some of the enterprise load balancers such as F5,nginx,HA proxy

User creates ingress resource.
Load balancing campanies will write thier own ingress contrller and 
place the ingress controller on github and provides required steps to install ingress controller.
Along with creating ingress resource user should deploy ingress controller.
