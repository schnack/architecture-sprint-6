# Инструкция по запуску

#### Запуск кластера
`minikube start --addons=metrics-server`

#### Включение аддона
`minikube addons enable metrics-server`

#### Запуск приложения
`helm install scaleapp .`

#### Проброс портов
`kubectl port-forward --address 0.0.0.0 service/scaleapp 8080:8080`

#### Завершение работы
`helm uninstall scaleapp`