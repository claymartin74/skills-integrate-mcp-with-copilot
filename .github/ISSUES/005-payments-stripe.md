# 005 — Integrate Stripe Payments for Bookings & Memberships

**Summary**
Add Stripe integration to accept payments for bookings and membership fees. Provide a secure server-side flow and record transactions.

**Motivation**
Payments enable monetization and ensure bookings are secured only after payment.

**Acceptance Criteria**
- Add server-side endpoints to create Stripe PaymentIntents and webhooks to confirm payments.
- Store transaction records with status and Stripe IDs in the DB.
- Only mark `Registration` as `confirmed` after successful payment webhook processing.
- Add environment setup instructions for Stripe keys and webhook testing (ngrok guidance).

**Labels**: enhancement, payments, backend