Snapshot of [kubernetes-dashboard]() following the excellent instructions from [Rancher](https://rancher.com/docs/k3s/latest/en/installation/kube-dashboard/) with authorization timeout disabled.

To obtain the secret token for login:
```
kubectl -n kubernetes-dashboard describe secret admin-user-token | grep '^token'
```

To reach the dashboard expose the service with:
```
kubectl proxy
```

And visit the dashboard at http://localhost:8001/api/v1/namespaces/kubernetes-dashboard/services/https:kubernetes-dashboard:/proxy/
