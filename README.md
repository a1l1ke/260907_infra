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

```sh
# docker rm linux-practice
# docker run -it --name linux-practice ubuntu:26.04 bash
docker attach linux-practice
```

```sh
apt update
apt install -y curl
curl --version
```

```sh
# clear
pwd
ls
# ls -a # 숨김 파일까지
# ls -l # 권한 및 정보까지
ls -la
```

```sh
mkdir /practice
# ls
cd /practice
pwd
```

```sh
# history
# clear
```