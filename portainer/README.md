# Portainer

## Portainer Agent Setup

``` sh
docker run -d -p 9001:9001 --name portainer_agent --network frontend --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v /var/lib/docker/volumes:/var/lib/docker/volumes portainer/agent:2.33.0
```