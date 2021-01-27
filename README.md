## Docker Role
=========

An ansible role to install [docker](https://docs.docker.com/engine/install/) on all supported linux distros, with the ability to choose between the `stable` , `nightly` and `test` release channels.

## Requirements
------------

None.


## Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

## Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

## Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      vars:
        docker_release_channel: "stable"
        enable_docker_compose: true
        docker_users:
          - user1
          - user2        
      roles:
         - { role: hybridadmin.docker }

## License
-------

[Apache License](./README.md)

## Author Information
------------------

Created by Hybridadmin.
