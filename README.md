Riemann-dash ansible role
=========

[![Build Status](https://travis-ci.org/cortwave/riemann-dash.svg?branch=master)](https://travis-ci.org/cortwave/riemann-dash)

dashboard for [Riemann](http://riemann.io)

Tested OS
--------------
Role works only on modern dystros with `systemd` support

- Debian 8
- Ubuntu 16.04
- Centos 7

Role Variables
--------------
`riemann_dash_port` dash port to listen (default 4567)

`riemann_dash_listen` address to listen (default "127.0.0.1")

`riemann_conf_dir` config directory (default /etc/riemann)

Dependencies
------------

ruby ~> 2.0

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: cortwave.riemann-dash, 
             riemann_dash_port: 8888 }

License
-------

GPLv2
