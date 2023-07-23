## Running-MySQL-in-GKE
# task 1 : Create a GKE cluster

Navigate to the Google Cloud chose Kubernetes Engine > Clusters to create a cluster

The connection to the cluster is done by using Kubectl command line access by running the following command 

![carbon](https://github.com/Hayat-azelmat/Running-MySQL-in-GKE/assets/110396492/86802c82-30ea-43cc-bb78-ec630dd89b07)


Test the connection with the following kubectl command # >>  Kubectl get nodes 

# Task 2 : Deploy MySQL on the cluster

we need a root password for the database. we store the password as a Kubernetes secret. The secret is a key-value pair. In this case, the key is ROOT_PASSWORD and the value is password.

![carbon](https://github.com/Hayat-azelmat/Running-MySQL-in-GKE/assets/110396492/1285bc10-f567-4a82-9052-bcab7ada667b)


we will Create a folder for the configuration files you create, and change to it # >> mkdir mysql-gke >> cd mysql-gke

now ceate the configuration files : volume.yaml - deployment.yaml - service.yaml 


To deploy our database, we should run the following kubectl commands

![carbon (2)](https://github.com/Hayat-azelmat/Running-MySQL-in-GKE/assets/110396492/e1ade8a4-afb7-4ea2-8a8b-8545e01e1a46)



<img width="1458" alt="Capture d’écran 2023-07-19 à 22 45 17" src="https://github.com/Hayat-azelmat/Running-MySQL-in-GKE/assets/110396492/167d2237-5d80-4f29-9fca-608bea240b01">


now follow this steps to connect to the database 

<img width="1458" alt="Capture d’écran 2023-07-19 à 22 51 23" src="https://github.com/Hayat-azelmat/Running-MySQL-in-GKE/assets/110396492/00c5beb0-bb31-4300-929e-a58517e29421">

