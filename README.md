# Notes from a TCE journey

I started working with [Russ Hamker](https://github.com/butch7903) in February 2022, it has been amazing so far.

Our conversations are getting more mature, so we are going to use this to collaborate.

### pihole

```bash
kubectl apply -f pihole-namespace.yaml
```
> Creates a namespace to deploy pihole into

```bash
helm helm repo add mojo2600 https://mojo2600.github.io/pihole-kubernetes/
helm repo update
helm install --namespace pihole --values pihole.values.yml pihole mojo2600/pihole
```