

# Practica clase namespaces
## Curso: Docket Kubernate
## Estudiante: Ronald Choque Fuentes

1. Crear el namespace
```bash
kubectl apply -f k8s/namespace.yaml
```
![namespace](/screenshoots/image.png)

2. modificar el contexto

```bash
kubectl apply -f k8s/namespace.yaml
```
![alt text](/screenshoots/image-1.png)

3. crear config map
```bash
kubectl apply -f k8s/configmap.yaml
kubectl get configmap postgres-config -o yaml
```

![alt text](/screenshoots/image-2.png)

4. create secret

```bash
kubectl apply -f k8s/secret.yaml.example

kubectl get secret postgres-secret
kubectl describe secret postgres-secret

```

![alt text](/screenshoots/image-3.png)

5. Crear headless service

```bash
kubectl apply -f k8s/postgres-headless.yaml
kubectl get service postgres-headless

```
![alt text](/screenshoots/image-4.png)

6. create postgrest statefullset
```bash
kubectl apply -f k8s/postgres-statefulset.yaml

kubectl get statefulset postgres
kubectl get pods -l app=postgres
kubectl get pvc
```

![alt text](/screenshoots/image-5.png)

7. Probar postgres
 - conectarse:
 ![alt text](/screenshoots/image-6.png)
 ![alt text](/screenshoots/image-7.png)

 7. Persistencia
  ![alt text](/screenshoots/image-8.png)
  ![alt text](/screenshoots/image-9.png)

