# Asta Fantacalcio

[English](asta-fantacalcio.md) | Italiano | [Tutti i progetti](../README.it.md)

Applicazione per gestire l'asta del fantacalcio, nelle modalità Classic e Mantra.

## Descrizione

La serata dell'asta è la più attesa della lega, ed è anche quella in cui un
errore costa di più: un conto sbagliato, un giocatore assegnato due volte, un
partecipante che resta senza crediti per completare la rosa. L'applicazione
tiene i conti mentre si rilancia, così al tavolo si pensa solo ai giocatori.

Crediti rimasti a ciascuno, posti ancora da riempire e crediti da tenere da parte
per quelli obbligatori sono sempre aggiornati, sullo schermo principale e sul
telefono di tutti. Funziona senza connessione a internet e può partire da una
chiavetta USB.

## Funzionalità

- Asta impostata con le regole della lega: budget, composizione della rosa e
  base d'asta.
- Rose flessibili, con un minimo e un massimo per ogni ruolo.
- Importazione del listone ufficiale da Excel.
- Una vista in sola lettura per i telefoni dei partecipanti.
- Ogni assegnazione si può annullare in qualsiasi momento della serata, e un
  giocatore che nessuno vuole si libera senza rallentare l'asta.
- Esportazione nel foglio che la lega usa già, con i totali per ruolo, i
  riepiloghi e i file CSV.
- Avvio con un doppio click, oppure da chiavetta USB su un computer senza
  Python.
- Guide per la serata, compreso come fare una copia di sicurezza a metà asta.

## Note tecniche

- I budget si ricavano sempre dagli acquisti registrati, quindi non possono
  scostarsi da quelli: era il difetto principale della versione precedente.
- La logica dell'asta è separata dall'interfaccia, e questo ha permesso di
  cambiare l'interfaccia senza riscrivere le regole.
- L'offerta massima mostrata su un telefono è sempre la stessa cifra che
  l'applicazione accetta.
- La composizione della rosa predefinita è stata ricostruita dai fogli delle
  stagioni passate.
- Provata con aste simulate dall'inizio alla fine, una delle quali fatta
  interamente dalla chiavetta USB.

## Tecnologie

| Area | Strumenti |
| --- | --- |
| Motore e API | Python, FastAPI |
| Dati | SQLite |
| Frontend | Next.js (TypeScript), Streamlit come ripiego |
| Importazione ed esportazione | pandas, openpyxl |
| Test | pytest con 310 test automatici, Playwright |

## Stato

Completa e provata con aste simulate. Il codice è in un repository privato,
disponibile su richiesta.
