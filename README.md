ansible-elixir
==============

Ansible role which installs elixir.

[![Build Status](https://travis-ci.org/thomasvolk/ansible-elixir.svg?branch=master)](https://travis-ci.org/thomasvolk/ansible-elixir)

Requirements
------------

Tested on ansible 2.4

Role Variables
--------------

```
elixir_release: 1.5.1
base_path: /opt
```

Dependencies
------------

* ANXS.erlang (https://github.com/ANXS/erlang)

Test
----

You have to install the tools first:
```
pip install docker ansible molecule
```

For tests just run molecule test:
```
molecule test
```

Example Playbook
----------------

Use ansible-elixir role together with a erlang role. Here is an example:

```
- hosts: all
  roles:
    - role: ANXS.erlang
    - role: ansible-elixir

```

Testing
-------

use molecule to the the role:

    molecule test

License
-------

Apache 2.0

Author Information
------------------

http://thomasvolk.de
