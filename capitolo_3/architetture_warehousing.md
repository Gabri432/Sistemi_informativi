## Architettura per il data warehousing
- Sorgenti dati operazionali.
- Monitoraggio e amministrazione.
- Data Mart.
- Strumenti di analisi.

## Sorgenti dati operazionali
- Interne o esterne, in generale eterogenee.
- Database relazionali, dati semistrutturati (es XML), pagine web, dati testuali, dati "social".
- Processo di costruzione DW complesso e richiede l'estrazione, trasformazione e integrazione dei dati operazionali.

## Architettura a 1 livello
- Scarsamente utilizzata nella pratica, non rispetta separazione tra OLTP e OLAP.
- DW generato da un software middleware.

## Architettura a 2 livelli
- Data Mart 
   - Un sottoinsieme o aggregazione dei dati presenti nel DW primario. Contiene informazioni rilevanti per una particolare area del business.

- ETL (Extraction, Transformation, Loading)
   - Strumenti per l'integrazione dei dati in una versione singola, dettagliata ed esauriente, che a sua volta alimenti il DW.
   - La riconciliazione avviene al primo popolamento del DW, e periodicamente ad ogni aggiormanento.

- I data mart **dipendenti** sono quelli alimentati dal DW primario.
   - Sono utili come blocchi costruttivi durante la realizzazione incrementale del DW, poichè delineano i contorni delle informazioni necessarie a un particolare tipo di utenti.
   - hanno prestazioni migliori data la loro dimensione inferiore.

- I data mart **indipendenti** alimentati da altre sorgenti.
   - Snellimento delle fasi progettuali.
   - Presenza di uno schema complesso di accesso ai dati.
   - Possibile rischio di inconsistenza tra i data mart.

### Vantaggi
- Disponibilità continua di informazione di buona qualità anche in caso di preclusione temporanea dell'accesso alle sorgenti.
- Nessuna interferenza con la gestione delle transizioni a livello operazionale durante interrogazione analitica effettuata su DW.
- Organizzazione logica DW su modello multidimensionale. Sorgenti su modelli relazionali o semi-strutturati.
- Discordanza temporale e di granularità tra sistemi OLTP e OLAP.
- Possibilità a livello di DW di impiegare tecniche per ottimizzare prestazione per applicazioni e reportistica.

## Architettura a 3 livelli
- Livello dei dati riconcilliati, dati operazionali ottenuti a valle del processo di integrazione e ripulitura dei dati sorgente. Quindi dati volatili, corretti e dettagliati.

### Vantaggi
- Creazione di un modello di dati comune e di riferimento per l'intera azienda.
- Separazione netta tra problematiche legate a estrazione e integrazione dati dalle sorgenti e quelle inerenti all'alimentazione del DW.
- Ulteriore rindondanza ai dati operazionali sorgente.

### [Modello Multidimensionale](https://github.com/Gabri432/Sistemi_informativi/blob/master/capitolo_3/modello_multidimensionale.md)

