Riemann-dash ansible role
=========

dashboard for [Riemann](http://riemann.io)

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
