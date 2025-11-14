# 001 — Add User Authentication & Role-Based Authorization

**Summary**
Add user accounts, authentication, and role-based access control so students, members, and admins can securely access the system. This should replace the current open endpoints that accept an email query parameter.

**Motivation**
Authentication enables secure actions (signups, cancellations) and allows future features like payment history tied to users and admin-only workflows.

**Acceptance Criteria**
- Implement Firebase Authentication (or an alternative: FastAPI + JWT) for email/password sign-in.
- Add endpoints for login/logout, registration, and user profile.
- Protect existing endpoints (`/activities/*/signup`, `/activities/*/unregister`) to require authenticated users.
- Add role-based access: at minimum `admin`, `member`, `user`. Admin endpoints are restricted.
- Document env variables and setup steps in `README.md`.

**Notes**
- If using Firebase, include `VITE_*` or `.env` guidance for local dev. For FastAPI + JWT, add dependency to `requirements.txt`.

**Labels**: enhancement, auth, backend