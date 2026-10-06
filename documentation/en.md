<!-- ELUCENIA technical documentation · abcd2 · en · no clinical/professional/rights approval -->

# ABCD² score

[conditions, sources and permissions](https://elucenia.org/en/tools/abcd2)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Age ≥ 60 years

`idade`

### Blood pressure ≥ 140/90 mmHg at initial assessment

`pa`

### Clinical presentation

`clinica`

- `0` — Other symptoms
- `1` — Speech disturbance without weakness
- `2` — Unilateral weakness

### Symptom duration

`duracao`

- `0` — \< 10 min
- `1` — 10 to 59 min
- `2` — ≥ 60 min

### Diabetes

`dm`

## Method edition

ABCD²/Johnston 2007: age/BP/clinical features/duration/diabetes, total 0–7

## Documented formula

Age ≥60: 1 · Blood pressure ≥140/90: 1 · Clinical features: unilateral weakness 2, speech without weakness 1 · Duration: ≥60 min 2, 10 to 59 min 1 · Diabetes 1. Total 0 to 7.

## Limits and population

A prognostic score after a TIA diagnosis, studied primarily for 2-day stroke risk, with additional analyses at 7 and 90 days. It does not confirm a TIA diagnosis. Probabilities observed in the original cohorts are not a universal individual prediction.

## References

- [Johnston SC et al. Validation and refinement of scores to predict very early stroke risk after transient ischaemic attack. Lancet, 2007.](https://doi.org/10.1016/S0140-6736(07)60150-0)

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

## Documented results

The information below preserves the method outputs for synthetic examples. It does not constitute independent clinical validation.

### 1

Low risk: stroke in 2 days of 1.0%

7 days: 1,2% · 90 days: 3,1%.


### 2

Moderate risk: stroke in 2 days of 4,1%

7 days: 5,9% · 90 days: 9,8%.


### 3

High risk: stroke in 2 days of 8,1%

7 days: 11,7% · 90 days: 17,8%.

