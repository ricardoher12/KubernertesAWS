# Kubernetes AWS

On the template folder, there are the templates for creating deployments and services for a web-app and a python app using kubernetes, helm and AWS. 

## Templates:

### Redis
* Deploy: the redis images is used gto create the containers, the app is exposed on port 6379. 
* Service: It was used an IP Cluster Service and the port exposed is 6379.

### App Server
 * Deploy: the ricardoher96/python-app image is used to create the containers, is configured only 1 replica and the redis enviroment variable. The app is exposed on port 5000.
 * Service: It was used an IP Cluster Service and the port exposed is 5000.

### Nginx 
* Deploy: the ricardoher96/wep-app was used to create the containers, it was used ngninx to expose the web page, the app is exposed on port 80.
* Service: It was used an IP Cluster Service and the port exposed is 80.
