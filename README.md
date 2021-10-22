rnp-tools-ansibleroles-settimezone
=========

Ansible Role - Set locale

![Overwiew](https://gitlab.com/rachuna-net.pl/tools/ansibleroles/rnp-tools-ansibleroles-settimezone/-/raw/develop/docs/settimezone.png)

Role Variables
--------------

Defaults role values:
```
input_time_zone:
  name: "Europe/Warsaw"
  src:  "/usr/share/zoneinfo/Europe/Warsaw"

input_locale_list:
  - en_US.UTF-8
  - pl_PL.UTF-8
```

Example Playbook
----------------

```
  - hosts: localhost
    remote_user: root
    tasks:
    - include_role:
        name: rnp-tools-ansible-roles-setimezone
      vars:
        input_time_zone:
          name: "Europe/Warsaw"
          src:  "/usr/share/zoneinfo/Europe/Warsaw"

        input_locale_list:
          - en_US.UTF-8
          - pl_PL.UTF-8
```

License
-------

BSD 3-Clause

Author Information
------------------

### Maciej Rachuna
SysOps/DevOps