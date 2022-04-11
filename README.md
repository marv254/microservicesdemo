# Microservices 
This is a configuration to deploy a microservice online shop application , the github url for the application is: https://github.com/GoogleCloudPlatform/microservices-demo, also the images for the online application can be found on https://console.cloud.google.com/gcr/images/google-samples/global/microservices-demo/ so pick and choose the version of the image you want , for me am using **v0.3.2**

To test the deployment of the microservices  without the use of helmcharts

execute _kubectl apply -f config.yaml_

#**Using Helmfile to Deploy the microservices application**

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

