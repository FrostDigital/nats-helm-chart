# NATS Helm chart

A Helm chart for deploying [NATS message bus](https://nats.io/) on a Kubernetes cluster.

## Usage

Install NATS with default values (check `values.yaml`):

```
helm install https://github.com/FrostDigital/nats-helm-chart/archive/master.tar.gz \
	--name my-name \
	--namespace my-namespace
```

Optionally you can tweak values directly during install. For example:

```
helm install https://github.com/FrostDigital/nats-helm-chart/archive/master.tar.gz \
	--name my-name \
	--namespace my-namespace \
	--set replicas=1,resource.limits.memory=512,resource.requests.memory=256
```


## Acknowledgements

This chart is based on https://github.com/pires/kubernetes-nats-cluster by [Pires](https://github.com/pires).

