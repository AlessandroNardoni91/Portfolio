# Volontiamo

[English](volontiamo.md) | Italiano | [Tutti i progetti](../README.it.md)

Applicazione web per coordinare i volontari, online su
[volontiamo.org](https://volontiamo.org).

## Descrizione

Una sagra, una giornata di sport o una cena di beneficenza hanno bisogno delle
persone giuste al posto giusto e all'ora giusta. Volontiamo permette a
un'associazione di organizzare i suoi eventi, dividerli in attività e turni, e
vedere a colpo d'occhio quali turni sono coperti e dove manca ancora qualcuno.

I volontari danno la loro disponibilità e si iscrivono dal telefono, anche senza
account, da un link che l'associazione condivide. Promemoria e avvisi partono da
soli, e le risposte dei volontari arrivano all'organizzazione.

## Funzionalità

- Associazioni con i loro circoli, che condividono soci, ruoli e permessi.
- Eventi fatti di attività, e attività divise in turni.
- Disponibilità dei volontari e iscrizioni, anche da un link pubblico senza
  account.
- La copertura di ogni evento a colpo d'occhio: coperto, sufficiente o critico.
- Chiusura delle iscrizioni per un evento, un'attività o un singolo turno.
- Accesso su invito, con cinque ruoli e una pagina iniziale adatta a ciascuno.
- Email per gli inviti, per reimpostare la password, per il promemoria del
  giorno prima e per gli avvisi. Ogni organizzazione sceglie l'indirizzo a cui
  arrivano le risposte dei volontari.
- Ogni organizzazione ha il suo fuso orario, usato ovunque compaia una data.
- Un primo passo suggerito sullo schermo quando un'organizzazione non ha ancora
  eventi o un evento non ha attività.
- Pensata prima di tutto per il telefono, in italiano e in inglese britannico,
  con il supporto ai lettori di schermo.
- Identità visiva e immagini di anteprima per i social disegnate per il
  progetto.

## Note tecniche

- I permessi li fa rispettare il database stesso, non solo l'interfaccia, e chi
  non ha un account non arriva mai al database direttamente.
- Le regole su chi può gestire chi stanno in un solo posto, e ogni modifica
  viene provata con tutti i ruoli.
- I link per reimpostare la password funzionano anche con i programmi di posta
  che aprono i link in anticipo.
- Due operatori che agiscono nello stesso momento non mandano due volte la
  stessa email.
- Le azioni delicate vengono registrate in un registro di controllo.
- Il modulo pubblico è protetto dalle iscrizioni automatiche.
- Ogni modifica viene provata in automatico su un database temporaneo, e il
  database di produzione viene copiato ogni notte, cifrato.

## Tecnologie

| Area | Strumenti |
| --- | --- |
| Frontend | Next.js, React, TypeScript, Tailwind CSS, shadcn/ui |
| Backend e dati | Supabase (Postgres, autenticazione, row level security) |
| Lingue e validazione | next-intl, Zod |
| Infrastruttura | Vercel, Cloudflare, Resend, Sentry |
| Automazioni | Lavori pianificati nel database, GitHub Actions |

## Stato

Online su [volontiamo.org](https://volontiamo.org) e pronto per le prime
organizzazioni. Il codice è in un repository privato, disponibile su richiesta.
