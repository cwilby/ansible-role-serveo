# Ansible Role: Serveo

Installs Serveo on Ubuntu.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    domain: "serveo.yourdomain.com"

The root domain which subdomains will sprout from, e.g. `abcdef.serveo.yourdomain.com`.

    serveo_user: "serveo"

The user that serveo should run for.

## Dependencies

None.

## Example Playbook

```yml
- hosts: utility
  vars:
    domain: serveo.yourdomain.com
  roles:
    - cwilby.serveo
```