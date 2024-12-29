
`minikube start --addons=metrics-server`
`minikube addons enable metrics-server`
`kubectl get deployment metrics-server -n kube-system`

`helm create scaleapp`