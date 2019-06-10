
Ansible Role: ansible-epel-repo
=========

[![Build Status](https://travis-ci.org/Protopopys/ansible-epel-repo.svg?branch=master)](https://travis-ci.org/Protopopys/ansible-epel-repo)

An Ansible Role that installs EPEL repository.

Requirements
------------

None.

Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

```yaml
  epel_repo_url: "https://dl.fedoraproject.org/pub/epel/epel-release-latest-{{ ansible_distribution_major_version }}.noarch.rpm"
  epel_repo_gpg_key_url: "/etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-{{ ansible_distribution_major_version }}"
  epel_repo_file_path: "/etc/yum.repos.d/epel.repo"
```

Dependencies
------------

None.

Example Playbook
----------------

```yaml
- hosts: all
  roles:
    - protopopys.ansible-epel-repo
```

License
-------

MIT

Author Information
------------------

This role was created in 2019 by Kirill Protopopov.
