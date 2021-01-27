## Docker Role

> An ansible role to install [docker](https://docs.docker.com/engine/install/) on all supported linux distros, with the ability to choose between the `stable` , `nightly` and `test` release channels.


## Requirements

None


## Role Variables

The variables can be edited in [defaults/main.yml](defaults/main.yml) to customize the deplohyment:

`docker_release_channel` : [default: stable]

`enable_docker_compose` : [default: true]

`docker_users` :


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
