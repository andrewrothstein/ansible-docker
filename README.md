andrewrothstein.docker
======

A role that installs and launches an optionally TLS secured Docker daemon with https://get.docker.io

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
	  insecure_registries :
	    - localhost:5000"
	  docker_mirror : "https://my.get.docker.io.alternative.io"
```

License
-------

MIT

Author Information
------------------

Andrew Rothstein <andrew.rothstein@gmail.com>
