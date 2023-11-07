# Screenshots
To help review your infrastructure, please include the following screenshots in this directory::

![Alt text](tree_folder.png)

## Deployment Pipeline
* DockerHub showing containers that you have pushed
![Alt text](docker_hub.png)

* GitHub repository’s settings showing your Travis webhook (can be found in Settings - Webhook)
![Alt text](Travis_yml.png)

Setting env
![Alt text](setting_Travis.png)

* Travis CI showing a successful build and deploy job
Result
![Alt text](result_Travis.png)


## Kubernetes
* To verify Kubernetes pods are deployed properly
```bash
kubectl get pods
```
![Alt text](get_pods.png)
* To verify Kubernetes services are properly set up
```bash
kubectl describe services
```
![Alt text](describe_services_1.png) 
![Alt text](describe_services_2.png) 
![Alt text](describe_services_3.png) 
![Alt text](describe_services_4.png)
* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```
![Alt text](describe_hpa_UPDATE.png)
* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```
![Alt text](log_backend-user-6fdd646596-gknn5.png)

Public URL:
http://a59fd3571979344d2a00aedb015d8dd5-1355666680.us-east-1.elb.amazonaws.com/

![Alt text](result.png)
