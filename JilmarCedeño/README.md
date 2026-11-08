# FORM-FB-01 — Fichas bibliográficas

## Datos académicos

**Universidad:** Universidad Técnica Estatal de Quevedo  
**Facultad:** Facultad de Ciencias de la Computación  
**Carrera:** Ingeniería de Software  
**Asignatura:** Aplicaciones Distribuidas (ISR-701)   
**Estudiante:** Cedeño Intriago Jilmar Jesus  
**Actividad:** FORM-FB-01 — Fichas bibliográficas: fundamentos de sistemas distribuidos y arquitecturas distribuidas  
**Fecha de elaboración:** Del 6 al 8 de noviembre de 2026  
**Modalidad:** Individual

## Descripción

Este repositorio contiene cinco fichas bibliográficas sobre arquitecturas de microservicios y sistemas distribuidos, elaboradas a partir de cinco artículos académicos publicados entre 2021 y 2024.

Cada ficha incluye una referencia en formato IEEE, DOI, síntesis del artículo, dato concreto con su ubicación y una nota personal sobre su utilidad para el informe académico TA-IND-01.

## Archivos del proyecto

| Archivo | Descripción |
|---|---|
| `Semana2AD.tex` | Documento principal elaborado en LaTeX. |
| `referencias.bib` | Referencias bibliográficas para BibLaTeX. |
| `Semana2AD.pdf` | PDF generado desde el archivo LaTeX. |
| `README.md` | Descripción e instrucciones de compilación. |

## Requisitos de compilación

Para compilar el documento se necesita:

- MiKTeX o TeX Live.
- Un compilador `pdfLaTeX`.
- Biber para procesar las referencias bibliográficas.
- Paquete `biblatex` con estilo `ieee`.
- Paquetes adicionales declarados en `Semana2AD.tex`.

## Instrucciones de compilación

1. Descargar o clonar el repositorio.
2. Abrir una terminal en la carpeta donde se encuentran `Semana2AD.tex` y `referencias.bib`.
3. Ejecutar los siguientes comandos en este orden:

```bash
pdflatex Semana2AD.tex
biber Semana2AD
pdflatex Semana2AD.tex
pdflatex Semana2AD.tex
```

El resultado será el archivo `Semana2AD.pdf`.

### Compilación mediante TeXstudio

Abrir `Semana2AD.tex` y configurar:

- Compilador predeterminado: **PdfLaTeX**.
- Herramienta bibliográfica predeterminada: **Biber**.

Ejecutar PdfLaTeX, Biber y nuevamente PdfLaTeX dos veces.

## Referencias bibliográficas

Las cinco referencias están registradas en `referencias.bib` mediante sus datos editoriales y DOI. La bibliografía se genera automáticamente con `biblatex`, utilizando el estilo IEEE.

## Uso de inteligencia artificial

La declaración de uso de inteligencia artificial se encuentra dentro del documento `Semana2AD.pdf`, en la sección correspondiente.