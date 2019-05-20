---
layout: post
title: Notas sobre VIM
---

Comando para remplazar información hasta un )

```sh
ci)
```

Comandos para comentar codigo con tcomment_vim:

`gcir` / `gcar` comment inside/around Ruby do/end block.
`gcim` / `gcam` comment inside/around Ruby method.
`gciM` / `gcaM` comment inside/around Ruby class.
Plus normal Commentary maps like `gcc` to comment a line, or `5gcc` to comment 5 lines

Para vel un tutotial en consola
vimtutorial

### Realizar Paginación en VIM

Para paginar hacia abajo se usa (page down) `CTRL-D` y para moverse hacia arriba page up `CTRL-U` 

### Abrir el menú para crear y borrar archivos NERDtree

Se debe usar la letra `m`

### Escribir despues de una palabra

`wi`o `ea`

### Guardar un archivo como

Para realizar esta actividad, solo se abre el archivo que se va a guardar como y se ejecuta el comando:

`:w %:h/other_filename`

### Plegado de lineas de codigo

Para realizar el pegado se deve estar en modo visual y seleccionar el codigo que se desea plegar
`zf`
y para colocarlo como estaba se usa `za`

### Realizar busqueda

Para realizar una busqueda se usa [fugitive](https://github.com/tpope/vim-fugitive).
La busqueda se realiza así: 
:Ggrep hola

Para moverse por los archivos con resultados se usa:
:cnext
:cprev
:copen
