---
layout: post
title: Colaborar en un proyecto en GitHub
---

Para colaborar en un proyecto GitHub, se deben seguir estos pasos:

1. **Fork del repositorio:** Realiza un copia exacta del repositorio en el perfil del usuario colaborador
2. **Clonar el repositorio:** `git clone https://github.com/User/NombreRepo.git`
3. **Entrar en la carpeta clonada:** Para entrar a la carpeta clonada desde una consola ubuntu use el comando `cd NombreRepo`
4. **Verificar las conexiones con fuentes remotas:** `git remote -v` por defecto se mostrara la conexión realizada cuando se clono el repositorio, por defecto es llamada `origin`
5. **Crear una conexión remota con el repositorio original** `git remote add upstream https://github.com/User/RepoOriginal(Forkeado)`
6. **Renombrar conexiones remotas:** Con el fin de tener un poco mas de claridad sobre cual es la conexión remota que estamas usando, se puede renombrar a gusto con el comando `git remote rename origin fork`

### Trabajo diario con requerimientos

1. **Actualizar rama master con ultimos cambios:** Para tener actualizado nuestro repositorio local con las ultimas actualizaciones del repositorio remoto original rama master `git pull -r upstream master`
2. **Crear requerimiento ó funcionalidad:** Cree un nuevo requerimiento en su herramienta de trabajo preferida Ej: trello ó GitHub
3. **Crear una rama donde se desarrollara la funcionalidad:** `git checkout -b feature-nombre-rama`
> **Nota:** Podemos usar el comando `git branch`para saber en cual rama estamos trabajando
4. **Hacer los cambios en el codigo:** Estos cambios se realizan utilizando su IDE favorito 
> **Nota:** Los cambios no necesariamente deben ser pequeños, se puede trabajar por horas hasta conseguir una caracterisitica de la funcionalidad podemos usar `git status`
5. **Adicionar archivos que se incluiran en el proximo commit:** Para incluir un solo archivo utilizamos `git add archivo` y para incluir todos los archivos modificados `git add .`
> **Nota:** Para confirmar el estado de los archivos podemos usar `git status`
6. **Commit a los cambios:** Una vez se logre un avance significativo de la funcionalidad o una caracteristica importante se debe realizar un `git commit -m "Descripción del avance"`
> **Nota:** Los commit se realizan para garantizar que no se pierdan las caracterisiticas desarrolladas y de esta manera avanzar a la siguiente
7. **Subir la rama con los cambios:** Una vez hemos desarrollado completamente la funcionalidad, procedemos a subirla con el comando `git push origin feature-nombre-rama` 
> **Nota:** Recordemos que se debe subir la rama al repositorio propiedad del colaborador (NO AL ORIGINAL)
8. **Solicitar que se incorporen cambios:** Entramos a nuestro usuario y reealizamos una solicitud de incorporación del codigo al proyecto original utilizando la opción Pull Request
9. **Eliminar rama en local:** Para eliminar una rama despues que fue incorporada por el propietario del repositorio, usaremos el comando `git branch -d feature-nombre-rama`
> **Nota:** si deseamos eliminarla sin usar el comando merge utilizaremos `git branch -D feature-nombre-rama`
10. **Eliminar rama en repositorio remoto:** Para eliminar una rama que esta en un repositorio remoto usaremos `git push origin --delete feature-nombre-rama`

### Unir Ramas

Para unir ramas dentro de nuestro repositorio local usaremos el comando `git merge feature-nombre-rama`, debemos estar ubicado en la rama que deseamos actualizar


<!-- Next you can update your site name, avatar and other options using the _config.yml file in the root of your repository (shown below).

![_config.yml]({{ site.baseurl }}/images/config.png)

The easiest way to make your first post is to edit this one. Go into /_posts/ and update the Hello World markdown file. For more instructions head over to the [Jekyll Now repository](https://github.com/barryclark/jekyll-now) on GitHub. -->
