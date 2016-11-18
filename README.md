ansible-logdna
=========

[![Build Status](https://travis-ci.org/mikoim/ansible-logdna.svg?branch=master)](https://travis-ci.org/mikoim/ansible-logdna)

Install LogDNA's collector agent.

Requirements
------------

This role requires Ansible 2.1 or higher.

Role Variables
--------------

```yaml
# API Key (recommended)
logdna_api_key: 0123456789abcdef0123456789abcdef

# Monitoring directories and files (optinal)
logdna_monitoring_directories:
  - /opt/foo/bar/log
  - /srv/hoge/logs
logdna_monitoring_files:
  - /opt/foo/bar/access.log
  - /srv/hoge/logs/errors.log
```

Dependencies
------------

None

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
     - { role: mikoim.logdna }
```

License
-------

MIT
