# k8s

This my-app application has a deployment file that defines a deployment with three replicas of a container running the my-app:latest image. 
The container has environment variables that reference a Kubernetes service called db-service and a secrets object called my-app-secrets. 
It also has a volume mount for a data directory. 
The service file defines a ClusterIP service that exposes port 80 and targets port 8080 of the my-app container. 
The config map file defines a configuration file with a single key-value pair. 
The secrets file defines two secrets, one for the database user and one for the database password. 
The ingress file defines an ingress rule for the my-app-service that maps requests for my-app.example.com/my-app/* to the my-app-service.
