Role Name
=========

Installation of the open source version of Artifactory.

Connect via `http://<some ip>:8081/artifactory/` using the credentials `admin`/`password`.
After logging into the system, you can opt to import my system configuration.  The
export folder is in the home directory of provisioned machine and is named `artifactory-system-export`.
When you imort the system, you must ensure that ` Exclude Content` and ` Exclude Metadata` have been selected.
Otherwise, the import will fail.

Requirements
------------

TODO

Role Variables
--------------

* artifactory_install: true

Dependencies
------------

* kurron.jdk

Example Playbook
----------------

```
- hosts: servers
  roles:
      - { role: kurron.artifactory }
```

License
-------

This project is licensed under the [Apache License Version 2.0, January 2004](http://www.apache.org/licenses/).

Author Information
------------------

[Author's website](http://jvmguy.com/).
