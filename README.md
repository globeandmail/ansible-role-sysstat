ansible-role-sysstat
======

This role will install sysstat, /etc/sysstat/sysstat (if defined), and will enable sysstat in /etc/default/sysstat (unless explicitly disabled)


Variables
------

```
ansible_role_sysstat_enable: true | false
ansible_role_sysstat_cfg_file: /path/to/group_files/sysstat/sysstat.cfg
```


Notes
------

All files will be copied statically (no templates)

ansible_role_sysstat_cfg_file should point to the sysstat config file - that which will be placed at /etc/sysstat/sysstat.  If this variable is undefined, the install play does not run.

ansible_role_sysstat_enable should be either 'true' or 'false' - the default value is 'true'
