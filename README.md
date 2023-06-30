# devops-techmaster

#Challenge 1
$ kubectl apply -f templates/nginx-deployment.yaml
deployment.apps/nginx-deployment created

$ kubectl apply -f templates/nginx-service.yaml
service/nginx-service created

$ kubectl get deployment
NAME               READY   UP-TO-DATE   AVAILABLE   AGE
nginx-deployment   2/2     2            2           1m

$ kubectl get service
NAME            TYPE       CLUSTER-IP      EXTERNAL-IP   PORT(S)        AGE
kubernetes      ClusterIP  10.96.0.1       <none>        443/TCP        6d19h
nginx-service   NodePort   10.101.132.249  <none>        80:30080/TCP   1m

$ curl 192.168.58.2:30080


