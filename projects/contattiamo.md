# Contattiamo

English | [Italiano](contattiamo.it.md) | [All projects](../README.md)

An assistant for finding organisations and professionals to contact, preparing
the messages and keeping track of every answer. It works inside Claude and never
sends anything by itself.

## Description

Finding new clients or partners is slow work: searching for the right
organisations, finding the right person inside each one, writing a message that
does not sound like a mass mailing, remembering who to call back and when.
Contattiamo does the searching, the checking and the writing, and leaves the
person in charge of what matters: reading every message and sending it from
their own mailbox.

The tool is the same for everybody. Everything personal, such as who is
writing, how they sign, who they are looking for and the history of the
contacts, lives in a Google spreadsheet that belongs to the person using it.

## Features

- Set up through a short conversation: who is writing, in which language and
  tone, which organisations and roles they are looking for, and what they want
  to ask.
- Search for contacts by sector, role and area, with no duplicates of
  organisations already in the register.
- Every contact comes with its public source and a clear status: verified,
  deduced or weak.
- Messages prepared for each contact: first message with a choice of subject
  lines, a follow-up, a closing message, and outlines for a phone call or a
  meeting. Everything is delivered on a page with copy buttons.
- A register of every contact in the person's own spreadsheet, updated from the
  replies that arrive in the mailbox, with a draft reply for each answer, a no
  included.
- A daily overview: replies to answer, follow-ups due, calls to make and new
  contacts to write to.
- Optional comparison of two different requests, with a warning while the
  numbers are still too small to mean anything.
- Works in Italian, French and English.

## Technical notes

- Nothing is ever sent automatically, and nothing is written into the mailbox:
  the person reads and sends every message.
- Only organisations and professionals in their working role are contacted,
  never private individuals.
- The rules on unsolicited messages and phone calls of each country are part of
  the instructions, starting with Italy and Switzerland, and sources whose terms
  forbid automated reading are only consulted by hand.
- No name, role or address is ever invented: a contact without a source does not
  enter the register.
- The text of an incoming email is treated as data, never as an instruction.
- The tool contains no personal data, so it can be handed to another person
  and installed on their own account.

## Technologies

| Area | Tools |
| --- | --- |
| Assistant | Claude skill: instructions, references and an HTML page template |
| Register | Google Sheets and Google Drive through Claude connectors |
| Mailbox | Gmail, read only |
| Research | Web search and reading of public pages |

## Status

In development. Setup, contact search and message preparation have been tested
on a test register; the daily overview and the update from the mailbox come
next. The source is available on request.
