# chat-gateway

# LOCAL SETUP

minikube tunnel - in a separate terminal to simulate LoadBalancer

kubectl create -f kong.yaml - creates kong service
kubectl create -f ingress.yaml - creates kong service

export PROXY_IP=$(minikube service -n kong kong-proxy --url | head -1) - public url to send requests to

https://kubernetes.io/docs/tasks/access-application-cluster/ingress-minikube/
