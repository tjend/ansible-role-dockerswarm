Setup Docker Swarm Cluster
==========================

Node Role
---------

Set variable `dockerswarm_node_role` to `manager` to be a manager/worker node.
Set variable `dockerswarm_node_role` to `worker` to be worker only node.

The first host in the hostgroup will always be a manager/worker node.

Networking
----------

Ensure TCP port 2377 is open on management nodes(cluster management).
Ensure TCP/UDP port 7946 is open on all nodes(network discovery).
Ensure UDP port 4789 is open on all nodes(ingress networking).
