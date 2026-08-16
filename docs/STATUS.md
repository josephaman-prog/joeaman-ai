# Status — JoeAman.ai

Updated: 2026-08-16 by Codex

## Now

JoeAman.ai is a personal website and project hub built with Astro and npm.
The current milestone is establishing the GitHub-to-Cloudflare Pages delivery
pipeline and connecting the joeaman.ai domain.

## Next steps

1. [ ] Authenticate GitHub CLI and create `josephaman-prog/joeaman-ai`.
2. [ ] Approve and push the initial `main` branch.
3. [ ] Connect the GitHub repository to Cloudflare Pages.
4. [ ] Add `joeaman.ai` to Cloudflare and review imported DNS records and DNSSEC.
5. [ ] Change the GoDaddy nameservers after the DNS review, then attach the custom domain.
6. [ ] Define and build the first content and visual-design milestone.

## Known issues

- `fnm` is installed, but automatic shell activation has not yet been added to
  the Mac's zsh configuration; run `eval "$(fnm env --use-on-cd --shell zsh)"`
  in a new shell until that is configured.

## Open questions

- Decide the URL and deployment boundary for the first sub-project when its
  requirements are known; the initial convention is `projects/<slug>/`.
- Decide whether `www.joeaman.ai` should redirect to the apex domain.

## Recent sessions

- 2026-08-16 — Selected Astro/npm, audited the Mac toolchain, adopted the project framework, and began the GitHub/Cloudflare bootstrap.
