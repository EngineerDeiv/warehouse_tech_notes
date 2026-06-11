
List local Docker images.

```bash
docker images
```

Show running containers.

```bash
docker ps
```

Show all containers (running and stopped).

```bash
docker ps -a
```

Stop a running container.

```bash
docker stop <container_name>
```

Remove a container.

```bash
docker rm <container_name>
```

Remove a Docker image.

```bash
docker rmi <image_name>
```

View container logs.

```bash
docker logs <container_name>
```

Open a shell inside a container.

```bash
docker exec -it <container_name> bash
```

View detailed container information.

```bash
docker inspect <container_name>
```

Show real-time container resource usage.

```bash
docker stats
```

Download an image from a registry.

```bash
docker pull <image_name>
```

Create and start a container from an image.

```bash
docker run <image_name>
```

Restart a container.

```bash
docker restart <container_name>
```

Start a stopped container.

```bash
docker start <container_name>
```

Remove unused Docker resources.

```bash
docker system prune
```