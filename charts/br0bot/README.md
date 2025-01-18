# br0bot

![Version: 0.3.4](https://img.shields.io/badge/Version-0.3.4-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 2.0.2](https://img.shields.io/badge/AppVersion-2.0.2-informational?style=flat-square)

Br0fessional b0t hosting

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| oci://registry-1.docker.io/bitnamicharts/postgresql | postgresql | 16.4.3 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.maxReplicas | int | `100` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| bot.buzzwords[0].reply | string | `"ein weiterer centimeter mehr, unsere Arschlöcher sind nun *%d* groß"` |  |
| bot.buzzwords[0].trigger | string | `"anal"` |  |
| bot.buzzwords[10].pattern | string | `"(vapoctl|klick)"` |  |
| bot.buzzwords[10].reply | string | `"🥦 schon wieder vaped sich einer gesund, Bereits *%d* mal wurde Medizin genommen"` |  |
| bot.buzzwords[10].trigger | string | `"vapoctl"` |  |
| bot.buzzwords[11].pattern | string | `"(zieh|ziehen|gezogen|ziags da nei|ziagsdanei|pep|pepp)"` |  |
| bot.buzzwords[11].reply | string | `"👃 ziagsdanei\\! Das *%d*te mal schon"` |  |
| bot.buzzwords[11].trigger | string | `"ziehen"` |  |
| bot.buzzwords[1].pattern | string | `"(huan|huso)"` |  |
| bot.buzzwords[1].reply | string | `"Und wieder wurde einer zum Huan ernannt. *Huan* ist jetzt auf *%d*"` |  |
| bot.buzzwords[1].trigger | string | `"huan"` |  |
| bot.buzzwords[2].reply | string | `"🙄 Schon wieder ist etwas am Arsch: *Tzn* ist jetzt auf *%d*"` |  |
| bot.buzzwords[2].trigger | string | `"tzn"` |  |
| bot.buzzwords[3].pattern | string | `"(bier|weißbier|pils|saufen|saufem)"` |  |
| bot.buzzwords[3].reply | string | `"🍻 Scho wieder am saufem, damit ist *Bier* jetzt auf *%d*"` |  |
| bot.buzzwords[3].trigger | string | `"bier"` |  |
| bot.buzzwords[4].reply | string | `"Nice\\! 🥦 *420* ist jetzt auf *%d*"` |  |
| bot.buzzwords[4].trigger | string | `"420"` |  |
| bot.buzzwords[5].pattern | string | `"(weggesynced|weggesynct)"` |  |
| bot.buzzwords[5].reply | string | `"`rm -rf /` *Weggesynced* ist jetzt auf *%d*"` |  |
| bot.buzzwords[5].trigger | string | `"weggesynct"` |  |
| bot.buzzwords[6].reply | string | `"Der Sync ist stark in diesem\\! *Sync* ist damit auf *%d*"` |  |
| bot.buzzwords[6].trigger | string | `"sync"` |  |
| bot.buzzwords[7].reply | string | `"Immer ist irgendwas kaputt\\! 🤬 *Obegfoin* ist jetzt auf *%d*"` |  |
| bot.buzzwords[7].trigger | string | `"obegfoin"` |  |
| bot.buzzwords[8].pattern | string | `"(lel|lol|rofl|relf|lmao)"` |  |
| bot.buzzwords[8].reply | string | `"Und schon wieder wurde extrem laut gelacht\\! *Lel* ist jetzt auf *%d*"` |  |
| bot.buzzwords[8].trigger | string | `"lel"` |  |
| bot.buzzwords[9].pattern | string | `"(kartoffel|pommes)"` |  |
| bot.buzzwords[9].reply | string | `"Kartoffel\\? 🤜🤛👊 Pommes\\! Schon *%d* Kilo zugenommen"` |  |
| bot.buzzwords[9].trigger | string | `"kartoffel"` |  |
| bot.telegram.apiKey | list | `[]` |  |
| bot.telegram.webhookurl | string | `"chart-example.local"` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"ghcr.io/br0-space/bot"` |  |
| image.tag | string | `""` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.annotations | object | `{}` |  |
| ingress.className | string | `""` |  |
| ingress.enabled | bool | `false` |  |
| ingress.hosts[0].host | string | `"chart-example.local"` |  |
| ingress.hosts[0].paths[0].path | string | `"/"` |  |
| ingress.hosts[0].paths[0].pathType | string | `"ImplementationSpecific"` |  |
| ingress.tls | list | `[]` |  |
| livenessProbe.httpGet.path | string | `"/"` |  |
| livenessProbe.httpGet.port | string | `"http"` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podLabels | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| postgresql.auth.database | string | `"b0t"` |  |
| postgresql.auth.existingSecret | string | `""` |  |
| postgresql.auth.password | string | `"b0t"` |  |
| postgresql.auth.username | string | `"b0t"` |  |
| postgresql.install | bool | `false` |  |
| postgresql.metrics.enabled | bool | `false` |  |
| postgresql.persistence.accessModes[0] | string | `"ReadWriteOnce"` |  |
| postgresql.persistence.enabled | bool | `false` |  |
| postgresql.persistence.size | string | `"8Gi"` |  |
| postgresql.persistence.storageClass | string | `""` |  |
| postgresql.postgresqlDatabase | string | `"kmptnz"` |  |
| postgresql.postgresqlPassword | string | `"kmptnz"` |  |
| postgresql.postgresqlUsername | string | `"kmptnz"` |  |
| readinessProbe.httpGet.path | string | `"/"` |  |
| readinessProbe.httpGet.port | string | `"http"` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| securityContext | object | `{}` |  |
| service.port | int | `3000` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.automount | bool | `true` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `""` |  |
| tolerations | list | `[]` |  |
| volumeMounts | list | `[]` |  |
| volumes | list | `[]` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.14.2](https://github.com/norwoodj/helm-docs/releases/v1.14.2)
