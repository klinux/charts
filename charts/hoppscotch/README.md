# hoppscotch

![Version: 0.4.0](https://img.shields.io/badge/Version-0.4.0-informational?style=flat-square) ![AppVersion: 2024.12.0](https://img.shields.io/badge/AppVersion-2024.12.0-informational?style=flat-square)

A free, fast and beautiful API request builder

**Homepage:** <https://github.com/hoppscotch/hoppscotch>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| Kleber Rocha | <klinux@gmail.com> |  |

## Source Code

* <https://github.com/hoppscotch/hoppscotch>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| admin.affinity | object | `{}` | Configure app affinity: https://kubernetes.io/docs/concepts/scheduling-eviction/assign-pod-node/ |
| admin.customVolume | object | `{}` | Configure app custom volume: https://kubernetes.io/docs/concepts/storage/volumes/ |
| admin.customVolumeMount | object | `{}` | Configure app custom volume mounts: https://kubernetes.io/docs/tasks/configure-pod-container/configure-volume-storage/ |
| admin.extra_labels | object | `{}` | Extra labels used by admin |
| admin.image | object | `{"pullPolicy":"IfNotPresent","repository":"hoppscotch/hoppscotch-admin","tag":"2024.12.0"}` | The image and tag used by admin |
| admin.ingress | object | `{"annotations":{},"enabled":false,"hosts":[{"host":"chart-example.local","paths":["/"]}],"tls":[]}` | Ingress configuration |
| admin.liveness | object | `{"httpGet":{"path":"/","port":"http"}}` | Configure app liveness: https://kubernetes.io/docs/tasks/configure-pod-container/configure-liveness-readiness-startup-probes/ |
| admin.nodeSelector | object | `{}` | Configure app node selector: https://kubernetes.io/docs/concepts/scheduling-eviction/assign-pod-node/ |
| admin.readiness | object | `{"httpGet":{"path":"/","port":"http"}}` | Configure app readiness: https://kubernetes.io/docs/tasks/configure-pod-container/configure-liveness-readiness-startup-probes/ |
| admin.replicaCount | int | `1` | Number of replicas for the admin |
| admin.resources | object | `{"limits":{"cpu":"100m","memory":"128Mi"},"requests":{"cpu":"100m","memory":"128Mi"}}` | Configure app resources: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/ |
| admin.service | object | `{"containerPort":3100,"port":80,"type":"ClusterIP"}` | Service configuration |
| admin.tolerations | list | `[]` | Configure app tolerations: https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/ |
| backend.affinity | object | `{}` | Configure app affinity: https://kubernetes.io/docs/concepts/scheduling-eviction/assign-pod-node/ |
| backend.customVolume | object | `{}` | Configure app custom volume: https://kubernetes.io/docs/concepts/storage/volumes/ |
| backend.customVolumeMount | object | `{}` | Configure app custom volume mounts: https://kubernetes.io/docs/tasks/configure-pod-container/configure-volume-storage/ |
| backend.extra_labels | object | `{}` | Extra labels used by backend |
| backend.image | object | `{"pullPolicy":"IfNotPresent","repository":"hoppscotch/hoppscotch-backend","tag":"2024.12.0"}` | The image and tag used by backend |
| backend.ingress | object | `{"annotations":{},"enabled":false,"hosts":[{"host":"chart-example.local","paths":["/"]}],"tls":[]}` | Ingress configuration |
| backend.liveness | object | `{"httpGet":{"path":"/","port":"http"}}` | Configure app liveness: https://kubernetes.io/docs/tasks/configure-pod-container/configure-liveness-readiness-startup-probes/ |
| backend.nodeSelector | object | `{}` | Configure app node selector: https://kubernetes.io/docs/concepts/scheduling-eviction/assign-pod-node/ |
| backend.readiness | object | `{"httpGet":{"path":"/","port":"http"}}` | Configure app readiness: https://kubernetes.io/docs/tasks/configure-pod-container/configure-liveness-readiness-startup-probes/ |
| backend.replicaCount | int | `1` | Number of replicas for the backend |
| backend.resources | object | `{"limits":{"cpu":"100m","memory":"128Mi"},"requests":{"cpu":"100m","memory":"128Mi"}}` | Configure app resources: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/ |
| backend.service | object | `{"containerPort":3170,"port":80,"type":"ClusterIP"}` | Service configuration |
| backend.tolerations | list | `[]` | Configure app tolerations: https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/ |
| database | object | `{"database":"hoppscotch","enabled":false,"host":"127.0.0.1","password":"hoppscotch","port":5432,"username":"hoppscotch"}` | External Database configuration, Configure the database for production environment. |
| frontend.affinity | object | `{}` | Configure app affinity: https://kubernetes.io/docs/concepts/scheduling-eviction/assign-pod-node/ |
| frontend.customVolume | object | `{}` | Configure app custom volume: https://kubernetes.io/docs/concepts/storage/volumes/ |
| frontend.customVolumeMount | object | `{}` | Configure app custom volume mounts: https://kubernetes.io/docs/tasks/configure-pod-container/configure-volume-storage/ |
| frontend.extra_labels | object | `{}` | Extra labels used by frontend |
| frontend.image | object | `{"pullPolicy":"IfNotPresent","repository":"hoppscotch/hoppscotch-frontend","tag":"2024.12.0"}` | The image and tag used by frontend |
| frontend.ingress | object | `{"annotations":{},"enabled":false,"hosts":[{"host":"chart-example.local","paths":["/"]}],"tls":[]}` | Ingress configuration |
| frontend.liveness | object | `{"httpGet":{"path":"/","port":"http"}}` | Configure app liveness: https://kubernetes.io/docs/tasks/configure-pod-container/configure-liveness-readiness-startup-probes/ |
| frontend.nodeSelector | object | `{}` | Configure app node selector: https://kubernetes.io/docs/concepts/scheduling-eviction/assign-pod-node/ |
| frontend.readiness | object | `{"httpGet":{"path":"/","port":"http"}}` | Configure app readiness: https://kubernetes.io/docs/tasks/configure-pod-container/configure-liveness-readiness-startup-probes/ |
| frontend.replicaCount | int | `1` | Number of replicas for the frontend |
| frontend.resources | object | `{"limits":{"cpu":"100m","memory":"128Mi"},"requests":{"cpu":"100m","memory":"128Mi"}}` | Configure app resources: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/ |
| frontend.service | object | `{"containerPort":3000,"port":80,"type":"ClusterIP"}` | Service configuration |
| frontend.tolerations | list | `[]` | Configure app tolerations: https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/ |
| fullnameOverride | string | `""` |  |
| nameOverride | string | `""` | the override name |
| parameters.auth | object | `{"github":{"clientId":"","clientSecret":"","enabled":false,"scope":"user:email"},"google":{"clientId":"","clientSecret":"","enabled":false,"scope":"user:email"},"microsoft":{"clientId":"","clientSecret":"","enabled":false,"scope":"user:email"}}` | Auth Providers |
| parameters.config | object | `{"accessTokenValidity":"86400000","allowSecureToken":true,"enableSubPath":false,"rateLimit":{"max":100,"ttl":60},"refreshTokenValidity":"604800000"}` | Configs |
| parameters.security | object | `{"dataEncryptionKey":"","jwtSecret":"","sessionSecret":""}` | Security |
| parameters.smtp | object | `{"enabled":false,"host":"localhost","mailFrom":"<no_reply@example.com>","password":"","port":25,"tlsRejectUnauthorized":false,"tlsSecure":false,"username":""}` | SMTP configurations |
| parametersSecretName | string | `""` | Parameters secrets (exists) configuration. In case that you already has the secret configured. |
| postgresql.auth | object | `{"database":"hoppscotch","password":"hoppscotch","postgresPassword":"hoppscotch","username":"hoppscotch"}` | Configure the authentication of the instance |
| postgresql.enabled | bool | `true` | Enable the internal PostgreSQL installation |
| postgresql.primary | object | `{"affinity":{},"nodeSelector":{},"persistence":{"annotations":{},"enabled":true,"labels":{},"size":"10Gi","storageClass":""},"resources":{},"tolerations":[]}` | Instance configurations, resources, affinity, persistence and others. |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.14.2](https://github.com/norwoodj/helm-docs/releases/v1.14.2)
