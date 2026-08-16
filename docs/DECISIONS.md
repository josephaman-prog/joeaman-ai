# Decisions — JoeAman.ai

Append-only, newest first. One entry per durable decision. When this file
passes ~15 entries, graduate to a `docs/decisions/` folder of numbered
records.

## 2026-08-16 — Start with one repository

**Decision:** Keep the main site at the repository root. When a distinct
sub-project appears, place it under `projects/<slug>/` and give its deployment
an independent build root.

**Why:** One repository is easier to navigate and operate while the site is
small. The directory boundary preserves the option to split a project into a
separate repository later.

**Instead of:** Creating several empty repositories now or committing to a
full workspace layout before any sub-project requirements exist.

## 2026-08-16 — Deploy main through Cloudflare Pages Git integration

**Decision:** Cloudflare Pages builds and deploys the `main` branch from
GitHub, using `npm run build` and the `dist/` output directory.

**Why:** This implements the desired edit → GitHub → Cloudflare workflow with
minimal local deployment tooling and provides branch preview deployments when
they are useful later.

**Instead of:** A custom GitHub Actions deployment workflow or manual Wrangler
uploads.

## 2026-08-16 — Use Astro and npm

**Decision:** Build the initial personal site with Astro and npm, with Node.js
22.19.0 pinned for local and Cloudflare builds.

**Why:** Astro is a small static-first foundation for a content-oriented
personal site and can add React components selectively when interactivity is
needed. Node 22.19 satisfies Astro's dependency floor while remaining within
the Node 22 line supported by Cloudflare Pages through `.node-version`.

**Instead of:** Starting with Next.js or a client-heavy React application
before those capabilities are required.

## 2026-08-16 — Adopted the project framework

**Decision:** This project follows the core framework layout: single living
handoff at `docs/STATUS.md`, this append-only decision log, and a dated
`docs/archive/`.

**Why:** Keeps multi-session work navigable for humans and AI agents; nothing
stale accumulates at the root.

**Instead of:** Ad-hoc per-session handoff and notes files.
