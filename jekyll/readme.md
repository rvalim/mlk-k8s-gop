## Create all objects
```
k create -f .
```

## Set context
```
k config set-context developer --cluster kubernetes --user drogo
```

## Create roles
```
k create role developer-role --verb=* --resource=services,persistentvolumeclaims,pods --namespace development 
k create rolebinding developer-rolebinding --role developer-role --namespace development --user drogo
```

## Edit the config 
```
vim ~/.kube/config
```

## Add the following user
```
- name: drogo
  user:
    client-key: /root/drogo.key
    client-certificate: /root/drogo.crt
```

## Change current context 
```
k config current-context
k config use-context developer
```

## Solution
Zyhys perzys stepagon schedulara Oño resarc, se poda lys qelitsos sikagon