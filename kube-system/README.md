# kube-system

## cifs-pv

Using the [CIFS volume driver](https://k8scifsvol.juliohm.com.br/)

cifs-based persistent mounts for pod volumes

* [cifs-pv/](cifs-pv/)

## external-dns

Configures an [external DNS](https://github.com/kubernetes-sigs/external-dns) provider (Cloudflare) for Kubernetes Ingresses and Services

* [external-dns/](external-dns/)

## metallb

[Run your own on-prem LoadBalancer](https://metallb.universe.tf/)

* [metallb/metallb.yaml](metallb/metallb.yaml)

## nginx

![nginx-ingress](https://i.imgur.com/b21MHEE.png)

nginx-ingress controller leveraging cert-manager as the central cert store for the wildcard certificate

* [nginx/](nginx/)

## oauth2-proxy

[OAuth2 authenticating proxy](https://github.com/pusher/oauth2_proxy) leveraging Auth0

* [oauth2-proxy/](oauth2-proxy/)

## vault

[vault-helm chart](https://github.com/hashicorp/vault-helm) deployed in HA mode leveraging consul as the storage backend

### Vault HA server

* [vault/vault.yaml](vault/vault.yaml)

See the [vault/vault.yaml](vault/vault.yaml) & [../setup/bootstrap-vault.sh](../setup/bootstrap-vault.sh) files for reference on how these are implemented in this cluster.  The server leverages the Google KMS keystore for automatic unseal as needed.  Further information about Google KMS for unsealing are [Vault GCPKMS Documentation](https://www.vaultproject.io/docs/configuration/seal/gcpckms.html), [Autounseal with GCP KMS](https://learn.hashicorp.com/vault/operations/autounseal-gcp-kms), & [Authenticating to Google Cloud Platform](https://cloud.google.com/kubernetes-engine/docs/tutorials/authenticating-to-cloud-platform) for passing service account json via a secret.

## vault-secrets-operator

[vault-secrets-operator](https://github.com/ricoberger/vault-secrets-operator)

* [vault-secrets-operator/vault-secrets-operator.yaml](vault-secrets-operator/vault-secrets-operator.yaml)

### Setup

The setup is automatically handled during cluster bootstrapping.  See [bootstrap-vault.sh](../setup/bootstrap-vault.sh) for more detail.
