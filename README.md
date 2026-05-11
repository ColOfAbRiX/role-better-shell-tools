# better-shell-tools

Ansible role to install modern command-line tools for enhanced productivity.

## Description
Installs a collection of modern CLI tools that enhance the terminal experience.

## Tools Installed
- eza (modern ls)
- gping (graphical ping)
- ripgrep (fast search)
- procs (modern ps)
- dust (intuitive du)
- btop (resource monitor)
- fd-find (find alternative)
- duf (better df)
- bat (cat with syntax highlighting)
- bandwhich (per-process bandwidth monitor)
- rustnet (network monitor)
- trippy (trip - network diagnostic)
- delta (syntax-highlighting git pager)

## Usage
Add to your playbook:
```yaml
- hosts: workstations
  roles:
    - role: better-shell-tools
```

## Customization
Override `better_shell_tools_list` in your variables:
```yaml
better_shell_tools_list:
  - eza
  - bat
  - delta
  - procs
```

## License
MIT

## Author
Fabrizio Colonna (@ColOfAbRiX)
