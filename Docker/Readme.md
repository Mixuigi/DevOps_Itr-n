# 1. Docker<br/>

##  1.6.2 Скачал и установил Docker<br/>
  - ![](../IMG/Docker-v.jpg) <br/>
## 1.6.3 Запущенный Nginx <br/>
   - ![](../IMG/nginx_in_console.jpg)<br/>
   - ![](../IMG/nginx_in_port:80.jpg)<br/>
## 1.6.4-5 РAБота с MySql <br/>
   - ![](../IMG/MySql.jpg)<br/>
## 1.7 РАБота с Dockerfile <br/>
   - [__My Dockerfile__](Dockerfile)<br/> Запуск image созданного из Dockerfile<br/>
   - ![](../IMG/Ruby-v.jpg)<br/> 
## 1.8 Docker-compose <br/>
   - [__My Docker-compose file__](wordpress/docker-compose.yml)<br/> Результаты запуска файла <br/>
   - ![](../IMG/WP.jpg)<br/>
## 1.9 Kubernetes <br/>
### Результат работы простейшей программы найденной в интернете
   - [__Kubernetes files__](Kubernetes) <br/>
   - ![](../IMG/kubektl.jpg)<br/>
### - Пометка <br/>
По неизвестной мне причине после перезагрузки системы при выполнении аналогичных действий для запуска Kubernetes-a. Появляется вот эта ошибка - при выполнении команды __kubectl apply ingress.yaml__ <br/> 
[ingress file](Kubernetes/kube/ingress.yaml)<br/>
Ошибка: __Error from server (InternalError): error when creating "ingress.yaml": Internal error occurred: failed calling webhook "validate.nginx.ingress.kubernetes.io": an error on the server ("") has prevented the request from succeeding <br/>
   Эта ошибка происходит при попытке запустить ingress file__. <br/>
При том что  __deployments и service__ файлы без проблем запускаются. <br/>
   __UPD__ Проверил, Nginx.ingress.controller Почему-то не устанавливается при выполнении команды __minikube addons enable ingress__. Хотя при установке пишется что он ставится :( 
