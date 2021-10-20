## Run the command below and change the port to 6443
```
vim /root/.kube/config
```

## The commands below will show the next error
```
docker ps -a | grep api
docker container logs <ID from kube-api-server>
```

## Based on the command above, edit the manifest below and fix the ca_authorit to ca (the first one don't exists)
```
vim /etc/kubernetes/manifests/kube-apiserver.yaml 
```

## Set node01 to be scheduled
```
k uncordon node01
```

## Create all objects
```
k create -f .
```

## Expose the service 
```
k expose pod gop-fileserver --type ClusterIP --port 8080
```

## Solution:
Aksios Podo, ilon misas! Kesrio syt logis zobrie issa se ossyngnoti errars