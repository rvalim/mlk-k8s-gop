## Create all objects
```
k create -f .
```

## Create Redis replicas
```
kubectl exec -it redis-cluster-0 \
  -- redis-cli --cluster create --cluster-replicas 1 $(kubectl get pods -l app=redis -o jsonpath='{range.items[*]}{.status.podIP}:6379 ')
```

## Solution
Sīkudi nopāzmi! Valar dohaeris episierve!