---
layout: post
title: Actividad del dragon
---

Estoy desarrollando un software con **Ruby on Rails** que maneja imagenes, me gusta usar [GitHub](https://github.com/){:target="_blank"} para mantener mi codígo actualizado. Despues de varios commits y push me pude dar cuenta que en el archivo .gitignore **NO** incluí la linea para evitar que las imagenes de ejemplo fueran objeto de control de codigo.

Googleando un poco encontre este recurso [Git ready](http://es.gitready.com/beginner/2009/01/19/ignoring-files.html){:target="_blank"}, donde el autor explica como sacar el archivo para luego ignorarlo.

El comando es muy sencillo `git rm --cached <file>`

> Creo que es un problema muy común y que se debe tener en cuenta para los proyectos.
