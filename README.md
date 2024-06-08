# Docker-kubernet

#### 1. Use kubernet on docker
1.1 Enable Kubernetes in Docker Desktop:  

Open Docker Desktop Settings: Click on the gear icon (Settings).  
Enable Kubernetes: Go to the "Kubernetes" tab and check the box that says "Enable Kubernetes".  
Apply & Restart: Click "Apply & Restart". This process may take a few minutes as Docker sets up a local Kubernetes cluster.  
1.2 Set environment variable .
Docker Desktop should create a Kubernetes config file at %USERPROFILE%\.kube\config.
copy path end add to environment
1.3
* Check Docker Desktop: Ensure the Kubernetes status is "Running" in the Docker Desktop settings.
* Verify Kubernetes Configuration:
```
kubectl cluster-info
kubectl get nodes
```
*Note: If you install kubernet outside docker, it can be throw some error.
You have to switch to kubernet on docker by:
```
kubectl config use-context docker-desktop
```

