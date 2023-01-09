+++
title = "Empieza a entender Hugo"
tags = ["go", "golang", "hugo", "desarrollo", "tutorial", "docs", "configuracion"]
date = "2023-01-01"
+++


## Paso 1. Instalar Hugo

Vaya a [Lanzamientos de Hugo](https://github.com/spf13/hugo/releases) y descargue el
versión adecuada para su sistema operativo y arquitectura.

Guárdelo en algún lugar específico, ya que lo usaremos en el siguiente paso.

Hay instrucciones más completas disponibles en [Instalar Hugo](https://gohugo.io/getting-started/installing/)

## Paso 2. Cree los documentos

Hugo tiene su propio sitio de ejemplo que también es el sitio de documentación.
estás leyendo ahora mismo.

Siga los siguientes pasos:

 1. Clone el [repositorio de Hugo](http://github.com/spf13/hugo)
 2. Entra en el repositorio
 3. Ejecute hugo en modo servidor y cree los documentos
 4. Abra su navegador en http://localhost:1313

Pseudocomandos correspondientes:

    clon de git https://github.com/spf13/hugo
    hugo
    /ruta/hacia/dónde/usted/instaló/servidor hugo --source=./docs
    > 29 páginas creadas
    > 0 índice de etiquetas creado
    > en 27ms
    > El servidor web está disponible en http://localhost:1313
    > Presione ctrl+c para detener

Una vez que haya llegado aquí, siga el resto de esta página en su compilación local.

## Paso 3. Cambiar el sitio de documentos

Detenga el proceso de Hugo presionando Ctrl+C.

Ahora vamos a ejecutar hugo nuevamente, pero esta vez con hugo en modo reloj.

    /ruta/hacia/hugo/desde/paso/1/servidor hugo --source=./docs --watch
    > 29 páginas creadas
    > 0 índice de etiquetas creado
    > en 27ms
    > El servidor web está disponible en http://localhost:1313
    > Observar cambios en /Users/spf13/Code/hugo/docs/content
    > Presione ctrl+c para detener


Abra su [editor favorito] (http://vim.spf13.com) y cambie una de las fuentes
páginas de contenido. ¿Qué tal cambiar este mismo archivo para *corregir el error tipográfico*? ¿Qué tal cambiar este mismo archivo para *corregir el error tipográfico*?

Los archivos de contenido se encuentran en `docs/content/`. A menos que se especifique lo contrario, los archivos
están ubicados en la misma ubicación relativa que la url, en nuestro caso
`docs/content/overview/quickstart.md`.

Cambie y guarde este archivo. Observe lo que sucedió en su terminal.

    > Cambio detectado, sitio de reconstrucción

    > 29 páginas creadas
    > 0 índice de etiquetas creado
    > en 26ms

Actualice el navegador y observe que el error tipográfico ya está corregido.

Note lo rápido que fue. Intente actualizar el sitio antes de que termine de construirse. Te recontra reto.
Tener comentarios casi instantáneos le permite hacer que su creatividad fluya sin esperar largas compilaciones.

## Paso 4. Diviértete

La mejor manera de aprender algo es jugar con ello.