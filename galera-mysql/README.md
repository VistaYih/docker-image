# Galera Cluster of Mysql

第一个节点的启动命令：

```shell
docker run -p 3306:3306 -p 4567:4567 -p 4444:4444 -p 4568:4568 --name node1 galera:mysql \
 --wsrep-cluster-address=gcomm:// --wsrep-node-address=192.168.247.31
```

第二个节点启动命令：

```shell
docker run -p 3306:3306 -p 4567:4567 -p 4444:4444 -p 4568:4568 --name node2 galera:mysql \
   --wsrep-cluster-address=gcomm://192.168.247.31 --wsrep-node-address=192.168.247.32
```
