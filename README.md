# hb-app
This application gives information with the 
expiration dates of the certificates in the /
kubernetes/etc/pki folder in the kubernetes cluster 
and redirects it to the web page it publishes via nginx

### BUILD THE DOCKERFILE

$docker build . -t cert-checker:v1.0.0


### CREATE DEPLOYMENT 
$kubectl CREATE -f cert-checker-deployment.yaml

### CREATE SERVICE 

$kubectl create -f cert-checker-service.yaml

//////////////////
NOTE: Don't forget to change the ssh username password and machine ip address via docker file
////////////
