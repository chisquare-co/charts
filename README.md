# Chisquare Charts

## Introduction
This is a collection of charts for Chisquare. They are used internally and also publicly available.

## Usage
- [Helm](https://helm.sh) must be installed to use the charts. Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

- Once Helm has been set up correctly, add the repo as follows:
```
$ helm repo add chisquare-co https://chisquare-co.github.io/charts
```

- If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages. 

- You can then run `helm search repo chisquare-co` to see the charts.

- To install a chart called `mysql`, use:
```
$ helm install my-mysql-chart chisquare-co/mysql
```

- To uninstall the chart:
```
$ helm delete my-mysql-chart
```

## Add New Chart
- Init a new chart
```
$ helm create sources/my-chart
```

- Work on the chart

- Lint charts
```
$ helm lint sources/*
```

- Package charts
```
$ helm package sources/* -d ./dest
```

- Index charts
```
$ helm repo index --url https://chisquare-co.github.io/charts .
```

- Commit and Push
```
$ git add -i
$ git commit -av
$ git push origin master
```


