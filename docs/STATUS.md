# Status — JoeAman.ai

Updated: 2026-08-16 by Codex

## Now

JoeAman.ai is a personal website and project hub built with Astro and npm.
The public GitHub repository now exists and the local `main` branch is ready
for its initial push. The current milestone is connecting Cloudflare Pages and
then the joeaman.ai domain.

## Next steps

1. [ ] Approve and push the initial `main` branch.
2. [ ] Connect the GitHub repository to Cloudflare Pages.
3. [ ] Add `joeaman.ai` to Cloudflare and review imported DNS records and DNSSEC.
4. [ ] Change the GoDaddy nameservers after the DNS review, then attach the custom domain.
5. [ ] Define and build the first content and visual-design milestone.

## Known issues

- `fnm` is installed, but automatic shell activation has not yet been added to
  the Mac's zsh configuration; run `eval "$(fnm env --use-on-cd --shell zsh)"`
  in a new shell until that is configured.

## Open questions

- Decide the URL and deployment boundary for the first sub-project when its
  requirements are known; the initial convention is `projects/<slug>/`.
- Decide whether `www.joeaman.ai` should redirect to the apex domain.

## Recent sessions

- 2026-08-16 — Selected Astro/npm, installed the Node toolchain, adopted the project framework, validated the site, and created the public GitHub repository.
