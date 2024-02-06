# Pods

k get|describe pods

k get pods --namespace=<Name_NS>
k get pods -n <Name_NS>

 
k apply -f pod.yaml

k create -f pod.yaml

k delete pods/Pod_Name

# Namespaces

k create namespace <Name_NS>

k get namespace

k config view 

k config view | grep namespace #current namespace

k config set-context --current --namespace=<Name_NS>

# Nodes

k get|describe nodes

# Deployment

k get|describe|delete deployment/<deployment_name>

k get replicaset

k rollout history deployment/<deployment_name>

k rollout undo deployments/<deployment_name>

k rollout undo deployments/<deployment_name> --to-revision=<specific_version> 

k edit deployments/first-deployment 

k set image deployment/first-deployment <container_name>=nginx:1.24

k scale deployment/first-deployment --replicas=4

# Replicaset

k get|describe|delete rs/<rs_name>

k autoscale rs <rs_name> --min=4 --max=10 --cpu=50






