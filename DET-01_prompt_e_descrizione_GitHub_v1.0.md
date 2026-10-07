# DET-01 — Bozza di determina

## Descrizione
Template didattico di prompt per predisporre una **bozza di determina** usando Google Notebook / NotebookLM con un insieme selezionato di fonti dell’Ente. Il modello può ordinare e redigere una prima bozza; non sostituisce l’istruttoria, la valutazione tecnico-amministrativa, la decisione o la validazione della persona competente.

## Classificazione
- **Codice:** DET-01
- **Titolo:** Bozza di determina
- **Categoria:** Redazione di atti — bozza
- **Strumento previsto:** Google Notebook / NotebookLM, nell’ambiente autorizzato dall’Ente
- **Livello di attenzione:** Alto
- **Stato:** Bozza didattica
- **Versione:** v1.0
- **Owner:** [ufficio]

## Scopo
Predisporre una prima bozza di determina conforme al format dell’Ente, basata esclusivamente su istruttoria, riferimenti normativi già verificati e fonti autorizzate.

## Input richiesti
- [UFFICIO]
- [ENTE]
- [OGGETTO]
- [RESPONSABILE/DESTINATARIO]
- [SCOPO DEL PROCEDIMENTO]
- Istruttoria o sintesi dei fatti
- Riferimenti normativi già verificati dall’ufficio
- Format ufficiale della determina
- Eventuali documenti ulteriori autorizzati

## Fonti ammesse
Solo le fonti selezionate nell’area Fonti del notebook, complete, aggiornate, pertinenti e autorizzate dall’ufficio.

## Output atteso
Una bozza con premesse, motivazione e dispositivo, corredata dai riferimenti alle fonti utilizzate e da un elenco finale degli elementi da verificare o completare.

## Controlli richiesti
- Riscontro tra fatti riportati nella bozza e istruttoria.
- Verifica di norme, articoli e commi sulle fonti ufficiali.
- Verifica di date, importi, termini e soggetti.
- Controllo della specificità della motivazione rispetto al caso concreto.
- Controllo di tono e format dell’Ente.
- Revisione e validazione secondo ruoli e procedimento applicabile.

## Limiti d’uso
- Non utilizzare fonti web, suggerite o non autorizzate.
- Non usare l’output come atto pronto per firma, adozione o trasmissione.
- Non delegare al modello giudizi tecnici, amministrativi o discrezionali.
- Non includere dati personali non necessari.

## Convenzione di denominazione
`DET-01_v1.0_YYYY-MM`

Esempio di file di lavoro: `oggetto_BOZZA_v0.1`, da adeguare alla convenzione documentale dell’Ente.

## Prompt

```text
DET-01 — Bozza di determina
Versione per Google Notebook / NotebookLM

PRIMA DI INIZIARE
Nell’area Fonti seleziona esclusivamente:
- l’istruttoria o la sintesi dei fatti;
- i riferimenti normativi già verificati dall’ufficio;
- il format ufficiale della determina dell’Ente;
- gli eventuali ulteriori documenti autorizzati.

Verifica che le fonti siano complete, aggiornate, pertinenti e autorizzate dall’ufficio.
Non utilizzare fonti web, fonti suggerite o altri documenti non autorizzati dall’ufficio.

CONTESTO
Lavori nell’ufficio [UFFICIO] dell’[ENTE].

Nell’area Fonti sono selezionati:
- l’istruttoria relativa a [OGGETTO];
- i riferimenti normativi verificati dall’ufficio;
- il format ufficiale della determina dell’Ente.

La bozza serve a [RESPONSABILE/DESTINATARIO] per [SCOPO DEL PROCEDIMENTO].

AZIONE
Prepara una BOZZA di determina sulla base esclusiva delle fonti selezionate nell’area Fonti.

Segui il format ufficiale dell’Ente e organizza il testo nelle sezioni:
1. premesse;
2. motivazione;
3. dispositivo.

VINCOLI
Usa esclusivamente i fatti contenuti nell’istruttoria e i riferimenti normativi presenti nelle fonti selezionate.

Non aggiungere norme, articoli, commi, date, importi, soggetti, motivazioni o circostanze non presenti nelle fonti.

Non utilizzare conoscenze esterne o fonti web.

Non formulare autonomamente il giudizio tecnico, amministrativo o discrezionale dell’ufficio.

Collega ogni passaggio della motivazione ai fatti documentati nell’istruttoria.

Evita formule generiche o motivazioni riutilizzabili indipendentemente dal caso concreto.

Se manca un dato necessario, scrivi: “[DA COMPLETARE]”.

Se una fonte presenta un’informazione ambigua, incompleta o incoerente, scrivi: “[DA VERIFICARE]”.

Non inserire dati personali non necessari alla bozza.

Per ogni riferimento normativo utilizzato indica la fonte e, se disponibile, l’articolo o il comma.

Applica le istruzioni di salvaguardia previste dall’Ente o dall’area di lavoro.

OUTPUT
Produci un testo completo, conforme al format selezionato, intestato:

“BOZZA — NON VALIDA FINO ALLA VALIDAZIONE DEL RESPONSABILE”.

La bozza deve contenere:
1. premesse basate esclusivamente sull’istruttoria;
2. motivazione collegata ai fatti documentati e ai riferimenti normativi forniti;
3. dispositivo coerente con l’oggetto e con l’istruttoria;
4. riferimenti alle fonti utilizzate;
5. elenco finale dei dati, passaggi o riferimenti da verificare o completare.

Non rimuovere la dicitura “BOZZA”.

La bozza non costituisce un atto, non sostituisce l’istruttoria e non può essere utilizzata per l’adozione, la firma o la trasmissione dell’atto senza la revisione e la validazione previste dal procedimento.
```
