# Strimzi Operator

- Versão: 1.2.0
- Namespace: prod
- Gerenciado pelo Argo CD com Server-Side Apply.

O campo vazio `properties: {}` de `status.clusterSecurity` foi removido porque o Kubernetes não o mantém no CRD armazenado, o que causava sincronizações contínuas e estado OutOfSync no Argo CD.
