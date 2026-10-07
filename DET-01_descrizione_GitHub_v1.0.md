<img width="1536" height="1024" alt="Designer 16 05 12" src="https://github.com/user-attachments/assets/f203bca6-ab89-43f3-900a-26d287c054fe" />

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
Vedere il file allegato `DET-01_prompt_Google_NotebookLM_v1.0.docx`.
