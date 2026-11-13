# Joandy business dashboard

A sales, expenses and profit tracker for a buy-and-sell business. One page, no server.

- **Dashboard:** net profit, cash on hand, revenue, cost of goods, salaries, other expenses, margin, product performance, cash flow and month-by-month results. Filter by month or show all time.
- **Sales:** log each sale (date, product, quantity, unit price, customer/notes). Revenue, cost of goods and gross profit are worked out per sale.
- **Expenses:** log salaries and operating costs by category, payee and payment method.
- **Products:** the catalog with selling price, unit cost, unit profit and margin.
- **More:** initial capital, print, backup and restore.
- Sign in to save figures online (Firebase Realtime Database). Everyone listed in the database rules shares and edits the same figures. Without signing in, data stays in the browser.

## Firebase setup

Project `joandy-pnl-projection`, Realtime Database.

- Authentication → Sign-in method: enable **Email/Password** (Google is optional).
- Authentication → Users → Add user: email `username@joandy-pnl-projection.firebaseapp.com` plus a password. People then sign in to the app with just `username` and the password.
- Realtime Database → Rules: paste `database.rules.json` with the real usernames in place of `USERNAME_1` / `USERNAME_2`.
- Authentication → Settings → Authorized domains: add `yakotrading44-code.github.io`.
## Put it online (GitHub Pages)

Settings → Pages → Source: **Deploy from a branch** → Branch: **main**, folder **/ (root)** → Save.
The app then opens at `https://yakotrading44-code.github.io/Joandy-PNL-projection/`.
