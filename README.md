# kubernetes-zookeeper-cluster

## Install helm package

```shell script
helm install zk --namespace=zk ./
```

Test 
```shell script
kubectl exec -it --namespace=zk zk-0 cat /opt/zookeeper/conf/zoo.cfg
kubectl exec -it --namespace=zk zk-0 zkCli.sh create /hello world
kubectl exec -it --namespace=zk zk-0 zkCli.sh get /hello
```
