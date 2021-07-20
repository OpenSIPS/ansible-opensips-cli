# OpenSIPS CLI
This role installs the
[`opensips-cli`](https://github.com/OpenSIPS/opensips-cli) tool from the
official OpenSIPS Repositories for [Debian](http://apt.opensips.org/) and
[RedHat](http://yum.opensips.org/).

Galaxy
----
Install your role using [Ansible
Galaxy](https://galaxy.ansible.com/razvancrainea/opensips-cli):

```
ansible-galaxy install razvancrainea.opensips-cli
```

Role Variables:
----
The following variables can be set to tune the role's install behavior:
* `opensips_build` - indicates the OpenSIPS build. Possible values are
releases and nightly. Default value is releases.
* `opensips_yum_release` - indicates the release of OpenSIPS that has been
used for RedHat packaging. Default is 6.
* `opensips_version` - indicates the OpenSIPS version. Default value is 3.1
(only for RedHat distributions where the repo includes the OpenSIPS SIP
 server). 

Examples:
----
The following is an example of a playbook that uses the `opensips-cli` role.
```
---
- hosts: all
  roles:
    - role: opensips-cli
```
 
License:
----
GPLv3
