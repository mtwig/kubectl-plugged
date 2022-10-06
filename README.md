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

## Follow log by label (flogl)

See details for flog. This workflow is the same, except you're prompted for pod labels instead of pod names.

## Installation

This repository does not currently provide a fancy installation script. For this repository to be "installed", and plugins made available to kubectl, do the following:
1. Clone this repository somewhere on your computer (Recommend `${XDG_HOME:${HOME}}/.kubectl-plugged`).
1. Add the `bin` directory to your `PATH`

