# mostlyaboutcode.com

Personal portfolio page, served via GitHub Pages.

## Deploying

1. Create a new **public** GitHub repo (any name works, e.g. `mostlyaboutcode`).
2. Push this folder to it (see commands below).
3. In the repo, go to **Settings → Pages**:
   - Source: `Deploy from a branch`
   - Branch: `main` / `/(root)`
4. Still in **Settings → Pages**, under "Custom domain" enter `mostlyaboutcode.com` and save (this repo already includes the `CNAME` file GitHub Pages needs).
5. At your domain registrar, point DNS at GitHub Pages:
   - Four `A` records for the apex domain (`mostlyaboutcode.com`) pointing to:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - A `CNAME` record for `www` pointing to `<your-github-username>.github.io`
6. Wait for DNS to propagate, then back in Settings → Pages check "Enforce HTTPS" once it's available.

## Editing

Everything lives in `index.html` (styles and script are inline, no build step). Edit the hero text, links, or project cards directly and push — GitHub Pages redeploys automatically.
