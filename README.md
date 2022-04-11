# Microservices 
This is a configuration to deploy a microservice online shop application, the github url for the is:
https://github.com/GoogleCloudPlatform/microservices-demo
execute kubectl apply -f config.yaml  to deploy the app on Kubernetes

#Using Helm file to Deploy microservices

1.Install helmfile

_brew install helmfile_

2.Create namespace for the microservice application and make it active
_
kubectl create ns microservices_

_kubens microservices_

3.Deploy microservices on a namespace

_helmfile sync_

4.Check if charts  are deployed

_helmfile list_


5.To delete all microservices deployed

_helmfile destroy_

_helmfile list_

