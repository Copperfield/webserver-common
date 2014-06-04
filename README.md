Webserver-common [![Build Status](https://travis-ci.org/Copperfield/webserver-common.svg?branch=master)](https://travis-ci.org/Copperfield/webserver-common)
================

Common tasks for any Ubuntu webserver machine. It includes the following:
* Installation of:
 * [spf13's vim distribution](https://github.com/spf13/spf13-vim)
 * zsh
 * [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)
* Firewall configuration
* Allowing an RSA access key without introducing a password

Requirements
------------

Tested on Ansible 1.4+

Role Variables
--------------

```yaml
webserver_common_iptables_file:
webserver_common_spf13_output_file_name:
```

See the [defaults](defaults/main.yml) to have a complete view of the variables. Make sure when editing variables, to copy all in your host/vars/... files, and tweak to your liking (actually it's only one variable containing a map ;) ).


Playbook Example
-------------------------
I just do:

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

Feedback, issues and questions are [welcome](https://github.com/Copperfield/webserver-common/issues)!
