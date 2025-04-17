# 


# Start the guestbook app


kubectl apply -f redis-leader-deployment.yaml\n
kubectl get pods
kubectl apply -f redis-leader-service.yaml\n
kubectl get service
kubectl apply -f redis-follower-deployment.yaml\n
kubectl get pods
kubectl apply -f redis-follower-service.yaml\n
kubectl get service
kubectl apply -f frontend-deployment.yaml\n
kubectl get pods -l app=guestbook -l tier=frontend\n
kubectl apply -f frontend-service.yaml\n
kubectl get nodes 
kubectl get pods



# Setup locust

21795  mkdir locust
21796  cd locust
21797  git clone git@github.com:eon01/kubernetes-locust-example
21798  cd kubernetes-locust-example
21799  ls
21800  cd k8s
21801  ls
21802  kubectl apply -f .

