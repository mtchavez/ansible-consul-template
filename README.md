Ansible Role - mtchavez.consul-template
=========
[![Latest Version](http://img.shields.io/github/release/mtchavez/ansible-consul-template.svg?style=flat-square)](https://github.com/mtchavez/ansible-consul-template/releases)
[![Build Status](https://travis-ci.org/mtchavez/ansible-consul-template.svg?branch=master)](https://travis-ci.org/mtchavez/ansible-consul-template)

[consul-template](https://github.com/hashicorp/consul-template) allows for generic template rendering and notifications with [Consul](https://github.com/hashicorp/consul)

Requirements
------------

No requirements needed to install consul-template

Role Variables
--------------

Useful variables to configure such as the version and arch or even where it is downloaded.

```yaml
consul_template_ver: "0.9.0"
consul_template_arch: "linux_amd64"
consul_template_dl_dir: "/tmp"
consul_template_bin_path: "/usr/local/bin"
```

Dependencies
------------

No external dependencies

Example Playbook
----------------

Install consul-template at a specific version

    - hosts: servers
      roles:
         - { role: mtchavez.consul-template, consul_template_ver: "0.9.0", become: yes }

License
-------

MIT

Author Information
------------------

mtchavez - 2015
