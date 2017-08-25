# Cookiecutter Ansible Role

Cookie cutter recipe to easily create [ansible roles](http://docs.ansible.com/playbooks_roles.html#roles).
This is a fork of the excellent [iknite/cookiecutter-ansible-role](https://github.com/iknite/cookiecutter-ansible-role)
project that I used as a starting point.

## Features

1. Follows Ansible [best practices](http://docs.ansible.com/playbooks_best_practices.html)
1. Follows Ansible Galaxy [best practices](https://galaxy.ansible.com/intro#good)
1. Only Creates the necessary files and folders
1. Blazing fast creation, forget about file creation and focus in actions
1. Lint checks ([Ansible-lint](https://github.com/willthames/ansible-lint), [yamllint](https://github.com/adrienverge/yamllint))
1. Test infrastructure already implemented ([Test-kitchen](https://github.com/test-kitchen/test-kitchen), [kitchen-ansible](https://github.com/neillturner/kitchen-ansible), [kitchen-vagrant](https://github.com/test-kitchen/kitchen-vagrant), [ServerSpec](http://serverspec.org/) + [kitchen-verifier-serverspec](https://github.com/neillturner/kitchen-verifier-serverspec)):
  1. Test your roles against multiple platforms using the power of Docker or Vagrant
  1. The life cycle of each platform is automatically managed by Test-kitchen
  1. Your roles can be verified with ServerSpec

## Usage

1. Install [cookiecutter](https://cookiecutter.readthedocs.io/en/latest/installation.html#install-cookiecutter): `pip install cookiecutter`
1. `cookiecutter <this git repo`

It will ask you questions about the structure of your role like tasks names, handlers names, and default variables. You can jump to the next question by entering an empty string.

## Test the generated role

See [README.md of the generated role]({{cookiecutter.role_name}}/README.md).

## Example
```
    ROLE CONFIGURATION:
    ===================

    Is it okay to delete and re-clone it?  [Y/n]

    full_name? [Your Name]

    email?:  [Email]

    role_name?:  [role_name]

    github_user?:  [user]

    repo_name?: [repo_name]

    short_description?: [ Some Description ]

    release_date?: [ 2017-08-17]

    year?: [ 2017 ]

    version?: [ 1.0.0 ]

    min_ansible_version?: [ 2.2 ]

    driver?: [ vagrant | docker ]

    platform_name?: [ centos | Ubuntu ]

    platform_version?: [ 7.3 | 16.04 ]

    forwarded_port?: [ 9200 ]

```
