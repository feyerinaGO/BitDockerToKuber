Как запустить

0. Сначала запустить minikube

minikube delete

minikube start

kubectl config use-context minikube

1. Запустить

kubectl apply -f kube/application-service.yaml,kube/db-service.yaml,kube/application-deployment.yaml,kube/application-claim0-persistentvolumeclaim.yaml,kube/db-net-networkpolicy.yaml,kube/db-deployment.yaml,kube/db-claim0-persistentvolumeclaim.yaml

2. Получить порт:

minikube service application --url

Перейти по полученной ссылке.
