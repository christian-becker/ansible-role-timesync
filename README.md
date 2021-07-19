timesync
========

This ansible role is to enable timesync on linux systems.
Please adjust timezone and ntp servers as needed.


Requirements
------------

This role has no special requirements.


Role Variables
--------------

Here is a list of variables defined in **defaults/main.yml**: 

```
# timesync_timezone_name - e.g. UTC or Europe/Berlin
timesync_timezone_name: Europe/Berlin

# timesync_timeservers - e.g. 192.168.1.1 or de.pool.ntp.org
timesync_timeservers:
  - 0.de.pool.ntp.org
  - 1.de.pool.ntp.org
  - 2.de.pool.ntp.org
  - 3.de.pool.ntp.org
```


Dependencies
------------

This role has no dependencies.


Example Playbook
----------------

This role can be used e.g. with the following playbook:
```
---
- name: enable timesync
  hosts: linux_server
  remote_user: root
  roles:
    - christian_becker.timesync
```


License
-------

MIT


Author Information
------------------

* **Christian Becker** - [christian-becker](https://github.com/christian-becker)  

