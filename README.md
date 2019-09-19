ansible-role-isdev
==================

Install InstallShield on Windows machines.

Requirements
------------

None.

This ansible role by default downloads InstallShield 2019 from Flexera. If you need to download and install another version, you must specify the version, source url and destination path in role variables.

This ansible role runs on both Windows and Linux.

Role Variables
--------------

Variable | Default  | Comment
-------- | -------- | -------
version  | `"2019"` | The InstallShield Release
url      | `https://flexerasoftware.flexnetoperations.com/control/inst/AnonymousDownload?dkey=14741887` | InstallShield Installer URL
dest     | `Downloads/InstallShield2019R2ProfessionalComp.exe` | Download location

Dependencies
------------

None.

Example Playbook
----------------

```yaml
#!/usr/bin/env ansible-playbook
---
- hosts: isdev
  gather_facts: no
  roles:
    - name: pallxk/isdev
      #version: "2019"
      #url: https://flexerasoftware.flexnetoperations.com/control/inst/AnonymousDownload?dkey=14741887
      #dest: Downloads/InstallShield2019R2ProfessionalComp.exe
```

License
-------

MIT

Author Information
------------------

[pallxk](https://github.com/pallxk)
[testcab](https://github.com/testcab)
