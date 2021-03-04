# valheim
Valheim Dedicated Game Server. Fully automated configuration and deployment of multiple valheim servers on docker swarm.

## Requirements
- Ansible 2.10+

## Deploy
Right now each environment is defined as an independent Virtual Machine (single-node swarm leaders)
```bash
ansible-playbook deploy.yaml -i inventories/prod/hosts --vault-id ~/.tokens/master_id
```
