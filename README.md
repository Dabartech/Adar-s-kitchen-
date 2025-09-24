# Adar's Foods — Next.js Payments & Orders (Demo)

This project is a minimal full-stack Next.js app for Adar's Foods with:
- Product catalog and checkout (Stripe & Paystack)
- Server API routes to create payments and handle webhooks
- SQLite orders DB (better-sqlite3)
- Admin dashboard (demo login) and daily sales summary
- CSV export for orders

## Quick start (development)

1. Copy `.env.example` to `.env.local` and fill keys.
2. Install deps:
   ```bash
   npm install
   ```
3. Run dev:
   ```bash
   npm run dev
   ```
4. Visit `http://localhost:3000`.

## Demo admin login
- email: `admin@adars.com`
- password: `12345`

## Deploy to Vercel
- Push repo to GitHub.
- Import into Vercel (Root dir = `/`).
- Add environment variables in Vercel Project Settings (use `.env.example`).
- Deploy. Configure webhook endpoints in Stripe/Paystack with the deployed URL:
  - `/api/webhooks/stripe`
  - `/api/webhooks/paystack`

