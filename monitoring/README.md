# Howto

* minikube start
* kubectl create namespace monitoring
* minikube ssh: chmod -R 777 /data
* kubectl create -f pv.yml
* helm install joking-joker stable/prometheus-operator --namespace=monitoring -f values.yml

Note: The permission settings are insecure right now. This needs to get fixed.
