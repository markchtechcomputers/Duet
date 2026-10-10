# Duet

**Duet** is a mobile-first dating app built around real accounts, adult profiles, mutual likes, private match chats, and basic safety controls.

## Live app

- Website: https://duet.manlungshop.co.ke
- Source: https://github.com/markchtechcomputers/Duet

## Live features

- Supabase email/password authentication
- Adult-only profile records (18+), editable name, age, gender, preferences, city, bio, interests and HTTPS photo URL
- Shared profile discovery (no seeded or fictional sample profiles)
- Persistent likes and mutual matching
- Private messages between match participants, with Realtime updates
- Report and block controls
- Row Level Security policies on all public application tables

## Architecture

- `index.html` — responsive Duet UI and Supabase client
- `prototype/Duet-original.html` — original uploaded concept preserved as reference
- Supabase project: `idbffhctfilafiaqqxqk`
- Vercel deployment is linked to the GitHub `main` branch

The browser uses only the Supabase publishable key. Do not add a Supabase secret or service-role key to client code.

## Important before broad public launch

The live account and matching foundation is connected, but this is not a claim of full commercial readiness. Before promoting it widely, finish and test photo uploads/storage, account deletion and data export, production moderation workflows, email delivery and redirect settings, rate limits/anti-spam, accessibility, security review, and published Terms of Service and Privacy Policy. Duet does not currently verify identity. Use the report/block controls and meet new people in public places.

## Development

No local build step is required. Open `index.html` in a modern browser or run:

```bash
python -m http.server 8000
```

Authentication and database features require the configured Supabase project and an allowed redirect URL.
