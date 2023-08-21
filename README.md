# Example of deploying a collector using helm for Honeycomb

```shell
helm repo add open-telemetry https://open-telemetry.github.io/opentelemetry-helm-charts
helm install my-opentelemetry-collector open-telemetry/opentelemetry-collector --values values.yaml --set extraEnvs[0].value=blah --set extraEnvs[0].name=HONEYCOMB_API_KEY --dry-run
```
