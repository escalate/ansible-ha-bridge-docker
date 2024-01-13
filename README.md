[![Test](https://github.com/escalate/ansible-ha-bridge-docker/actions/workflows/test.yml/badge.svg?branch=master&event=push)](https://github.com/escalate/ansible-ha-bridge-docker/actions/workflows/test.yml)

# Ansible Role: ha-bridge-docker

An Ansible role that manages ha-bridge Docker container with systemd on Raspbian and Debian OS.
This role is compatible with OS version Stretch (9) and Jessie (8).

## Requirements

The Docker daemon should be already installed and running on the host side.
I recommend using of the Ansible Galaxy role [angstwad.docker_ubuntu](https://github.com/angstwad/docker.ubuntu) to manage the Docker daemon.

This role is tested with Ansible version greater equal 2.4.

## Install

```
$ ansible-galaxy install escalate.ha-bridge-docker
```

## Role Variables

Please see [defaults/main.yml](https://github.com/escalate/ansible-ha-bridge-docker/blob/master/defaults/main.yml) for a complete list of variables that can be overridden.

## Dependencies

None

## Example Playbook

```
- hosts: all
  roles:
    - escalate.ha-bridge-docker
```

## License

MIT
