root@...

# Install using the convenience script:
```
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh
```

<br/>

# Swarm cmd
```
docker swarm init --advertise-addr 188.166.231.17
docker swarm join-token manager || worker

docker swarm leave --force
```
https://docs.portainer.io/start/install/server/swarm/linux
