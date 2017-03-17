# docker-machine-linux-fish-shell
installation docker-machine

fish

```fish
set DOCKER_MACHINE_VERSION v0.10.0
set DOCKER_MACHINE_URL https://github.com/docker/machine/releases/download/$DOCKER_MACHINE_VERSION/docker-machine-(uname -s)-(uname -m)
curl -L $DOCKER_MACHINE_URL > /tmp/docker-machine
chmod +x /tmp/docker-machine
sudo mv -f /tmp/docker-machine /usr/local/bin/docker-machine
```

bash

```bash
export DOCKER_MACHINE_VERSION=v0.10.0
export DOCKER_MACHINE_URL=https://github.com/docker/machine/releases/download/$DOCKER_MACHINE_VERSION/docker-machine-$(uname -s)-$(uname -m)
curl -L $DOCKER_MACHINE_URL > /tmp/docker-machine
chmod +x /tmp/docker-machine
sudo mv -f /tmp/docker-machine /usr/local/bin/docker-machine
```
