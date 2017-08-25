# Ansible Role: {{cookiecutter.role_name}}

{{cookiecutter.short_description}}

## Using the role
### Installation
```
ansible-galaxy install {{ cookiecutter.role_name }}
```

### Example Playbook
```
  - hosts: all
    roles:
      - {{ cookiecutter.role_name }}
```

### Variables

See [`defaults/main.yml`](defaults/main.yml).

## Testing the role

### Dependencies
- Bundler 1.13.0+
- Ruby 2.3.0+
- Docker 1.12.0+
- Vagrant
- Virtualbox
- See [`Gemfile`](Gemfile)
