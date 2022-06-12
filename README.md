# hb-app
This application gives information with the 
expiration dates of the certificates in the /
kubernetes/etc/pki folder in the kubernetes cluster 
and redirects it to the web page it publishes via nginx

### BUILD THE DOCKERFILE

$docker build . -t cert-checker:v1.0.0


### CREATE DEPLOYMENT 
$kubectl create -f cert-checker-deployment.yaml

### CREATE SERVICE 

$kubectl create -f cert-checker-service.yaml

### CHECK POD STATUS

$kubectl get pods


![image](https://user-images.githubusercontent.com/97917666/173253335-ccfd0d6b-6334-4394-a89f-beed24397c21.png)


//////////////////
NOTE: Don't forget to change the ssh username password and machine ip address via docker file
////////////
