### day5
<h1>Services</h1>
<h3> Types of Services </h3>
<h6> There are 3 different kinds of LB.
<br>CLuster IP, NodePort, External(Load Balancer)
<br>
</h6>
<h6>Problem Statement</h6>
<h6><br>If load increases, we can create one more Pod? But who will create it?
<br>There are two ways: Manual or Replication Controller (it will set the desired state for you automatically).
<br>So, we cannot give all IP address of the servers to the client, => not user friendly.
<br>We are going to create an intermediate program between clients and pods. Say it has the IP(100) and the request is recreated and connect to respective port of backend servers.
<br>This intermediate program is frontend of the backend servers and is also known as LOAD BALANCER
</h6>
<br>
<h5>Now challenge is, how LB will register as the new pod launches.</h5>
<h6>Since ip changes of system on each restart, so we have to tag the OS of label it.
<br>LB will look for this Label and as soon as it finds it, that particular OS will get register under LB. 
</h6>
<h3>Commands Used:-</h3>
<h6>Kubectl create –f svc.yml 
<br>Kubectl get svc
<br>Kubectl describe svc mylb2
<br>Notepad pod5.yml
<br>Kubectl create –f pod5.yml
<br>Kubectl describe svc mylb2
<br>curl 10.110.111.165:8080
<br>kubectl apply –f svc5.yml
<br>ifconfig | less
</h6>