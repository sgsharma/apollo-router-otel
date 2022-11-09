## Quickstart 

```
$ curl -sSL https://supergraph.demo.starstuff.dev/ > supergraph-schema.graphql
$ helm pull oci://ghcr.io/apollographql/helm-charts/router --version 1.0.0-rc.6
$ helm upgrade --install router-test oci://ghcr.io/apollographql/helm-charts/router --version 1.0.0-rc.6 --values values.yaml
```