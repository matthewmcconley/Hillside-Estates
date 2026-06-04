# Hillside Estates at Franklin — Website

Static HTML/CSS site for Hillside Estates at Franklin, a mobile home community in Franklin, NJ.
No build step, no frameworks — plain HTML/CSS hosted on GitHub Pages.

## Pages
- `index.html` — Home
- `homes-for-sale.html` — Homes for Sale
- `information.html` — Information (buyer/resident resources, rules & regulations)
- `contact.html` — Contact Us
- `appfolio.html` — AppFolio resident portal

## Assets
- `assets/` — images, logo, favicons
- `assets/docs/credit-check.pdf` — credit check authorization form (linked from Information + footer)

## Deploy to GitHub Pages
1. Create a new GitHub repo and push these files to the `main` branch (repo root).
2. Repo **Settings → Pages** → Source: **Deploy from a branch** → Branch: **main** / **/(root)** → Save.
3. The site publishes at `https://<username>.github.io/<repo>/` within a minute or two.

## Custom domain (hillsideestatesatfranklin.com)
- The `CNAME` file is set to `hillsideestatesatfranklin.com`. **Edit it to match the exact domain you configure**, or delete it if you are not using a custom domain yet.
- In your DNS, point the domain at GitHub Pages:
  - Apex (`hillsideestatesatfranklin.com`): add GitHub Pages A records (185.199.108–111.153) — see GitHub docs for current IPs.
  - `www`: add a CNAME record to `<username>.github.io`.
- In Settings → Pages, set the Custom domain and enable **Enforce HTTPS**.

## To do / notes
- **Application form**: the "Application for Tenancy" links currently point to the Contact page as a placeholder. Drop the real PDF into `assets/docs/`, then point the Application links to it.
