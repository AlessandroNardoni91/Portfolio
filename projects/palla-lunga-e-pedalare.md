# Palla Lunga e Pedalare

English | [Italiano](palla-lunga-e-pedalare.it.md) | [All projects](../README.md)

Instagram page about the players of the Italian Serie A, in Italian, with posts
prepared by AI and approved by a person. Online at
[instagram.com/pallalungaepedalare](https://www.instagram.com/pallalungaepedalare/).

## Description

A football page lives on regularity: a new post every day, with real facts and
an opinion worth arguing about. Palla Lunga e Pedalare is run by an editorial
pipeline that does the heavy work, from the research to the finished graphic,
and leaves one decision to a person: approving the post, from the phone, with a
reply to an email.

The posts are about players, not teams: rankings by role, duels before the big
matches, the team of the matchday, themed grids and guessing games. Every post
is marked on Instagram as AI-generated content.

## Features

- Several recurring formats: rankings in instalments, duels with an open
  verdict, the team of the matchday from the ratings, grids of eight players on
  a theme, carousels of clues to guess a player, and the overreactions of the
  week.
- Graphics produced automatically from templates, with the page's own visual
  identity: logo, colours and fonts.
- Every post comes with a sheet of the facts it is based on, gathered from
  results, ratings and the news of the week.
- Approval by email: the post arrives with its graphic and caption, and a reply
  approves it, asks for changes with a note, or discards it.
- Scheduled publication at a fixed time every day, even with the computer
  switched off.
- If nothing has been approved for the day, a reserve post goes out instead of
  an empty evening.
- A daily editor working in the cloud prepares the next posts every morning and
  applies the requested changes by itself.

## Technical notes

- An approval belongs to one exact version of the post: if the graphic or the
  text changes, it has to be approved again.
- An automatic quality check runs before every approval: the numbers in the
  graphic against the facts sheet, how recent the data is, the player wearing
  the shirt of his current club, and the layout of the graphic.
- Captions follow written style rules, and a check rejects the ones that sound
  machine-written.
- Rankings follow a written method that weighs statistics and football
  judgement together.
- Everything runs on free services.

## Technologies

| Area | Tools |
| --- | --- |
| Pipeline | Python |
| Graphics | HTML templates, Jinja2, Playwright |
| Publishing | Instagram Graph API |
| Approval and scheduling | GitHub Issues and GitHub Actions, email |
| Editor in the cloud | Claude Code scheduled routines |

## Status

Online since September 2026, with one post a day. The source of the editorial
pipeline is in a private repository, available on request.
