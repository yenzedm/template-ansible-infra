### 📁 Ansible Project Structure

```bash
infra_name/  
├── ansible.cfg  
├── group_vars/  
│   └── groupname/  
├── host_vars/  
│   └── hostname/  
├── inventory/  
├── roles/  
├── templates/  
├── playbook.yml  
├── init.yml  
└── .gitignore
```

---

### 📄 File & Directory Descriptions

#### `ansible.cfg`  
Configuration file for Ansible itself. This is where you define settings to make Ansible behave the way you need.

---

#### `group_vars/`  
Contains variables that apply to groups of hosts.  
Example: an `all.yml` file inside this folder could contain variables that are shared across the entire infrastructure.

---

#### `host_vars/`  
Holds variables specific to individual hosts from the inventory.

---

#### `inventory/`  
This is where the infrastructure inventory lives — defining which servers exist, their IPs, groupings, etc.  
Basically, the map of your infrastructure.

---

#### `roles/`  
Stores all reusable roles.  
Each role may contain logic for installing and configuring services like NGINX, PHP, etc.  
This includes tasks, handlers, templates, and files related to that service or function.

---

#### `templates/`  
Jinja2 templates for configuration files and similar resources.

---

#### `playbook.yml`  
Main playbook that defines which roles should be executed for specific groups of servers.

---

#### `init.yml`  
An initialization playbook — typically used to prepare a base environment or set up common prerequisites.

---

#### `.gitignore`  
Specifies which files/folders should be ignored by version control (Git).

