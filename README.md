# Ansible role: ttrss
PHP-based RSS reader

## Requirements
Only tested on Debian stable, for now.

## Role Variables
+ 

## Dependencies
+ nginx
+ php-fpm
+ PostgreSQL

## Example Playbook

```
- hosts: ttrss
  roles:
    - { role: ho-ansible.ttrss }
```

## License
MIT

## Author Information
Sean Ho, https://github.com/ho-ansible/
