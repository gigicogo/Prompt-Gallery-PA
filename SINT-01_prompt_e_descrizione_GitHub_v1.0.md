# SINT-01 — Sintesi di circolari, leggi e atti

## Descrizione
Template didattico per ricavare una sintesi operativa di una circolare, una legge o un altro atto, usando Google Notebook / NotebookLM e il solo documento selezionato come fonte. La sintesi aiuta a individuare contenuti, obblighi, soggetti, scadenze e possibili ricadute per l’ufficio. Non sostituisce la lettura e la verifica del documento originale, né l’interpretazione o la valutazione di competenza dell’Ente.

## Classificazione
- **Codice:** SINT-01
- **Titolo:** Sintesi di circolari, leggi e atti
- **Categoria:** Analisi e sintesi documentale
- **Strumento previsto:** Google Notebook / NotebookLM, nell’ambiente autorizzato dall’Ente
- **Livello di attenzione:** Medio
- **Stato:** Bozza didattica
- **Versione:** v1.0
- **Owner:** [ufficio]

## Scopo
Predisporre una sintesi breve e operativa del documento selezionato, basata esclusivamente sui suoi contenuti. La sintesi deve aiutare il destinatario a orientarsi tra oggetto, ambito, obblighi, soggetti coinvolti, scadenze, possibili impatti per l’ufficio ed eventuali punti da verificare.

## Input richiesti
- [UFFICIO]
- [ENTE]
- [TIPO DOCUMENTO]
- [NUMERO/IDENTIFICATIVO]
- [TEMA]
- [DESTINATARIO]
- [SCOPO OPERATIVO]
- Documento originale da sintetizzare, completo e pertinente

## Fonti ammesse
Esclusivamente il documento originale selezionato nell’area Fonti del notebook. Non utilizzare altre fonti del notebook, fonti web o contenuti suggeriti dallo strumento.

## Output atteso
Una sintesi operativa di massimo una pagina, in tono amministrativo e con frasi brevi, che riporti gli elementi richiesti dal prompt. Le informazioni devono essere riconducibili al documento originale tramite citazioni o riferimenti ad articoli e paragrafi, quando disponibili. I contenuti assenti o incerti devono essere segnalati, senza completarli per deduzione.

## Controlli richiesti
- Verificare la sintesi confrontandola con il documento originale.
- Controllare che obblighi, soggetti e scadenze siano riportati correttamente e nel relativo contesto.
- Verificare citazioni, articoli e paragrafi indicati.
- Distinguere ciò che è esplicitamente presente nella fonte da ciò che richiede interpretazione o approfondimento.
- Approfondire eventuali rinvii, eccezioni o passaggi ambigui direttamente sulla fonte e, se necessario, con gli uffici competenti.

## Limiti d’uso
- Non considerare la sintesi sostitutiva del documento originale.
- Non usare la sintesi come interpretazione giuridica o come indicazione definitiva di adempimenti senza le verifiche previste dall’Ente.
- Non aggiungere informazioni, obblighi o scadenze non presenti nel documento.
- Non utilizzare fonti web, altre fonti del notebook o contenuti non autorizzati.
- Non includere dati personali non necessari.

## Convenzione di denominazione
`SINT-01_v1.0_YYYY-MM`

Esempio di file di lavoro: `tema_SINTESI_v0.1`, da adeguare alla convenzione documentale dell’Ente.

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
