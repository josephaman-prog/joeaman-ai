# Status — JoeAman.ai

Updated: 2026-08-16 by Codex

## Now

JoeAman.ai is a personal website and project hub built with Astro and npm.
The public GitHub repository is connected to Cloudflare Pages, automatic
deployments from `main` are enabled, and the first production deployment is
live at <https://joeaman.ai>. Cloudflare provides authoritative DNS, HTTPS,
and DNSSEC; GoDaddy remains the registrar. `www.joeaman.ai` redirects to the
apex domain. The current milestone is defining the site's first content and
visual-design release.

## Next steps

1. [ ] Define and build the first content and visual-design milestone.
2. [ ] Verify that the DNSSEC DS record is visible from the `.ai` registry after propagation.
3. [ ] Resolve or remove the preserved local duplicate files after reviewing them with Joe.

## Known issues

- `fnm` is installed, but automatic shell activation has not yet been added to
  the Mac's zsh configuration; run `eval "$(fnm env --use-on-cd --shell zsh)"`
  in a new shell until that is configured.
- Three untracked duplicate files (`.gitignore 2`, `README 2.md`, and
  `src/pages/index 2.astro`) are present locally. They were preserved and are
  not part of the GitHub repository or deployed site.
- DNSSEC is enabled and its DS record is saved at GoDaddy; the `.ai` registry
  had not yet exposed the DS record when the custom domain was first verified.

## Open questions

- Decide the URL and deployment boundary for the first sub-project when its
  requirements are known; the initial convention is `projects/<slug>/`.

## Recent sessions

- 2026-08-16 — Selected Astro/npm, installed the Node toolchain, adopted the project framework, created the public GitHub repository, connected Cloudflare Pages, and launched `joeaman.ai` with HTTPS, a `www` redirect, and DNSSEC.
