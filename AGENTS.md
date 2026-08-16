# JoeAman.ai — Agent Instructions

Personal website and project hub for Joe Aman, published at joeaman.ai.

These instructions apply to the whole repository, for any AI tool.

## Session start

1. Run `git status --short --branch` and skim recent history. Do not assume
   the checked-out branch holds the accepted implementation.
2. Read `README.md` and `docs/STATUS.md`.
3. Read only the docs the task needs (doc map below). Do not bulk-load `docs/`.
4. Verify important claims against code, tests, and configuration.
5. If docs and code disagree, say so and fix it as part of the work — never
   silently trust stale prose.

Evidence priority: the user's current instruction > executable behavior and
tests > authoritative docs > active work notes > git history.

## Doc map

| Read | For |
| --- | --- |
| `docs/STATUS.md` | Current state, in-flight work, next steps |
| `docs/DECISIONS.md` | Why durable choices were made |

`docs/archive/` is history — do not read it for current state unless the task
is explicitly about the past.

## Session close

When the user wants to wrap up, hand off, or stop for the day:

1. List every file created or changed this session; separate code from
   doc-like files.
2. Reconcile each doc-like artifact: states a current fact → merge into its
   owning doc, then delete it · records a decision → append to
   `docs/DECISIONS.md`, then delete it · session-specific but worth keeping →
   move to `docs/archive/YYYY-MM-DD-<slug>.md` · everything else → delete.
   When in doubt, archive — never delete.
3. Rewrite `docs/STATUS.md` in full (all sections, new date; add a one-line
   entry under Recent sessions and drop the oldest beyond 5).
4. Sweep the root: only `README.md`, `AGENTS.md`, `CLAUDE.md`, `LICENSE`,
   `.gitignore`, tool config files, and directories belong there.
5. Show the complete plan of edits, moves, and deletions — deletions listed
   individually — and wait for approval before applying.
6. Commit docs housekeeping as `chore(docs): session close YYYY-MM-DD`,
   separate from code commits when practical.

## Rules

- `docs/STATUS.md` is the only handoff document. Never create `handoff.md`,
  `notes.md`, `project_memory.md`, dated summaries, or a second backlog.
- Every new document must have one owner, one purpose, and a known lifecycle;
  otherwise don't create it.
- Generated output goes to gitignored `artifacts/`; scratch work to gitignored
  `scratch/`. Neither is ever committed.
- Never commit secrets, credentials, databases, or personal data.
- Ask before destructive actions, deployments, DNS changes, or git pushes.

## Project specifics

- Build / run: `fnm use`, `npm install`, `npm run dev`; production build is
  `npm run build`, and `npm run preview` serves the built site locally.
- Checks before done: run `npm run build`; add focused checks when the project
  gains behavior that the build does not cover.
- Safety boundaries: do not push, deploy, or change Cloudflare/GoDaddy DNS
  without Joe's approval; keep credentials in ignored environment files or
  provider secret stores only.
- Conventions to respect: Astro is static-first, npm is the package manager,
  Node is pinned by `.node-version`, and Cloudflare Pages deploys `main`.
  Keep the main site at the repository root. Add a future self-contained app
  under `projects/<slug>/` only when it exists, then configure its build root
  independently. Use Astro's official documentation for framework behavior.

---

This project follows Joe's project framework (repo: "Coding and Project
Frameworks"). These instructions are self-contained — you do not need that
repo to work here.

<!-- project-framework: v1 2026-07-21 -->
