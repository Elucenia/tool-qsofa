<!-- ELUCENIA technical documentation · qsofa · it · no clinical/professional/rights approval -->

# qSOFA (SOFA rapido)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/qsofa)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Frequenza respiratoria ≥ 22 atti/min

`fr`

### Alterazione dello stato mentale (Glasgow \< 15)

`mental`

### Pressione sistolica ≤ 100 mmHg

`pas`

## Edizione del metodo

qSOFA/Sepsis-3/Seymour 2016: FR≥22/PAS≤100/alterazione mentale, 0–3; SSC 2021 non raccomanda screening isolato

## Formula documentata

Un punto per: frequenza respiratoria ≥ 22/min, alterazione mentale e sistolica ≤ 100 mmHg. Positivo con 2 o più punti.

## Limiti e popolazione

qSOFA 2016 è uno strumento di valutazione del rischio negli adulti con sospetta infezione, non una diagnosi né un test isolato per escludere la sepsi. Un punteggio basso non elimina il sospetto clinico. La SSC 2021 raccomanda di non usare qSOFA come unico strumento di screening; le indicazioni ufficiali SSC 2026 continuano a preferire altri strumenti per lo screening ospedaliero. La valutazione e il trattamento d’emergenza non devono attendere il punteggio. Questa soglia per adulti non stabilisce l’applicazione pediatrica.

## Riferimenti

- [Seymour CW et al. Assessment of clinical criteria for sepsis: for the Third International Consensus Definitions for Sepsis and Septic Shock (Sepsis-3). JAMA, 2016.](https://doi.org/10.1001/jama.2016.0288)

- [Singer M et al. The Third International Consensus Definitions for Sepsis and Septic Shock (Sepsis-3). JAMA, 2016.](https://doi.org/10.1001/jama.2016.0287)

- [Evans L et al. Surviving sepsis campaign: international guidelines for management of sepsis and septic shock 2021. Intensive Care Med, 2021.](https://doi.org/10.1007/s00134-021-06506-y)

- [SSC adult guidelines2021](https://www.sccm.org/clinical-resources/guidelines/guidelines/surviving-sepsis-guidelines-2021)

- [SSC adult guidelines2026, current official page as observed2026-10-03](https://www.sccm.org/survivingsepsiscampaign/guidelines-and-resources/surviving-sepsis-campaign-adult-guidelines)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
