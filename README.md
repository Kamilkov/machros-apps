# machros.app

Source of the [machros.app](https://machros.app/) umbrella site — the family
page for Kamil Kovac's apps:

- **Tesouros** (iPhone) — personal collections tracker; privacy policy at
  [`/tesouros/privacy`](https://machros.app/tesouros/privacy)
- **JSON Analyzer** (macOS) — [jsonanalyzer.com](https://jsonanalyzer.com/)
- **UsageBar** (macOS) — [github.com/Kamilkov/subscriptions-dashboard](https://github.com/Kamilkov/subscriptions-dashboard)
- **FanBoost** (macOS) — [github.com/Kamilkov/fanboost](https://github.com/Kamilkov/fanboost)

Static HTML, no build step. The repo root is the deploy directory.

## Deploy

Pushes to `main` deploy automatically via GitHub Actions to the Cloudflare
Pages project `machros` (serves machros.app + machros.pages.dev).

Manual deploy from a checkout:

```
npx wrangler pages deploy . --project-name machros
```
