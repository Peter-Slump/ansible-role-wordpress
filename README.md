# Ansible role Wordpress

Version: 0.0.1

Supported OS: Ubuntu

Ansible role for Wordpress

## Role variables

```
wordpress_user: wordpress
wordpress_group: "{{ wordpress_user }}"
wordpress_home: "/home/{{ wordpress_user }}"

wordpress_version: 4.8
wordpress_install_dir: "{{ wordpress_home }}"

wordpress_db_name: 'wordpress'
wordpress_db_user: 'wordpress'
wordpress_db_password: ' ** CHANGE ME TO A SUPER SECRET PASSWORD ** '
wordpress_db_host: 'localhost'
wordpress_db_charset: 'utf8'
wordpress_db_collate: ''
wordpress_table_prefix: 'wordpress_'
wordpress_debug: false

wordpress_fs_method: 'direct'
wordpress_lang: ''
```

## example

```
- hosts: all
  roles:
    - role: wordpress
```
