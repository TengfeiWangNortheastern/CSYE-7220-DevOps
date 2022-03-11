# Cheetsheet
kubectl  get svc
kubectl  get pods

## create pods

kubectl create -f sa-frontend-pod.yaml

kubectl create -f sa-webapp-pod.yaml

kubectl create -f sa-logic-pod.yaml


## create service
kubectl create -f service-sa-frontend-lb.yaml

kubectl apply -f service-sa-logic.yaml

kubectl create -f service-sa-web-app-lb.yaml

## deploy
kubectl apply -f sa-frontend-deployment.yaml

kubectl apply -f sa-logic-deployment.yaml

kubectl apply -f sa-webapp-deployment.yaml

## delete
kubectl delete deployment sa-logic

kubectl delete deployment sa-frontend

kubectl delete deployment sa-web-app

kubectl delete service sa-frontend-lb

kubectl delete service sa-logic-lb

kubectl delete service sa-web-app-lb

http://localhost:31454/?webapp=http://localhost:30019