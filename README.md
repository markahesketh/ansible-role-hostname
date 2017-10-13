# Ansible Role: Hostname

[![Build Status](https://travis-ci.org/markahesketh/ansible-role-hostname.svg?branch=master)](https://travis-ci.org/markahesketh/ansible-role-hostname)

Ansible role to set hostname and hosts using the playbook's inventory.

## Installation

```
ansible-galaxy install markahesketh.hostname
```

## Role Variables

This role does not use standard Ansible role variables.

The hostname will be set based upon the host's inventory within the playbook.

```
[production]
myinstance ansible_host=0.0.0.0
```

This instance would have it's hostname set to `myinstance`.

## Dependencies

None.

## Example Playbook

```yml
- hosts: web
  roles:
    - markahesketh.hostname
```

## Testing

    molecule test

Requires [Molecule](https://molecule.readthedocs.io/en/latest/) and [Docker](https://docs.docker.com/engine/installation/).

## License

This role is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT).

## Author

By [Mark Hesketh](https://www.markhesketh.co.uk/), a web developer from Manchester, UK.

* Blog: [markhesketh.co.uk](https://www.markhesketh.co.uk/)
* Twitter: [twitter.com/markahesketh](https://www.twitter.com/markahesketh/)
* GitHub: [github.com/markahesketh](http://www.github.com/heskethm/)
* Email: [contact@markhesketh.co.uk](mailto:contact@markhesketh.co.uk)
