Haevas.powerpill
===

[![Build Status](http://img.shields.io/travis/Haevas/Haevas.powerpill.svg?style=flat-square)](https://travis-ci.org/Haevas/Haevas.powerpill)
[![Galaxy](http://img.shields.io/badge/galaxy-Haevas.powerpill-blue.svg?style=flat-square)](https://galaxy.ansible.com/list#/roles/5797)

An Ansible role for installing `powerpill`, `pacserve` and `reflector` on Arch
Linux based systems.

#### Requirements & dependencies

None

#### Role Variables

```yaml
powerpill_enabled: yes                                 # The role in enabled
powerpill_sync_deps: yes                               # Sync db and base-devel
```

See [this file](defaults/main.yml) for a full list and their default values.

#### Usage

Add `Haevas.powerpill` to your roles and enable it.

```yaml
- hosts: all

  roles:
  - Haevas.powerpill

  vars:
  - powerpill_enabled: yes
  - powerpill_sync_deps: yes
```

#### Contributing

Issues, feature requests, ideas are [appreciated](https://github.com/Haevas/Haevas.powerpill/issues). Pull requests are also very welcome. Preferably, create a topic branch and when submitting, squash your commits into one (with a descriptive message).

#### License

BSD. See the LICENSE file for details.
