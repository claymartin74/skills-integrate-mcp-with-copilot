# 003 — Build Admin Dashboard (Web UI)

**Summary**
Provide an admin interface to manage activities, view registrations, approve or reject signups, and manage users.

**Motivation**
Admin controls are required for approving registrations, managing capacity, and updating activity details.

**Acceptance Criteria**
- Create a basic admin dashboard (can be server-rendered or a small React app) accessible only to `admin` role users.
- Dashboard views: Activities list (create/edit/delete), Registrations list (approve/reject), Users list (promote/demote role).
- Hook the dashboard into the new persistent backend and auth system.

**Labels**: enhancement, frontend, admin