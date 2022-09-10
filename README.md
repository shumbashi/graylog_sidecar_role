Graylog Sidecar Role
=========

Ansible role to install Graylog-Sidecar replacing Collector-Sidecar on Linux servers

Tested on:
  - CentOS 7
  - CloudLinux 7

TODO:
  - Add Windows support

Requirements
------------

None

Role Variables
--------------

The role accepts two variables:
- `graylog_url` string (required) Graylog API URL
- `graylog_api_token` string (required) Graylog API Token

Dependencies
------------

- libyanspider.firewall_ansible_role

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: libyanspider.graylog_sidecar_role, graylog_url: https://graylog.server.com/api/, graylog_api_token: "SECRETTOKEN" }

License
-------

BSD

Author Information
------------------

Ahmed Shibani (Twitter: @ashibani, Github: [shumbashi](https://github.com/shumbashi))