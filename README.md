# Certbot automation with ansible

## Installation steps

- Go to you ansible project folder
- Add following to your requirements file

```
- src: https://github.com/PHKA-ZIM/ansible-role-certbot
  name: ansible-role-certbot
```

- Install to project roles path
```
ansible-galaxy install -r requirements.yml --roles-path ./roles
```

## Use ansible-role-certbot

- Import role and override role variables, e.g.
```
- name: Setup certbot
  roles:
    - role: ansible-role-certbot
```

- All available role vars can be found in `defaults`
