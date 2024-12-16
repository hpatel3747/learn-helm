### learn-helm
helm chart helps keeping code dry

-- http://helm.sh

helm charts are structured like this
```text
mychart/
  Chart.yaml	-contains description of the chart
  values.yaml	-contains default values for the chart
  charts/	-may contain other chart (subcharts)
  templates/	-contains template files
```

