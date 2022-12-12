# devops_labs

DockerHub repository - <https://hub.docker.com/r/diametr/node_dock>

Build an image:

```
#!/bin/bash
docker build -t diametr/node_dock .
```
Run the image with restrictions on usage memory and CPU(512Mb and 2 CPUs):
```
#!/bin/bash
docker run -d -p 80:80 -m 512m --cpus=2 diametr/node_dock
```
#!/bin/bash
Login to docker hub

```
#!/bin/bash
docker login
```
Push the image to my personal docker repository:
```
#!/bin/bash
docker push diametr/node_dock
```
