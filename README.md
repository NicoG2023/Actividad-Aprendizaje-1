# Actividad de Aprendizaje 1 — Arquitectura de Seguridad

Documento del proyecto elaborado en **LaTeX** con la clase `apa7` (formato APA 7, portada de estudiante generada por la clase).

## Estructura

- `main.tex`: documento principal. Contiene el preámbulo (paquetes y configuración general), los metadatos de la portada (`\title`, `\authorsnames`, `\authorsaffiliations`, `\course`, `\professor`, `\duedate`) y el ensamblado de las secciones. No escribir contenido directamente aquí salvo que se agregue una nueva sección.
- `secciones/`: contenido del documento, un archivo por sección.
- `secciones/casos/`: casos de negocio de los integrantes.
- `imagenes/`: imágenes utilizadas en el documento.
- `referencias.bib`: referencias bibliográficas en BibLaTeX.

## Cómo trabajar

Antes de empezar, actualizar la rama local:

Cada integrante debe editar únicamente el archivo `.tex` correspondiente a la sección en la que esté trabajando. Para agregar una referencia bibliográfica, incluirla en `referencias.bib` y citarla desde LaTeX con `\textcite{clave}` o `\parencite{clave}`.

Para compilar el documento desde la raíz del proyecto:

```bash
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

El resultado se genera en `main.pdf`.
