# RankBid MVP

Original pay-to-rank leaderboard concept for India + global markets. This MVP is a frontend demo: bids are stored only in browser memory and no real money is charged.

## Run
```bash
npm install
npm run dev
```
Open http://localhost:3000

## Production architecture
- Next.js App Router
- PostgreSQL/Supabase for listings, bids, users and audit logs
- Payment gateway with server-side order creation + webhook verification
- Authentication and admin moderation
- Currency/FX layer
- Anti-fraud/rate limits
- Click analytics
- KYC/business verification as required

## Important
Never put payment secrets in client-side code. Real ranking must change only after a verified payment webhook. Add terms, refund policy, privacy policy, advertiser disclosures, and applicable tax/compliance checks before accepting money.
