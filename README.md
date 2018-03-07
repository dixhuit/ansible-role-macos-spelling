# Ansible role: macOS custom spelllingz

[![Build Status](https://travis-ci.org/danbohea/ansible-role-spelling.svg?branch=master)](https://travis-ci.org/danbohea/ansible-role-spelling)

Creates & populates a custom LocalDictionary file on macOS.


## Requirements

- Ansible >= 2.1
- macOS 10.13, 10.12, 10.11 or 10.10


## Role Variables

```yaml

# Words to add to the custom LocalDictionary file.
# These do not have to be in alphabetical order
# (the role will take care of sorting for you).
spelling_localdictionary_words:
  - Ansible
  - idempotence
  - Macsible

```


## Dependencies

None.


## Example Playbook

```yaml
- hosts: all

  roles:
    - role: ansible-role-spelling
```

## License

MIT


## Author Information

This role was created by [Dan Bohea](http://bohea.co.uk) primarily for use with [Macsible](https://github.com/macsible/macsible).
