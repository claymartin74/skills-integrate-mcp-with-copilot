# 006 — Add Coupon / Discount System

**Summary**
Implement a coupon system to allow admins to create discount codes applied to bookings and memberships.

**Motivation**
Coupons support promotions and member discounts.

**Acceptance Criteria**
- Create `Coupon` model with code, discount type (percentage/fixed), usage limit, expiry date, and usage counter.
- Add API endpoints to create/validate/redeem coupons (admin-only for creation).
- Apply coupon discounts in PaymentIntent creation and store applied coupon in transaction records.

**Labels**: enhancement, backend, coupons