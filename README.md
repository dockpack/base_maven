[![Galaxy](https://img.shields.io/badge/galaxy-dockpack.base__maven-blue.svg?style=flat)](https://galaxy.ansible.com/dockpack/base_maven)
![Build Status](https://travis-ci.com/dockpack/base_maven.svg?branch=master)

Maven - Maven is good at building Java projects in a cross-platform way. It manages dependencies, and actually the whole life cycle of a project. This is an ansible-role to install Maven.

Requirements
------------

This role was built for Ubuntu Trusty or RedHat systems like RHEL 6, Centos 7. It needs dockpack.base_java8.

Role Variables
--------------
You can set the maven\_version:, now 3.5.0

There are 3 variables that you would store in a vault file:

mvn\_master\_password:

mvn\_repo\_username:

mvn\_repo\_password:


Dependencies
------------

Maven needs Java8. This role depends on dockpack.base_java8, which will be installed automatically if you use this one.



Example Playbook
----------------
For a complete example with this role check out my buildserver:
git clone https://github.com/bbaassssiiee/buildserver.git

Example of how to use this role:

    - hosts: servers
      roles:
         - { role: dockpack.base_maven }

License
-------

MIT

Author Information
------------------
Bas Meijer @bbaassssiiee
