# FORM-FB-01 — Fichas bibliográficas

## Datos académicos

**Universidad:** Universidad Técnica Estatal de Quevedo  
**Facultad:** Facultad de Ciencias de la Computación  
**Carrera:** Ingeniería de Software  
**Asignatura:** Aplicaciones Distribuidas (ISR-701) — 7.º nivel, paralelo B  
**Docente:** Gleiston Cicerón Guerrero Ulloa, PhD  
**Estudiante:** Sánchez Vera Darwin Joel  
**Actividad:** FORM-FB-01 — Fichas bibliográficas: fundamentos de sistemas distribuidos y arquitecturas distribuidas  
**Semana:** 2 (2 al 8 de noviembre de 2026)  
**Modalidad:** Individual

## Descripción

Esta carpeta contiene cinco fichas bibliográficas sobre sistemas distribuidos y arquitecturas de microservicios, elaboradas a partir de cinco artículos de revistas indexadas publicados entre 2021 y 2025, todos con DOI verificado. Cada ficha incluye la referencia en formato IEEE (generada con `biblatex` desde el archivo `.bib`), el DOI, un resumen de alrededor de 100 palabras, un dato concreto con su sección o página y una nota personal sobre su uso en el informe TA-IND-01. El documento incluye también la declaración de uso de inteligencia artificial.

## Archivos

| Archivo | Descripción |
|---|---|
| `FORM_FB_01_SanchezDarwin.tex` | Documento principal en LaTeX. |
| `referencias.bib` | Base de datos bibliográfica para BibLaTeX. |
| `FORM_FB_01_SanchezDarwin.pdf` | PDF compilado a partir del documento principal. |
| `README.md` | Este archivo, con las instrucciones de compilación. |

## Dependencias

- Distribución LaTeX: **TeX Live** (2023 o superior) o **MiKTeX**.
- Compilador: **pdfLaTeX**.
- Procesador de bibliografía: **Biber** (no BibTeX).
- Paquetes usados: `inputenc`, `fontenc`, `babel` (opción `spanish`), `lmodern`, `microtype`, `geometry`, `setspace`, `csquotes`, `booktabs`, `tabularx`, `biblatex` (con el estilo `ieee` del paquete `biblatex-ieee`) y `hyperref`.

En TeX Live (Linux) los paquetes se instalan con:

```bash
sudo apt install texlive-latex-extra texlive-lang-spanish texlive-bibtex-extra biber
```

En MiKTeX, los paquetes que falten se instalan automáticamente durante la primera compilación.

## Compilación

Archivo principal: `FORM_FB_01_SanchezDarwin.tex`

Desde una terminal ubicada en esta carpeta (`DarwinSanchez`), ejecutar los comandos en este orden:

```bash
pdflatex FORM_FB_01_SanchezDarwin.tex
biber FORM_FB_01_SanchezDarwin
pdflatex FORM_FB_01_SanchezDarwin.tex
pdflatex FORM_FB_01_SanchezDarwin.tex
```

1. La primera ejecución de `pdflatex` registra las citas.
2. `biber` procesa `referencias.bib` y genera la bibliografía en estilo IEEE.
3. Las dos últimas ejecuciones de `pdflatex` insertan la bibliografía y resuelven las referencias cruzadas.

El resultado es `FORM_FB_01_SanchezDarwin.pdf`.

### Con TeXstudio

En *Opciones → Configurar TeXstudio → Compilar*, seleccionar **PdfLaTeX** como compilador predeterminado y **Biber** como herramienta de bibliografía predeterminada. Luego ejecutar PdfLaTeX, Biber y PdfLaTeX dos veces.

### Con Overleaf

Subir el `.tex` y el `.bib`, y en *Menu → Settings* elegir el compilador **pdfLaTeX**. Overleaf ejecuta Biber automáticamente.

## Fuentes

1. Rodrigues, Rito Silva y Avritzer (2025), *Journal of Systems and Software* — DOI: 10.1016/j.jss.2025.112500
2. Soldani y Brogi (2023), *ACM Computing Surveys* — DOI: 10.1145/3501297
3. Henning y Hasselbring (2022), *Empirical Software Engineering* — DOI: 10.1007/s10664-022-10162-1
4. Laigner et al. (2021), *Proceedings of the VLDB Endowment* — DOI: 10.14778/3484224.3484232
5. Karabey Aksakalli et al. (2021), *Journal of Systems and Software* — DOI: 10.1016/j.jss.2021.111014