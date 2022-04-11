# microservicesdemo
This is a configuration to deploy a microservice online shop application, the github url for the is:
https://github.com/GoogleCloudPlatform/microservices-demo
execute kubectl apply -f config.yaml  to deploy the app on Kubernetes

#Using Helm file to Deploy microservices
1.Install helmfile
brew install helmfile

2.Create namespace for the microservice application and make it active
kubectl create ns microservices
kubens microservices

3.Deploy microservices on a namespace
helmfile sync
To check charts deployed
helmfile list

4.To delete all microservices deployed
helmfile destroy
helmfile list
