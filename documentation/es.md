<!-- ELUCENIA technical documentation · abcd2 · es · no clinical/professional/rights approval -->

# Puntuación ABCD²

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/abcd2)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Edad ≥ 60 años

`idade`

### Presión arterial ≥ 140/90 mmHg en la primera evaluación

`pa`

### Manifestación clínica

`clinica`

- `0` — Otros síntomas
- `1` — Alteración del habla sin debilidad
- `2` — Debilidad unilateral

### Duración de los síntomas

`duracao`

- `0` — \< 10 min
- `1` — 10 a 59 min
- `2` — ≥ 60 min

### Diabetes

`dm`

## Edición del método

ABCD²/Johnston 2007: edad/PA/clínica/duración/diabetes, total 0–7

## Fórmula documentada

A edad ≥60: 1 · B presión ≥140/90: 1 · C clínica: debilidad unilateral 2, habla sin debilidad 1 · D duración: ≥60 min 2, 10 a 59 min 1 · Diabetes 1. Total 0 a 7.

## Límites y población

Puntuación pronóstica tras un diagnóstico de AIT, estudiada principalmente para el riesgo de ictus a 2 días, con análisis adicionales a 7 y 90 días. No confirma el diagnóstico de AIT. Las probabilidades observadas en las cohortes originales no representan una predicción individual universal.

## Referencias

- [Johnston SC et al. Validation and refinement of scores to predict very early stroke risk after transient ischaemic attack. Lancet, 2007.](https://doi.org/10.1016/S0140-6736(07)60150-0)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

La información siguiente conserva las salidas del método para ejemplos sintéticos. No constituye una validación clínica independiente.

### 1

Bajo riesgo: AVC en 2 días de 1,0%

7 días: 1,2% · 90 días: 3,1%.


### 2

Riesgo moderado: ACV en 2 días de 4,1%

7 días: 5,9% · 90 días: 9,8%.


### 3

Alto riesgo: ACV en 2 días de 8,1%

7 días: 11,7% · 90 días: 17,8%.

