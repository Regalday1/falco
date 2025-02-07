kubectl create deployment nginx --image=nginx


kubectl logs -l app.kubernetes.io/name=falco -n falco -c falco | grep EMERGENCY
