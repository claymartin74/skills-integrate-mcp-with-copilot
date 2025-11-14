# 004 — Implement Booking Lifecycle & Approval Workflow

**Summary**
Introduce a booking lifecycle (pending → approved → confirmed) and server-side logic for capacity checks and admin approvals.

**Motivation**
Ensure fair allocation of limited slots and let admins manage bookings before confirmation and payment.

**Acceptance Criteria**
- Add `status` field to `Registration` model with values: `pending`, `approved`, `confirmed`, `cancelled`.
- Signup endpoint creates a `pending` registration; admins can `approve` or `reject` registrations via API.
- When approved, registration can be paid/confirmed; capacity checks prevent overbooking.
- Update client UI to reflect statuses and show actions for admins and users.

**Labels**: enhancement, backend, workflow