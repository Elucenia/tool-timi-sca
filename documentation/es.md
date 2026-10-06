<!-- ELUCENIA technical documentation · timi-sca · es · no clinical/professional/rights approval -->

# Puntuación TIMI (SCA sin elevación del ST)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/timi-sca)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Edad ≥ 65 años

`idade`

### ≥ 3 factores de riesgo de enfermedad coronaria

`fr`

### Estenosis coronaria conocida ≥ 50%

`dac`

### Uso de ácido acetilsalicílico en los últimos 7 días

`aas`

### ≥ 2 episodios de angina en 24 horas

`angina`

### Desviación del ST ≥ 0,5 mm

`st`

### Marcador de necrosis elevado

`marc`

## Edición del método

TIMI UA/NSTEMI/Antman 2000: 7 factores 0–1, total 0–7; no TIMI STEMI

## Fórmula documentada

Un punto por cada ítem presente (total de 0 a 7).

## Límites y población

Esta versión TIMI se desarrolló en angina inestable e infarto sin elevación del ST para desenlaces compuestos a 14 días; no es la versión TIMI para STEMI. Los factores tienen definiciones temporales y clínicas específicas. Las tasas de los ensayos históricos no determinan el riesgo individual ni el tratamiento actual sin la evaluación y la guía correspondientes.

## Referencias

- [Antman EM et al. The TIMI risk score for unstable angina/non–ST elevation MI. JAMA, 2000.](https://doi.org/10.1001/jama.284.7.835)

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

Beneficio de una estrategia invasiva precoz

| Detalles del resultado | |
| --- | --- |
| Muerte, IAM o revascularización urgente en 14 días | 13,2% |


### 2

Beneficio de una estrategia invasiva precoz

| Detalles del resultado | |
| --- | --- |
| Muerte, IAM o revascularización urgente en 14 días | 26,2% |


### 3

Riesgo bajo

| Detalles del resultado | |
| --- | --- |
| Muerte, IAM o revascularización urgente en 14 días | 4,7% |

