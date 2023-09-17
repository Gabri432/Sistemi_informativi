## Progettazione DM/DW
- Rispetto alla progettazione di una base di dati operazionale, i dati da memorizzare hanno caratteristiche diverse.
- La progettazione è vincolata dalle basi di dati esistenti ma guidata da criteri progettuali diversi.
- Necessaria l'analisi delle sorgenti esistenti, l'integrazione e la progettazione concettuale, logica, fisica.
- Quindi i requisiti, le esigenze aziendali di analisi, la descrizione delle basi di dati aziendali (una documentazione), e la descrizione di altre sorgenti formative (possibile correlazione con dati esterni).

## Analisi delle sorgenti operazionali
- **Selezione delle sorgenti informative**, cioè l'analisi preliminare del patrimonio informativo aziendale e l'identificazione di priorità tra schemi.
- **Traduzione in un modello concettuale di riferimento**.
- **Analisi delle sorgenti informative (operazionali)**.

## Integrazione
- Attività di fusione dei dati rappresentati in più sorgenti in un'unica base di dati globale, rappresentante l'intero patrimonio informativo aziendale.
- Lo scopo è l'identificazione di tutte le porzioni delle diverse sorgenti formative che si riferiscono a uno stesso aspetto della realtà di interesse.
- Approccio orientato alla identificazione, analisi, risoluzione dei conflitti.

## Progettazione
- L'integrazione porta allo **schema riconciliato**, una descrizione globale del patrimonio informativo aziendale.
- Non descrive ancora tutti i dati di interesse per il DM.
- La progettazione **concettuale** porta a completare la rappresentazione dei concetti dimensionali necessari per l'analisi (es: dati storici e geografici).
- La progettazione **logica** porta alla implementazione con un modello logico, miglior compromesso tra necessità aggregare dati e normalizzarli.
- La progettazione **fisica** porta alla definizione di indici per ottimizzare le prestazioni.

## Ricognizione e normalizzazione
- La ricognizione è un esame approfondito degli schemi locali mirato alla piena comprensione del dominio applicativo.
- La normalizzazione è una correzione degli schemi locali al fine di modellare in modo più accurato il dominio applicativo.
- Si vuole inoltre individuare le eventuali porzioni di schemi non utili per futuro DW.

## Reverse engineering
- Attività di derivazione di uno schema concettuale a partire da uno schema logico.
- Svolto in modo semiautomatico dagli strumenti di progettazione CASE.

### [Conflitti](https://github.com/Gabri432/Sistemi_informativi/blob/master/capitolo_3b/conflitti.md)