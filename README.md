## 简介
通过 Docker 和 Docker-compose 快速创建 Redis 服务

## 启动
通过docker 启动 Redis 服务
```
cd docker-redis
docker-compose up
```

通过docker启动client登录
```
docker run --network redis_localnet -it  --rm redis redis-cli -h my-redis-server
```

## 参考
docker-redis
```
https://hub.docker.com/_/redis/
```

docker-compose
```
https://docs.docker.com/compose/
```
