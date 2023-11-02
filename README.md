## htop

[![CI](https://github.com/Oefenweb/ansible-htop/workflows/CI/badge.svg)](https://github.com/Oefenweb/ansible-htop/actions?query=workflow%3ACI)
[![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-htop-blue.svg)](https://galaxy.ansible.com/Oefenweb/htop)

Set up htop in Debian-like systems.

#### Requirements

None

#### Variables

* `htop_htoprc_destinations` [default: `{skell: dest: /etc/skel/.config/htop, current: dest: "{{ ansible_env.HOME }}/.config/htop"}`]: Destinations to copy the htoprc file to
* `htop_htoprc_destinations.key`: The identifier of the file (e.g. `skel`)
* `htop_htoprc_destinations.key.dest`: The remote path of the file to copy (e.g. `/etc/skel`)
* `htop_htoprc_destinations.key.owner`: The name of the user that should own the file (optional, default `root`)
* `htop_htoprc_destinations.key.group`: The name of the group that should own the file (optional, default `owner`, then `root`)
* `htop_htoprc_destinations.key.mode`: The mode of the file, such as 0644 (optional, default `0644`)

* `htop_replace_htoprc`: [default: `true`]: Whether or not to overwrite existing htoprc files

## Dependencies

None

#### Example

```yaml
---
- hosts: all
  roles:
    - oefenweb.htop
```

#### License

MIT

#### Author Information

Mischa ter Smitten

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Oefenweb/ansible-htop/issues)!
