---
layout: post
title: Ignorar un archivo despues de un push en GitHub
---

Estoy desarrollando un software con **Ruby on Rails** que maneja imagenes, me gusta usar [GitHub](https://github.com/) para mantener mi codígo actualizado. Despues de varios commits y push me pude dar cuenta que en el archivo .gitignore **NO** incluí la linea para evitar que las imagenes de ejemplo fueran objeto de control de codigo.

Googleando un poco encontre este recurso [Git ready](http://es.gitready.com/beginner/2009/01/19/ignoring-files.html), donde el autor explica como sacar el archivo para luego ignorarlo.

El comando es muy sencillo `git rm --cached <file>`

> Creo que es un problema muy común y que se debe tener en cuenta para los proyectos.
