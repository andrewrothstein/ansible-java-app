andrewrothstein.java-app
=========

Downloads and injects a named and versioned Java uber jar. Useful for deploying Java applications out of [Artifactory](https://www.jfrog.com/artifactory/).

Requirements
------------

See [meta/main.yml](meta/main.yml)

Role Variables
--------------

See [defaults/main.yml](defaults/main.yml)

Dependencies
------------

See [meta/main.yml](meta/main.yml)

Please install a valid JRE to run the uber jar.

Example Playbook
----------------

```yml
- hosts: servers
  roles:
    - role: andrewrothstein.java-app
	  java_app_mirror: https://myartifactory/libs-releases-local/foo/bar
	  java_app_name: myapp
	  java_app_ver: v1.0.0
```

License
-------

MIT

Author Information
------------------

Andrew Rothstein <andrew.rothstein@gmail.com>
