# Movo — Your money. Your moves.

Movo is a personal finance and money-planning app. It doesn't just log what you spent — it tells you **what's actually safe to spend right now**, what your money looks like a few weeks from now, and lets you test big decisions before you make them.

It's a single self-contained web app: one HTML file, no backend, no server. Everything you enter is stored privately in your own browser — nothing is ever sent anywhere.

---

## What it actually does

Most expense trackers only answer one question: *"where did my money go?"* Movo answers five:

1. Where did my money go?
2. Where is my money right now?
3. How much of it is already spoken for?
4. How much is actually safe to spend?
5. What might my money look like in the future?

### The three core features

- **🟢 Safe to Spend** — your real, spendable balance: total money minus upcoming bills/EMIs minus savings you've already committed to. Always shown with a transparent breakdown, never a black box.
- **📅 Future Money** — a day-by-day projection of your balance over the next 7/30/60/90 days, based on your recurring income, bills, and loan EMIs.
- **🔮 What If…?** — simulate a big purchase, a new loan, a salary change, or an increased SIP *before* it happens, and see the effect on your Safe to Spend and Net Worth. Nothing is applied to your real data unless you confirm it.

### Everything else it tracks

- Multiple accounts — bank, cash, wallet, credit cards
- Income, expenses (with who you paid, who paid, payment method, date *and* time), and transfers
- Loans & EMI tracking, with a proper amortization-based EMI calculator
- FDs & investments, kept clearly separate from everyday spending
- Budgets (with 75%/90% warnings) and savings goals
- Bills & recurring transactions (salary, rent, subscriptions, SIPs)
- **Trips & Events** — group expenses under a trip, wedding, festival, or party with its own budget
- Net worth over time, monthly reports, a financial calendar, and plain-language insights
- CSV export, full JSON backup/restore, dark/light theme, optional PIN lock

## Who it's for

Built with Indian users in mind (₹, Indian categories, Indian financial products like FDs/EMIs), but nothing about it is India-specific under the hood.

## Privacy

There is no database and no login. Every account, transaction, loan, and goal you add lives only in your browser's local storage on the device you're using. Nobody — including whoever's hosting this file — can see your data. This also means:

- It doesn't sync across devices on its own. Use **Settings → Export backup** on one device and **Restore backup** on another to move your data.
- Clearing your browser's site data will erase it. Export a backup regularly.

## Running it

This is a static site — there is nothing to build or install.

- **Locally**: just open `index.html` in a browser.
- **Hosted**: deploy this repo to [Vercel](https://vercel.com), [Netlify](https://netlify.com), GitHub Pages, or any static host. No environment variables, no build step, no server.

### Add it to your phone's home screen

Open the hosted link in Safari (iPhone) or Chrome (Android) → **Add to Home Screen**. It opens full-screen with its own icon, like a real app.

## Tech

Plain HTML, CSS, and React (loaded via CDN, compiled in-browser with Babel) — one file, nothing to install. All calculations (EMI, projections, net worth, Safe to Spend) run entirely client-side.

## Limitations

This is a personal, single-user tool — not a production fintech product. There's no real authentication, no encryption, and no server-side validation, because there's no server at all. It doesn't connect to your bank; everything is entered manually.

---

*Movo — your money. your moves.*
