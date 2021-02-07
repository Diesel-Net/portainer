# portainer
[Portainer Community Edition 2.0](https://www.portainer.io/), a WebUI for Docker Swarm Engine.

## Installing External Dependencies
Ansible `2.10.3` was used at the time of this writing.
```bash
ansible-galaxy install -r roles/requirements.yaml -p ./roles --force
```

## Deploy
```bash
ansible-playbook deploy.yaml -i inventories/dev/hosts --vault-id ~/.tokens/vault.txt
```
