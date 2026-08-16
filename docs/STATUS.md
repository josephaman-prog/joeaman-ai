# Status — JoeAman.ai

Updated: 2026-08-16 by Codex

## Now

JoeAman.ai is a live personal website and project hub built with Astro and
npm. GitHub `main` deploys automatically through Cloudflare Pages to
<https://joeaman.ai>. Cloudflare provides authoritative DNS, HTTPS, and
publicly validated DNSSEC; GoDaddy remains the registrar. `www.joeaman.ai`
redirects permanently to the apex domain.

The current milestone is choosing and building the first subpage in a new
session.

## Next steps

1. [ ] Choose the first subpage and define its route, content, and acceptance criteria.
2. [ ] Build the subpage and link it from the home page.
3. [ ] Add focused checks when the site gains behavior not covered by the Astro build.

## Known issues

- `fnm` is installed, but automatic shell activation has not yet been added to
  the Mac's zsh configuration; run `eval "$(fnm env --use-on-cd --shell zsh)"`
  in a new shell until that is configured.

## Open questions

- Which subpage should be built first?
- Decide the URL and deployment boundary for the first self-contained project
  when its requirements are known; the initial convention is
  `projects/<slug>/`.

## Recent sessions

- 2026-08-16 — Created the Astro/npm project and public GitHub repository, adopted the project framework, connected Cloudflare Pages, and launched `joeaman.ai` with HTTPS, an apex-domain redirect, and publicly validated DNSSEC.
