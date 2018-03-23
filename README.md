# Ansible Role: mongo-hacker [![Build Status](https://travis-ci.org/eilgin/ansible-role-mongo-hacker.svg?branch=master)](https://travis-ci.org/eilgin/ansible-role-mongo-hacker)

This will install the latest mongodb shell enhancements in the home directory of the defined user.

## Requirements

Requires `git` and `make` on the host machine. See the [limitations](https://github.com/TylerBrock/mongo-hacker#warnings) of this script.

Tests have been done on **Debian** machines (and its variants) but this role should work on any Linux machines that respect the FHS.

## Role Variables

- `user`: define where the script will be installed (default is `ansible_user`).
- `mongo_hacker_dir`: define where the clone repository will be installed on the home directory of the `user` (default is `.mongo-hacker`)

## Dependencies

None.

## Example Playbook

```yml
- hosts: localhost
  roles:
    - { role: eilgin.mongo-hacker }
```

## License

MIT

## Author Information

eilgin
