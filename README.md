# Ansible Role: mongo-hacker

This will install the latest mongodb shell enhancements in the home directory of the defined user.

## Requirements

Requires git on the host machine. See the [limitations](https://github.com/TylerBrock/mongo-hacker#warnings) of this script.

## Role Variables

- `user`: define where the script will be installed (default is `remote_user`).

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
