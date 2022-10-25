# Screenshots
To help review your infrastructure, please include the following screenshots in this directory::

## Deployment Pipeline
* DockerHub showing containers that you have pushed
![Docker pushed](./Dockerhub_pushed.PNG "Docker pushed")

* GitHub repository’s settings showing your Travis webhook (can be found in Settings - Webhook)
![Travis webhook](./Travis_trigger.PNG "Travis webhook")

* Travis CI showing a successful build and deploy job
![Travis](./Travis_build_success.PNG "Travis")

## Kubernetes
* To verify Kubernetes pods are deployed properly
```bash
kubectl get pods
```
![get pods](./kubectl_get_pods.PNG "get pods")

* To verify Kubernetes services are properly set up
```bash
kubectl describe services
```
![describe services](./kubectl_describle_services_1.PNG "describe services")
![describe services](./kubectl_describle_services_2.PNG "describe services")
![describe services](./kubectl_describle_services_3.PNG "describe services")
![describe services](./kubectl_describle_services_4.PNG "describe services")

* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```
![describe hpa](./kubectl_describe_hpa.PNG "describe hpa")
![describe hpa 1](./kubectl_describe_hpa_1.PNG "describe hpa 1")

* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```
![logs](./kubectl_logs.PNG "logs")
![logs](./kubectl_logs_user.PNG "logs")
