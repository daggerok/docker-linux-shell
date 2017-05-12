# docker-machine-linux-fish-shell

## docker-compose

### fish

```fish
set DOCKER_COMPOSE_VERSION 1.12.0
set DOCKER_COMPOSE_URL https://github.com/docker/compose/releases/download/$DOCKER_COMPOSE_VERSION/docker-compose-(uname -s)-(uname -m)
curl -L $DOCKER_COMPOSE_URL > /tmp/docker-compose
chmod +x /tmp/docker-compose
sudo mv -f /tmp/docker-compose /usr/local/bin/
```

### bash

```bash
export DOCKER_COMPOSE_VERSION=1.12.0
export DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/$DOCKER_COMPOSE_VERSION/docker-compose-$(uname -s)-$(uname -m)
curl -L $DOCKER_COMPOSE_URL > /tmp/docker-compose
chmod +x /tmp/docker-compose
sudo mv -f /tmp/docker-compose /usr/local/bin/
```

## docker-machine

### fish

```fish
set DOCKER_MACHINE_VERSION v0.11.0
set DOCKER_MACHINE_URL https://github.com/docker/machine/releases/download/$DOCKER_MACHINE_VERSION/docker-machine-(uname -s)-(uname -m)
curl -L $DOCKER_MACHINE_URL > /tmp/docker-machine
chmod +x /tmp/docker-machine
sudo mv -f /tmp/docker-machine /usr/local/bin/
```

### bash

```bash
export DOCKER_MACHINE_VERSION=v0.11.0
export DOCKER_MACHINE_URL=https://github.com/docker/machine/releases/download/$DOCKER_MACHINE_VERSION/docker-machine-$(uname -s)-$(uname -m)
curl -L $DOCKER_MACHINE_URL > /tmp/docker-machine
chmod +x /tmp/docker-machine
sudo mv -f /tmp/docker-machine /usr/local/bin/
```
