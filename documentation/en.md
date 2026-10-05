<!-- ELUCENIA technical documentation · timi-sca · en · no clinical/professional/rights approval -->

# TIMI score (non-ST-elevation ACS)

[conditions, sources and permissions](https://elucenia.org/en/tools/timi-sca)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Age ≥ 65 years

`idade`

### ≥ 3 risk factors for coronary artery disease

`fr`

### Known coronary stenosis ≥ 50%

`dac`

### Aspirin use in the last 7 days

`aas`

### ≥ 2 angina episodes in 24 hours

`angina`

### ST deviation ≥ 0.5 mm

`st`

### Elevated necrosis marker

`marc`

## Method edition

TIMI UA/NSTEMI/Antman 2000: 7 factors 0–1, total 0–7; excludes TIMI STEMI

## Documented formula

One point per present item (total 0 to 7).

## Limits and population

This TIMI version was developed in unstable angina and non-ST-elevation infarction for 14-day composite outcomes; it is not the TIMI version for STEMI. The factors have specific temporal and clinical definitions. Rates from historical trials do not determine individual risk or current treatment without corresponding assessment and guidelines.

## References

- [Antman EM et al. The TIMI risk score for unstable angina/non–ST elevation MI. JAMA, 2000.](https://doi.org/10.1001/jama.284.7.835)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
