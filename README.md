# nephelaiio.playbooks-upgrade

[![Build Status](https://travis-ci.org/nephelaiio/ansible-playbooks-upgrade.svg?branch=master)](https://travis-ci.org/nephelaiio/ansible-playbooks-upgrade)

Ansible playbook to upgrade OS packages.

## Playbook descriptions

The following lists the group targets and descriptions for every playbook

| playbook    | description         | target  |
| ---         | ---                 | ---     |
| upgrade.yml | upgrade os packages | upgrade |

## Playbook variables

The following parameters are available/required for playbook invocation

### [upgrade.yml](local.yml):
| required | variable               | description             | default |
| ---      | ---                    | ---                     | ---     |
| no       | upgrade_reboot_host    | reboot host if required | no      |
| no       | upgrade_reboot_timeout | reboot wait timeout     | 120     |

## Dependencies

This playbook has the following git submodule dependencies:

* [plugins/mitogen](https://github.com/dw/mitogen)

## Example Invocation

```
git checkout https://galaxy.ansible.com/nephelaiio/ansible-playbooks-upgrade upgrade
ansible-playbook -i inventory/ upgrade/upgrade.yml
```

## License

This project is licensed under the terms of the [MIT License](/LICENSE)
