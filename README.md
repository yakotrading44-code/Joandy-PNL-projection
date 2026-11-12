# Joandy P&L projection

A simple profit and loss tracker for a buy-and-sell business. One page, no server.

- Pick a month, enter units sold per product and the month's expenses.
- Revenue, cost of goods, gross profit and net profit calculate automatically.
- "All months" shows every month side by side.
- Sign in with Google to save figures online (Firebase Realtime Database) and see them on any device. Without signing in, data stays in the browser (localStorage).
- **Download backup** / **Restore backup** keep a copy as a file.

## Firebase setup

Project `joandy-pnl-projection`. Enable Google sign-in under Authentication, add `yakotrading44-code.github.io` to Authorized domains, and paste `database.rules.json` into Realtime Database → Rules.

## Put it online (GitHub Pages)

Settings → Pages → Source: **Deploy from a branch** → Branch: **main**, folder **/ (root)** → Save.
The app then opens at `https://yakotrading44-code.github.io/Joandy-PNL-projection/`.
