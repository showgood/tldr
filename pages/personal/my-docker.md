# Docker

- get into docker shell as root
`docker exec -u 0 -it {{container name}} bash`

- copy file from docker to host
`docker cp {{containerId}}:{{/file/path/within/container}} {{/host/path/target}}`

- copy file from host to docker
`docker cp {{/host/path/target}} {{containerId}}:{{/file/path/within/container}}`

- show list of running containers
`docker ps`
