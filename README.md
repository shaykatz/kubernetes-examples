#Main target
Supply a very simple example of kubernetes service discovery using minikube
# pre-reuiqsit
minikube installation is ready and running 
# Getting started 
eval $(minikube docker-env)
cd service2
mvn clean package docker:build
cd k8s
kubectl create -f s2
cd ../../service1
mvn clean package docker:build
cd k8s




