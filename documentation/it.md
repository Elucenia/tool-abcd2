<!-- ELUCENIA technical documentation · abcd2 · it · no clinical/professional/rights approval -->

# Punteggio ABCD²

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/abcd2)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Età ≥ 60 anni

`idade`

### Pressione arteriosa ≥ 140/90 mmHg alla prima valutazione

`pa`

### Manifestazione clinica

`clinica`

- `0` — Altri sintomi
- `1` — Disturbo del linguaggio senza debolezza
- `2` — Debolezza unilaterale

### Durata dei sintomi

`duracao`

- `0` — \< 10 min
- `1` — 10 a 59 min
- `2` — ≥ 60 min

### Diabete

`dm`

## Edizione del metodo

ABCD²/Johnston 2007: età/pressione/clinica/durata/diabete, totale 0–7

## Formula documentata

A età ≥60: 1 · B pressione ≥140/90: 1 · C clinica: debolezza unilaterale 2, linguaggio senza debolezza 1 · D durata: ≥60 min 2, 10 a 59 min 1 · Diabete 1. Totale 0 a 7.

## Limiti e popolazione

Punteggio prognostico dopo una diagnosi di TIA, studiato principalmente per il rischio di ictus a 2 giorni, con analisi aggiuntive a 7 e 90 giorni. Non conferma la diagnosi di TIA. Le probabilità osservate nelle coorti originali non rappresentano una previsione individuale universale.

## Riferimenti

- [Johnston SC et al. Validation and refinement of scores to predict very early stroke risk after transient ischaemic attack. Lancet, 2007.](https://doi.org/10.1016/S0140-6736(07)60150-0)

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
