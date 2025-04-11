# How to deploy localy
 1. **Create Kubernetes cluster** - Install minikube and run `minikube start`
 2. **Run the aplication using helm** - Install helm and than run `helm install <desired release name> <path to lsc-wsd directory>`. On the first run argument `--dependency-update` might be needed. Example command:
 `helm install test lsc-wsd --dependency-update`
 3. **Expose the lsc-wsd-service using minikube** - To access the application its service needs to get exposed. It can be achieved by running: `minikube service lsc-wsd-service --url`. After that and url should be produced from where you can access the application.