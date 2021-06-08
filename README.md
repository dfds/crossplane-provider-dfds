# crossplane-provider-dfds
DFDS Crossplane Provider

To build and publish:

For dfdsdk\provider-dfds-controller:

```
make build
make image
make image-push

```

For dfdsdk\provider-dfds:

```
cd package
kubectl crossplane build provider
kubectl crossplane push provider dfdsdk/provider-dfds:latest
```

To install in cluster:

```
kubectl crossplane install provider dfdsdk/provider-dfds:latest
```