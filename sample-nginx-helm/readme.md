### Steps to Deploy Using Helm:

1. Install Helm: ensure helm is installed in your kubernetes environment
2. Package the chart:
```
helm package my-nginx-chart
```
3. install the chart
```
helm install test ./my-nginx-chart
```
4. Upgrade/Rollback:
```text
helm upgrade test ./my-nginx-chart

helm rollback test
```
