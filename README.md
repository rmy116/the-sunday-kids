# The Sunday Kids — static site

Lean HTML/CSS rebuild of [thesundaykids.com](https://www.thesundaykids.com) for **GitHub Pages**.

## What’s included

- Home (mission)
- About Us
- Projects hub + one gallery page per project (clean slugs)
- Get Involved → Join (mailto only) + Follow (Facebook, Instagram, email)
- Shared footer with `info@thesundaykids.com`, Facebook, Instagram

**Not included (by design):** Fund Us / PayPal, Help Us, contact forms.

## Preview locally

From this folder:

```bash
python3 -m http.server 8080
```

Open http://localhost:8080/

Pretty URLs (`/projects/`, `/about/`, etc.) work because each section is a folder with `index.html`.

## Deploy to GitHub Pages

1. Create a repo (e.g. `thesundaykids` or `the-sunday-kids`).
2. Push the contents of this directory to the default branch (or a `gh-pages` branch).
3. In **Settings → Pages**, set source to GitHub Actions or “Deploy from a branch” → `/ (root)`.
4. Optional custom domain: add a `CNAME` file with `www.thesundaykids.com`, then update DNS (www CNAME → `<user>.github.io`; keep Mailgun MX/SPF for email).

No build step is required.

## Project slug map

Old Wix `copy-of-*` paths map to human slugs under `/projects/`. See the Projects hub for titles and galleries.
