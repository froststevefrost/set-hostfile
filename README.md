Set-Hostfile
=========

Role will grab all of the hosts defined in the default inventory and create a typical /etc/hosts file, similar to:

```
127.0.0.1   localhost localhost.localdomain localhost4 localhost4.localdomain4
::1         localhost localhost.localdomain localhost6 localhost6.localdomain6

192.168.1.50 controller.example.com controller
192.168.1.51 node1.example.com node1
192.168.1.52 node2.example.com node2
```


Requirements
------------

No requirements.

Role Variables
--------------

No role variables.


Dependencies
------------

No dependencies.

Example Playbook
----------------

```yaml
  - name: Set /etc/hosts file to Ansible inventory hosts
    hosts: servers
    become: true
    roles:
      - role: 
```
License
-------

GPL-3.0-or-later

Author Information
------------------

Steve Frost (froststevefrost)
