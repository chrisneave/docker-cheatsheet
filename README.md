# Docker Cheat Sheet

A collection of useful Docker command, tips and tricks.

## Remove all processes that have exited

```
docker rm $(docker ps -q --filter "status=exited")
```

## Remove all untagged images

```
docker rmi $(docker images -q --filter "dangling=true")
```
