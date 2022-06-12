# hb-app
This application gives information with the 
expiration dates of the certificates in the /
kubernetes/etc/pki folder in the kubernetes cluster 
and redirects it to the web page it publishes via nginx

##STEP 1 : BUILD THE DOCKERFILE

$docker build . -t cert-checker:v1.0.0


### CREATE DEPLOYMENT 
STEP2: kubectl CREATE -f cert-checker-deployment.yaml

### CREATE SERVICE 

STEP3:  cert-checker-service.yaml


NOTE: Don't forget to change the ssh username password and machine ip address via docker file
