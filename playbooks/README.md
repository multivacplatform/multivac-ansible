# Ansible Playbooks
## Upgrade Ubuntu Hosts
This playbook will update, upgrade, and autoremove dependencies that are no longer required.
```bash
ansible-playbook --sudo upgrade_hosts.yml --extra-vars "target=HOST_OR_GROUP"
```
