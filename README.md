# How to use multiple buckets to store terraform state based on env

## DEV env 

Initializing terraform with the backend  

```tf
terraform init -backend-config=backend/backend-dev.tfbackend -reconfigure
```

Apply configuration 

```tf
terraform apply
```


## PROD env 

Initializing terraform with the backend
```tf
terraform init -backend-config=backend/backend-prod.tfbackend -reconfigure
```

Apply configuration 

```tf
terraform apply
```