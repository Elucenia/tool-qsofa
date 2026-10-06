<!-- ELUCENIA technical documentation · qsofa · en · no clinical/professional/rights approval -->

# qSOFA (quick SOFA)

[conditions, sources and permissions](https://elucenia.org/en/tools/qsofa)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Respiratory rate ≥ 22 breaths/min

`fr`

### Altered mental status (Glasgow \< 15)

`mental`

### Systolic pressure ≤ 100 mmHg

`pas`

## Method edition

qSOFA/Sepsis-3/Seymour 2016: RR≥22/SBP≤100/altered mental status, 0–3; not recommended as sole screening by SSC 2021

## Documented formula

One point each: respiratory rate ≥ 22/min, altered mental status and systolic pressure ≤ 100 mmHg. Positive at 2 or more points.

## Limits and population

qSOFA 2016 is a risk-assessment tool for adults with suspected infection, not a diagnosis or a stand-alone test to rule out sepsis. A low score does not eliminate clinical suspicion. SSC 2021 recommends against qSOFA as the sole screening tool; official SSC 2026 guidance continues to favor other tools for hospital screening. Emergency assessment and treatment must not wait for the score. This adult threshold does not establish pediatric application.

## References

- [Seymour CW et al. Assessment of clinical criteria for sepsis: for the Third International Consensus Definitions for Sepsis and Septic Shock (Sepsis-3). JAMA, 2016.](https://doi.org/10.1001/jama.2016.0288)

- [Singer M et al. The Third International Consensus Definitions for Sepsis and Septic Shock (Sepsis-3). JAMA, 2016.](https://doi.org/10.1001/jama.2016.0287)

- [Evans L et al. Surviving sepsis campaign: international guidelines for management of sepsis and septic shock 2021. Intensive Care Med, 2021.](https://doi.org/10.1007/s00134-021-06506-y)

- [SSC adult guidelines2021](https://www.sccm.org/clinical-resources/guidelines/guidelines/surviving-sepsis-guidelines-2021)

- [SSC adult guidelines2026, current official page as observed2026-10-03](https://www.sccm.org/survivingsepsiscampaign/guidelines-and-resources/surviving-sepsis-campaign-adult-guidelines)

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

negative qSOFA (< 2)

Does not exclude sepsis: continue reassessing and calculate SOFA if organ dysfunction is suspected.


### 2

positive qSOFA (≥ 2): higher risk of in-hospital mortality

Investigate organ dysfunction (SOFA), start the sepsis bundle and consider ICU.


### 3

positive qSOFA (≥ 2): higher risk of in-hospital mortality

Investigate organ dysfunction (SOFA), start the sepsis bundle and consider ICU.

