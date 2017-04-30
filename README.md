andrewrothstein.docker
======
[![Build Status](https://travis-ci.org/andrewrothstein/ansible-docker.svg?branch=master)](https://travis-ci.org/andrewrothstein/ansible-docker)

A role that installs and launches an optionally TLS secured [Docker](https://docker.io) daemon. Only listens remotely if secured with TLS.

Requirements
------------
See [meta/main.yml](meta/main.yml)


Role Variables
--------------

See [defaults/main.yml](defaults/main.yml)

Dependencies
------------

See [meta/main.yml](meta/main.yml)

Example Playbook
----------------

```yml
- hosts: servers
  roles:
    - role: andrewrothstein.docker
	  docker_insecure_registries :
	    - localhost:5000
```

License
-------

MIT

Author Information
------------------

Andrew Rothstein <andrew.rothstein@gmail.com>
