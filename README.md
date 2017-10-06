apache_php
==========

[![Build Status](https://travis-ci.org/andrelohmann/ansible-role-apache_php.svg?branch=master)](https://travis-ci.org/andrelohmann/ansible-role-apache_php)

Use this role to install the apache2, php from the deb.sury.org repository on your debian or ubuntu server.

Requirements
------------

This role requires debian or ubuntu.

Example Playbook
----------------

    - hosts: all
      roles:
         - { role: andrelohmann.apache_php }

License
-------

MIT

Author Information
------------------

https://github.com/andrelohmann
