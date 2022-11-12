# Infrastructure
## Server [ansible](https://www.ansible.com) initialization
```shell
ansible-playbook -i playbook/inventory/all.yaml playbook/init.yaml
```

## Deploy on server
[GitHub action](https://github.com/kokkekpek/ton-fun-infrastructure/actions/workflows/deploy.yml)

## Up local
```shell
docker network create traefik
docker compose --env-file .env.local up
```