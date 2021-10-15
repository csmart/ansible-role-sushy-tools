Role Name
=========

Super basic role to install and start Sushy Tools as root, talking to `libvirtd`.

Requirements
------------

none

Role Variables
--------------

You can set a few variables:

 - `sushy_user` - the user to run as, defaults to `root` (note that a non-root user will need to be able to talk to `libvirtd` unauthenticated)
 - `sushy_ip` - the IP address to listen on, defaults to `0.0.0.0`
 - `sushy_port` - the port to listen on, defaults to `8080`

Dependencies
------------

none

Example Playbook
----------------


```yaml
---
- hosts: all
  roles:
    - csmart.sushy
```

License
-------

GPLv3+

Author Information
------------------

Chris Smart https://blog.christophersmart.com
