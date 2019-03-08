---
layout: post
title: Colaborar en un proyecto en GitHub
---

Para colaborar en un proyecto GitHub, se deben seguir estos pasos:

1. **Fork del repositorio:** Realiza un copia exacta del repositorio en el perfil del usuario colaborador
2. **Clonar el repositorio:** 
  `
  git clone https://github.com/User/NombreRepo.git
  `
  
3. **Entrar en la carpeta clonada:** Para entrar a la carpeta clonada desde una consola ubuntu use el comando `cd NombreRepo`

 
4. **Verificar las conexiones con fuentes remotas:** `git remote -v` por defecto se mostrara la conexión realizada cuando se clono el repositorio, por defecto es llamada `origin`
 
5. **Crear una conexión remota con el repositorio original** `git remote add upstream https://github.com/User/RepoOriginal(Forkeado)`

6. **Renombrar conexiones remotas:** Con el fin de tener un poco mas de claridad sobre cual es la conexión remota que estamas usando, se puede renombrar a gusto con el comando `git remote rename origin fork`

7. **Actualizar rama master con ultimos cambios:** Para tener actualizado nuestro repositorio local con las ultimas actualizaciones del repositorio remoto original rama master `git pull -r upstream master`


5. Crear una rama
6. Hacer los cambios
7. Hacer un Pull Request

```sh

git checkout -b feature-nombre-rama
git push origin feature-nombre-rama
```
<!-- Next you can update your site name, avatar and other options using the _config.yml file in the root of your repository (shown below).

![_config.yml]({{ site.baseurl }}/images/config.png)

The easiest way to make your first post is to edit this one. Go into /_posts/ and update the Hello World markdown file. For more instructions head over to the [Jekyll Now repository](https://github.com/barryclark/jekyll-now) on GitHub. -->
