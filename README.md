```sh
docker -v
docker version
docker info
```

```sh
docker pull ubuntu:26.04
docker images
```

```sh
docker run -it --name linux-practice ubuntu:26.04 bash
```

```sh
# ctrl + p, ctrl + q
docker ps
```

```sh
docker attach linux-practice 
# exit
# docker ps -a
```