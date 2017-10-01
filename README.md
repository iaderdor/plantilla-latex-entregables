# Instrucciones

El presente documento pretende recopilar las instrucciones de uso de las plantillas de entregables de `LaTeX` hechas por Ismael Aderdor <aderdor@gmail.com>. La motivación principal de este proyecto es evitar los típicos archivos con "código espagueti" en el que suelen acabar todas las cosas que toca un físico.

### Objetivo

Con este documento se pretende tener una plantilla que pueda usarse para realizar entregables, trabajos, informes de laboratorio y demás documentos necesarios para la universidad.

### Licencias

Si está interesado acerca de las licencias que cubren estos archivos, puede echar un vistazo al archivo `LICENCIAS.md`.

### Archivos

A continuación se encuentra una lista que describe lo que hace (o debería de hacer) cada archivo y carpeta.

#### `entregable.tex`

Es el archivo principal del documento. Es el que hay que compilar en caso de que se desee sacar el documento entero.

#### `INSTRUCCIONES.md`

Es el presente documento.

#### `LICENCIAS.md`

Este archivo contiene la totalidad de las licencias que afectan al código.

#### `img/`

Dentro de estas carpetas deberían de ir las distintas imágenes que estén dentro del documento.

#### `sty/comandos.sty`

En este archivo se hallan definidos algunos comandos de `LaTeX`. Debería modificarse según la necesidad de el trabajo a realizar.

**IMPORTANTE**: Todas las definiciones de comandos, teoremas, ambientes y demás debería de realizarse en este archivo para que si en algún momento se decidiese cambiar algo afectase al documento entero y no únicamente a partes.

### `sty/paquetes.sty`

Este archivo carga todos los paquetes necesarios para que compile el documento, así como algunas opciones de los propios paquetes. Declarándolos aquí en vez de en `apuntes.tex` conseguimos mayor limpieza y modularidad en el documento.

### `sty/titulo.sty`

En este archivo se encuentran las variables que modifican el título, descripción, autor y editor que posteriormente se aplicarán a la portada del documento.

#### `tex/`

Dentro de esta carpeta deberían de ir la totalidad de los archivos `.tex`, a excepción de `apuntes.tex`, que es el documento padre.

Cada tema o sección del entregable debería de estar en un archivo a parte.

#### `tex/titulo.tex`

Este documento es el que genera la portada de los apuntes.

#### `tex/modelo.tex`

Este archivo es un modelo para generar los distintos capítulos de los que estén conformados los apuntes.

## Funcionamiento

#### Compilar

Para compilar los archivos generados es necesario usar `XeTeX` o `XeLaTeX`. Personalmente, uso el IDE `TeXmaker` para trabajar con este tipo de proyectos. Sin embargo, puede usarse directamente el comando `xelatex` con las opciones necesarias.
