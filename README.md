ansible-elixir
==============

Ansible role which installs elixir.

Requirements
------------

Tested on ansible 2.4

Role Variables
--------------

```
erlang_version: 20.1
erlang_build_flags: ""
elixir_release: 1.5.1
base_path: /opt
```

Dependencies
------------

* ANXS.erlang (https://github.com/ANXS/erlang)

Example Playbook
----------------


```
- hosts: all
  roles:
    - role: ansible-elixir

```

Testing
-------

run the test script:

    ./test.sh

License
-------

Apache 2.0

Author Information
------------------

http://thomasvolk.de
