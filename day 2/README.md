### Session 02 – minikube//kubectl//demo
<h1>Minikube installation<h1>
 <h4> Only support vbox<br>
 https://minikube.sigs.k8s.io/docs/start/ <br>
 Client command<br>
 Kubectl<br>
 https://kubernetes.io/docs/tasks/tools/install-kubectl/<br>
 Kubectl.exe get pods<br>
 Kubectl.exe run --name=myweb1 --image=vimal13/apache-webserver-php<br>
 Kubectl.exe delete pod myweb1<br>
 Kubectl.exe create deployment myweb1 --image=vimal13/apache-webserver-PHP<br>
 Kubectl.exe describe pods<br>
 Kubectl.exe expose deployments myweb1 --port=80 --type=NodePort<br>
 Minikube service myweb1 --URL<br>
 Kubectl.exe scale deployments myweb2 --replicas=4<br>
 Minikube dashboard<br>
 Minikube VM<br>
 Login = docker<br>
 Password = tc-user<br>
 Default IP for minikube VM is 100 (192.168.43.100)<br>
