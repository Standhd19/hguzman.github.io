---
layout: post
title: Eliminar ultimo commit en git
---

Cuando usted de manera errada realiza cambios en su programa y ejecuta commit, usted le gustaria dejarlo en el estado anterior.

Recuerde que despues de ejecutado el comando se perderan todos los cambios realizados en el ultimo commit

```sh
git reset --hard HEAD~1
```
Usted tambien puede quitar el ultimo commit pero dejando los ultimos cambios.

```sh
git reset HEAD~1
```
