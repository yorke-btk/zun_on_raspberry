Deploy Zun-compute on Raspberry Pi

冪等性とか考えてません、、
====

## Overview
This project is Ansible code sets to deploy Zun-compute on Raspberry Pi.  
Zun is an OpenStack container service.  

## Environment
OpenStack version: pike  
host OS (controller node): Ubuntu 16.04  
host OS (raspberry pi): raspbian 9.4  

I'm going to add the description to deploy zun(controller) on OpenStack latter.   


## Description
I'm writing them based on <https://docs.openstack.org/zun/latest/install/compute-install.html>.  
The role of these codes is following.  

- check_ansible.sh: Checking grammer of *.yml
- run_ansible.sh: run ansible

- container_compute_deploy.yml: main yml file in this project
- etcd_deploy.yml: yml file to deploy etcd.
- kuryr_deploy.yml: yml file to deploy kuryr-libnetwork.
- zun_compute_deploy.yml: yml file to deploy zun-compute.
- ovs_deploy.yml: yml file to deploy OpenvSwitch 


- files/: Some files to execute daemons (zun-compute.service, zun.conf, etc...)  
          You may replace some parameters ( user name, password) in these files for your environment.
 
- inventory/: configure compute node IP Address.  
              You may replace some IP Addresses in these files for your environment.

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

