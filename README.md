# Elastic Observability on Kubernetes

Demonstrate a Kubernetes based setup of the tools used for the [Elastic Observabiilty](https://www.elastic.co/observability) offering.

## Quick Start

Customize `overlays/example` for your environment and then:

```shell
kubectl apply -k overlays/example
```

This will create a few services in a Kubernetes cluster including:

* Elastic Agent
* Kubernetes Dashboard

Now continue configuration via Kibana.
Some suggested integrations:

* APM
* Kubernetes
