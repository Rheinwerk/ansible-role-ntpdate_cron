ntpdate cron
=========

This role installs an hourly cronjob for ntpdate.

[![Build Status](https://travis-ci.org/Rheinwerk/ansible-role-ntpdate_cron.svg?branch=master)](https://travis-ci.org/Rheinwerk/ansible-role-ntpdate_cron)

Requirements
------------

None.

Role Variables
--------------

There is one main variable that drives this role: `_ntpdate_cron`. It is a map that contains all configuration and settings for this role.
Please see `defaults/main.yml` for details.

Dependencies
------------

None.


Example Playbook
----------------

The general contract of this role is to take the variables map `_ntpdate_cron` from `defaults/main.yml` as a template for your configuration and pass that configuration as a parameter to this role.

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      var:
        NTPDATE_CRON:
          ...
      roles:
         - { role: ntpdate_cron, tags: [ 'ntpdate-cron' ], _ntpdate_cron: "{{ NTPDATE_CRON }}" }

License
-------

Please see LICENSE.

Author Information
------------------

Original author is [Daniel Schneller](https://github.com/dschneller) as member of the [Rheinwerk](https://github.com/Rheinwerk) project.

