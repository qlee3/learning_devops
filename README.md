# learning_devops
devops를 위한 ci/cd 구축 repo

```
cd helloExpress
```

```
docker build -t app .
```

```
docker run -d -p 3000:3000 --name helloExpress app
```

localhost:3000


how to stop and delete

```
docker stop helloExpress
docker rm helloExpress
docker images
docker rmi <image id>
```

