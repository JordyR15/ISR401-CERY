# Compilación de `PFC\E1\main.tex` (`TA-PFC-E1`)

## Compiladores y dependencias necesarios

Para compilar de forma reproducible `PFC\E1\main.tex` y generar `PFC\E1\main.pdf` con las referencias en formato **IEEE**, se requieren:

* **Compilador / distribución LaTeX (`pdfLaTeX`):** **MiKTeX** (o TeX Live) con el motor `pdflatex`.
* **Procesador bibliográfico (`Biber`):** Incluido con MiKTeX; procesa `biblatex` (`style=ieee, sorting=none`) y lee la base bibliográfica (`referencias/referencias.bib` o `referencias.bib`).
* **Paquetes LaTeX utilizados en `main.tex`:** `inputenc`, `fontenc`, `babel` (`spanish`), `csquotes`, `geometry`, `lmodern`, `xcolor`, `array`, `tabularx`, `longtable`, `booktabs`, `graphicx`, `enumitem`, `fancyhdr`, `titlesec`, `biblatex` y `hyperref`.
* **Editor LaTeX (opcional):** **TeXworks** (u otro editor compatible) si se desea compilar desde interfaz gráfica.

## Archivo principal y orden de compilación

* **Archivo principal:** `PFC\E1\main.tex`
* **Archivo de salida:** `PFC\E1\main.pdf`

Ubícate en la carpeta `PFC\E1` y ejecuta estos comandos en orden para compilar el documento y **cargar las referencias bibliográficas**:

```bat
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex