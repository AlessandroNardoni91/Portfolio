# Torre degli Agli

English | [Italiano](torre-degli-agli.it.md) | [All projects](../README.md)

Guest guide for a short-let apartment in Florence, opened from a QR code in the
flat. Online at
[alessandronardoni91.github.io/torre-degli-agli](https://alessandronardoni91.github.io/torre-degli-agli/).

## Description

Guests arriving in a city they do not know have the same questions: how do I get
in, how does the oven work, which bus goes to the centre, where do we eat
tonight. Instead of a folder on the table or a long message, the flat has a QR
code. One scan opens a guide in the guest's own language, made for a phone held
in one hand.

The guide exists in English, Italian, Spanish and French, and opens directly in
the language of the phone.

## Features

- Arrival and self check-in explained step by step, with screenshots.
- House rules, public transport, restaurants and walks nearby.
- A page for every appliance, with pictures of the controls and of the buttons
  mentioned in the text, and the original manuals to download.
- A photo gallery of the flat.
- Language chosen from a menu with flags, and remembered from one page to the
  next.
- Light pages that load quickly on a phone connection.
- Not listed on search engines: the guide is for the people who have the QR
  code.

## Technical notes

- A plain static site, with no framework and no build step: editing a page
  means editing one file, and publishing it is one push.
- The four languages of a page live together in the same file, so they cannot
  drift apart.
- An automatic check runs before every publication: the same content in every
  language, no broken link or missing image, the weight of each page, and none
  of the private details of the host.
- Privacy is part of the design: the exact address and the phone numbers of the
  host never appear, not even in the map screenshots.

## Technologies

| Area | Tools |
| --- | --- |
| Site | HTML, CSS and JavaScript, with no dependencies |
| Hosting | GitHub Pages |
| Checks | Python |

## Status

Online, and the QR code in the apartment leads to it. The source is public at
[github.com/AlessandroNardoni91/torre-degli-agli](https://github.com/AlessandroNardoni91/torre-degli-agli).
