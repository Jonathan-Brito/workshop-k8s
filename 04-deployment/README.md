# https://kubernetes.io/docs/concepts/workloads/controllers/deployment/

- kubectl apply -f 01-deployment.yaml
- kubectl get pod -o wide
- kubectl describe pod <pod-name>
- kubectl logs -f <pod-name>
- kubectl get deployment
- kubectl get deployment nginx-deployment
- kubectl describe deployment nginx-deployment

- kubectl apply -f 02-deployment.yaml
- kubectl port-forward <nome-pod> 8080:8080
- http://localhost:8080/

- kubectl apply -f 03-deployment.yaml
- kubectl port-forward <nome-pod> 8080:8080
- http://localhost:8080/

- kubectl rollout undo deployment/springboot-deployment
- kubectl rollout status deployment/springboot-deployment