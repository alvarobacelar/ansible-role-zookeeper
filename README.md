ansible-role-zookeeper
=========

[![Build Status](https://travis-ci.org/alvarobacelar/ansible-role-zookeeper.svg?branch=master)](https://travis-ci.org/alvarobacelar/ansible-role-zookeeper)

Role of installation of ZooKeeper

Role Variables
--------------

This role have some defaults variables on file _main.yml_ that is available on the defaults directory.

Dependencias
------------

This role depends of another role for installation java of owner geerlingguy.java. For download this role execute the command following: 
```shell
# ansible-galaxy install geerlingguy.java
```

Exemple of Playbook
----------------

The host group for install the ZooKeeper, in your inventory, must be exactly follow on the example of playbook bellow:

    - hosts: zookeeper
      become: true
      roles:
         - alvarobacelar.zookeeper

License
-------

BSD

About Author
------------------
Alvaro Bacelar - Infraestructure especialist, enthusiastic DevOps and Infra As Code
