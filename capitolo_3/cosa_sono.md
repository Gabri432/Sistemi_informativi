## Data Warehouse
- Collezione di dati di supporto per il processo decisionale.
- è orientata ai soggetti di interesse (chi lo usa), integrata e consistente, rappresentativa dell'evoluzione temporale, non volatile.
- **Integrata e consistente**, perchè si appoggia a più fonti di dati eterogenee, dati estratti dall'ambiente di produzione o anche dati provenienti da sistemi informativi esterni all'azienda. Ne mostra una versione unificata.
- **Rappresentativa dell'evoluzione temporale**, ricco contenuto storico, il tempo è parte delle chiavi.
- **Non volatile**, nessuna necessità di tecniche sofisticate di gestione delle transazioni, sono centrali il query-throughput e la resilienza.

## Tipi di elaborazione
### OLTP
- On-line Transaction Processing.
- Operazioni predefinite e relativamente semplici.
- Dati al dettaglio e aggiornati.
- Proprietà ACIDE (atomicità, consistenza, isolamento, durabilità) delle trasmissioni sono essenziali.

### OLAP
- On-line Analytical Processing.
- Operazioni complesse ed estemporanee.
- Dati storici e aggregati, non sempre attualissimi.
- Proprietà ACIDE non necessarie poichè le operazioni sono in sola lettura (query).

[Architetture Warehousing](https://github.com/Gabri432/Sistemi_informativi/blob/master/capitolo_3/architetture_warehousing.md)