<!-- ELUCENIA technical documentation · qsofa · es · no clinical/professional/rights approval -->

# qSOFA (SOFA rápido)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/qsofa)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Frecuencia respiratoria ≥ 22 respiraciones/min

`fr`

### Alteración del estado mental (Glasgow \< 15)

`mental`

### Presión sistólica ≤ 100 mmHg

`pas`

## Edición del método

qSOFA/Sepsis-3/Seymour 2016: FR≥22/PAS≤100/alteración mental, 0–3; SSC 2021 no recomienda cribado aislado

## Fórmula documentada

Un punto por: frecuencia respiratoria ≥ 22/min, alteración mental y presión sistólica ≤ 100 mmHg. Positivo con 2 o más.

## Límites y población

qSOFA 2016 es una herramienta de evaluación del riesgo en adultos con sospecha de infección, no un diagnóstico ni una prueba aislada para descartar sepsis. Una puntuación baja no elimina la sospecha clínica. La SSC 2021 recomienda no usar qSOFA como único instrumento de cribado; la orientación oficial SSC 2026 mantiene la preferencia por otros instrumentos de cribado hospitalario. La evaluación y el tratamiento de urgencia no deben esperar a la puntuación. Este umbral para adultos no establece la aplicación pediátrica.

## Referencias

- [Seymour CW et al. Assessment of clinical criteria for sepsis: for the Third International Consensus Definitions for Sepsis and Septic Shock (Sepsis-3). JAMA, 2016.](https://doi.org/10.1001/jama.2016.0288)

- [Singer M et al. The Third International Consensus Definitions for Sepsis and Septic Shock (Sepsis-3). JAMA, 2016.](https://doi.org/10.1001/jama.2016.0287)

- [Evans L et al. Surviving sepsis campaign: international guidelines for management of sepsis and septic shock 2021. Intensive Care Med, 2021.](https://doi.org/10.1007/s00134-021-06506-y)

- [SSC adult guidelines2021](https://www.sccm.org/clinical-resources/guidelines/guidelines/surviving-sepsis-guidelines-2021)

- [SSC adult guidelines2026, current official page as observed2026-10-03](https://www.sccm.org/survivingsepsiscampaign/guidelines-and-resources/surviving-sepsis-campaign-adult-guidelines)

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

qSOFA negativo (< 2)

No excluye sepsis: continúe reevaluando y calcule el SOFA si se sospecha disfunción orgánica.


### 2

qSOFA positivo (≥ 2): mayor riesgo de mortalidad hospitalaria

Investigar disfunción orgánica (SOFA), iniciar el paquete de sepsis y considerar UCI.


### 3

qSOFA positivo (≥ 2): mayor riesgo de mortalidad hospitalaria

Investigar disfunción orgánica (SOFA), iniciar el paquete de sepsis y considerar UCI.

