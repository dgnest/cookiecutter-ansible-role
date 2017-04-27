# Ansible Role Cookiecutter

[![Build Status](https://travis-ci.org/dgnest/cookiecutter-ansible-role.svg)](https://travis-ci.org/dgnest/cookiecutter-ansible-role)
[![GitHub issues](https://img.shields.io/github/issues/dgnest/cookiecutter-ansible-role.svg)](https://github.com/dgnest/cookiecutter-ansible-role/issues)
[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/dgnest/cookiecutter-ansible-role.svg)](http://isitmaintained.com/project/dgnest/cookiecutter-ansible-role "Average time to resolve an issue")
[![Percentage of issues still open](http://isitmaintained.com/badge/open/dgnest/cookiecutter-ansible-role.svg)](http://isitmaintained.com/project/dgnest/cookiecutter-ansible-role "Percentage of issues still open")
[![GitHub license](https://img.shields.io/github/license/mashape/apistatus.svg?style=flat-square)](LICENSE)

Cookie cutter recipe to easily create [ansible roles][link-playbooks-roles]
It infuses antigravity (or maybe not).

## Features

  * Follows [best practices][link-best-practices].
  * Only Creates the necessary files and folders.
  * Blazing fast creation, forget about file creation and focus in actions.


## Requirements

 - Linux
   - none
 - OSX
   - none

## Usage

    cookiecutter https://github.com/dgnest/cookiecutter-ansible-role.git

It begin to ask you configuration variables then you can enter tasks names,
handlers names, and default variables.

Inside a `Add <some> name i.e (<example>)` you can go to next section by entering
an empty string.


Example:

    ROLE CONFIGURATION:
    ===================

    Should it have files?  [Y/n] y

This will generate this folders (Please note the absence of templates folder):

    ├── CHANGELOG.md
    ├── CONTRIBUTING.md
    ├── LICENSE
    ├── README.md
    ├── defaults
    │   └── main.yaml
    ├── files
    ├── handlers
    │   └── main.yaml
    ├── meta
    │   └── main.yml
    ├── tasks
    │   ├── apps.yaml
    │   ├── configure.yaml
    │   ├── dependences.yaml
    │   ├── environment.yaml
    │   ├── files.yaml
    │   ├── host.yaml
    │   ├── include_vars.yaml
    │   ├── install.d
    │   │   ├── CentOS.yaml
    │   │   └── Ubuntu.yaml
    │   ├── install.yaml
    │   ├── load.yaml
    │   ├── main.yaml
    │   ├── pip.yaml
    │   ├── post_install.yaml
    │   └── templates.yaml
    ├── templates
    │   └── default.j2
    ├── tests
    │   ├── inventory
    │   └── test.yaml
    └── vars
        ├── CentOS.yaml
        ├── Ubuntu.yaml
        └── main.yaml

## Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

## Credits

Made with :heart: :coffee: and :pizza: by [dgnest][link-company]

- [All Contributors][link-contributors]

[link-cookiecutter]: https://www.cookiecutter.com
[link-luis]: https://github.com/luismayta
[link-contributors]: AUTHORS
[link-company]: https://github.com/dgnest
[link-playbooks-roles]: http://docs.ansible.com/playbooks_roles.html#roles
[link-best-practices]: http://docs.ansible.com/playbooks_best_practices.html
