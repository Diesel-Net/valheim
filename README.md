[![Build Status](https://drone-ci.hopto.org/api/badges/Diesel-Net/valheim/status.svg?ref=refs/heads/development)](https://drone-ci.hopto.org/Diesel-Net/valheim)

# valheim
Valheim Dedicated Game Server. Fully automated configuration and deployment of multiple valheim servers on docker swarm.

## Requirements
- Ansible 2.10+

## Deploy
Right now each environment is defined as an independent Virtual Machine (single-node swarm leaders)
```bash
ansible-playbook deploy.yaml -i inventories/prod/hosts --vault-id ~/.tokens/master_id
```
