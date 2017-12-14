Ansible Role: Docker Conf
=========

Configure docker daemon on Linux.

Requirements
------------

Docker installed.

Role Variables
--------------

`docker_opts`: Options for docker daemon.

Detailed options you can find in https://docs.docker.com/engine/reference/commandline/dockerd/

Dependencies
------------

None.

Example Playbook
----------------

```yml
- hosts: servers
  vars:
    docker_opts:
      dns:
        - 8.8.8.8
        - 8.8.4.4
      debug: false
  roles:
    - { role: djx339.docker-conf }
```

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
