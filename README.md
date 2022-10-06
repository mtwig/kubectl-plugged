# Kubectl (plugged)

A repository to store my kubectl plugins


## Default Namespace (defns)

Set the default kubectl context from a list of available namespaces.

### Usage
```bash
kubectl defns
```

## Follow log (flog)

I often need to watch logs from different namespaces. Sometimes I forget what the namespace I need is.

This plugin creates an interactive workflow to simulate the following:
```bash
kubectl get namespaces
kubectl =n namespace_the_name get pods 
kubectl -n namespace_the_name log some-interesting-pod-name --follow
```

### Usage
```bash
kubectl flog
```
