## Role Name: Apache2

Ansible role for installing Apache2 on Debian systems.

## Requirements

None.

## Role Variables

Default port configuration file
````yaml
apache_port_config_file: /etc/apache2/ports.conf
````

Virtual host configuration file
````yaml
apache_virtualhost_config_file: /etc/apache2/sites-enabled/000-default.conf
````

Switch to any port depending on your needs. Default port used by Apache2 is 80.
````yaml
apache_http_port: 80
````


## Dependencies

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

## Example Playbook

````yaml
    - hosts: all
      become: yes
      roles:
         - apache2
````

## License

MIT

## Author Information

Role created by Piotr Kurylak.