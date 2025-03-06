[![Test](https://github.com/escalate/ansible-ha-bridge-docker/actions/workflows/test.yml/badge.svg?branch=master&event=push)](https://github.com/escalate/ansible-ha-bridge-docker/actions/workflows/test.yml)

# Ansible Role: Raspberry - ha-bridge (Docker)

An Ansible role that manages [ha-bridge](https://github.com/bwssytems/ha-bridge) Docker container with systemd on Raspberry Pi OS (Debian Bookworm).

## Role Variables

Please see [defaults/main.yml](https://github.com/escalate/ansible-ha-bridge-docker/blob/master/defaults/main.yml) for a complete list of variables that can be overridden.

## Dependencies

This role relies on the following dependencies:

- Roles: None
- Collections: None

## Install

```
$ ansible-galaxy role install escalate.ha_bridge
```

## Example Playbook

```
- hosts: all
  roles:
    - role: escalate.ha_bridge
      tags: habridge
```

## License

MIT
