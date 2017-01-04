[![CircleCI](https://circleci.com/gh/andrewrothstein/ansible-docker.svg?style=svg)](https://circleci.com/gh/andrewrothstein/ansible-docker)

andrewrothstein.docker
======

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
