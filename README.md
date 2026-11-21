# Repositorio ISR-401 — TA-PFC-E1

Proyecto Fin de Curso: **Sistema de Gestión para Restaurante con Módulo de
Inteligencia Artificial**, organización cliente: El Balcón Restaurant
(Quevedo, Los Ríos).

**Nombre del repositorio (norma 7.1):** `ISR-401-NRS`, público en GitHub.
Corresponde al Paralelo B; la sigla `NRS` identifica al equipo por las iniciales
de los apellidos Naranjo, Robinson y Sánchez.

**URL del repositorio:** https://github.com/Roselyn15/ISR-401-NRS

## Integrantes y roles

- Robinson Espinoza Jeanpierre — líder; visión, alcance, gestión del proyecto, carta de aceptación, consentimiento y custodia LOPDP, integración final y compilación.
- Naranjo Alfonzo Anthony Alexander — elicitación y modelado; técnicas por fuente, instrumentos, diagrama de contexto y matriz poder–interés (fuentes `.puml`), tabla de las ocho perspectivas.
- Sánchez Centeno Roselyn Andreina — análisis y calidad documental; partes interesadas, estrategia de participación, coherencia y trazabilidad, referencias IEEE y revisión del PDF.

## Estructura prevista

```
PFC/E1/
├── main.tex
├── referencias.bib
├── main.pdf
├── secciones/
│   ├── 01_ficha_alcance.tex
│   ├── 02_partes_interesadas.tex
│   ├── 03_contexto.tex
│   ├── 03_plan_elicitacion.tex
│   └── 04_gestion_proyecto.tex
├── instrumentos/
│   ├── guion_entrevista.tex
│   ├── cuestionario.tex
│   └── guia_observacion_taller.tex
├── modelos/
│   ├── contexto.puml
│   └── poder_interes.puml
├── figuras/
└── evidencias/
    └── MANIFIESTO.md
```

## Compilación reproducible

**Compilador:** MiKTeX actualizado o TeX Live 2023 en adelante (`pdflatex` + `biber`).

**Archivo principal:** `PFC/E1/main.tex`.

**Orden de comandos** (ejecutar desde la carpeta `PFC/E1`):

```bash
pdflatex -interaction=nonstopmode main.tex
biber main
pdflatex -interaction=nonstopmode main.tex
pdflatex -interaction=nonstopmode main.tex
pdflatex -interaction=nonstopmode main.tex
```

> **Usar `biber`, NO `bibtex`.** El preámbulo carga
> `\usepackage[backend=biber,style=ieee]{biblatex}` y el documento cierra con
> `\printbibliography`. Con `bibtex` no se genera el `.bbl` y la bibliografía
> queda vacía o con referencias sin resolver.

**Dependencias LaTeX:** `babel-spanish`, `geometry`, `array`, `tabularx`,
`booktabs`, `colortbl`, `xcolor`, `enumitem`, `fancyhdr`, `lastpage`,
`tcolorbox` (opción `most` y librería `breakable`), `csquotes`, `inputenc`,
`fontenc`, `hyperref`, `biblatex` con estilo IEEE y el ejecutable `biber`.

## Verificación del PDF resultante

Tras la secuencia anterior, `main.pdf` debe cumplir:

```bash
pdfinfo main.pdf | grep Pages
pdftotext -layout main.pdf - | grep -c "de 19"
pdftotext -layout main.pdf - | grep -c "??"
grep -c "Overfull \\hbox" main.log
grep -c "undefined" main.log
```

Valores esperados: `Pages: 19`, `19` pies con `de 19`, `0` ocurrencias de
`??`, `0` desbordamientos y `0` referencias sin resolver. La bibliografía debe
mostrar seis entradas IEEE. Los archivos auxiliares (`.aux`, `.bbl`, `.bcf`,
`.blg`, `.log`, `.out`, `.toc`, `main.run.xml`) no se versionan.

## Normas del repositorio

- Compilar siempre el árbol fusionado de `PFC/E1/`, nunca las carpetas de reparto
  de commits por integrante.
- Si se inserta una figura, el nombre y la extensión en `\includegraphics{}`
  deben coincidir exactamente con el archivo real subido.
- No publicar datos personales, grabaciones, actas ni consentimientos firmados.
  Las evidencias privadas se registran solo en `evidencias/MANIFIESTO.md`.
- El historial debe mostrar trabajo sustantivo en al menos tres días distintos
  (19, 20 y 21 de noviembre de 2026).
