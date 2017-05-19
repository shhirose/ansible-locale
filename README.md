# ansible-locale

This is Ansible role for change locale for RedHat Enterprise Linux, Ubuntu and Debian.

## Requirements

None

## Role Variables

* locale - The value for variable LANG

## Dependencies

None

## Example Playbook

Example:

```yaml
- hosts: servers
  become: yes
  roles:
     - { role: shhirose.locale }
  vars:
    locale: "ja_JP.UTF-8"
```

Result (CentOS):

```
$ sudo localectl
   System Locale: LANG=ja_JP.UTF-8
       VC Keymap: us
      X11 Layout: n/a
```

## License

MIT
