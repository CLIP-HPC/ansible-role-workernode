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

    grid_worker_install_htc_ce_client: false

Install HTCondor CE client

## Dependencies

*   hephyvienna.grid

## Example Playbook

    - hosts: all
      roles:
        - role: geerlingguy.repo-epel
        - role: hephyvienna.grid
          vars:
            grid_vos:
              - cms
              - alice
              - belle
            grid_umd_repo_exclude:
              - dpm-*
              - lfc-*
              - lcgdm-*
        - role: hephyvienna.grid-worker


## License

MIT

## Author Information

Written by [Dietrich Liko](http://hephy.at/dliko) in May 2019

[Institute for High Energy Physics](http://www.hephy.at) of the
[Austrian Academy of Sciences](http://www.oeaw.ac.at)
