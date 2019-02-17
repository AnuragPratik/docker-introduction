# Docker commands

## simple commands

```
* docker version
* docker info
* docker images
* docker ps /-a/-aq
```

## setting up docker machines

```
* docker-machine ls
* docker-machine rm worker1
* docker-machine create -d hyperv --hyperv-virtual-switch "External Switch" manager1
* docker-machine create -d hyperv --hyperv-virtual-switch "External Switch" worker1
* docker-machine create -d hyperv --hyperv-virtual-switch "External Switch" worker2
* docker-machine create -d hyperv manager1
```

## docker swarm mode

```
docker swarm leave --force
docker swarm init --advertise-addr 192.168.1.195:2377 --listen-addr 192.168.1.19578:2377
docker swarm join --token SWMTKN-1-4d2zjb3k6qzl42olmdejl08djietandzpoldhuud8ecnesml1b-c2c6ryh6h1r7l0qehjyycxnse 192.168.1.195:2377
```