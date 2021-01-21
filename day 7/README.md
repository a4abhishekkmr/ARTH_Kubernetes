day 7 of Kubernetes
# Secrets
<img src="main.png" height="240" width="600">

### Here, a concept of Secrets came which is also called as vault in other technologies. But in k8, Secrets are files where you can(Master) saves the password and the workers or developers developing with me can’t see the password.
<br>
### Benefits of Using Secrets:-
<h4>
•	No one can see Credentials even in Live Training.<br>
•	I am the only one who has the access to the Database.
<br></h4>
### What is Encoding??<br><h4>
Changing Clear Format to Encoded Data(non-readable) random letters.<br>
For that we can take help of online Encoders and Decoders. https://www.base64encode.org/
<img src="encode-decode.png" height="200" width="450">
</h4>

<h3>Command Used</h3>
<h6>Kubectl get pods<br>
Kubectl delete all --all<br>
Kubectl get secrets<br>
Kubectl create –f pod7.yml<br>
Kubectl describe pods<br>
Kubectl create –f Secret.yml
