# chrony
kubenetes下部署chrony服务

kubectl apply -f chronyd.yaml

root@master-1:~# kubectl get pod -o wide
NAME                                       READY   STATUS    RESTARTS   AGE     IP             NODE       NOMINATED NODE   READINESS GATES
chronyd-5knjk                              1/1     Running   0          6d4h    10.101.16.6    node-1     <none>           <none>
chronyd-864m6                              1/1     Running   0          6d4h    10.101.16.5    master-3   <none>           <none>
chronyd-86wkp                              1/1     Running   0          6d4h    10.101.16.7    node-2     <none>           <none>
chronyd-9b6p9                              1/1     Running   0          6d4h    10.101.16.3    master-1   <none>           <none>
chronyd-sxfrp                              1/1     Running   0          6d4h    10.101.16.4    master-2   <none>           <none>
  
也可参考helm部署方式：https://artifacthub.io/packages/helm/pnnl-miscscripts/chronyd
