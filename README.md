
NOTE: Most of this is obsolete.

cmk-utils
=========

A few ansible snippets for checkmk, to include in your playbooks.

These are provided as-is in the hope they will be useful, but with no warranty of any kind.

This is a personal project, not maintained nor endorsed by CheckMK authors.

Features
--------

* have a look at the tasks directory and at comments in the snippets.

How to Use
----------

One way to use the snippets is to include them in your playbooks/roles like this:

```
- name: Run CheckMK plugin installation
  include_role:
    name: cmk-utils
    tasks_from: install_mkp.yml
  vars:
    name: robotmk
    url: "{{ robotmk_download_url }}"
```

Dependencies
------------

* tribe29.checkmk >= 0.16.0
