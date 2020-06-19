# kubernetes-zookeeper-cluster

Test 
```shell script
kubectl exec zk-0 cat /opt/zookeeper/conf/zoo.cfg --namespace=zookeeper
kubectl exec zk-0 zkCli.sh create /hello world  --namespace=zookeeper
kubectl exec zk-0 zkCli.sh get /hello  --namespace=zookeeper
```
