## Docker Role
![CI](https://github.com/hybridadmin/ansible-role-docker/workflows/CI/badge.svg?branch=main)

> An ansible role to install [`docker`](https://docs.docker.com/engine/install/) on all supported linux distros, with the ability to choose between the `stable` , `nightly` and `test` release channels.


## Requirements

None


## Role Variables

The variables below can be edited in [`defaults/main.yml`](defaults/main.yml) to customize the deployment:

* `docker_release_channel`:[default: `stable`] The release channel from which docker should be installed.
* `enable_docker_compose `:[default: `true`] Specify whether docker compose should be installed as well.
* `docker_users` : The users that should be added to the docker group. If left empty only the user running
the playbook will be added.


## Dependencies

None

## Example Playbook

The playbook definition below can be used to deploy docker using the `stable` release channel:

```yaml
    - hosts: servers
      vars:
        docker_release_channel: "stable"
        enable_docker_compose: true
        docker_users:
          - user1
          - user2
      roles:
         - { role: hybridadmin.docker }
```

## License

[Apache License](./LICENSE)


## Author Information

Created by Hybridadmin.
