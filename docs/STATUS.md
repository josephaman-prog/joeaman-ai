# Status — JoeAman.ai

Updated: 2026-08-16 by Codex

## Now

JoeAman.ai is a live personal website and project hub built with Astro and
npm. GitHub `main` deploys automatically through Cloudflare Pages to
<https://joeaman.ai>. Cloudflare provides authoritative DNS, HTTPS, and
publicly validated DNSSEC; GoDaddy remains the registrar. `www.joeaman.ai`
redirects permanently to the apex domain.

The first subpage is live at <https://joeaman.ai/birthday/2026/>. It is a
responsive, unlisted invitation for Joe's September 5, 2026 pool party and
barbecue at Verve Suites. The page includes a full-frame original/sequel photo
gallery, a placeholder for the planned third photo, a Grill Lineup prep photo,
an editable guest list and menu, and a route-specific social preview image.
Page-specific assets, data, and styles are colocated with the route in
underscored support folders.

## Next steps

1. [ ] Add the event start time when known.
2. [ ] Update the guest list, drinks, and contributed dishes as plans develop.
3. [ ] Replace the third-photo placeholder after the September 5 barbecue.
4. [ ] Add focused checks when the site gains behavior not covered by the Astro build.

## Known issues

- `fnm` is installed, but automatic shell activation has not yet been added to
  the Mac's zsh configuration; run `eval "$(fnm env --use-on-cd --shell zsh)"`
  in a new shell until that is configured.

## Open questions

- What time should the September 5 birthday party begin?
- Which drinks, sides, and guest contributions should be added to the menu?
- Decide the URL and deployment boundary for the first self-contained project
  when its requirements are known; the initial convention is
  `projects/<slug>/`.

## Recent sessions

- 2026-08-16 — Built and deployed the `/birthday/2026/` pool-party invitation with responsive photos, editable party data, the Grill Lineup, and a social preview card.
- 2026-08-16 — Created the Astro/npm project and public GitHub repository, adopted the project framework, connected Cloudflare Pages, and launched `joeaman.ai` with HTTPS, an apex-domain redirect, and publicly validated DNSSEC.
