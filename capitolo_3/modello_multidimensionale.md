## Modello multidimensionale
- **Fatto**, le occorrenze dei fatti corrispondono ad eventi accaduti (es: vendita, telefonata, ricovero).
- **Misura**, proprietà numerica di un fatto da analizzare che descrive quantitativamente il fatto da diversi punti di vista (es: quantità venduta, incasso, costo, durata).
- **Dimensione**, prospettiva lungo la quale fare l'analisi (es: prodotto, tempo, reparto, paziente).
- I dati multidimensionali sono rappresentati in cubi:
   - ogni cella è un evento (fatto) e contiene un valore per ogni misura;
   - ongi asse rappresenta una dimensione di interesse per analisi.
- Le dimensioni sono organizzate in gerarchie che rappresentano i possibili livelli di aggregazione (**attributi dimensionali**) per i dati.

## Tecniche di base per analisi automatica del DW
- Restrizione
   - Ritagliare porzione di cubo circoscrivendo il campo di analisi. Riduzione della dimensionalità del cubo fissando uno o più valori per le dimensioni.
- Aggregazione
   - Raggruppamento degli eventi nel cubo in macro-celle formate da celle correlate sfruttando i livelli gerarchici delle dimensioni.

## Accesso al DW
### Reportistica
- Orientato agli utenti che hanno necessità di accedere, a intervalli di tempo predefiniti, a informazioni strutturate, in modo pressochè invariabile;
- **Interrogazione**, quindi selezione e aggregazione di dati multidimensionali;
- **Presentazione**, in formato tabellare o grafico di risultato dell'interrogazione.
- Report generati su richiesta o automaticamente distribuiti.

### OLAP
- Agli utenti le cui necessità non sono facilmente identificabili a priori viene consentito di analizzare ed esplorare interattivamente i dati sulla base del modello multidimensionale;
- Costruzione attiva di sessione di analisi dei risultati ottenuti al passo precedente;
- Estemporaneità delle sessioni di lavoro;
- Richiesta approfondita conoscenza dei dati;
- Orientamento verso utenti non esperti di informatica;
- Risultati visualizzati tramite tabelle, istogrammi, grafici, torte, ecc...;
-

#### Operazioni su dati multidimensionali
- **Roll-up**, aggregazione dei dati.
- **Drill-down**, disaggrega i dati.
- **Slice and dice**, seleziona e proietta.
- **Pivot**, riorientazione del cubo.

### [Data Mining](https://github.com/Gabri432/Sistemi_informativi/blob/master/capitolo_3/data_mining.md)