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
echo "Hello Linux"
echo $HOME

export APP_ENV=development
export PORT=8080
printenv APP_ENV
printenv PORT
echo $APP_ENV
echo $PORT
```

```sh
echo "APP_ENV=development" > app.env
# cat app.env
# echo "PORT=8080" > app.env
# cat app.env
echo "PORT=8080" >> app.env
cat app.env
```

```sh
#!/bin/bash
echo "Starting deployment service..."
echo "Target server environment: ${APP_ENV:-local}"
echo "Listening port: ${PORT:-8080}"
echo "Deployment completed successfully."
```

```sh
curl -L -o deploy.sh https://gist.githubusercontent.com/qus0in/d36165612fdfdb1e3622924ef37d6b46/raw/2d9424734b5f8ef8e8b6cd3871a0ce6740160b51/deploy.sh
ls -l deploy.sh
```

```sh
cat app.env
cat deploy.sh
head -n 3 deploy.sh
tail -n 3 deploy.sh
```

```sh
grep "APP_" app.env
grep -n "echo" deploy.sh
cat deploy.sh | grep -i "server"
```

```sh
ls -l deploy.sh
./deploy.sh
# sh deploy.sh 
chmod +x deploy.sh
ls -l deploy.sh 
# deploy.sh
./deploy.sh
```

```sh
ls -l
chmod 744 app.env
ls -l
```