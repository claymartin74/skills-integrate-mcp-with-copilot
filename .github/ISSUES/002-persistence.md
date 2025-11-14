# 002 — Add Persistent Storage for Activities & Signups

**Summary**
Replace the in-memory `activities` dictionary with a persistent database (SQLite for starters) and models for activities, users, and registrations.

**Motivation**
Current in-memory storage is lost on restart and prevents multi-process scaling. Persistence is required for audit logs, analytics, and robust booking workflows.

**Acceptance Criteria**
- Add a lightweight ORM (e.g., SQLModel or SQLAlchemy) and configure a local SQLite DB.
- Create models: `User`, `Activity`, `Registration` (linking users to activities, with status and timestamps).
- Migrate initial seed data from the existing `activities` dict into the DB on first run.
- Update API handlers to use the DB for GET/POST/DELETE operations.
- Add database migration guidance (alembic optional) and update `requirements.txt`.

**Labels**: enhancement, backend, persistence