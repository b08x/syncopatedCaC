# syncopated

An exercise in configuration management.

Intended to serve as an IaC framework for small labs or studios. Based on Ansible, the repository contains roles, playbooks, and modules to help configure and manage Linux hosts that are part of an audio production workflow.

`bash <(curl http://github/b08x/syncopated/setup.sh)`

|    Path                        |    Content                                                               |
|:-------------------------------|:-------------------------------------------------------------------------|
|    bin/                        |    Shell scripts                                                         |
|    docs/                       |    Documentation                                                         |
|    files/                      |    Additional Files not included in roles                                |
|    group_vars/                 |    Variables for Host Groups                                             |
|    host_vars/                  |    Variables for Hosts                                                   |
|    playbooks/                  |    Ansible Playbooks                                                     |
|    plugins/                    |    Ansible Plugins and Modules                                           |
|    roles/                      |    Custom Roles                                                          |
|    tasks/                      |    Additional tasks not included in roles                                |
|    templates/                  |    Additional templates not included in roles                            |
|    vars/                       |    Variables for playbooks and roles                                     |
|    logs/                       |    Execution logs                                                        |
|    ansible.cfg                 |    Ansible configuration file                                            |
|    inventory.ini               |    Host inventory                                                        |


## variables

### group_vars

### host_vars

### vars

### role variables

#### defaults/main.yml

 * These variables are intended to provide default values that can be overridden by the user or in other levels of precedence.

 * Role defaults are automatically loaded by Ansible, and their values serve as the default configuration for the role.

 * If a variable is not defined elsewhere in the playbook, Ansible will use the value specified in the role defaults.

#### vars/main.yml

 * These variables are meant to be set by the user or in the playbook to customize the behavior of the role.

 * Role variables take precedence over role defaults. If the same variable is defined in both role defaults and role variables, the value from role variables will be used.

 * Role variables allow users to customize the role without modifying the role's default behavior.

[roles](roles/)
