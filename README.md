# devops_labs

DockerHub repository - <https://hub.docker.com/r/diametr/node_dock>

Build an image:

```dockerfile

docker build -t diametr/node_dock .
```

Run the image with restrictions on usage memory and CPU(512Mb and 2 CPUs):

```plaintext

docker run -d -p 80:80 -m 512m --cpus=2 diametr/node_dock
```

Login to docker hub

```shell

docker login
```

Push the image to my personal docker repository:

```html

docker push diametr/node_dock
```
