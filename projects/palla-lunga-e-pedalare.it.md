# Palla Lunga e Pedalare

[English](palla-lunga-e-pedalare.md) | Italiano | [Tutti i progetti](../README.it.md)

Pagina Instagram sui giocatori della Serie A, con post preparati dall'AI e
approvati da una persona. Online su
[instagram.com/pallalungaepedalare](https://www.instagram.com/pallalungaepedalare/).

## Descrizione

Una pagina di calcio vive di costanza: un post nuovo ogni giorno, con fatti veri
e un'opinione su cui discutere. Palla Lunga e Pedalare è portata avanti da una
redazione automatica che fa il lavoro pesante, dalla ricerca alla grafica
finita, e lascia a una persona una sola decisione: approvare il post dal
telefono, rispondendo a un'email.

I post parlano di giocatori, non di squadre: classifiche per ruolo, duelli alla
vigilia delle partite importanti, la squadra della giornata, griglie a tema e
giochi a indovinello. Su Instagram ogni post è segnalato come contenuto generato
con l'AI.

## Funzionalità

- Diversi formati fissi: classifiche a puntate, duelli con il verdetto lasciato
  ai lettori, la squadra della giornata ricavata dai voti, griglie di otto
  giocatori su un tema, caroselli di indizi per indovinare un giocatore e le
  reazioni esagerate della settimana.
- Grafiche prodotte in automatico da modelli, con l'identità visiva della
  pagina: logo, colori e caratteri.
- Ogni post ha la sua scheda dei fatti, raccolti da risultati, voti e notizie
  della settimana.
- Approvazione via email: il post arriva con la grafica e la didascalia, e con
  una risposta lo si approva, si chiede di rifarlo con una nota o lo si scarta.
- Uscita programmata ogni giorno alla stessa ora, anche a computer spento.
- Se per quel giorno non c'è niente di approvato, esce un post di riserva invece
  di una serata vuota.
- Un redattore che lavora nel cloud prepara ogni mattina i post successivi e
  applica da solo le modifiche richieste.

## Note tecniche

- L'approvazione vale per una versione precisa del post: se cambiano la grafica
  o il testo, va approvato di nuovo.
- Prima di ogni approvazione gira un controllo automatico di qualità: i numeri
  della grafica confrontati con la scheda dei fatti, quanto sono recenti i dati,
  la maglia del giocatore che deve essere quella della squadra di oggi,
  l'impaginazione della grafica.
- Le didascalie seguono regole di scrittura messe per iscritto, e un controllo
  respinge quelle che sembrano scritte da una macchina.
- Le classifiche seguono un metodo scritto che tiene insieme le statistiche e il
  giudizio di chi il calcio lo guarda.
- Tutto gira su servizi gratuiti.

## Tecnologie

| Area | Strumenti |
| --- | --- |
| Redazione automatica | Python |
| Grafiche | Modelli HTML, Jinja2, Playwright |
| Pubblicazione | Instagram Graph API |
| Approvazione e programmazione | GitHub Issues e GitHub Actions, email |
| Redattore nel cloud | Routine programmate di Claude Code |

## Stato

Online da settembre 2026, con un post al giorno. Il codice della redazione è in
un repository privato, disponibile su richiesta.
