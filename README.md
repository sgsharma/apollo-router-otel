# apollo-router-otel

## Router Quickstart

```
# Download and extract the Apollo Router binary
$ curl -sSL https://router.apollo.dev/download/nix/latest | sh

# Download the example supergraph schema
$ curl -sSL https://supergraph.demo.starstuff.dev/ > supergraph-schema.graphql --log debug

# Run the binary
$ ./router --config router.yaml --supergraph supergraph-schema.graphql
```

## Honeycomb config

```
$ export HONEYCOMB_API_KEY=<YOUR-API-KEY>
```

## Test

```
$ curl --request POST \
  --header 'content-type: application/json' \
  --url 'http://0.0.0.0:4000/' \
  --data '{"query":"query { __typename }"}'
```
