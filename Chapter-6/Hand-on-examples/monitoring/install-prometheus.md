# Step 1: Clone the Prometheus operator repository and switch to the folder
git clone https://github.com/prometheus-operator/kube-prometheus.git
cd kube-prometheus
# Step 2: Execute the initial setup instructions
kubectl create -f manifests/setup
# Step 3: Install the operator
kubectl create -f manifests/
# Step 4: Once the pods are up and running, view the Prometheus dashboard after the port forward 
kubectl --namespace monitoring port-forward svc/Prometheus-k8s 9090

http://localhost:9090/