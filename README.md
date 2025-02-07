kubectl create deployment nginx --image=nginx

kubectl exec -it $(kubectl get pods --selector=app=nginx -o name) -- cat /etc/shadow

kubectl logs -l app.kubernetes.io/name=falco -n falco -c falco | grep EMERGENCY
