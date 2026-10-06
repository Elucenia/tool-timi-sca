<!-- ELUCENIA technical documentation · timi-sca · it · no clinical/professional/rights approval -->

# Punteggio TIMI (SCA senza sopraslivellamento ST)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/timi-sca)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Età ≥ 65 anni

`idade`

### ≥ 3 fattori di rischio per malattia coronarica

`fr`

### Stenosi coronarica nota ≥ 50%

`dac`

### Uso di acido acetilsalicilico negli ultimi 7 giorni

`aas`

### ≥ 2 episodi di angina in 24 ore

`angina`

### Deviazione del ST ≥ 0,5 mm

`st`

### Marcatore di necrosi elevato

`marc`

## Edizione del metodo

TIMI UA/NSTEMI/Antman 2000: 7 fattori 0–1, totale 0–7; senza TIMI STEMI

## Formula documentata

Un punto per ogni item presente (totale da 0 a 7).

## Limiti e popolazione

Questa versione TIMI è stata sviluppata nell’angina instabile e nell’infarto senza sopraslivellamento ST per esiti compositi a 14 giorni; non è la versione TIMI per STEMI. I fattori hanno definizioni temporali e cliniche specifiche. I tassi degli studi storici non determinano il rischio individuale o il trattamento attuale senza la valutazione e la linea guida corrispondenti.

## Riferimenti

- [Antman EM et al. The TIMI risk score for unstable angina/non–ST elevation MI. JAMA, 2000.](https://doi.org/10.1001/jama.284.7.835)

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

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

Beneficio di una strategia invasiva precoce

| Dettagli del risultato | |
| --- | --- |
| Morte, IM o rivascolarizzazione urgente entro 14 giorni | 13,2% |


### 2

Beneficio di una strategia invasiva precoce

| Dettagli del risultato | |
| --- | --- |
| Morte, IM o rivascolarizzazione urgente entro 14 giorni | 26,2% |


### 3

Rischio basso

| Dettagli del risultato | |
| --- | --- |
| Morte, IM o rivascolarizzazione urgente entro 14 giorni | 4,7% |

