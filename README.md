### Install zabbix-server  Ansible 

- [Overview](#overview)
  - [Operating systems](#operating-systems)
  - [Zabbix Versions](#zabbix-versions)
    - [Zabbix 4.0](#zabbix-40)
- [Installation](#installation)
- [Roles](#roles)
- [Documentation](#documentation)
- [Author Information](#author-information)

# Overview
This is a role for installing and maintaining the zabbix-server.

This is one of the 'ansible-install-and-config-zabbix-server
 roles which configures your whole zabbix environment.


## Operating systems

This role will work on the following operating systems:

 * Red Hat
 * Debian
 * Ubuntu
  
So, you'll need one of those operating systems.. :-)
Please send Pull Requests or suggestions when you want to use this role for other Operating systems.

## Zabbix Versions

See the following list of supported Operating systems with the Zabbix releases:

### Zabbix 4.0

  * CentOS 7.x
  * Amazon 7.x
  * RedHat 7.x
  * Ubuntu 18.04
  * Debian 8

# Installation

Installing this role is very simple: `ansible-playbook -i inventario site.yml`

# Roles

  * extra_configs
      - Install and configure host to receive required packages
  
  * repos
      - Install zabbix-server repository and packages
  
  * packages
      - Install repository and standard packages (at your discretion)    
  
  *  databases
      - Install e configure databases

  * zabbix-server
      - All installation and configuration of zabbix-server. After performing this role just access your ip http: //...../zabbix   

# Documentation

    - https://docs.ansible.com/

# Author Information

This is my first attempt to create an ansible role, so please send suggestion or pull requests to make this role better.
