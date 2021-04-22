# Remote JMX
This example demonstrates how to enable remote JMX access for Cassandra.

It assumes a secret named `jmx-credentials` exists in the namespace in which the CassandraDatacenter will be created. The secret should have two keys - `username` and `password`.

You can created the secret as follows:

```
$ kubectl create secret generic jmx-credentials \
    --from-literal=username=cassandra \
    --from-literal=password=cassandra
```

Check out the Kubernetes [docs](https://kubernetes.io/docs/tasks/configmap-secret/managing-secret-using-kubectl/) for more details on ways to create secrets.