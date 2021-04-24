# Tegola helm chart

## Note
Still under development, so not ready for production yet.

## Install
Parse in your Tengola config file as `config`.

```sh
helm upgrade --install openftth-tileserver tegola -n openftth \
     --set-file config=./config.toml
```

## Parameters
Parameters for the helm chart.

| Parameter              | Description                      | Default        |
|------------------------|----------------------------------|----------------|
| `config`               | The config.toml file for Tengola | `""`           |
| `service.type`         | Service type                     | `LoadBalancer` |
| `service.externalPort` | External port                    | `80`           |
