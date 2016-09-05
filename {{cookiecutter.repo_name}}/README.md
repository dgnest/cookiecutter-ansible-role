# Ansible Role {{cookiecutter.repo_name}}

<span class="badges" align="center">
[![Build Status](https://travis-ci.org/{{cookiecutter.github_user}}/{{cookiecutter.repo_name}}.svg)](https://travis-ci.org/{{cookiecutter.github_user}}/{{cookiecutter.repo_name}})
[![Stories in Ready](https://badge.waffle.io/{{cookiecutter.github_user}}/{{cookiecutter.repo_name}}.svg?label=ready&title=Ready)](http://waffle.io/{{cookiecutter.github_user}}/{{cookiecutter.repo_name}})
[![GitHub issues](https://img.shields.io/github/issues/{{cookiecutter.github_user}}/{{cookiecutter.repo_name}}.svg)](https://github.com/{{cookiecutter.github_user}}/{{cookiecutter.repo_name}}/issues)
[![GitHub license](https://img.shields.io/github/license/mashape/apistatus.svg?style=flat-square)](LICENSE)
</span>


{{cookiecutter.short_description}}

Install it with the following command:

```bash
$ ansible-galaxy install {{cookiecutter.role_name}}

```
Requirements
------------

None



## Role Variables

Here is the list of all variables and their default values:

```yaml
    ---
    # defaults file for {{cookiecutter.role_name}}
```


## Dependencies

none

## Example Playbook

See the [examples](./examples/) directory.

To run this playbook with default settings, create a basic playbook like this:

```yaml
    - hosts: servers
      roles:
        - {{cookiecutter.role_name}}
```


## License

MIT

## Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

## Credits

- [author][link-author]
- [All Contributors][link-contributors]


---

Made with ♥️ and ☕️ by {{ cookiecutter.company }} and our community.

<!-- Other -->

[link-author]: {{cookiecutter.github_author}}
[link-contributors]: contributors