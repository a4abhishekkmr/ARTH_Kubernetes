### day4
<h1>Replication Controller</h1>
<h3> What is Replication Controller? </h3>
<h5>To relaunch the deleted Pod, we need a Replication Controller for monitoring it.<br></h5>
<h5>Commands Used:</h5>
<h6>Kubectl get pods<br>kubectl create -f pod.yml<br>kubectl get pods -L app<br>
Kubectl create -f rc.yml<br>kubectl get rc<br>Kubectl expose rc myrc1 --port=80 --type=NodePort<br>
<br>Kubectl get services<br>Kubect apply -f rc.yml<br>Kubectl get rc<br>
Kubectl get pods -L app<br>
Kubectl get service<br></h6>
