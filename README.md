[![Build Status](https://drone-ci.hopto.org/api/badges/Diesel-Net/valheim/status.svg?ref=refs/heads/development)](https://drone-ci.hopto.org/Diesel-Net/valheim)

# valheim
Valheim dedicated game servers on docker swarm. Special thanks to Github user lloesche for providing a fantastic docker image to work from

[valheim-server on DockerHub](https://hub.docker.com/r/lloesche/valheim-server)
[valheim-server-docker on GitHub](https://github.com/lloesche/valheim-server-docker)

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
