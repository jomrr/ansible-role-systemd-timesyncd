# Ansible role timesyncd

![GitHub](https://img.shields.io/github/license/jomrr/ansible-role-timesyncd) ![GitHub last commit](https://img.shields.io/github/last-commit/jomrr/ansible-role-timesyncd) ![GitHub issues](https://img.shields.io/github/issues-raw/jomrr/ansible-role-timesyncd)

**Ansible role to configure systemd-timesyncd.**

## Description

This Ansible role installs and configures timesyncd on supported platforms.

## Prerequisites

This role has no special prerequisites.

### System packages (Fedora)

- `python3` (>= 3.9)

### Python (requirements.txt)

- ansible >= 2.15

## Dependencies (requirements.yml)

This role has no dependencies.

## Supported Platforms

| OS Family | Distribution | Version | Container Image |
|-----------|--------------|---------|-----------------|
| RedHat | AlmaLinux | latest | [jomrr/molecule-almalinux:latest]( https://hub.docker.com/r/jomrr/molecule-almalinux ) |
| Archlinux | Archlinux | latest | [jomrr/molecule-archlinux:latest]( https://hub.docker.com/r/jomrr/molecule-archlinux ) |
| Debian | Debian | latest | [jomrr/molecule-debian:latest]( https://hub.docker.com/r/jomrr/molecule-debian ) |
| RedHat | Fedora | latest | [jomrr/molecule-fedora:latest]( https://hub.docker.com/r/jomrr/molecule-fedora ) |
| Suse | OpenSuse Leap | latest | [jomrr/molecule-opensuse-leap:latest]( https://hub.docker.com/r/jomrr/molecule-opensuse-leap ) |
| Debian | Ubuntu | latest | [jomrr/molecule-ubuntu:latest]( https://hub.docker.com/r/jomrr/molecule-ubuntu ) |

## Role Variables

No role default variables specified, see [defaults/main.yml](defaults/main.yml).

## Example Playbook

Example playbooks(s) that show how to use this role.

## Simple example playbook

A simple default example playbook for using jomrr.timesyncd.
```yaml
---
# name: "jomrr.timesyncd"
# file: "playbook_timesyncd.yml"

- name: "PLAYBOOK | timesyncd"
  hosts: "timesyncd_hosts"
  gather_facts: true
  roles:
    - role: "jomrr.timesyncd"
```

## Author(s) and License

- :octocat:                 Author::    [jomrr](https://github.com/jomrr)
- :triangular_flag_on_post: Copyright:: 2024, Jonas Mauer
- :page_with_curl:          License::   [MIT](LICENSE)


---
