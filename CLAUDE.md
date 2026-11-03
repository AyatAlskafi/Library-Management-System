# Library Management System

Web app for managing a library. Arabic (RTL) + English (LTR), light/dark mode.

## Roles
- **Admin**: manage users and staff (add/delete, set role).
- **Librarian**: manage books, lend, return.
- **Member**: borrower, appears in the lending list.

## Features
Book search, availability status, borrowing history.

## Structure
- `public/index.html` — whole front end (vanilla JS, data in localStorage for now).
- `.claude/skills/frontend-design` — design skill, read it before any UI change.

## Rules
- Every user-facing string goes in the `T` dictionary in both `ar` and `en`.
- Use logical CSS (`margin-inline-start`, `text-align:start`), never left/right.
- Colors come from the CSS variables in `:root` and `[data-theme=dark]`.

## Next steps
1. Node.js + Express backend with SQLite.
2. Hash passwords (scrypt/bcrypt) and use sessions/JWT.
3. Enforce roles on the server, not only in the UI.
4. Tests for lend/return logic.
