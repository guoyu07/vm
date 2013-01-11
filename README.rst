================
Vagrant based VM
================

This repository contains the vagrant specification for a VM to run the Zeta
Components tests. This currently is focussed on the Database components tests,
since it requires multiple databases.

Currently the VM includes:

* Current PHP

* MySQL

* PostGreSQL

Initialize and start the VM using::

    vagrant up
    vagrant ssh

To run the tests do something like this in the VM::

    cd zeta/Database
    ant


..
   Local Variables:
   mode: rst
   fill-column: 79
   End: 
   vim: et syn=rst tw=79
