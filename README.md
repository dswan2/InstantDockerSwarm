Summmary:   This vagrantfile will create a docker swarm cluster for a self training environment.   The swarm will be initialized, and will join worker nodes to the swarm.   
All configurations allow running containers, but base configuration limits you to deploying services to a single node.   With more nodes, you can experience with increasing 
the number of service replicas, and testing failover by killing a replica. 


Minimum: Hardware Prereqs: 12 GB Ram, 4 CPU threads.

Software Prereqs:  Git, Vagrant, Virtualbox:
	https://git-scm.com/downloads
	https://www.vagrantup.com/downloads.html
	https://www.virtualbox.org/wiki/Downloads

Quickstart:
1.  git clone  https://github.com/dswan2/InstantDockerSwarmCluster
2.  cd InstantDockerSwarmCluster
3.  Edit vagrantfile to customize WORKER_NODES, MANAGERMEM, MANAGERCPUS, WORKERMEM, and WORKERCPUS.   
4.  Install plugin to allow shared Filesystem:  vagrant plugin install vagrant-vbguest
5.  Vagrant up




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






Presentation:  
1.  Some on this call are full experts, and others have never been exposed.    Hopefully I'll hit somewhere in the middle.    I'll stop periodically for questions,
but otherwise ask you hold them.