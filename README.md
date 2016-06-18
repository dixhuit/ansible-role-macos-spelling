# Ansible role: OS X custom spelllingz

[![Build Status](https://travis-ci.org/danbohea/ansible-role-spelling.svg?branch=master)](https://travis-ci.org/danbohea/ansible-role-spelling)

Creates & populates a custom LocalDictionary file on Mac OS X.


## Requirements

- Mac OS 10.9+


## Role Variables

All role default variables are listed below along with their respective default values.

```
spelling_localdictionary_words:
  - Ansible
  - idempotence
  - Macsible
```

Words to add to the custom LocalDictionary file. These do not have to be in alphabetical order (the role will take care of sorting for you).


## Dependencies

None.


## Example Playbook

```
- hosts: macbook
  connection: local

  roles:
    - role: ansible-role-spelling
```

## License

MIT


## Author Information

This role was created by [Dan Bohea](http://bohea.co.uk) primarily for use with [Macsible](https://github.com/danbohea/macsible).
