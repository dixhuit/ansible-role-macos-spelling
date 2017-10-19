# Ansible role: macOS custom spelllingz

[![Build Status](https://travis-ci.org/danbohea/ansible-role-spelling.svg?branch=master)](https://travis-ci.org/danbohea/ansible-role-spelling)

Creates & populates a custom LocalDictionary file on macOS.


## Requirements

- macOS 10.10, 10.11 or 10.12


## Role Variables

All role default variables are listed below along with their respective default values.

```yaml
spelling_localdictionary_words:
  - Ansible
  - idempotence
  - Macsible
```

Words to add to the custom LocalDictionary file. These do not have to be in alphabetical order (the role will take care of sorting for you).


## Dependencies

None.


## Example Playbook

```yaml
- hosts: macbook
  connection: local

  roles:
    - role: ansible-role-spelling
```

## License

MIT


## Author Information

This role was created by [Dan Bohea](http://bohea.co.uk) primarily for use with [Macsible](https://github.com/macsible/macsible).
