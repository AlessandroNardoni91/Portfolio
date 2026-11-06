# Torre degli Agli

[English](torre-degli-agli.md) | Italiano | [Tutti i progetti](../README.it.md)

Guida per gli ospiti di un appartamento a Firenze, che si apre da un QR code in
casa. Online su
[alessandronardoni91.github.io/torre-degli-agli](https://alessandronardoni91.github.io/torre-degli-agli/).

## Descrizione

Chi arriva in una città che non conosce ha sempre le stesse domande: come entro,
come si accende il forno, quale autobus va in centro, dove mangiamo stasera. Al
posto della cartellina sul tavolo o di un lungo messaggio, in casa c'è un QR
code. Basta inquadrarlo per aprire una guida nella propria lingua, fatta per un
telefono tenuto in una mano.

La guida è in inglese, italiano, spagnolo e francese, e si apre direttamente
nella lingua del telefono.

## Funzionalità

- Arrivo e check-in autonomo spiegati passo per passo, con gli screenshot.
- Regole della casa, mezzi pubblici, ristoranti e passeggiate nei dintorni.
- Una pagina per ogni elettrodomestico, con le immagini dei comandi e dei tasti
  citati nel testo, e i manuali originali da scaricare.
- Una galleria di foto dell'appartamento.
- La lingua si sceglie da un menu con le bandierine e resta la stessa da una
  pagina all'altra.
- Pagine leggere, che si caricano in fretta anche con la rete del telefono.
- Non compare sui motori di ricerca: la guida è per chi ha il QR code.

## Note tecniche

- Un sito statico semplice, senza framework e senza compilazione: modificare
  una pagina vuol dire modificare un file, e pubblicarla è un push.
- Le quattro lingue di una pagina stanno nello stesso file, quindi non possono
  allontanarsi fra loro.
- Prima di ogni pubblicazione gira un controllo automatico: stesso contenuto in
  tutte le lingue, nessun link rotto e nessuna immagine mancante, il peso di
  ogni pagina, e nessuno dei dati riservati del proprietario.
- La riservatezza fa parte del progetto: l'indirizzo esatto e i numeri di
  telefono del proprietario non compaiono mai, nemmeno negli screenshot delle
  mappe.

## Tecnologie

| Area | Strumenti |
| --- | --- |
| Sito | HTML, CSS e JavaScript, senza dipendenze |
| Pubblicazione | GitHub Pages |
| Controlli | Python |

## Stato

Online, e il QR code dell'appartamento porta qui. Il codice è pubblico su
[github.com/AlessandroNardoni91/torre-degli-agli](https://github.com/AlessandroNardoni91/torre-degli-agli).
