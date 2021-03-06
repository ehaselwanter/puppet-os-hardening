# Changelog

## 0.1.3

**API-change**: `dry_run_on_unkown` is now `dry_run_on_unknown`

* feature: allow configuration of custom modules (if module loading is disabled)
* improvement: only remove SUID/SGID if necessary
* improvement: clarify SUID/SGID options
* improvement: use thias/sysctl to configure sysctls (also fixes previous bugs with the template)
* improvement: add spec tests for sysctl options
* improvement: puppet-lint everything
* improvement: add travis testing for lint+specs
* improvement: use file resource instead of exec for access minimization
* bugfix: fix typo dry_run_on_unkown -> dry_run_on_unknown
* bugfix: don't run update initramfs on each run, only when requiered
* bugfix: deactivation of kernel module loading wasn't implemented
* bugfix: ip_forwarding wasn't activated correctly

## 0.1.2

* feature: add additional ipv6 hardening to sysctl
* feature: add test kitchen
* improvement: remove unnecessary attributes from os_hardening::pam
* bugfix: remove cracklib if passwdqc is used

## 0.1.1

* feature: add configurable system environment
* feature: remove suid/sgid bits from blacklist
* feature: remove suid/sgid bits from unkown files

## 0.1.0

* port from chef-os-hardening and monolithic puppet implementation
