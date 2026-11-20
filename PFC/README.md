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

## Compilación de la entrega (`PFC\E1`)

Para generar `PFC\E1\main.pdf` y cargar las referencias bibliográficas en estilo **IEEE**, revisa los compiladores y dependencias detallados en `PFC\E1\README.md` y ejecuta desde `PFC\E1`:

```bat
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex