# OpenSIPS CLI
This role installs the
[`opensips-cli`](https://github.com/OpenSIPS/opensips-cli) tool from the
official OpenSIPS Repositories for [Debian](http://apt.opensips.org/) and
[RedHat](http://yum.opensips.org/).

Galaxy
----
Install your role using [Ansible
Galaxy](https://galaxy.ansible.com/razvancrainea/opensips_cli):

```
ansible-galaxy install razvancrainea.opensips_cli
```

Role Variables:
----
The following variables can be set to tune the role's install behavior:
* `opensips_build` - indicates the OpenSIPS build. Possible values are
releases and nightly. Default value is nightly.
* `opensips_yum_release` - pins the release of the `opensips-repo` RPM that
configures the yum repository (not the OpenSIPS version). By default it is
not set and the current `repository.rpm` is used.
* `opensips_version` - indicates the OpenSIPS version whose repository is
used. Default value is 4.0.

Examples:
----
The following is an example of a playbook that uses the `opensips-cli` role.
```
---
- hosts: all
  roles:
    - role: opensips_cli
```
 
License:
----
GPLv3
