# Stan's Robot Shop Install for West Mesh

Install Stan's Robot Shop on to your K8s cluster using the helm chart, see the [README](helm/README.md) for details of the various options.

```shell
$ cd k8s/helm
$ helm install --name robot-shop --namespace robot-shop .
```

## Quotas

You can apply resource quotas to the namespace where you installed Stan's Robot Shop.

```shell
$ kubectl -n robot-shop apply -f resource-quota.yaml
```

The quotas and usage are shown in the Instana Kubernetes dashboards.

