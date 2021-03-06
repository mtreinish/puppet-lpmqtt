lpmqtt
=======

#### Table of Contents

1. [Overview - What is the lpmqtt module?](#overview)
2. [Module Description - What does the module do?](#module-description)
3. [Setup - The basics of getting started with lpmqtt](#setup)
4. [Implementation - An under-the-hood peek at what the module is doing](#implementation)
5. [Limitations - OS compatibility, etc.](#limitations)
6. [Development - Guide for contributing to the module](#development)
7. [Contributors - Those with commits](#contributors)

Overview
--------

The lpmqtt module is a part of [OpenStack-infra](http://docs.openstack.org/infra/system-config/), an effort by the OpenStack infrastructure team to provide continuous integration testing and code review for OpenStack-infra projects.

Module Description
------------------

The lpmqtt module is a thorough attempt to make Puppet capable of managing the entirety of lpmqtt.  This includes manifests to provision the expected features of this module.  Types are shipped as part of the lpmqtt module to assist in manipulation of configuration files.

Setup
-----

### Installing lpmqtt

    lpmqtt is not currently in Puppet Forge, but is anticipated to be added soon.  Once that happens, you'll be able to install lpmqtt with:
    puppet module install openstack-infra/lpmqtt

### Beginning with lpmqtt

To utilize the lpmqtt module's functionality please check the README.

Implementation
--------------

### lpmqtt

lpmqtt is a combination of Puppet manifests to delivery configuration and extra functionality through types and providers.

Beaker-Rspec
------------

This module has beaker-rspec tests

To run the tests on the default vagrant node:

```shell
bundle install
bundle exec rake acceptance
```

For more information on writing and running beaker-rspec tests visit the documentation:

* https://github.com/puppetlabs/beaker/wiki/How-to-Write-a-Beaker-Test-for-a-Module

Development
-----------

Developer documentation for the entire puppet-infra project.

* http://docs.openstack.org/infra/system-config/puppet.html
