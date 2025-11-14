# 007 — Add Notifications & Announcement System

**Summary**
Add an announcement system where admins can post messages to users and basic notifications for booking/payment events.

**Motivation**
Improves communication for schedule changes, payments, and club news.

**Acceptance Criteria**
- Admin endpoint to create announcements (title, body, audience: all/members/individuals) and store them.
- API to fetch recent announcements for clients.
- Trigger notifications (email/simpler in-app notifications) on booking approval, payment confirmation, and cancellations.

**Labels**: enhancement, notifications, admin