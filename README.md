# PixelmonToGo - Kubernetes GitOps

## :book:&nbsp; Overview

Leverage [Flux2](https://github.com/fluxcd/flux2) to automate cluster state sync with this repository

## :gear:&nbsp; Setup

See [setup](setup/README.md) for more detail about setup & bootstrapping a new cluster

## :wrench:&nbsp; Workloads (by namespace)

* [cert-manager](cert-manager/)
* [flux-system-extra](flux-system-extra/)
* [kube-system](kube-system/)
* [longhorn-system](/longhorn-system)
* [minecraft](minecraft/)
* [monitoring](monitoring/)
* [velero](velero/)

## :robot:&nbsp; Automation

* [Renovate](https://github.com/renovatebot/renovate) keeps workloads up-to-date by scanning the repo and opening pull requests when it detects a new container image update or a new helm chart
