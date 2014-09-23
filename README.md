newrelic-php
============

An Ansible role to setup New Relic PHP agent: 
https://docs.newrelic.com/docs/php/new-relic-for-php


Requirements
------------

Ubuntu Trusty with PHP installed. This role tries to restart PHP-FPM and/or the Apache web server.


Role Variables
--------------

The variables that can be passed to this role and a brief description about them are as follows

    # License key (required)
    newrelic_license_key: ~

    # Application name (required)
    newrelic_appname: "{{ ansible_hostname }} PHP"


Dependencies
------------

Requires the New Relic repository to be set up; depends on [sivel.newrelic](https://github.com/sivel/ansible-newrelic) for this purpose.


License
-------

MIT

