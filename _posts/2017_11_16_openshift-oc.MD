# Manual de referencia de OpenShift oc

Cargar un nuevo template al cluster OpenShift.

Cargar template a nivel de cluster.
`$ oc create -f <filename>`

Cargar template a nivel proyecto.
`$ oc create -f <filename> -n <project>`

Ejemplo
___

```$ wget https://raw.githubusercontent.com/sclorg/mongodb-container/master/examples/petset/mongodb-petset-persistent.yaml
$ oc create -f mongodb-petset-persistent.yaml```

> template "mongodb-petset-replication" created
