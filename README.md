apache_php
==========

[![Build Status](https://travis-ci.org/andrelohmann/ansible-role-apache_php.svg?branch=master)](https://travis-ci.org/andrelohmann/ansible-role-apache_php)

Use this role to install the apache2, php from the deb.sury.org repository on your debian or ubuntu server.

Requirements
------------

This role requires debian or ubuntu.

Role Variables
--------------

The following can be set in group_vars/host_vars

    php_ini_settings:
    - key: post_max_size
      value: 512M
    - key: upload_max_filesize
      value: 512M
    - key: max_execution_time
      value: 600
    - key: max_input_time
      value: 600
    php_additional_packages:
    - php7.1-gd
    - php7.1-mysql
    - php7.1-curl
    - php7.1-mcrypt
    - php7.1-tidy
    - php7.1-zip
    - php-imagick
    - php-geoip
    - geoip-bin
    apache_additional_modules:
    - name: rewrite
      state: present

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
