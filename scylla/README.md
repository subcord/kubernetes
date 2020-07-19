# Scylla DB configuration

## Order to deploy
- StorageClass
- Service
- ConfigMap
- PersistentVolume
- StatefulSet

Things probably would work in another order, but for simplicity this is the order I (@j03b) deploy things.

## Confirm deployment

Run `kubectl exec -n subcord scylla-0 -- nodetool status` to see the ring status.

## Sources

https://github.com/scylladb/scylla-code-samples/blob/master/kubernetes-scylla
