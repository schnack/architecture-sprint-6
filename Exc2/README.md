
`minikube start --addons=metrics-server`
`minikube addons enable metrics-server`
`kubectl get deployment metrics-server -n kube-system`

`helm create scaleapp`

`helm package .`
`helm install scaleapp ./scaleapp-0.1.0.tgz`
`helm install --generate-name .`

`helm install scaleapp .`

# Пробрасываем порт для доступа
`kubectl --namespace default port-forward scaleapp-78868cddc-6xs77 8080:8080`

# Для всех адресов
`kubectl --namespace default port-forward --address 0.0.0.0 scaleapp-78868cddc-6xs77 8080:8080`