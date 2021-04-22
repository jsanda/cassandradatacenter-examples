# Overview
This repo is a collection of CassandraDatacenter manifests that illustrate different features and functionality. 

The examples have been built and tested with [cass-operator 1.6.0](https://github.com/datastax/cass-operator/tree/v1.6.0).

# Setup
Use the Helm Chart from [k8ssandra](https://github.com/k8ssandra/k8ssandra) to install cass-operator.

```
$ helm repo add k8ssandra https://helm.k8ssandra.io/stable

$ helm repo update

$ helm install cass-operator k8ssandra/cass-operator
```
# Examples
* [Cassandra and JVM Configuration](./cassandra-jvm)
* [Cluster Topology](./cluster-topology)
* [Cassandra Pod Resources](./cassandra-pod-resources)
* [Custom Pod Labels](./pod-labels)