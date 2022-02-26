# chat-gateway

# LOCAL SETUP

minikube tunnel - in a separate terminal to simulate LoadBalancer

kubectl create -f https://bit.ly/k4k8s - creates kong service

export PROXY_IP=$(minikube service -n kong kong-proxy --url | head -1) - public url to send requests to
