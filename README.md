## htop [![Build Status](https://travis-ci.org/Oefenweb/ansible-htop.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-htop)

Set up htop in Debian-like systems.

#### Requirements

None

#### Variables

* `htop_htoprc_destinations`: [default: `[/etc/skel/.config/htop, {{ ansible_env.HOME }}/.config/htop]`]: Destinations to copy the htoprc file to
* `htop_replace_htoprc`: [default: `false`]: Whether or not to overwrite existing htoprc files

## Dependencies

None

#### Example

```yaml
---
- hosts: all
  roles:
  - htop
```

#### License

MIT

#### Author Information

Mischa ter Smitten

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Oefenweb/ansible-htop/issues)!
