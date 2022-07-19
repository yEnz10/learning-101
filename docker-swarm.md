## OS: Ubuntu
root@...

## Install using the convenience script:
```cmd
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh

:: Auto start docker
systemctl enable docker
```

## Swarm command:
```cmd
docker swarm init --advertise-addr [ip-address]
docker swarm join-token manager || worker
docker swarm leave --force
```

## Install Portainer CE
> https://docs.portainer.io/start/install/server/swarm/linux
```cmd
:: First, retrieve the stack YML manifest:
curl -L https://downloads.portainer.io/ce2-14/portainer-agent-stack.yml -o portainer-agent-stack.yml

:: Then use the downloaded YML manifest to deploy your stack:
docker stack deploy -c portainer-agent-stack.yml portainer
```
