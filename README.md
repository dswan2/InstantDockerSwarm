# Instant Docker Swarm Cluster


## Summmary:   
	This vagrantfile will create a docker swarm cluster for a self training environment.   The swarm will be initialized, and will join worker nodes to the swarm.   


### Minimum Hardware Prereqs: 
	12 GB Ram, 4 CPU threads.


### Initial setup:

1.  Download and install Git, Vagrant, and Virtualbox.
	https://git-scm.com/downloads
	https://www.vagrantup.com/downloads.html
	https://www.virtualbox.org/wiki/Downloads

2.  Open a Git-Bash prompt from the program manager.

3.  Install plugin to allow shared Filesystem:  vagrant plugin install vagrant-vbguest


### Usage:

1.  git clone  https://github.com/dswan2/InstantDockerSwarmCluster

2.  cd InstantDockerSwarmCluster

3.  Vagrant up

4.  Vagrant ssh docker0


### Notes:

- Edit vagrantfile to customize:

	Absolute minimum (Needs 4vcpus/12GB):
		WORKER_NODES = 1
		MANAGERMEM = 3000
		MANAGERCPUS = 1
		WORKERMEM = 2000
		WORKERCPUS = 1

	Recommended (Needs 8vcpus/16GB):
		WORKER_NODES = 3
		MANAGERMEM = 3000
		MANAGERCPUS = 2
		WORKERMEM = 2500
		WORKERCPUS = 2

