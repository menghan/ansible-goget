goget
=====

run goget on:

* Ubuntu 14.04+
* Debian Jessie (8.5+) and Stretch


**Example Play**:

Very basic install utilizing the role defaults:

```
---
- name: goget present
  hosts: all
  vars:
    goget_app: github.com/golang.org/x/tools/present
  roles:
    - menghan.goget
```


Requirements
------------

None.

Role Variables
--------------

Please see [defaults/main.yml](https://github.com/menghan/ansible-goget/blob/master/defaults/main.yml) for a comprehensive list of variables that can be overridden.

Dependencies
------------

None.

Testing
-------

To test the role in a Vagrant environment just run `vagrant up`.  This will
create some VMs:

* Ubuntu 12.04
* Ubuntu 14.04
* Ubuntu 16.04
* Debian Jessie 8.5
* Debian Stretch 9.0

and it will provision them by applying this role with Ansible.

Requires `ansible-playbook` to be in the path.

License
-------

Apache v2.0
