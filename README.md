# nexgig.github.io — Nexgig marketing site

The public marketing site for Nexgig (title *"Nexgig — Book, Play, Manage"*): a one-page landing site plus a support
page. It introduces the product to venue managers and artists and sends them to sign in or download the app. It is a
plain **static site — there is no build step and no backend.**

## Before you work on this site — direction comes from the departments

The repo is enough on its own for **technical** edits only (HTML/CSS, assets, hosting). **Product copy, messaging,
screenshots and branding are owned by the departments — do not change them from the repo alone.** Read the owning
department's entry guide first:

- [Marketing & Video — START-HERE](../../Departments/Marketing%20%26%20Video/START-HERE.md) — marketing copy, messaging and website references.
- [Brand — START-HERE](../../Departments/Brand/START-HERE.md) — logos, fonts and brand originals.

Those links are paths in the founder's local workspace (they open only there). **If you are an outside contributor without
that workspace, you still must get the founder-approved brief for any copy / branding / content change** — use this README
for setup only, and do **not** infer product or brand direction from the current page or old notes.

## Structure (what is actually in this repo)

| File / asset | What it is |
|---|---|
| `index.html` | The landing page. All CSS is **inline** in a single `<style>` block (no separate stylesheet). Includes the "Request access" form. |
| `support.html` | The support page (*"Nexgig — Support"*). |
| `CNAME` | `www.nexgigapp.com` — the custom domain for GitHub Pages. |
| `GeneralSans-*.otf`, `ClashDisplay-Bold.otf` | Bundled brand fonts (General Sans for text, Clash Display for the wordmark). |
| `favicon.png`, `apple-touch-icon.png` | Site icons. |
| `shot-schedule.png`, `shot-budget.png`, `shot-invoices.png` | Product screenshots shown on the landing page. |

### Where the page links out to
- **Sign in** → `https://app.nexgigapp.com/` (the manager web app — a separate repository, `Nexgig/manager-web`).
- **Download for iPhone** → the App Store listing (`apps.apple.com/ae/app/nexgig/id6784020757`).
- **Privacy Policy** and **Terms of Service** → `https://nexgig.github.io/legal/...`, which are served by the **separate
  legal repository** (`Nexgig/legal`), not by this repo. Do not add or edit legal/policy pages here.

## Hosting and deployment

- Hosted on **GitHub Pages** from this repository (`nexgig.github.io`), with the custom domain **www.nexgigapp.com** set
  by the `CNAME` file. GitHub Pages serves the static files directly on push to the published branch; there is no build
  or bundler.
- This README describes the repository's configuration as it stands. **The current live/deploy status is not verified
  here** — confirm it in the GitHub Pages settings or by loading the site before relying on it.
- Editing content is editing `index.html` / `support.html` directly. There are no templates, no framework and no npm.

## Direction and assets

Marketing copy/messaging and brand assets are **owned by the departments**, not this repo — see *Before you work on this
site* at the top: [Marketing & Video](../../Departments/Marketing%20%26%20Video/START-HERE.md) and
[Brand](../../Departments/Brand/START-HERE.md) (founder-workspace paths). A copy/branding/content change needs the current
founder-approved brief; technical edits (HTML/CSS/assets/hosting) can be made from this repo.

Unused historical `hero-icon.png` was archived on 20 October in [Design archive](../../Departments/Design/Archive/2026-10-20-marketing-site-unused-assets/). Current pages do not reference it.
