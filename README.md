# 🗂️ Prompt Gallery PA — Libreria dei prompt per la Pubblica Amministrazione

**Prompt Gallery PA** è una web app didattica per compilare, organizzare, riutilizzare e controllare le schede di una libreria di prompt destinati alla Pubblica Amministrazione.

L’app aiuta a trasformare i prompt da testi dispersi in risorse documentate: ogni scheda può descrivere scopo, input, fonti ammesse, output atteso, controlli e limiti d’uso.

## 🎯 A chi è rivolto

La libreria è pensata per:

- funzionari ed esecutori della Pubblica Amministrazione;
- uffici che vogliono standardizzare l’uso dei prompt;
- referenti ICT, formazione e trasformazione digitale;
- responsabili di procedimento e figure di controllo;
- formatori e docenti che vogliono insegnare un uso tracciabile dell’AI generativa.

## 🧠 L’idea

Un prompt efficace non è solo una frase da copiare in una chat: è uno strumento di lavoro che dovrebbe dichiarare:

- a cosa serve;
- quali informazioni richiede;
- quali fonti può utilizzare;
- quale output deve produrre;
- quali controlli richiede;
- quali limiti e rischi comporta.

**Prompt Gallery PA** offre una struttura comune per raccogliere queste informazioni e rendere i prompt più facili da riusare, revisionare e governare.

## 🕹️ Come funziona

L’app permette di:

- creare schede di prompt;
- classificarle per categoria, strumento, livello di attenzione e stato;
- registrare input, fonti ammesse, output atteso e controlli richiesti;
- salvare, cercare e riorganizzare le schede;
- esportare o copiare le schede sul proprio dispositivo;
- collegare facoltativamente la libreria a Google Drive.

Ogni scheda può assumere uno di questi stati:

| Stato | Significato |
|---|---|
| **Bozza** | La scheda è in fase di predisposizione. |
| **In revisione** | La scheda è in fase di verifica o aggiornamento. |
| **Attivo** | La scheda è disponibile per l’uso, nei limiti indicati. |
| **Archiviato** | La scheda non è più utilizzata, ma resta come riferimento. |

Un prompt attivo può essere modificato o disattivato se cambiano fonti, strumenti, procedimenti o regole dell’ente.

## 📄 Prompt inclusi

Il repository include due schede didattiche pronte per essere studiate, adattate e riutilizzate.

| Codice | Titolo | Categoria | Livello di attenzione |
|---|---|---|---|
| [`DET-01`](DET-01_prompt_e_descrizione_GitHub_v1.0.md) | Bozza di determina | Redazione di atti — bozza | Alto |
| [`SINT-01`](SINT-01_prompt_e_descrizione_GitHub_v1.0.md) | Sintesi di circolari, leggi e atti | Analisi e sintesi documentale | Medio |

### DET-01 — Bozza di determina

Il prompt `DET-01` aiuta a predisporre una prima bozza di determina usando Google Notebook / NotebookLM con un insieme selezionato di fonti dell’ente.

L’output atteso include:

- premesse basate sull’istruttoria;
- motivazione collegata ai fatti documentati;
- dispositivo coerente con l’oggetto;
- riferimenti alle fonti utilizzate;
- elenco finale degli elementi da verificare o completare.

La bozza è intestata:

> **BOZZA — NON VALIDA FINO ALLA VALIDAZIONE DEL RESPONSABILE**

### SINT-01 — Sintesi di circolari, leggi e atti

Il prompt `SINT-01` aiuta a ricavare una sintesi operativa da una circolare, una legge o un altro atto, usando esclusivamente il documento selezionato come fonte.

L’output atteso include:

- oggetto e ambito del documento;
- obblighi principali;
- soggetti coinvolti;
- scadenze;
- possibili impatti per l’ufficio;
- punti ambigui, eccezioni o rinvii.

La sintesi è intestata:

> **BOZZA — DA VERIFICARE SULLA FONTE ORIGINALE**

## 🧩 Struttura di una scheda

Ogni scheda di prompt può contenere:

| Campo | A cosa serve |
|---|---|
| Codice | Identificare il prompt in modo univoco. |
| Titolo | Descrivere sinteticamente la funzione. |
| Categoria | Raggruppare i prompt per tipo di attività. |
| Strumento previsto | Indicare l’ambiente o il servizio previsto per l’uso. |
| Livello di attenzione | Segnalare il grado di cautela richiesto. |
| Stato | Descrivere il ciclo di vita della scheda. |
| Owner | Indicare l’ufficio o il responsabile del riferimento. |
| Scopo | Definire l’obiettivo concreto del prompt. |
| Input richiesti | Elencare informazioni e documenti necessari. |
| Fonti ammesse | Delimitare le fonti utilizzabili. |
| Output atteso | Descrivere il risultato da ottenere. |
| Controlli richiesti | Indicare le verifiche umane necessarie. |
| Limiti d’uso | Precisare cosa non fare. |
| Convenzione di denominazione | Standardizzare i file di lavoro. |
| Prompt | Contenere il testo completo da utilizzare. |

## 💻 Come usare l’app

L’app è una **pagina web autonoma**: si apre nel browser e non richiede installazione.

### Avvio locale

1. Scarica o clona il repository.
2. Apri `index.html` con un browser moderno.
3. Crea o importa le schede della libreria.
4. Compila i campi e salva il lavoro secondo le funzioni disponibili.

### Clonare il repository

```bash
git clone [https://github.com/gigicogo/Prompt-Gallery-PA.git](https://github.com/gigicogo/Prompt-Gallery-PA.git)
cd Prompt-Gallery-PA
```

## 🔐 Dati e privacy

I dati restano nel browser, salvo quando si sceglie esplicitamente una funzione di salvataggio o un’integrazione esterna.

- Scaricare un file o copiarlo negli appunti lo salva sul dispositivo di chi usa la pagina.
- Attivando l’integrazione con Google Drive, i dati della libreria vengono trasferiti a Google e sono soggetti alle sue condizioni.
- La pagina non contiene credenziali.
- Per usare Google Drive occorre inserire il Client ID OAuth fornito dall’amministratore dell’ente, tramite il campo «Impostazioni e guida» oppure la costante `GOOGLE_CLIENT_ID` nello script.

## ⚠️ Natura e limiti della soluzione

Questa è una **demo didattica**. Aiuta a organizzare, riutilizzare e controllare i prompt, ma:

- non certifica la conformità normativa né la sicurezza di uno strumento o di un prompt;
- non autorizza strumenti di IA: il campo «Strumento autorizzato» registra un’informazione inserita da chi compila la scheda, non un’autorizzazione;
- non valida automaticamente gli output: i controlli indicati nella scheda vanno eseguiti da una persona;
- non sostituisce le regole dell’ente, né il ruolo del RTD, dell’ICT, del DPO o del responsabile del procedimento;
- non deve ricevere dati reali o riservati.

Non inserire dati personali, sanitari, giudiziari, riservati, documenti interni o informazioni relative a procedimenti reali. Usa soltanto dati fittizi o già pubblici.

## 🧪 Possibili evoluzioni

- Aggiunta di nuove schede per comunicazioni, FAQ, verbali, report e analisi documentale.
- Filtri e ricerca avanzata nella libreria.
- Versione multiutente con ruoli e permessi.
- Integrazioni aggiuntive con ambienti documentali autorizzati.
- Esportazione in formati standardizzati.
- Versione inglese dell’interfaccia.
- Raccolta di casi d’uso reali, resi anonimi.

## 🤝 Contribuire

Sono benvenuti suggerimenti su nuove schede, miglioramenti dell’interfaccia, correzioni e materiali didattici.

1. Apri una Issue per proporre un nuovo prompt o segnalare un problema.
2. Oppure apri una Pull Request con una nuova scheda o una modifica.
3. Mantieni la struttura comune delle schede: scopo, input, fonti, output, controlli e limiti.

---

## 📄 Licenza

Da definire: si suggerisce una licenza aperta (es. MIT o CC BY 4.0) per favorire il riuso da parte di altri formatori o altri enti. Sostituisci questo paragrafo con il testo della licenza scelta e il file `LICENSE` del repo.

## 👤 Autore e contesto

**Gianluigi Cogo**  
Content creator e technical writer interessato ad AI generativa, automazioni, viaggi e strumenti digitali. Consulente e docente sui temi dell’IA generativa nella Pubblica Amministrazione.

L’app nasce come esercitazione nel percorso operativo **“L’IA nella Pubblica Amministrazione — Percorso operativo per l’uso consapevole, sicuro e governato dell’IA generativa”** (20 ore: percorso base per funzionari ed esecutori + modulo governance per direttori e dirigenti). Per info sul corso contattami usando i social qui sotto.

- 📮 **Newsletter:** [gigicogo.substack.com](https://gigicogo.substack.com)
- 📝 **Blog:** [medium.com/webeconoscenza](https://medium.com/webeconoscenza)
- ▶️ **YouTube:** [youtube.com/@gigicogo](https://youtube.com/@gigicogo)
- 💼 **LinkedIn:** [linkedin.com/in/gigicogo](https://www.linkedin.com/in/gigicogo)
