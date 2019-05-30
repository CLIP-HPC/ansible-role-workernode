# grid-worker

[![pipeline status](https://gitlab.cern.ch/hephyvienna/ansible/role-grid-worker/badges/master/pipeline.svg)](https://gitlab.cern.ch/hephyvienna/ansible/role-grid-worker/commits/master)
<!-- TODO Add badge -->
<!-- [![galaxy](https://img.shields.io/badge/galaxy-dietrichliko.grid-worker-40775.svg?logo=galaxy)](https://galaxy.ansible.com/dietrichliko/grid-worker) -->

Ansible role for installation of WLCG/EGI woker node or user interface


# Requirements

-   EL6/7
-   EPEL

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    grid_worker_ui: false

Request installation of user interface

Dependencies
------------

* hephyvienna.grid
* hephyvienna.cvmfs

## Example Playbook

## License

MIT

## Author Information

Written by [Dietrich Liko](http://hephy.at/dliko) in May 2019

[Institute for High Energy Physics](http://www.hephy.at) of the
[Austrian Academy of Sciences](http://www.oeaw.ac.at)
