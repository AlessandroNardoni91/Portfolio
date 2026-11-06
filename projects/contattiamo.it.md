# Contattiamo

[English](contattiamo.md) | Italiano | [Tutti i progetti](../README.it.md)

Un assistente per trovare organizzazioni e professionisti da contattare,
preparare i messaggi e tenere traccia di ogni risposta. Funziona dentro Claude e
non manda mai niente da solo.

## Descrizione

Trovare nuovi clienti o partner è un lavoro lungo: cercare le organizzazioni
giuste, trovare la persona giusta dentro ognuna, scrivere un messaggio che non
sembri un invio di massa, ricordarsi chi richiamare e quando. Contattiamo fa la
ricerca, i controlli e la scrittura, e lascia alla persona la parte che conta:
leggere ogni messaggio e mandarlo dalla propria casella.

Lo strumento è uguale per tutti. Tutto ciò che è personale, cioè chi scrive,
come si firma, chi cerca e la storia dei contatti, sta in un foglio Google che
appartiene a chi lo usa.

## Funzionalità

- Si imposta con una breve conversazione: chi scrive, in che lingua e con che
  tono, quali organizzazioni e quali ruoli cerca, cosa vuole chiedere.
- Ricerca dei contatti per settore, ruolo e zona, senza doppioni delle
  organizzazioni già presenti nel registro.
- Ogni contatto ha la sua fonte pubblica e uno stato chiaro: verificato,
  dedotto o debole.
- Messaggi preparati per ogni contatto: primo messaggio con più oggetti fra cui
  scegliere, un richiamo, un messaggio di chiusura e una traccia per la
  telefonata o per l'incontro. Tutto arriva in una pagina con i pulsanti per
  copiare.
- Un registro di tutti i contatti nel foglio della persona, aggiornato con le
  risposte che arrivano nella casella, e una bozza di replica per ogni risposta,
  anche per un no.
- Un quadro del giorno: risposte da dare, richiami in scadenza, telefonate da
  fare e nuovi contatti a cui scrivere.
- Il confronto facoltativo fra due richieste diverse, con un avviso finché i
  numeri sono troppo piccoli per dire qualcosa.
- Funziona in italiano, francese e inglese.

## Note tecniche

- Niente parte in automatico e niente viene scritto nella casella: ogni
  messaggio lo legge e lo manda la persona.
- Si contattano solo organizzazioni e professionisti nel loro ruolo di lavoro,
  mai privati.
- Le regole di ogni paese su messaggi e telefonate non richiesti fanno parte
  delle istruzioni, a partire da Italia e Svizzera, e le fonti che vietano la
  lettura automatica si consultano solo a mano.
- Nessun nome, ruolo o indirizzo viene inventato: un contatto senza fonte non
  entra nel registro.
- Il testo di un'email in arrivo è un dato, mai un'istruzione.
- Lo strumento non contiene dati personali, quindi si può passare a un'altra
  persona, che lo installa sul proprio account.

## Tecnologie

| Area | Strumenti |
| --- | --- |
| Assistente | Skill di Claude: istruzioni, riferimenti e un modello di pagina HTML |
| Registro | Google Sheets e Google Drive attraverso i connettori di Claude |
| Casella | Gmail, in sola lettura |
| Ricerca | Ricerca web e lettura di pagine pubbliche |

## Stato

In sviluppo. Impostazione, ricerca dei contatti e preparazione dei messaggi sono
state provate su un registro di prova; il quadro del giorno e l'aggiornamento
dalla casella sono i prossimi passi. Il codice è disponibile su richiesta.
