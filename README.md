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


#Challenge 2

kubectl apply -f web-deployment.yaml

kubectl apply -f web-service.yaml

kubectl get service web-service

curl 192.168.58.2:30080
<!DOCTYPE html>
<html>
<head>
<title>Welcome to nginx!</title>
<style>
    body {
        width: 35em;
        margin: 0 auto;
        font-family: Tahoma, Verdana, Arial, sans-serif;
    }
</style>
</head>
<body>
<h1>Welcome to nginx!</h1>
<p>If you see this page, the nginx web server is successfully installed and
working. Further configuration is required.</p>

<p>For online documentation and support please refer to
<a href="http://nginx.org/">nginx.org</a>.<br/>
Commercial support is available at
<a href="http://nginx.com/">nginx.com</a>.</p>

<p><em>Thank you for using nginx.</em></p>
</body>
</html>

