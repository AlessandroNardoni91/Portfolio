# Vociamo

English | [Italiano](live-interpretation-platform.it.md) | [All projects](../README.md)

Live captions and AI translation for guided tours, lectures and conferences.
Online at [vociamo.app](https://vociamo.app). Live Interpretation Platform is the
technical name of the repository.

## Description

No one is left out. At a tour, a lesson or a conference, the people who cannot
hear read what is being said, the people who cannot speak write their questions,
and the people who speak another language listen to a translated voice or read
captions in their own language.

The speaker talks as usual. The audience scans a QR code, picks a language and
follows on their phone, with no app to install and no account. Each language is
one shared channel, so the cost of an event depends on the languages offered,
not on the number of people in the room.

## Features

- Three kinds of event: guided tour, lecture and conference, each with its own
  words and settings.
- For the audience: translated voice or captions, the speaker's original words,
  large text, high contrast and screen reader support, the whole text to read
  back during the event and to download afterwards.
- Written questions and a raised hand, translated for the speaker.
- Conferences with guest speakers invited by a personal link, the floor passed
  from one speaker to the next, and the name of whoever is speaking on every
  line.
- Twenty-six languages, twenty-three of them verified for the speaker, and a
  speaker can switch between two languages during the same talk.
- Terminology of the event, such as place names and technical words, prepared
  in advance so that it is recognised, translated and pronounced correctly.
- For the organisation: colleagues and roles, events prepared and run from the
  browser, recordings for the stops of a tour, a voice for each language, a
  record of what each event consumed, and limits on daily spending.
- Presentation page, help guides and legal texts in Italian and English.

## Technical notes

- A real-time chain of speech recognition, translation and speech synthesis,
  running several languages in parallel for a whole event.
- Captions are a way of following the event in their own right, designed and
  tested for people who cannot hear, with automatic accessibility checks on
  every page.
- The service keeps running when a provider or a server fails: another route or
  another machine takes over, and the audience does not have to reconnect.
- Spending is under control at three levels: the single event, the organisation
  and the whole platform.
- Nothing a machine proposes for the terminology is used until a person has
  approved it.
- A language is called verified only after it has been measured on public
  recordings of speech.
- Every change to the live service is checked from where the audience sits, on
  the text and the voice that actually reach a phone.
- Data is processed in European regions, and the providers' keys never reach
  the browser.

## Technologies

| Area | Tools |
| --- | --- |
| Language and tooling | TypeScript, pnpm workspaces, Turborepo, ESLint, Playwright, GitHub Actions |
| Frontend | Next.js |
| Realtime media | LiveKit, Node.js |
| AI services | Google Cloud Speech-to-Text, Cloud Translation and speech synthesis, plus services of its own in Python |
| Data | Supabase (Postgres, authentication, row level security) |
| Hosting | Vercel and a virtual server in Frankfurt |

## Status

Online at [vociamo.app](https://vociamo.app), with tours, lectures and
conferences working on the hosted service. Before the first pilot with a
customer, what remains is a day of trials on real phones. The source is in a
private repository, available on request.
