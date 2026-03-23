# Diataxis

Orderer interface for [katastroma](https://github.com/katastroma). Defines the
service contract for ordering Kubernetes manifests into a safe apply sequence.

An orderer takes manifests and ensures they are in an order safe for sequential
apply — namespaces before resources that live in them, CRDs before custom
resources, RBAC before workloads that depend on service accounts, etc.
