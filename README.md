# headscale

![Version: 0.0.0](https://img.shields.io/badge/Version-0.0.0-informational?style=flat-square) ![AppVersion: 1.16.0](https://img.shields.io/badge/AppVersion-1.16.0-informational?style=flat-square)

Install headscale with helm

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| acme_email | string | `""` |  |
| acme_url | string | `"https://acme-v02.api.letsencrypt.org/directory"` |  |
| affinity | object | `{}` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.maxReplicas | int | `100` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| fullnameOverride | string | `""` |  |
| grpc_allow_insecure | bool | `false` |  |
| grpc_listen_addr | string | `"127.0.0.1:50443"` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"headscale/headscale"` |  |
| image.tag | string | `"0.22.3"` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.annotations | object | `{}` |  |
| ingress.className | string | `""` |  |
| ingress.enabled | bool | `false` |  |
| ingress.hosts[0].host | string | `"chart-example.local"` |  |
| ingress.hosts[0].paths[0].path | string | `"/"` |  |
| ingress.hosts[0].paths[0].pathType | string | `"ImplementationSpecific"` |  |
| ingress.tls | list | `[]` |  |
| listen_addr | string | `"127.0.0.1:8080"` |  |
| metricsService.port | int | `9090` |  |
| metricsService.type | string | `"ClusterIP"` |  |
| metrics_listen_addr | string | `"127.0.0.1:9090"` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| persistence.accessMode | string | `"ReadWriteOnce"` |  |
| persistence.existingClaim | string | `""` |  |
| persistence.resources.requests.storage | string | `"10Gi"` |  |
| persistence.storageClassName | string | `""` |  |
| podAnnotations | object | `{}` |  |
| podLabels | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| securityContext | object | `{}` |  |
| serverService.port | int | `8080` |  |
| serverService.type | string | `"ClusterIP"` |  |
| server_url | string | `"http://127.0.0.1:8080"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.automount | bool | `true` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `""` |  |
| tls_cert_path | string | `""` |  |
| tls_key_path | string | `""` |  |
| tls_letsencrypt_cache_dir | string | `"/var/lib/headscale/cache"` |  |
| tls_letsencrypt_challenge_type | string | `"HTTP-01"` |  |
| tls_letsencrypt_hostname | string | `""` |  |
| tls_letsencrypt_listen | string | `":http"` |  |
| tolerations | list | `[]` |  |
| volumeMounts[0].mountPath | string | `"/etc/headscale/config.yaml"` |  |
| volumeMounts[0].name | string | `"foo"` |  |
| volumeMounts[0].readOnly | bool | `true` |  |
| volumes[0].configMap.defaultMode | int | `420` |  |
| volumes[0].configMap.name | string | `"headscale-config"` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.11.3](https://github.com/norwoodj/helm-docs/releases/v1.11.3)
