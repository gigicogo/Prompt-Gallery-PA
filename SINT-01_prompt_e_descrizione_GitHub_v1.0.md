# SINT-01 — Sintesi di circolari, leggi e atti

## Descrizione
Template didattico di prompt per predisporre una **sintesi di circolare** usando Google Notebook / NotebookLM con un insieme selezionato di fonti dell’Ente. Il modello può ordinare e redigere una prima bozza; non sostituisce l’istruttoria, la valutazione tecnico-amministrativa, la decisione o la validazione della persona competente.

## Classificazione
- **Codice:** SINT-01
- **Titolo:** Sintesi di circolare
- **Categoria:** Redazione di atti — bozza
- **Strumento previsto:** Google Notebook / NotebookLM, nell’ambiente autorizzato dall’Ente
- **Livello di attenzione:** Medio
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
`SINT-01_v1.0_YYYY-MM`

Esempio di file di lavoro: `oggetto_BOZZA_v0.1`, da adeguare alla convenzione documentale dell’Ente.

## Prompt

```text
PRIMA DI INIZIARE
Nell’area Fonti, seleziona esclusivamente il documento da sintetizzare. Verifica che la fonte selezionata sia completa, aggiornata e pertinente al compito.
Non utilizzare altre fonti web, fonti suggerite o altri documenti presenti nel Notebook.

CONTESTO
Lavori nell’ufficio [UFFICIO] dell’[ENTE].

Nell’area Fonti è selezionato [TIPO DOCUMENTO] n. [NUMERO/IDENTIFICATIVO], relativo a [TEMA].
La sintesi serve a [DESTINATARIO]per [SCOPO OPERATIVO].

AZIONE
Prepara una sintesi operativa basata esclusivamente sul documento selezionato nell’area Fonti.

VINCOLI
Usa soltanto le informazioni contenute nella fonte selezionata.
Non integrare la risposta con conoscenze esterne, fonti web, altre fonti del Notebook o interpretazioni non esplicitamente contenute nel documento.
 Non aggiungere norme, date, obblighi, soggetti, importi o riferimenti non presenti nella fonte.
Se un’informazione non è presente nella fonte, scrivi: “NON PRESENTE NELLA FONTE”.
Se un passaggio è ambiguo, incompleto o richiede un controllo, segnalalo come: “[DA VERIFICARE]”. 
Per ogni affermazione rilevante, inserisci la citazione 'generata da Google Notebook' e indica, se disponibile,l’articolo o il paragrafo del documento.

Applica le istruzioni di salvaguardia presenti nelle fonti.
OUTPUT
Produci una BOZZA di massimo una pagina, in tono amministrativo e con frasi brevi.

La bozza deve contenere:
1. Oggetto e ambito del documento.
2. Obblighi principali.
3. Soggetti coinvolti.
4. Scadenze, in una tabella con le colonne:
   obbligo | soggetto | scadenza | articolo/paragrafo | citazione.

5. Possibili impatti per l’ufficio [UFFICIO],
   limitatamente a quanto ricavabile dalla fonte selezionata.

6. Punti ambigui, eccezioni o rinvii ad altri atti o documenti.

Concludi con la dicitura: “BOZZA — DA VERIFICARE SULLA FONTE ORIGINALE”.
