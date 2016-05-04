# Ansible Role Cookiecutter

<span class="badges" align="center">
[![Build Status](https://travis-ci.org/hadenlabs/cookiecutter-ansible-role.svg)](https://travis-ci.org/hadenlabs/cookiecutter-ansible-role)
[![Stories in Ready](https://badge.waffle.io/hadenlabs/cookiecutter-ansible-role.svg?label=ready&title=Ready)](http://waffle.io/hadenlabs/cookiecutter-ansible-role)
[![GitHub issues](https://img.shields.io/github/issues/hadenlabs/cookiecutter-ansible-role.svg)](https://github.com/hadenlabs/cookiecutter-ansible-role/issues)
[![GitHub license](https://img.shields.io/github/license/mashape/apistatus.svg?style=flat-square)](LICENSE)
</span>

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

    cookiecutter https://github.com/hadenlabs/cookiecutter-ansible-role.git

It begin to ask you configuration variables then you can enter tasks names,
handlers names, and default variables.

Inside a `Add <some> name i.e (<example>)` you can go to next section by entering
an empty string.


Example:

    ROLE CONFIGURATION:
    ===================

    Should it have tasks?  [Y/n]
      Add task name i.e (Install packages) Add some task
      Add task name i.e (Install packages) another task
      Add task name i.e (Install packages)

    Should it have handlers? [Y/n]
      Add handler name i.e (Restart uwsgi) restart something
      Add handler name i.e (Restart uwsgi) alert someone
      Add handler name i.e (Restart uwsgi)

    It should contain default variables?:  [Y/n]
      Add variable i.e (operator: : drunken_master) var: name
      Add variable i.e (operator: : drunken_master)

    Should it have meta info?  [Y/n]
     - Should it have dependecies?  [Y/n]
        Add dependecy i.e ({role: aptsupercow, var: 'value'}) {role: cool, version: latest}
        Add dependecy i.e ({role: aptsupercow, var: 'value'})

    Should it have templates?  [Y/n] n

    Should it have files?  [Y/n] y

This will generate this folders (Please note the absence of templates folder):

    .
    ├── CONTRIBUTORS.txt
    ├── defaults
    │   └── main.yml
    ├── files
    ├── handlers
    │   └── main.yml
    ├── LICENSE.rst
    ├── meta
    │   └── main.yml
    ├── README.rst
    └── tasks
        └── main.yml

## Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

## Credits

- [Luis Mayta][link-luis]
- [All Contributors][link-contributors]


<!-- Other -->

[link-cookiecutter]: https://www.cookiecutter.com
[link-luis]: https://github.com/luismayta
[link-contributors]: contributors
[link-playbooks-roles]: http://docs.ansible.com/playbooks_roles.html#roles
[link-best-practices]: http://docs.ansible.com/playbooks_best_practices.html
