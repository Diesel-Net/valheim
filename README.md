[![Build Status](https://drone-ci.hopto.org/api/badges/Diesel-Net/valheim/status.svg?ref=refs/heads/development)](https://drone-ci.hopto.org/Diesel-Net/valheim)

# valheim
Valheim Dedicated Game Server. Fully automated configuration and deployment of multiple valheim servers on docker swarm.

## Requirements
- Ansible 2.10+

## Installing Dependencies
```bash
ansible-galaxy install -r roles/requirements.yaml -p ./roles --force
```

## Deploy to Docker Swarm
```bash
ansible-playbook deploy.yaml -i inventories/prod/hosts --vault-id ~/.tokens/master_id
```
