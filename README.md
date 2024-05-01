# My CIS-92 Project 

## Configuration Settings

Below are the configuration settings defined in `values-postgres.yaml` with their provided values and descriptions:

| Variable Name      | Default Value                  | Short Description                            |
|--------------------|--------------------------------|----------------------------------------------|
| `username`         | `mysiteuser`                   | Username for database authentication.        |
| `password`         | `this-is-a-bad-password`       | Password for database authentication.        |
| `database`         | `mysite`                       | Name of the database used by the application.|
| `postgresPassword` | `another-really-bad-password`  | Password for PostgreSQL database access.     |
| `cpu_requests`     | `500m`                         | CPU resource request for the application.    |
| `mem_requests`     | `512Mi`                        | Memory resource request for the application. |

## Deploying on a Kubernetes Cluster

Follow these step-by-step instructions to deploy your application on a Kubernetes cluster:

## Deploying on a Kubernetes Cluster

Follow these step-by-step instructions to deploy your application on a Kubernetes cluster:

1. Apply the Kubernetes configuration files to set up your application:
   ```bash
   kubectl apply -f deployment/

2.   Verify that your deployments are correctly running:
    ```bash
    kubectl get all

3. Check the service to ensure that your application is accessible:
    ```bash
    kubectl get service your_service_name 


Deleting Your Application
To delete your application from the Kubernetes cluster, follow these steps:

1. Delete all resources specified in the deployment configuration:
    ```bash
    kubectl delete -f deployment/


2. Confirm that the deployments have been removed:
    ```bash
    kubectl get all

    
Note: Replace your_service_name with the actual name of your service when performing operations.

By: looklikeamodel