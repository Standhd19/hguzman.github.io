---
layout: post
title: Instrucciones para copiar archivos en S3
---

En la actualidad pago los servicios de Amason AWS para mantener el proyect fleteo.co en funcionamiento.

Me encontre con la necesidad de usar el servicio S3 para mantener copia de mis archivos en la nube, pero no estaba familiarizado con los comandos necesarios para realizar dicha actividad.

Para realizar la copia desde consola, instale el cliente:
`brew install awscli`

Despues, solo resta usar los siguiente comandos:

### Crear buckets
aws s3 mb s3://lab01-storage
### Listar buckets
aws s3 ls
### Eliminar Buckets
aws s3 rb s3://lab02-storage
### Copiar archivos - local Remoto
aws s3 cp foo.txt  s3://lab01-storage
### Copiar archivos - Remoto local
aws s3 cp s3://lab01-storage/bar.txt bar.txt
### Listar archivos
aws s3 ls s3://lab01-storage
### Mover archivo remoto
aws s3 mv s3://lab01-storage/foo.txt s3://lab01-storage/bar.txt
### Borrar archivo remoto
aws s3 rm s3://lab01-storage/bar.txt
### sincronizar carpeta
aws s3 sync test/ s3://lab01-storage --recursive
### Sincronizar borrando los archivos que ya no estan en el local
aws s3 sync test s3://lab01-storage --delete
### Copiar carpeta - local Remoto
aws s3 cp foo.txt  s3://lab01-storage --recursive --exclude "*.log"

### Comando suado para Sincronizar.
`aws s3 sync CopiaSeguridad/ s3://hguzman-store --delete`
