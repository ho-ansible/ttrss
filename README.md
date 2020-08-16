# Ansible role: ttrss
PHP-based RSS reader

## DEPRECATED
Installation of this app has been moved to kubernetes,
so this ansible role is no longer maintained.

## Requirements
Only tested on Debian stable, for now.

## Role Variables
+ `ttrss_host`: nginx virtual hostname
+ `ttrss_url` (default: "http://{{ ttrss_host }}/"):
  URL by which the instance will be accessed
+ `ttrss_www` (default: /var/www/tt-rss): dir in which to install TT-RSS, accessible by nginx
+ `ttrss_user` (default: ttrss) unprivileged user to run fetch cronjob
+ `ttrss_db_pw`: password for PostgreSQL user
+ `ttrss_listen`: list of nginx "listen" directives. by default, only listens on localhost:80.

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
