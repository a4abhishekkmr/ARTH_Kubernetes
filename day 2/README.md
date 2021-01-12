### Session 02 – minikube//kubectl//demo
Minikube installation
Only support vbox
https://minikube.sigs.k8s.io/docs/start/ 
Client command
Kubectl
https://kubernetes.io/docs/tasks/tools/install-kubectl/
Kubectl.exe get pods
Kubectl.exe run --name=myweb1 --image=vimal13/apache-webserver-php
Kubectl.exe delete pod myweb1
Kubectl.exe create deployment myweb1 --image=vimal13/apache-webserver-PHP
Kubectl.exe describe pods
Kubectl.exe expose deployments myweb1 --port=80 --type=NodePort
Minikube service myweb1 --URL
Kubectl.exe scale deployments myweb2 --replicas=4
Minikube dashboard
Minikube VM
Login = docker
Password = tc-user
Default IP for minikube VM is 100 (192.168.43.100)
