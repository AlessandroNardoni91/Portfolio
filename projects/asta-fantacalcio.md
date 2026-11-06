# Asta Fantacalcio

English | [Italiano](asta-fantacalcio.it.md) | [All projects](../README.md)

Application for running a fantasy football draft auction, in both the Classic and
Mantra formats.

## Description

The auction evening is the most awaited night of a fantasy football league, and
the one where mistakes cost the most: a wrong sum, a player assigned twice, a
manager left without enough credits to complete the squad. The application keeps
the accounts while the bidding goes on, so the room can think about the players.

Credits left for each manager, places still to fill and credits to keep aside for
the mandatory ones are always up to date, on the main screen and on everybody's
phone. It works without an internet connection, and it can run from a USB stick.

## Features

- Auction set up with the rules of the league: budget, squad composition and
  starting price.
- Flexible squads, with a minimum and a maximum for each position.
- Import of the official player list from Excel.
- A read-only view for the managers' phones.
- Any assignment can be cancelled at any point of the evening, and a player
  nobody wants is released without slowing the auction down.
- Export to the spreadsheet the league already uses, with totals per position,
  summaries and CSV files.
- Start with a double click, or from a USB stick on a computer without Python.
- Guides for the evening, including how to take a backup halfway through.

## Technical notes

- Budgets are always derived from the purchases recorded, so they cannot drift
  away from them, which was the main problem of the earlier version.
- The auction logic is separate from the interface, which made it possible to
  replace the interface without rewriting the rules.
- The maximum bid shown on a phone is always the same figure the application
  will accept.
- The default squad composition was rebuilt from the spreadsheets of past
  seasons.
- Tested with complete simulated auctions, including one run entirely from the
  USB stick.

## Technologies

| Area | Tools |
| --- | --- |
| Engine and API | Python, FastAPI |
| Data | SQLite |
| Frontend | Next.js (TypeScript), Streamlit as a fallback |
| Import and export | pandas, openpyxl |
| Testing | pytest with 310 automated tests, Playwright |

## Status

Complete and rehearsed with simulated auctions. The source is in a private
repository, available on request.
