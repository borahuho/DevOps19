# DevOps19

This vagrant will install 4 Linux Ubuntu machines, 1 Ansible server, 1 master node/server and 2 worker nodes/servers. This DevOps is to practice with a Kubernetes cluster.
It will add some default users, groups and directory's.
This Vagrant is to practice with Ansible and the intial setup for Kubernetes.
This repository is intended for educational purpose only.


## Prerequisites

Works on Windows 10 and tested on macOS (macOS needs the Virtualbox extension pack).

Software needed:
* Virtualbox 5.0 or higher
* Git bash for Windows
* Vagrant 2.2.6 or higher
* DevNet account at Cisco 


## Demo installation && use Vagrant

Youtube: https://youtu.be/KABnIuaA8SM


## Demo initial setup Kubernetes

Youtube: https://youtu.be/FRM_lXmAS_A


## Installation

* Install Virtualbox: https://www.virtualbox.org/wiki/Downloads
* Install Git bash for Windows: https://gitforwindows.org/
* Install Vagrant for Windows: https://www.vagrantup.com/downloads.html
* Create an free account at DevNet: https://developer.cisco.com/

## Run this Vagrant VM
Open **Git Bash** in Windows
```
cd Documents
mkdir vagrant && cd vagrant
git clone https://github.com/borahuho/DevOps19
cd DevOps19
vagrant up
vagrant ssh ansible
```
## Mission

Read your mission in ~/vagrant/mission (on Ansible server)

## Network
Vagrant VM will be set up with 2 network adapters
```
Nat : DHCP
Localhost (ansible): 192.168.10.150

Nat : DHCP
Localhost (master): 192.168.10.155

Nat : DHCP
Localhost (worker1): 192.168.10.156

Nat : DHCP
Localhost (worker2): 192.168.10.157
```
## Vagrant commands
Start VM's with Vagrant
```
vagrant up
```
Pause a VM
```
vagrant suspend
```
Restart a paused VM
```
vagrant resume
```
Stop and shutdown a VM
```
vagrant halt
```
Remove a VM
```
vagrant destroy
```
ssh in to the VM
```
vagrant ssh ansible
vagrant ssh master
vagrant ssh worker1
vagrant ssh worker2
```

