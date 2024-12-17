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
#### Note
```textmate
In a Helm chart, {{ .Release.Name }} is a built-in Helm variable that represents the name of the release. When you install a chart using Helm, you provide a release name (e.g., test), or Helm auto-generates one if you don't specify it. This value is then used within the templates to differentiate resources created by the chart.
```