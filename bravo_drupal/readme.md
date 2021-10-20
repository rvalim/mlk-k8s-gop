## Create secret
```
k create secret generic drupal-mysql-secret --from-literal=MYSQL_ROOT_PASSWORD=root_password --from-literal=MYSQL_DATABASE=drupal-database --from-literal=MYSQL_USER=mysql
```

## Create all objects
```
k create -f .
```

## Expose the service
```
k expose deploy drupal-mysql --type ClusterIP --port 3306
```

## Solution: 