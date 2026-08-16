# Status — JoeAman.ai

Updated: 2026-08-16 by Codex

## Now

JoeAman.ai is a personal website and project hub built with Astro and npm.
The public GitHub repository is connected to Cloudflare Pages, automatic
deployments from `main` are enabled, and the first production deployment is
live at <https://joeaman-ai.pages.dev>. The current milestone is connecting
the `joeaman.ai` custom domain.

## Next steps

1. [ ] Add `joeaman.ai` to Cloudflare and review imported DNS records and DNSSEC.
2. [ ] Change the GoDaddy nameservers after the DNS review, then attach the custom domain.
3. [ ] Define and build the first content and visual-design milestone.

## Known issues

- `fnm` is installed, but automatic shell activation has not yet been added to
  the Mac's zsh configuration; run `eval "$(fnm env --use-on-cd --shell zsh)"`
  in a new shell until that is configured.
- Three untracked duplicate files (`.gitignore 2`, `README 2.md`, and
  `src/pages/index 2.astro`) are present locally. They were preserved and are
  not part of the GitHub repository or deployed site.

## Open questions

- Decide the URL and deployment boundary for the first sub-project when its
  requirements are known; the initial convention is `projects/<slug>/`.
- Decide whether `www.joeaman.ai` should redirect to the apex domain.

## Recent sessions

- 2026-08-16 — Selected Astro/npm, installed the Node toolchain, adopted the project framework, created the public GitHub repository, connected Cloudflare Pages, and verified the first production deployment.
