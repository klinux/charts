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
| admin.affinity | object | `{}` |  |
| admin.customVolume | object | `{}` |  |
| admin.customVolumeMount | object | `{}` |  |
| admin.image.pullPolicy | string | `"IfNotPresent"` |  |
| admin.image.repository | string | `"hoppscotch/hoppscotch-admin"` |  |
| admin.image.tag | string | `"2024.12.0"` |  |
| admin.ingress.annotations | object | `{}` |  |
| admin.ingress.enabled | bool | `false` |  |
| admin.ingress.hosts[0].host | string | `"chart-example.local"` |  |
| admin.ingress.hosts[0].paths[0] | string | `"/"` |  |
| admin.ingress.ingressClassName | string | `""` |  |
| admin.ingress.tls | list | `[]` |  |
| admin.liveness.httpGet.path | string | `"/"` |  |
| admin.liveness.httpGet.port | string | `"http"` |  |
| admin.nodeSelector | object | `{}` |  |
| admin.readiness.httpGet.path | string | `"/"` |  |
| admin.readiness.httpGet.port | string | `"http"` |  |
| admin.replicaCount | int | `1` |  |
| admin.resources.limits.cpu | string | `"100m"` |  |
| admin.resources.limits.memory | string | `"128Mi"` |  |
| admin.resources.requests.cpu | string | `"100m"` |  |
| admin.resources.requests.memory | string | `"128Mi"` |  |
| admin.service.containerPort | int | `3100` |  |
| admin.service.port | int | `80` |  |
| admin.service.type | string | `"ClusterIP"` |  |
| admin.tolerations | list | `[]` |  |
| backend.affinity | object | `{}` |  |
| backend.customVolume | object | `{}` |  |
| backend.customVolumeMount | object | `{}` |  |
| backend.image.pullPolicy | string | `"IfNotPresent"` |  |
| backend.image.repository | string | `"hoppscotch/hoppscotch-backend"` |  |
| backend.image.tag | string | `"2024.12.0"` |  |
| backend.ingress.annotations | object | `{}` |  |
| backend.ingress.enabled | bool | `false` |  |
| backend.ingress.hosts[0].host | string | `"chart-example.local"` |  |
| backend.ingress.hosts[0].paths[0] | string | `"/"` |  |
| backend.ingress.tls | list | `[]` |  |
| backend.liveness.httpGet.path | string | `"/"` |  |
| backend.liveness.httpGet.port | string | `"http"` |  |
| backend.nodeSelector | object | `{}` |  |
| backend.readiness.httpGet.path | string | `"/"` |  |
| backend.readiness.httpGet.port | string | `"http"` |  |
| backend.replicaCount | int | `1` |  |
| backend.resources.limits.cpu | string | `"100m"` |  |
| backend.resources.limits.memory | string | `"128Mi"` |  |
| backend.resources.requests.cpu | string | `"100m"` |  |
| backend.resources.requests.memory | string | `"128Mi"` |  |
| backend.service.containerPort | int | `3170` |  |
| backend.service.port | int | `80` |  |
| backend.service.type | string | `"ClusterIP"` |  |
| backend.tolerations | list | `[]` |  |
| database.database | string | `"hoppscotch"` |  |
| database.enabled | bool | `false` |  |
| database.host | string | `"127.0.0.1"` |  |
| database.password | string | `"hoppscotch"` |  |
| database.port | int | `5432` |  |
| database.username | string | `"hoppscotch"` |  |
| frontend.affinity | object | `{}` |  |
| frontend.customVolume | object | `{}` |  |
| frontend.customVolumeMount | object | `{}` |  |
| frontend.image.pullPolicy | string | `"IfNotPresent"` |  |
| frontend.image.repository | string | `"hoppscotch/hoppscotch-frontend"` |  |
| frontend.image.tag | string | `"2024.12.0"` |  |
| frontend.ingress.annotations | object | `{}` |  |
| frontend.ingress.enabled | bool | `false` |  |
| frontend.ingress.hosts[0].host | string | `"chart-example.local"` |  |
| frontend.ingress.hosts[0].paths[0] | string | `"/"` |  |
| frontend.ingress.ingressClassName | string | `""` |  |
| frontend.ingress.tls | list | `[]` |  |
| frontend.liveness.httpGet.path | string | `"/"` |  |
| frontend.liveness.httpGet.port | string | `"http"` |  |
| frontend.nodeSelector | object | `{}` |  |
| frontend.readiness.httpGet.path | string | `"/"` |  |
| frontend.readiness.httpGet.port | string | `"http"` |  |
| frontend.replicaCount | int | `1` |  |
| frontend.resources.limits.cpu | string | `"100m"` |  |
| frontend.resources.limits.memory | string | `"128Mi"` |  |
| frontend.resources.requests.cpu | string | `"100m"` |  |
| frontend.resources.requests.memory | string | `"128Mi"` |  |
| frontend.service.containerPort | int | `3000` |  |
| frontend.service.port | int | `80` |  |
| frontend.service.type | string | `"ClusterIP"` |  |
| frontend.tolerations | list | `[]` |  |
| fullnameOverride | string | `""` |  |
| nameOverride | string | `""` | the override name |
| parameters.auth.github.clientId | string | `""` |  |
| parameters.auth.github.clientSecret | string | `""` |  |
| parameters.auth.github.enabled | bool | `false` |  |
| parameters.auth.github.scope | string | `"user:email"` |  |
| parameters.auth.google.clientId | string | `""` |  |
| parameters.auth.google.clientSecret | string | `""` |  |
| parameters.auth.google.enabled | bool | `false` |  |
| parameters.auth.google.scope | string | `"user:email"` |  |
| parameters.auth.microsoft.clientId | string | `""` |  |
| parameters.auth.microsoft.clientSecret | string | `""` |  |
| parameters.auth.microsoft.enabled | bool | `false` |  |
| parameters.auth.microsoft.scope | string | `"user:email"` |  |
| parameters.config.accessTokenValidity | string | `"86400000"` |  |
| parameters.config.allowSecureToken | bool | `true` |  |
| parameters.config.enableSubPath | bool | `false` |  |
| parameters.config.rateLimit.max | int | `100` |  |
| parameters.config.rateLimit.ttl | int | `60` |  |
| parameters.config.refreshTokenValidity | string | `"604800000"` |  |
| parameters.security.dataEncryptionKey | string | `""` |  |
| parameters.security.jwtSecret | string | `""` |  |
| parameters.security.sessionSecret | string | `""` |  |
| parameters.smtp.enabled | bool | `false` |  |
| parameters.smtp.host | string | `"localhost"` |  |
| parameters.smtp.mailFrom | string | `"<no_reply@example.com>"` |  |
| parameters.smtp.password | string | `""` |  |
| parameters.smtp.port | int | `25` |  |
| parameters.smtp.tlsRejectUnauthorized | bool | `false` |  |
| parameters.smtp.tlsSecure | bool | `false` |  |
| parameters.smtp.username | string | `""` |  |
| parametersSecretName | string | `""` |  |
| postgresql | object | `{"auth":{"database":"hoppscotch","password":"hoppscotch","postgresPassword":"hoppscotch","username":"hoppscotch"},"enabled":true,"primary":{"affinity":{},"nodeSelector":{},"persistence":{"annotations":{},"enabled":true,"labels":{},"size":"10Gi","storageClass":""},"resources":{},"tolerations":[]}}` | Postgresql Database configuration. We do not recommend to use this configuration for production environment. |
| postgresql.auth | object | `{"database":"hoppscotch","password":"hoppscotch","postgresPassword":"hoppscotch","username":"hoppscotch"}` | Configure the authentication of the instance |
| postgresql.enabled | bool | `true` | Enable the internal PostgreSQL installation |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.14.2](https://github.com/norwoodj/helm-docs/releases/v1.14.2)
