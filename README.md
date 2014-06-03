Webserver-common [![Build Status](https://travis-ci.org/Copperfield/webserver-common.svg?branch=master)](https://travis-ci.org/Copperfield/webserver-common)
================

Common task for any  Ubuntu webserver machine.

Requirements
------------

Tested on Ansible 1.4+

Role Variables
--------------

```yaml
webserver_common_iptables_file:
webserver_common_spf13_output_file_name:
```

See the [defaults](defaults/main.yml) to have the complete view. Make sure, if you edit them, to copy all of them in your host/vars/... files, and change the ones that need tweaking (it’s in fact only one variable, containing a map.)


Example Playbook
-------------------------
 Just I do:

```yaml
    - hosts: servers
      roles:
         - { role: webserver-common }
```
License
-------

MIT

Author Information
------------------

Feedback, issues and question....
You are [welcome](https://github.com/Copperfield/webserver-common/issues)!
