Summmary:   This vagrantfile will create a docker swarm cluster for training purposes.   The swarm will be initialized, and will join worker nodes to the swarm.   All configurations allow running containers, 
but base configuration limits you to deploying a service to a single node.   With more nodes, you can experience with increasing the number of replicas, and killing off a replica to see failover.


Minimum: Hardware Prereqs: 12 GB Ram, 4 CPU threads.

Software Prereqs:  Git, Vagrant, Virtualbox:
	https://git-scm.com/downloads
	https://www.vagrantup.com/downloads.html
	https://www.virtualbox.org/wiki/Downloads

Quickstart:
1.  git pull  https://github.com/dswan2/InstantDockerSwarmCluster
2.  cd InstantDockerSwarmCluster
3.  Edit vagrantfile to customize WORKER_NODES, MANAGERMEM, MANAGERCPUS, WORKERMEM, and WORKERCPUS.   
4.  Install plugin to allow shared Filesystem:  vagrant plugin install vagrant-vbguest



Deeper dive:






	Absolute minimum:
		WORKER_NODES = 2
		MANAGERMEM = 3000
		MANAGERCPUS = 1
		WORKERMEM = 2000
		WORKERCPUS = 1
	Recommended:
		WORKER_NODES = 3
		MANAGERMEM = 4000
		MANAGERCPUS = 2
		WORKERMEM = 3000
		WORKERCPUS = 2




