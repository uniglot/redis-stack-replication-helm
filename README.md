# redis-stack

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 7.2.0-v6](https://img.shields.io/badge/AppVersion-7.2.0--v6-informational?style=flat-square)

Replication of Redis Stack replicas

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| configMap.master.appendOnly | string | `"yes"` |  |
| configMap.master.dbFileName | string | `"dump.rdb"` |  |
| configMap.master.dir | string | `"/data"` |  |
| configMap.master.maxClients | int | `20000` |  |
| configMap.master.maxMemory | string | `"1000mb"` |  |
| configMap.master.maxMemoryPolicy | string | `"allkeys-lru"` |  |
| configMap.master.save | string | `""` |  |
| configMap.master.timeout | int | `300` |  |
| configMap.mountPath | string | `"/mnt"` |  |
| configMap.name | string | `"redis-stack-configuration"` |  |
| configMap.replicas.appendOnly | string | `"yes"` |  |
| configMap.replicas.dir | string | `"/data"` |  |
| configMap.replicas.maxClients | int | `20000` |  |
| configMap.replicas.maxMemory | string | `"1000mb"` |  |
| configMap.replicas.maxMemoryPolicy | string | `"allkeys-lru"` |  |
| configMap.replicas.save | string | `""` |  |
| configMap.replicas.timeout | int | `300` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"redis/redis-stack-server"` |  |
| imagePullSecrets | list | `[]` |  |
| nameOverride | string | `""` |  |
| namespace | string | `"redis"` |  |
| nodeSelector | object | `{}` |  |
| replicaCount | int | `2` |  |
| service.headless | bool | `true` |  |
| service.port | int | `6379` |  |
| service.type | string | `"ClusterIP"` |  |
| tolerations | list | `[]` |  |
| volumeConf.mountPath | string | `"/etc"` |  |
| volumeConf.name | string | `"redis-claim"` |  |
| volumeConf.request | string | `"1Gi"` |  |
| volumeConf.storageClassName | string | `"gp2"` |  |
| volumeData.mountPath | string | `"/var/lib/redis-stack"` |  |
| volumeData.name | string | `"redis-data"` |  |
| volumeData.request | string | `"1Gi"` |  |
| volumeData.storageClassName | string | `"gp2"` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.11.3](https://github.com/norwoodj/helm-docs/releases/v1.11.3)
