# ansible-role-jetbrains-toolbox

[![molecule](https://github.com/diodonfrost/ansible-role-jetbrains-toolbox/workflows/molecule/badge.svg)](https://github.com/diodonfrost/ansible-role-jetbrains-toolbox/actions)
[![Ansible Galaxy](https://img.shields.io/badge/galaxy-diodonfrost.jetbrains_toolbox-660198.svg)](https://galaxy.ansible.com/diodonfrost/jetbrains_toolbox)

Install JetBrains Toolbox

## Example Playbook

This example is taken from molecule/default/converge.yml and is tested on each push, pull request and release.

    - name: converge
      hosts: all
      roles:
         - role: diodonfrost.jetbrains_toolbox

## Local Testing

This project uses [Molecule](http://molecule.readthedocs.io/) to aid in the
development and testing.

To develop or test you'll need to have installed the following:

* Linux (e.g. [Ubuntu](http://www.ubuntu.com/))
* [Docker](https://www.docker.com/)
* [Python](https://www.python.org/) (including python-pip)
* [Ansible](https://www.ansible.com/)
* [Molecule](http://molecule.readthedocs.io/)

### Testing with Docker

    # Install requirements
    pip install -r requirements-dev.txt
    
    # Test ansible role with ubuntu 20.04
    molecule test
    
    # Test ansible role with debian 11
    image=ansible-debian:11 molecule test
    
    # Create debian 11 instance
    image=ansible-debian:11 molecule create
    
    # Apply role on debian 11 instance
    image=ansible-debian:11 molecule converge
    
    # Launch tests on debian 11 instance
    image=ansible-debian:11 molecule verify

## License

Apache-2.0

## Author Information

This role was created in 2021 by diodonfrost.
