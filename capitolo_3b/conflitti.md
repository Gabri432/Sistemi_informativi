## Conflitti
- Problema centrale del processo di integrazione.
- Può causarsi da diversi livelli di astrazione, uso di costrutti diversi, specifiche incompatibili.
- Conflitti **terminologici** (sui nomi), **strutturali** (costrutti del modello), **semantici** (livello di astrazione della modellazione).

## Conflitti terminologici
- Omonimia, stesso nome ma significati diversi in sorgenti diverse (articolo->prezzo; prodotto->prezzo).
- Sinonimia, nomi diversi ma stesso significato in sorgenti diverse (articolo; prodotto).

## Conflitti strutturali
- Stesso concetto ma costrutti diversi in sorgenti diversi.
   - Stesso concetto ha identificatori diversi in sorgenti diverse (persona->CodiceFiscale; persona->ID).
   - Stessa proprietà espressa con costrutti diversi in sorgenti diverse (persona->nome; persona->nome,cognome).
   - Correlazione di due o più concetti con vincoli diversi in sorgenti diverse (impiegato->0:N progetti; impiegato->1:N progetti).

## Conflitti semantici
- Stessa porzione di mondo reale ma diversi livelli di astrazione/dettaglio in sorgenti diverse (cliente-azienda-città; cliente-città).


### [Risoluzione conflitti](https://github.com/Gabri432/Sistemi_informativi/blob/master/capitolo_3b/risoluzione_conflitti.md)