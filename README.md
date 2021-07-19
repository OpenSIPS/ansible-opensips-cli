# Role name
This role installs `opensips-cli` from the official OpenSIPS Repositories for Debian and RedHat.

Galaxy
----
Install the role using Ansible Galaxy:
#todo

Role Variables:
----
The following variables can be set to tune the role's install behavior:
* `opensips_build` - indicates the OpenSIPS build. Possible values are releases and nightly. Default value is releases.
* `opensips_yum_release` - indicates the release of OpenSIPS that has been used for RedHat packaging. Default is 6.
* `opensips_version` - indicates the OpenSIPS version. Default value is 3.1 (only for RedHat distributions where the repo includes the OpenSIPS SIP server). 

Examples:
----
The following is an example of a playbook that uses the `opensipscli` role.
```
---
- hosts: all
  roles:
    - role: opensipscli
```
 
License:
----
GPLv3
