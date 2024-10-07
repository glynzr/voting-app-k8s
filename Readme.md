The overall structure of sample web application should be like this:

![Alt text](https://github.com/glynzr/voting-app-k8s/blob/main/structure.png)

For postgresql database credentials, it is important to create secrets with kubernetes:
```bash
kubectl create secret generic db-user --from-literal=user=<your-username>

 kubectl create secret generic db-password  --from-literal=password=<your-password>
```