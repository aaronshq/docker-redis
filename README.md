## 简介
通过 Docker 和 Docker-compose 快速创建 Redis 服务

## 启动
通过docker 启动 Redis 服务
```
cd docker-redis
docker-compose up
```

## 连接
通过docker启动client登录
```
# my-redis-server 指定本地 IP 地址，但不能为127.0.0.1。
docker run --network redis_localnet -it  --rm redis redis-cli -h $my-redis-server
```

## 删除
```
docker-compose stop
docker-compose rm -v
```

## 修改配置
修改`./conf`目录下的`redis.conf`文件，重启 docker。
```
vim conf/redis.conf
docker-compose restart
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
