# Volontiamo

English | [Italiano](volontiamo.it.md) | [All projects](../README.md)

Web application for coordinating volunteers, online at
[volontiamo.org](https://volontiamo.org).

## Description

A village festival, a sports day or a charity dinner needs people at the right
place at the right time. Volontiamo lets an association plan its events,
split them into activities and shifts, and see at a glance which shifts are
covered and which are still missing someone.

Volunteers give their availability and sign up from their phone, even without an
account, from a link the association shares. Reminders and notifications go out
by themselves, and the replies of the volunteers reach the organisation.

## Features

- Associations with local branches, sharing members, roles and permissions.
- Events made of activities, and activities split into shifts.
- Availability of volunteers and sign-ups, also from a public link with no
  account.
- Coverage of every event at a glance: covered, adequate or critical.
- Sign-up deadlines for an event, an activity or a single shift.
- Access by invitation, with five roles and a home page suited to each one.
- Emails for invitations, password reset, a reminder the day before the event
  and notifications. Each organisation chooses the address where replies from
  volunteers arrive.
- Each organisation has its own time zone, used everywhere dates appear.
- A first step suggested on screen when an organisation has no events yet or an
  event has no activities.
- Designed for the phone first, in Italian and British English, with screen
  reader support.
- Visual identity and social preview images designed for the project.

## Technical notes

- Permissions are enforced by the database itself, not only by the interface,
  and visitors without an account never reach the database directly.
- The rules on who can manage whom live in one place, and every change is
  tested against all the roles.
- Password reset links keep working with email clients that open links in
  advance.
- Two operators acting at the same moment do not send the same email twice.
- Sensitive actions are recorded in an audit log.
- The public form is protected against automated sign-ups.
- Every change is tested automatically on a temporary database, and the
  production database is copied every night, encrypted.

## Technologies

| Area | Tools |
| --- | --- |
| Frontend | Next.js, React, TypeScript, Tailwind CSS, shadcn/ui |
| Backend and data | Supabase (Postgres, authentication, row level security) |
| Localisation and validation | next-intl, Zod |
| Infrastructure | Vercel, Cloudflare, Resend, Sentry |
| Automation | Scheduled database jobs, GitHub Actions |

## Status

Online at [volontiamo.org](https://volontiamo.org) and ready for its first
organisations. The source is in a private repository, available on request.
