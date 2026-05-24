# Attalis Briefing

Personal finance/deals briefing dashboard for Kavan Mehta.

## What is live now

- Daily email briefing task: runs at 6:00am Australia/Sydney and scans the prior calendar day.
- Weekly newsletter task: runs Monday at 6:00am Australia/Sydney and scans the previous Monday-Sunday week.
- This repo folder contains the briefing UI shell and the prior React prototype.

## Important architecture note

The uploaded React artifact is a front-end prototype. It cannot reliably send scheduled email by itself, and it should not expose private API keys from a browser. The scheduled email work is handled by the ChatGPT recurring tasks.

For a fully self-hosted production version later, use:
- GitHub Actions cron or Vercel Cron
- a server-side API route
- Gmail API / SendGrid / Resend
- OpenAI/Claude web-search summarisation server-side
- GitHub Pages or Vercel for the static archive/dashboard

## Current schedule

- Daily: 6:00am Sydney time, prior-day scan
- Weekly: Monday 6:00am Sydney time, prior Mon-Sun scan
