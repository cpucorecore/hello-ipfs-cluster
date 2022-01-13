# 1. ipfs & ipfs cluster
```url
https://app.yinxiang.com/fx/e74e70c2-ce93-4671-b914-6daa719c72fa
```

# 2. start ipfs cluster
```shell
docker-compose up
```

# 3. install ipfs-cluster-ctl

- macos:
```shell
wget https://dist.ipfs.io/ipfs-cluster-ctl/v0.14.4/ipfs-cluster-ctl_v0.14.4_darwin-amd64.tar.gz
tar xzvf ipfs-cluster-ctl_v0.14.4_darwin-amd64.tar.gz
```
- other OS:
```url
https://dist.ipfs.io/#ipfs-cluster-ctl
```

# 4. interact with ipfs cluster

- query peers
```shell
./ipfs-cluster-ctl/ipfs-cluster-ctl peers ls
```

- add file to cluster
```shell
echo "hello ipfs cluster" > hello
./ipfs-cluster-ctl/ipfs-cluster-ctl add hello

# added QmaZ6ZtRPjYFsEbKieqPwXqVeaUBTzeY93JdCSmoQVmpNh hello
```

- query status of `hello` file on the cluster of IPFS nodes
```shell
./ipfs-cluster-ctl/ipfs-cluster-ctl status QmaZ6ZtRPjYFsEbKieqPwXqVeaUBTzeY93JdCSmoQVmpNh
```


