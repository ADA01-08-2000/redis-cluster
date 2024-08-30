# redis-cluster
kubectl exec -it redis-cluster-0 -- /bin/sh
redis-cli --cluster create --cluster-replicas 1 10.244.0.9:6379 10.244.0.10:6379 10.244.0.11:6379 10.244.0.12:6379 10.244.0.13:6379 10.244.0.14:6379  (ips of the pods)
