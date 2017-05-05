---
layout: post
title: Colaborar en un proyecto en GitHub
---

Para colaborar en un proyecto GitHub, se deben seguir estos pasos:

1. Fork del repositorio
2. Clonar el repositorio
3. Actualizar la rama master
4. Crear una rama
5. Hacer los cambios
6. Hacer un Pull Request

```sh
git clone https://github.com/User/NombreRepo.git
git remote -v
git remote add upstream https://github.com/User/RepoOriginal(Forkeado)
git pull -r upstream master
git checkout -b feature-nombre-rama
git push origin feature-nombre-rama
```
<!-- Next you can update your site name, avatar and other options using the _config.yml file in the root of your repository (shown below).

![_config.yml]({{ site.baseurl }}/images/config.png)

The easiest way to make your first post is to edit this one. Go into /_posts/ and update the Hello World markdown file. For more instructions head over to the [Jekyll Now repository](https://github.com/barryclark/jekyll-now) on GitHub. -->
