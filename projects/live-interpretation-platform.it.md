# Vociamo

[English](live-interpretation-platform.md) | Italiano | [Tutti i progetti](../README.it.md)

Sottotitoli dal vivo e traduzione con l'AI per visite guidate, lezioni e
conferenze. Online su [vociamo.app](https://vociamo.app). Live Interpretation
Platform è il nome tecnico del repository.

## Descrizione

Nessuno resta fuori. In una visita guidata, a lezione o a una conferenza, chi non
sente legge quello che viene detto, chi non può parlare scrive le sue domande, e
chi parla un'altra lingua ascolta una voce tradotta o legge i sottotitoli nella
propria lingua.

Chi parla lo fa come sempre. Il pubblico inquadra un QR code, sceglie la lingua
e segue dal telefono, senza installare niente e senza registrarsi. Ogni lingua è
un unico canale condiviso, quindi il costo di un evento dipende dalle lingue
offerte e non da quante persone ci sono in sala.

## Funzionalità

- Tre tipi di evento: visita guidata, lezione e conferenza, ognuno con le sue
  parole e le sue impostazioni.
- Per il pubblico: voce tradotta o sottotitoli, le parole originali di chi
  parla, testo grande, alto contrasto e lettore di schermo, il testo completo da
  rileggere durante l'evento e da scaricare alla fine.
- Domande scritte e mano alzata, tradotte per chi parla.
- Conferenze con relatori ospiti invitati da un link personale, la parola che
  passa da un relatore all'altro e il nome di chi parla su ogni riga.
- Ventisei lingue, di cui ventitré verificate per chi parla, e la possibilità di
  passare da una lingua all'altra durante lo stesso intervento.
- La terminologia dell'evento, come i nomi dei luoghi e le parole tecniche,
  preparata prima perché venga riconosciuta, tradotta e pronunciata bene.
- Per l'organizzazione: collaboratori e ruoli, eventi preparati e condotti dal
  browser, registrazioni per le tappe di una visita, una voce per ogni lingua, il
  registro di quanto ha consumato ogni evento e un tetto alla spesa giornaliera.
- Pagina di presentazione, guide d'aiuto e testi legali in italiano e in
  inglese.

## Note tecniche

- Una catena in tempo reale di riconoscimento del parlato, traduzione e sintesi
  vocale, con più lingue in parallelo per tutta la durata dell'evento.
- I sottotitoli sono un modo di seguire l'evento a tutti gli effetti, progettati
  e provati per chi non sente, con controlli automatici di accessibilità su ogni
  pagina.
- Il servizio continua a funzionare quando un fornitore o un server si guasta:
  subentra un'altra strada o un'altra macchina, e il pubblico non deve
  ricollegarsi.
- La spesa è sotto controllo a tre livelli: il singolo evento, l'organizzazione
  e la piattaforma intera.
- Niente di quello che una macchina propone per la terminologia viene usato
  prima che una persona l'abbia approvato.
- Una lingua si dice verificata solo dopo essere stata misurata su registrazioni
  pubbliche di parlato.
- Ogni modifica al servizio online si controlla dal posto del pubblico, sul
  testo e sulla voce che arrivano davvero al telefono.
- I dati vengono elaborati in regioni europee, e le chiavi dei fornitori non
  arrivano mai al browser.

## Tecnologie

| Area | Strumenti |
| --- | --- |
| Linguaggio e strumenti | TypeScript, pnpm workspaces, Turborepo, ESLint, Playwright, GitHub Actions |
| Frontend | Next.js |
| Media in tempo reale | LiveKit, Node.js |
| Servizi di AI | Google Cloud Speech-to-Text, Cloud Translation e sintesi vocale, più servizi propri in Python |
| Dati | Supabase (Postgres, autenticazione, row level security) |
| Hosting | Vercel e un server virtuale a Francoforte |

## Stato

Online su [vociamo.app](https://vociamo.app): visite guidate, lezioni e
conferenze funzionano sul servizio ospitato. Prima del primo pilota con un
cliente resta una giornata di prove sui telefoni veri. Il codice è in un
repository privato, disponibile su richiesta.
