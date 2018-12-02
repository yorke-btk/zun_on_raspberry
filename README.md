Deploy Zun-compute of Openstack Projects on Raspberry Pi
====

Overview
This project is Ansible code sets to deploy Zun-compute on Raspberry Pi.
These are still TBD.

= my environment
OpenStack version: pike
host OS (controller node): Ubuntu 16.04
host OS (raspberry pi): raspbian 9.4

I'm going to add the description to deploy zun(controller) on OpenStack latter. 


## Description
I'm writing them based on <https://docs.openstack.org/zun/latest/install/compute-install-ubuntu.html#install-and-configure-components>.
The role of these codes is following.

- check_ansible.sh: Checking grammer of *.yml
- run_ansible.sh: run ansible

- container_compute_deploy.yml: main yml file in this project
- etcd_deploy.yml: yml file to deploy etcd.
- kuryr_deploy.yml: yml file to deploy kuryr-libnetwork.
- zun_compute_deploy.yml: yml file to deploy zun-compute.
- ovs_deploy.yml(TBD): yml file to deploy OpenvSwitch 
- l3_agent_deploy.yml(TBD): yml file to deploy neutron-l3-agent


- files/: Some files to execute daemons (zun-compute.service, zun.conf, etc...)
          You may replace some parameters (IP Address, user name, password) in these files for your environment.
 
- inventory/: configure compute node IP Address.
              You may replace some parameters (IP Address, user name, password) in these files for your environment.

## Demo

## VS. 

## Requirement

## Usage

## Install

## Contribution

## Licence

[Apache License 2.0](https://github.com/yorke-btk/zun_on_raspberry/LICENCE)

## Author

[yorke-btk](https://github.com/yorke-btk)

