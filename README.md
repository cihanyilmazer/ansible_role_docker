Ansible Role Docker
=========

This role installs and configures docker, containerd and docker-compose on Ubuntu 20.04+.

Requirements
------------

Operating System Support: Ubuntu 20.04 or later

Role Variables
--------------

```
# docker_user: root
docker_address_pool_custom: false
# docker_address_pool_base: 172.20.0.0/16
# docker_address_pool_size: 24
```

Dependencies
------------

No dependency.

Example Playbook
----------------

Install
```
ansible-galaxy install cihanyilmazer.ansible_role_docker
```

    - hosts: servers
      roles:
         - cihanyilmazer.ansible_role_docker

Run with Custom Tags (at least one tag must be provided)
- docker
- docker-install
- docker-configure

```
ansible-playbook -i hosts playbook.yml --tags initial --limit servers
```

License
-------

MIT

Author Information
------------------

Cihan Yilmazer<br />
https://www.cihanyilmazer.com<br />
https://www.github.com/cihanyilmazer<br />
https://galaxy.ansible.com/cihanyilmazer<br />