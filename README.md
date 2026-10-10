# Duet

**Duet** is an early-stage dating-app prototype focused on thoughtful profiles, mutual interest, and safer connections.

## What's included

- `index.html` — responsive, mobile-first Duet design with a pink/coral gradient, profile cards, Explore, Likes, Chats, Profile editor, date ideas, astrology tab, theme toggle, and local demo interactions.
- `prototype/Duet-original.html` — the original uploaded concept, preserved without deleting it.
- `.gitignore` — ignores common local/editor files and secrets.

## Run locally

No build tools are required. Open `index.html` in a modern browser, or run:

```bash
python -m http.server 8000
```

Then visit http://localhost:8000.

## Important: prototype, not production

The current `index.html` is a **browser-only demo**. It uses fictional sample profiles and stores demo interactions in the current browser's `localStorage`. Likes and messages are not sent to other people. There is no real account system, shared database, server-side messaging, moderation service, identity verification, or production privacy/security implementation. Some matching behavior is simulated for demonstration.

The original concept file depended on a custom `claude.use(...)` host integration and remains preserved in `prototype/Duet-original.html`; that integration is not provided by GitHub Pages or a normal browser.

Before launching a real dating service, implement and test authentication, age assurance, profiles/photos, mutual matching, private messaging, reporting/blocking, moderation, rate limiting, data export/deletion, and secure access rules. Publish reviewed Terms of Service and Privacy Policy, and never claim verification or safety controls that are not actually implemented.

## Project status

- [x] Responsive standalone UI prototype
- [x] Profile editing and local demo state
- [x] Explore, Likes, Chats, and theme toggle
- [x] Reset control for demo data
- [ ] Production backend and authentication
- [ ] Real multi-user matching and messaging
- [ ] Safety/moderation and privacy review
- [ ] Automated tests and deployment checks
