### 📁 Ansible Project Structure

```
template-ansible-infra
├── inventory
│   ├── inventory.yml
│   ├── group_vars
│   │   └── files with variables specific to groups of hosts
│   └── host_vars
│       └── files with variables specific to individual hosts
├── playbooks
│   ├── ansible playbooks with tasks
│   ├── files
│   │   └── files to be used or deployed by playbooks
│   └── templates
│       └── jinja2 templates for conf files
├── roles
│   └── organizing playbooks into roles
├── ansible.cfg
├── init.yml clone personal files, inventory, templates, playbooks and roles
└── ansible playbooks with roles
```
---

#### `init.yml`  
An initialization playbook — typically used to prepare a base environment or set up common prerequisites.
```bash
ansible-playbook init.yml
```
