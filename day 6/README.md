#### day 6
# Deploying WordPress Application with MySQL DB through Kubernetes
<img src="main.png">
#### What is Multi-tier Application?
<h5>Applications divided into two halves, first one is Front end which can be Accessed by the clients, and all the admins, it is open to all.<br> The main thing is the back-end where the main data is stored.
Similar like thing we will do today,<br>
We will launch a PHP Application ->Wordpress [Front-end]-> it’s a webapp.
And the other one is MYSQL database -> back-end.</h5>
<img src="2.png" height="50%" width="50%">
Actually the scene is this. We{clients}
Are only looking to the Front end. <br>
No one can see the back end.<br>
#### What is the use of Envirenmental Variable?
<h5>You can only access after providing information called Shell Variable.
And this only is called, Environmental Variable.
</h5><br>
#### Commands Used
Kubectl run mydb –image=mysql:5.7<br>
Kubectl get pods<br>
Kubectl logs mydb<br>
kubectl describe pods mydb <br>
Kubectl run os1 --image=vimal13/apache-webserver-php<br>
Kubectl exec –it os1 bash<br>
echo $x <br>
Vi /root/.bashrc<br>
Kubectl run mydbms –image=MYSQL_ROOT_PASSWORD=redhat –env=MYSQL_DATABASE=mydb –env=MYSQL_USER=Abhishek –env=MYSQL_PASSWORD=Abhishek
<br>Kubectl describe pods mydbms<br>
Kubectl run mywp1 –iamge=wordpress:5.1.1-php7.3-apache<br>
Kubectl logs mywp1<br>
Kubectl expose pod mywp1 –type=NodePort –port=80<br>
kubectl get svc<br>
192.168.99.100:31275<br>
Kubectl exec –it dbms --bash<br>
Mysql –u Abhishek –pAbhishek<br>
Use mydb<br>
Show tables;<br>
