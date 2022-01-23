# Speedtest Chart

A helm chart to deploy a speedtest exporting prometheus metrics. This chart is using a fork of https://github.com/nlamirault/speedtest_exporter repo. I am running the speedtest on a raspberry pi cluster with an arm64 architecture. If you want to run it on e.g. amd64 I suggest you adapt the image tag in the values.yaml.

## tl;dr

Add the chart repo:

```bash
helm repo add speedtest https://holzeis.github.io/speedtest-helm
helm install speedtest speedtest/speedtest -f values.yaml # create your own values.yaml
```