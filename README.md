# ansible-rkt-binary

[![Build Status](https://travis-ci.org/suzuki-shunsuke/ansible-rkt-binary.svg?branch=master)](https://travis-ci.org/suzuki-shunsuke/ansible-rkt-binary)

ansible role to install [rkt](https://github.com/rkt/rkt) from binary.

https://galaxy.ansible.com/suzuki-shunsuke/rkt-binary/

## Requirements

Nothing.

## Role Variables

name | required | default | description
--- | --- | --- | ---
rkt_binary_version | yes | | installed binary version
rkt_binary_install_dir | no | /usr/local/bin | The install path. This directory is generated if it doesn't exist

## Dependencies

Nothing.

## Example Playbook

```yaml
- hosts: servers
  roles:
    - role: suzuki-shunsuke.rkt-binary
      rkt_binary_version: v1.28.1
      rkt_binary_install_dir: /usr/local/bin
      become: yes
```

## Change Log

See [CHANGELOG.md](CHANGELOG.md).

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

[MIT](LICENSE)
