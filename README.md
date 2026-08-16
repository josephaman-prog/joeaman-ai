# JoeAman.ai

Joe's personal website and project hub at [joeaman.ai](https://joeaman.ai).
The site starts as a lightweight Astro project and can grow to include
independent personal projects without coupling them to the main site.

## Quick start

```bash
fnm use
npm install
npm run dev
```

Create a production build with `npm run build`. Cloudflare Pages builds the
`main` branch with that command and publishes the `dist/` directory.

## Deployment

- Cloudflare Pages project: `joeaman-ai`
- Production branch: `main` with automatic deployments enabled
- Production URL: [joeaman.ai](https://joeaman.ai)
- Pages fallback URL: [joeaman-ai.pages.dev](https://joeaman-ai.pages.dev)
- `www.joeaman.ai` redirects permanently to the apex domain
- GoDaddy remains the registrar; Cloudflare provides authoritative DNS and DNSSEC

## Project docs

- Current state and next steps: [`docs/STATUS.md`](docs/STATUS.md) — start here
- Why things are the way they are: [`docs/DECISIONS.md`](docs/DECISIONS.md)
- Rules for AI agents: [`AGENTS.md`](AGENTS.md)
