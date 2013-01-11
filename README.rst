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

Issues
======

There is still an issue with the postgres user, which I currently resolve
manually in the VM, which is far from optimal.

We need to get a "postgres" user without password to work properly, and ensure
PHP connects properly to that user


..
   Local Variables:
   mode: rst
   fill-column: 79
   End: 
   vim: et syn=rst tw=79
