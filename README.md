# Screenly

Screenly works out your average daily screen time. Type in how long you were on your screen each day and it shows your daily average, weekly and yearly totals, weekday and weekend averages, and how you're doing against an optional goal.

Use it at https://screenly.ajith.ai

One static page, `index.html`, with inline CSS and JS. No accounts, no tracking. Entries stay in the browser's localStorage.

## Hosting

- GitHub Pages from the `main` branch root. `CNAME` holds `screenly.ajith.ai`.
- DNS: `screenly` CNAME to `ajithjoseph.github.io` in Cloudflare, DNS only (not proxied).
- The repo has the `ajith-app` topic, so it shows up in the app list on [ajith.ai](https://ajith.ai).

## Shutting it down

1. Remove the `ajith-app` topic, or archive the repo. It drops off ajith.ai on the next daily refresh.
2. Delete the `screenly` DNS record in Cloudflare. Do this every time. A record that points at a dead Pages site can be taken over.
