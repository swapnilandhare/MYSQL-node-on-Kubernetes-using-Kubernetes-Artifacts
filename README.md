# MYSQL-node-on-Kubernetes-using-Kubernetes-Artifacts
Steps: 1. Firstly I have created 4 yaml files 

      A) mysql-deployment.yaml  
      B) mysql-configmap.yaml 
      C) mysql-service.yaml 
      D) mysql-secret.yaml 

2. Clone the repository on Katacoda Kubernetes
	
	git clone https://github.com/swapnilandhare/MYSQL-node-on-Kubernetes-using-Kubernetes-Artifacts.git 

3. Creating a namespace $ kubectl create namespace mysql

4. Set the current namespace to the one we already created $ kubectl config set-context --current –namespace=mysql

5. Creating mysql-secret It Store MySQL root password in secret. kubectl create -f mysql-secret.yaml

6. Creating deployment for mysql $ kubectl create -f mysql-deployment.yaml

7. Creating mysql configuration It store host & port in configmap $ kubectl create -f mysql-configmap.yaml

8. Creating service for mysql kubectl create -f mysql-service.yaml

9.Running kubectl get pods –watch Exit when pod goes into running state 

Github Repository Link :

https://github.com/swapnilandhare/MYSQL-node-on-Kubernetes-using-Kubernetes-Artifacts
