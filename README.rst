docker-centos
=============

Centos base image with systemd added and some packages to allow testing with puppetlabs Beaker

https://hub.docker.com/r/timhughes/centos/


See https://hub.docker.com/_/centos/ for the CentOS details



::

    docker pull centos7_ruby1.9


::

    .
    ├── 6
    │   ├── buildpack-deps
    │   └── ruby
    │       ├── 1.8
    │       ├── 1.9
    │       ├── 2.0
    │       ├── 2.1
    │       └── 2.2
    └── 7
        ├── buildpack-deps
        └── ruby
            ├── 1.9
            ├── 2.0
            ├── 2.1
            └── 2.2

