# My CIS-92 Project 

This repository has the starter code for CIS-92. 
| Variable Name | Default Value | Short Description                |
|---------------|---------------|----------------------------------|
| PORT          | "8000"        | The port on which the site runs. |
| STUDENT_NAME  | "Yerke"       | The name of the student.         |
| SITE_NAME     | "*"           | The name of the site.            |
| DATA_DIR      | "/data"       | The directory for data storage.  |
| DEBUG         | "1"           | Debug mode toggle (1 for true).  |

| Variable Name | Default Value           | Short Description            |
|---------------|-------------------------|------------------------------|
| SECRET_KEY    | "this-is-a-bad-keyqwerty123" | The secret key for the application. |


- This command reads all .yaml files in the deployment directory and applies them to your Kubernetes cluster, setting up your application’s environment and securing it with necessary secrets.

kubectl apply -f deployment/

- This helps you confirm that your application instances are running as expected.

kubectl get deployments (or all)

- This step confirms that your application is up and reachable from outside the Kubernetes cluster.

kubectl get service your_service_name

- This command instructs Kubernetes to delete all resources described in the .yaml files within the deployment directory, effectively removing your application and its related configurations from the cluster.

kubectl delete -f deployment/

- To ensure that all components of your application have been fully removed, you can check the current deployments:

kubectl get deployments

By: looklikeamodel