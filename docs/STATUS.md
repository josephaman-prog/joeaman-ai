# Status — JoeAman.ai

Updated: 2026-08-16 by Codex

## Now

JoeAman.ai is a live personal website and project hub built with Astro and
npm. GitHub `main` deploys automatically through Cloudflare Pages to
<https://joeaman.ai>. Cloudflare provides authoritative DNS, HTTPS, and
publicly validated DNSSEC; GoDaddy remains the registrar. `www.joeaman.ai`
redirects permanently to the apex domain.

The first subpage is `/birthday/2026/`: a responsive, unlisted birthday
invitation for Joe's September 6 pool party and barbecue at Verve Suites. It
includes the supplied barbecue photos, an editable guest list and menu, a
placeholder for the planned third photo, and a route-specific social preview
image. It is part of `main` and deploys through the existing Cloudflare Pages
Git integration.

## Next steps

1. [ ] Review the birthday page copy and design; add the event time when known.
2. [ ] Update the guest, drinks, and contribution data as plans develop.
3. [ ] Add focused checks when the site gains behavior not covered by the Astro build.

## Known issues

- `fnm` is installed, but automatic shell activation has not yet been added to
  the Mac's zsh configuration; run `eval "$(fnm env --use-on-cd --shell zsh)"`
  in a new shell until that is configured.

## Open questions

- What time should the September 6 birthday party begin?
- Which drinks, sides, and guest contributions should be added to the menu?
- Decide the URL and deployment boundary for the first self-contained project
  when its requirements are known; the initial convention is
  `projects/<slug>/`.

## Recent sessions

- 2026-08-16 — Created the Astro/npm project and public GitHub repository, adopted the project framework, connected Cloudflare Pages, and launched `joeaman.ai` with HTTPS, an apex-domain redirect, and publicly validated DNSSEC.
