# Duet

**Duet** is an early-stage dating-app prototype focused on thoughtful profiles, mutual interest, and safer connections.

## What is in this repository?

- `index.html` — responsive, standalone prototype with Discover, Likes, Chat, and Profile demo sections.
- `prototype/Duet-original.html` — the original uploaded single-file concept, preserved for reference.

## Run locally

No build tools are required. Open `index.html` in a modern browser, or run a local static server:

```bash
python -m http.server 8000
```

Then visit http://localhost:8000.

## Important: prototype, not production

The current `index.html` is a **browser-only demo**. It uses fictional sample profiles and stores demo interactions in the current browser's `localStorage`. Likes and messages are not sent to other people. There is no real account system, shared database, server-side messaging, moderation service, identity verification, or production privacy/security implementation.

The original concept file depended on a custom `claude.use(...)` host integration and is preserved in `prototype/`; that integration is not provided by GitHub Pages or a normal browser.

Before launching a real dating service, implement and test a backend for authentication, age assurance, profiles/photos, mutual matching, private messaging, reporting/blocking, moderation, rate limiting, data export/deletion, and secure access rules. Publish reviewed Terms of Service and Privacy Policy, and never claim verification or safety controls that are not actually implemented.

## Project status

- [x] Responsive standalone prototype
- [x] Accessible tab controls and form labels
- [x] Escaped user-entered text before rendering
- [x] Local demo state and reset control
- [ ] Production backend and authentication
- [ ] Real multi-user matching and messaging
- [ ] Safety/moderation and privacy review
- [ ] Automated tests and deployment checks
