# Libreria dei prompt per la PA (demo didattica)

Pagina web autonoma (`libreria-prompt-pa.html`) per compilare, organizzare e salvare le schede di una libreria di prompt. Si apre in un browser; non richiede installazione.

## Natura e limiti dell’artefatto

Questo artefatto è una **demo didattica**. Aiuta a organizzare, riutilizzare e controllare i prompt, ma:

- **non certifica la conformità normativa** né la sicurezza di uno strumento o di un prompt;
- **non autorizza strumenti di IA**: il campo «Strumento autorizzato» registra un’informazione inserita da chi compila la scheda, non un’autorizzazione;
- **non valida automaticamente gli output**: i controlli indicati nella scheda vanno eseguiti da una persona;
- **non sostituisce le regole dell’ente**, né il ruolo del RTD, dell’ICT, del DPO o del responsabile del procedimento, che restano i riferimenti per ogni decisione;
- **non deve ricevere dati reali o riservati**: usa solo dati fittizi o già pubblici. Non inserire dati personali, sanitari, giudiziari, riservati, documenti interni o informazioni relative a procedimenti reali.

Gli stati della scheda (Bozza, In revisione, Attivo, Archiviato) descrivono il punto in cui si trova il prompt nel lavoro di chi lo gestisce. Un prompt attivo può essere modificato o disattivato se cambiano fonti, strumenti, procedimenti o regole dell’ente.

## Dati e privacy

I dati restano nel browser, salvo quando si sceglie esplicitamente una funzione di salvataggio o un’integrazione esterna. Scaricare un file o copiarlo negli appunti lo salva sul dispositivo di chi usa la pagina. Attivando l’integrazione con Google Drive, i dati della libreria vengono trasferiti a Google e sono soggetti alle sue condizioni.

La pagina non contiene credenziali. Per usare Google Drive occorre inserire il Client ID OAuth fornito dall’amministratore dell’ente (campo «Impostazioni e guida» o costante `GOOGLE_CLIENT_ID` nello script).
