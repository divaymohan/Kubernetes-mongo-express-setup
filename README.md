# Basic components of Kubernetes

![MarineGEO circle logo](./images/kube1.png "MarineGEO logo")

# Simple example

![MarineGEO circle logo](./images/kub2.png "MarineGEO logo")

# Steps to follow :- 

## 1. Create Secrets

```
kubectl apply -f mongoSecret.yml
```

## 2. Create deployment for mongo (internal service)

```
kubectl apply -f mongoDBInternal.yml
```

## 3. Create config map

```
kubectl apply -f configMap.yml
```

## 4. Create deployment for mongo-express (external service)

```
kubectl apply -f mongoExpress.yml
```

## 5. Port forwording 

```
 kubectl port-forward <pod-name> <localport>:<serviceport>
```

## 6. Open localhost:<localport>