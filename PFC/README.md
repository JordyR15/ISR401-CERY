# Proyecto Fin de Curso (`TA-PFC-E1`) — Ingeniería de Requerimientos (`ISR-401`)

Repositorio y documentación del **Proyecto Fin de Curso (PFC)** para la asignatura **Ingeniería de Requerimientos (`ISR-401`)**, 4.° nivel, Paralelo A, Universidad Técnica Estatal de Quevedo (UTEQ), período 2026--2027 SPA[cite: 3].

## Integrantes del equipo (Equipo CERY)

| Integrante | Rol / Responsabilidad | Usuario de GitHub |
| :--- | :--- | :--- |
| **Jordy Fabián Rivas Bodero** | Scrum Master / Backend | [@JordyR15](https://github.com/JordyR15) |
| **Luis Antonio Yepez Guagua** | Product Owner / SMTP & Config  | [@Luisin221](https://github.com/Luisin221) |
| **Yerai David Chalacán Toala** | Developer | [@ElGh0sty](https://github.com/ElGh0sty) |
| **Angelo Maximiliano Espinoza Pivaque** | Developer | [Espinoza-P-1007](https://github.com/Espinoza-P-1007) |

## Estructura de carpetas

* `PFC\README.md`: Información general del PFC, tabla de integrantes y estructura de carpetas[cite: 5].
* `PFC\E1\`: Entrega 1 (**`TA-PFC-E1`** — *Visión, alcance, partes interesadas, contexto y plan de elicitación*)[cite: 3, 4]:
  * `PFC\E1\main.tex`: Documento principal en LaTeX[cite: 5].
  * `PFC\E1\referencias\referencias.bib` (o `PFC\E1\referencias.bib`): Bibliografía en formato **IEEE**[cite: 5, 6].
  * `PFC\E1\figuras\`: Imágenes exportadas de los modelos y capturas[cite: 5].
  * `PFC\E1\modelos\`: Fuentes editables de diagramas y modelos (diagrama de contexto, matriz poder--interés, etc.)[cite: 4, 5].
  * `PFC\E1\evidencias\`: Evidencias anonimizadas y `MANIFIESTO.md` de evidencias privadas[cite: 4, 5, 6].
  * `PFC\E1\instrumentos\`: Guion de entrevista, cuestionario y guía de observación o taller[cite: 4].
  * `PFC\E1\main.pdf`: Documento PDF compilado[cite: 5].
  * `PFC\E1\README.md`: Compiladores, dependencias y secuencia de comandos para compilar `main.tex`[cite: 5, 6].

# Compilación de `PFC\E1\main.tex` (`TA-PFC-E1`)

## Compiladores y dependencias necesarios

Para compilar de forma reproducible `PFC\E1\main.tex` y generar `PFC\E1\main.pdf` con las referencias en formato **IEEE**, se requieren:

* **Compilador / distribución LaTeX (`pdfLaTeX`):** **MiKTeX** (o TeX Live) con el motor `pdflatex`.
* **Procesador bibliográfico (`Biber`):** Incluido con MiKTeX; procesa `biblatex` (`style=ieee, sorting=none`) y lee la base bibliográfica (`referencias/referencias.bib` o `referencias.bib`).
* **Paquetes LaTeX utilizados en `main.tex`:** `inputenc`, `fontenc`, `babel` (`spanish`), `csquotes`, `geometry`, `lmodern`, `xcolor`, `array`, `tabularx`, `longtable`, `booktabs`, `graphicx`, `float`, `enumitem`, `fancyhdr`, `titlesec`, `biblatex` y `hyperref`.
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
