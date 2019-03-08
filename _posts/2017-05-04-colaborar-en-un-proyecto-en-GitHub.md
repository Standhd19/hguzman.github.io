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

### Trabajo diario con requerimientos

1. **Crear requerimiento ó funcionalidad:** Cree un nuevo requerimiento en su herramienta de trabajo preferida Ej: trello ó GitHub

2. **Crear una rama donde se desarrollara la funcionalidad:** `git checkout -b feature-nombre-rama`
3. **Hacer los cambios en el codigo:** Estos cambios se realizan utilizando su IDE favorito 
> **Nota:** Los cambios no necesariamente deben ser pequeños, se puede trabajar por horas hasta conseguir una caracterisitica de la funcionalidad

4. **Adicionar archivos que se incluiran en el proximo commit:** Para incluir un solo archivo utilizamos `git add archivo` y para incluir todos los archivos modificados `git add .`

> **Nota:** Para confirmar el estado de los archivos podemos usar `git status`

4. **Commit a los cambios:** Una vez se logre un avance significativo de la funcionalidad o una caracteristica importante se debe realizar un `git commit -m "Descripción del avance"`

> **Nota:** Los commit se realizan para garantizar que no se pierdan las caracterisiticas desarrolladas y de esta manera avanzar a la siguiente

5. **

7. Hacer un Pull Request

```sh

git checkout -b feature-nombre-rama
git push origin feature-nombre-rama
```
<!-- Next you can update your site name, avatar and other options using the _config.yml file in the root of your repository (shown below).

![_config.yml]({{ site.baseurl }}/images/config.png)

The easiest way to make your first post is to edit this one. Go into /_posts/ and update the Hello World markdown file. For more instructions head over to the [Jekyll Now repository](https://github.com/barryclark/jekyll-now) on GitHub. -->
