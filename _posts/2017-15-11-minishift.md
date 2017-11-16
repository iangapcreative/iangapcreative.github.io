# Introducción a minishift

## Iniciar minishift

### Indicar que minishift descargue un ISO particular para crear la VM. 

`$ minishift start --iso-url https://github.com/minishift/minishift-centos-iso/releases/download/v1.0.0/minishift-centos7.iso`

**NOTA**: Imagen usada por defecto boot2docker.iso

### Indicar que se use un archivo ISO local como base para VM

`$ minishift start --iso-url file:///<path_to_ISO_image>`

**NOTA**: Mas detalles en https://docs.openshift.org/latest/minishift/using/basic-usage.html#choosing-iso-image

Esto puede ser de utilidad cuando no se cuenta con acceso a Internet, ya que una imagen ISO tiene un tamaño del ordeb de los Gigabytes

### Cambiar la configuracion de RAM asignada a una VM de minishift
`$ minishift config set memory 4096`

Una vez aplicado el comando la proxima vez que inicie la VM el cambio tendra efecto

**NOTA**: La cantidad de memoria RAM por defecto asignada a la VM de minishift es de 2 GB.
**NOTA**: La memoria es expresada en Megabytes.
