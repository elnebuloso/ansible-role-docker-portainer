# Ansible Role - Portainer for Docker

[![Build Status](https://travis-ci.org/elnebuloso/ansible-role-docker-portainer.svg?branch=master)](https://travis-ci.org/elnebuloso/ansible-role-docker-portainer)

## Requirements

This role requires Ansible 2.0 or higher, and platform requirements are listed in the metadata file.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```
docker_portainer_state: "started"
docker_portainer_version: "1.11.1"
docker_portainer_container_name: "portainer"
docker_portainer_container_volume_base: "/opt/docker"
docker_portainer_port: "9000"
docker_portainer_initial_database_file: "files/portainer/portainer.db"
```

## Example Playbook

```
- hosts: localhost
  roles:
    - { role: elnebuloso.docker-portainer }
```

## Dependencies

- `docker` should be installed and working (you can use the `elnebuloso.docker` role to install).

##  License

MIT

##  Author Information

This role was created in 2017 by [elnebuloso](https://github.com/elnebuloso/)