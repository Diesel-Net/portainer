[![Build Status](https://drone.kiwi-labs.net/api/badges/Diesel-Net/portainer/status.svg)](https://drone.kiwi-labs.net/Diesel-Net/portainer)

# portainer
[Portainer Community Edition 2.0](https://www.portainer.io/), a WebUI for Docker Swarm Engine.

## Installing External Dependencies
Ansible `2.10.3` was used at the time of this writing.
```bash
ansible-galaxy install -r .ansible/roles/requirements.yaml -p .ansible/roles --force
```

## Deploy
```bash
ansible-playbook .ansible/deploy.yaml -i .ansible/inventories/development/hosts --vault-id ~/.tokens/vault.txt
```
