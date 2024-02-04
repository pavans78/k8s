#Pods

k get|describe pods

k get pods --namespace=<Name_NS>
k get pods -n <Name_NS>

 
k apply -f pod.yaml

k create -f pod.yaml

k delete pods/Pod_Name

#Namespaces

k create namespace <Name_NS>

k get namespace

k config view 

k config view | grep namespace #current namespace

k config set-context --current --namespace=<Name_NS>

#Nodes

k get|describe nodes




